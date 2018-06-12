---
title: Cabeçalhos x provisão usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 45a99a14-a85f-47f8-af48-18eb6c6cc230
description: Saiba como provisionar cabeçalhos x para uma caixa de correio usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: de572764921da432cfa203b3dcf166d1d34dd0cd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750809"
---
# <a name="provision-x-headers-by-using-ews-in-exchange"></a>Cabeçalhos x provisão usando o EWS no Exchange

Saiba como provisionar cabeçalhos x para uma caixa de correio usando a API gerenciada de EWS ou EWS no Exchange.
  
Cabeçalhos X são padronizados cabeçalhos que são adicionados à coleção de cabeçalho de um email para comunicar informações. Por exemplo, troca mensagens de carimbos com o cabeçalho **X-MS-Exchange-organização-SCL** para indicar o nível de confiança de spam (SCL) atribuído ao email. Clientes de email, como o Outlook pode usar essas informações para determinar que tipo de ação a ser executada no email (por exemplo, Outlook pode impedir que imagens sejam exibidas, a menos que o usuário realiza uma ação). 
  
Exchange adiciona cabeçalhos x entrados com o esquema de caixa de correio como um horário de propriedade nomeada o primeiro, que ele recebe um email com esse cabeçalho x. O valor de cabeçalho x não serão salvas no primeiro e-mail; No entanto, ele é salvo em todos os emails subsequentes que incluem o cabeçalho x. Por esse motivo, o seu aplicativo deve provisionar cabeçalhos x antes de você espera usá-las. O mapeamento entre uma propriedade nomeada e um cabeçalho x ocorre na entrega de transporte de email na caixa de correio. Isso significa que você precisa receber o email por meio de entrega de transporte; Você simplesmente não é possível salvar um email que inclui o cabeçalho x uma caixa de correio para criar o mapeamento para uma propriedade nomeada.
  
> [!NOTE]
> Se você achar que os cabeçalhos x não estão sendo salvas, determine se um [agente de transporte](http://code.msdn.microsoft.com/Exchange-2013-Build-an-32f62f5a) ou um [firewall de cabeçalho](http://technet.microsoft.com/en-us/library/bb232136%28v=exchg.150%29.aspx) está filtrando suas cabeçalhos x que eles cheguem à caixa de correio. 
  
## <a name="provision-an-x-header-by-using-the-ews-managed-api"></a>Provisionar um cabeçalho x usando a API gerenciada de EWS
<a name="bk_example1"> </a>

O exemplo de código a seguir mostra como usar o método de API gerenciada de EWS [EmailMessage.Send](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) para provisionar um cabeçalho x para uma caixa de correio. Este exemplo pressupõe que esse **serviço** é válida [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) objeto e que a caixa de correio de destino ainda não excedido as [propriedades nomeadas de cota](http://technet.microsoft.com/en-us/library/bb851492%28v=EXCHG.80%29.aspx).
  
```cs
private static void ProvisionCustomXHeaderByEmail(ExchangeService service)
{
    // Create a definition for an extended property that will represent a custom x-header. X-headers must be created in the
    // InternetHeaders property set. The x-header name must match the name of the x-header sent in the subsequent emails so
    // the x-header and value are saved on the email.
    ExtendedPropertyDefinition xExperimentalHeader = new ExtendedPropertyDefinition(DefaultExtendedPropertySet.InternetHeaders,
                                                                                            "X-Experimental",
                                                                                            MapiPropertyType.String);
    // Create an item that is used to provision the custom x-header.
    EmailMessage email = new EmailMessage(service);
    email.ToRecipients.Add("user@contoso.com");
    email.SetExtendedProperty(xExperimentalHeader, "Provision X-Experimental Internet message header");
    try
    {
        // The mapping of the named property happens in transport delivery.
        email.Send();
        if (service.ServerInfo.MajorVersion == 12)
        {
            Console.WriteLine("Provisioned the X-Experimental across the mailbox database that hosts the user's mailbox.");
        }
        else // For versions of Exchange starting with Exchange 2010
        {
            Console.WriteLine("Provisioned the X-Experimental for the user's mailbox. You will need to run this " +
                                "for each mailbox that needs to process this x-header.");
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error: {0}", ex.Message);
    }
}
```

## <a name="provision-an-x-header-by-using-ews"></a>Provisionar um cabeçalho x usando o EWS
<a name="bk_example1"> </a>

O exemplo de código a seguir mostra como usar a operação de EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) para criar e enviar um email para provisionar uma caixa de correio com um cabeçalho x. Essa é a solicitação XML que é enviada pela API gerenciada de EWS quando você [provisionar um cabeçalho x usando a API gerenciada de EWS](#bk_example1).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendOnly">
      <m:Items>
        <t:Message>
          <t:ExtendedProperty>
            <t:ExtendedFieldURI DistinguishedPropertySetId="InternetHeaders"
                                PropertyName="X-Experimental"
                                PropertyType="String" />
            <t:Value>Provision X-Experimental Internet message header</t:Value>
          </t:ExtendedProperty>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>user@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

## <a name="version-differences"></a>Diferenças de versão
<a name="bk_example1"> </a>

Na primeira vez que você provisionar um cabeçalho x no Exchange Online, Exchange Online como parte do Office 365 ou uma versão local do Exchange, começando com o Exchange Server 2010, o valor de um novo cabeçalho x personalizado não será gravado à mensagem armazenada. Isso ocorre porque o cabeçalho x primeiro deve ser mapeado para uma propriedade nomeada na caixa de correio do usuário. O mapeamento ocorre após a primeira solicitação para adicionar as propriedades nomeadas. Quando uma solicitação subsequente para criar a propriedade nomeada ocorre, a propriedade e o valor são armazenados na mensagem. No Exchange 2007, na primeira vez que um cabeçalho x é gravado em um banco de dados de caixa de correio, um mapeamento é criado para o cabeçalho x para uma propriedade nomeada entre o banco de dados de caixa de correio. Quando uma solicitação subsequente para criar a propriedade nomeada ocorre, o cabeçalho x é processado e armazenado para qualquer caixa de correio no banco de dados do Exchange 2007.
  
## <a name="next-steps"></a>Próximas etapas
<a name="bk_example1"> </a>

Este artigo mostra como provisionar um cabeçalho x para uma única caixa de correio, enviando um email para um usuário. Você também pode provisionar um cabeçalho x de muitos usuários, [enviando um e-mail de lote para uma lista de destinatários](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md) na organização do chamador. 
  
## <a name="see-also"></a>Confira também


- [Propriedades e as propriedades estendidas no EWS no Exchange](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Exchange 2013: Provisionar cabeçalhos X personalizados programaticamente](http://code.msdn.microsoft.com/exchange/Exchange-2013-Provision-d4ef5719)
    
- [Propriedades, nomeadas cabeçalhos X e você](http://blogs.technet.com/b/exchange/archive/2009/04/06/3407221.aspx)
    
- [Propriedades nomeadas, arredondar 2: O que vem pela frente](http://blogs.technet.com/b/exchange/archive/2009/06/12/3407672.aspx)
    
- [Firewall de cabeçalho](http://technet.microsoft.com/en-us/library/bb232136%28v=exchg.150%29.aspx)
    
- [EWS, MIME e os cabeçalhos das mensagens de Internet ausentes](http://msdn.microsoft.com/library/office/hh545614%28v=exchg.140%29.aspx)
    
- [Processar as mensagens de email em lotes, usando o EWS no Exchange](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    

