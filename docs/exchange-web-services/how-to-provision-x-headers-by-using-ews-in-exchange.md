---
title: Provisionar cabeçalhos x usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 45a99a14-a85f-47f8-af48-18eb6c6cc230
description: Saiba como provisionar cabeçalhos x para uma caixa de correio usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 409ddb944bbac7a60242de39cdf7ae13b17cc76a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527765"
---
# <a name="provision-x-headers-by-using-ews-in-exchange"></a>Provisionar cabeçalhos x usando o EWS no Exchange

Saiba como provisionar cabeçalhos x para uma caixa de correio usando a API gerenciada do EWS ou o EWS no Exchange.
  
Os cabeçalhos X são cabeçalhos não padrão adicionados à coleção de cabeçalho de um email para comunicar informações. Por exemplo, o Exchange carimba mensagens com o cabeçalho **X-MS-Exchange-Organization-SCL** para indicar o nível de confiança de spam (SCL) atribuído ao email. Clientes de email como o Outlook podem usar essas informações para determinar o tipo de ação a ser tomada no email (por exemplo, o Outlook pode impedir a exibição de imagens, a menos que o usuário execute uma ação). 
  
O Exchange adiciona cabeçalhos x de entrada ao esquema de caixa de correio como uma propriedade nomeada na primeira vez que recebe um email com esse cabeçalho x. O valor do cabeçalho x não é salvo nesse primeiro email; no entanto, ele é salvo em todos os emails subsequentes que incluem o cabeçalho x. Por esse motivo, seu aplicativo deve provisionar cabeçalhos x antes de você esperar usá-los. O mapeamento entre uma propriedade nomeada e um cabeçalho x ocorre na entrega de transporte do email para a caixa de correio. Isso significa que você precisa receber o email via entrega de transporte; Você não pode apenas salvar um email que inclua o cabeçalho x em uma caixa de correio para criar o mapeamento para uma propriedade nomeada.
  
> [!NOTE]
> Se você descobrir que os cabeçalhos x não estão sendo salvos, determine se um [agente de transporte](https://code.msdn.microsoft.com/Exchange-2013-Build-an-32f62f5a) ou um firewall de [cabeçalho](https://technet.microsoft.com/library/bb232136%28v=exchg.150%29.aspx) está filtrando seus cabeçalhos x antes de chegar à caixa de correio. r
  
## <a name="provision-an-x-header-by-using-the-ews-managed-api"></a>Provisionar um cabeçalho x usando a API gerenciada do EWS
<a name="bk_example1"> </a>

O exemplo de código a seguir mostra como usar o método API gerenciada do EWS [EmailMessage. Send](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) para provisionar um cabeçalho x para uma caixa de correio. Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que a caixa de correio de destino não excedeu a [cota para propriedades nomeadas](https://technet.microsoft.com/library/bb851492%28v=EXCHG.80%29.aspx).
  
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

O exemplo de código a seguir mostra como usar a operação EWS [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) para criar e enviar um email para provisionar uma caixa de correio com um cabeçalho x. Esta é a solicitação XML que é enviada pela API gerenciada do EWS quando você [provisiona um cabeçalho x usando a API gerenciada do EWS](#bk_example1).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

Na primeira vez que você provisionar um cabeçalho x no Exchange Online, o Exchange Online como parte do Office 365 ou uma versão local do Exchange que comece com o Exchange Server 2010, o valor de um novo cabeçalho x personalizado não será gravado na mensagem armazenada. Isso ocorre porque o cabeçalho x deve primeiro ser mapeado para uma propriedade nomeada na caixa de correio do usuário. O mapeamento ocorre na primeira solicitação para adicionar as propriedades nomeadas. Quando uma solicitação subsequente para criar a propriedade nomeada ocorre, a propriedade e o valor são armazenados na mensagem. No Exchange 2007, a primeira vez que um cabeçalho x é gravado em um banco de dados de caixa de correio, um mapeamento é criado para o cabeçalho x para uma propriedade nomeada no banco de dados de caixa de correio. Quando uma solicitação subsequente para criar a propriedade nomeada ocorre, o cabeçalho x é processado e armazenado para qualquer caixa de correio no banco de dados do Exchange 2007.
  
## <a name="next-steps"></a>Próximas etapas
<a name="bk_example1"> </a>

Este artigo mostra como provisionar um cabeçalho x para uma única caixa de correio enviando um email para um usuário. Você também pode provisionar um cabeçalho x para muitos usuários [enviando um email em lotes para uma lista de destinatários](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md) na organização do chamador. 
  
## <a name="see-also"></a>Confira também


- [Propriedades e propriedades estendidas no EWS no Exchange](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Exchange 2013: provisionar cabeçalhos X personalizados de forma programática](https://code.msdn.microsoft.com/exchange/Exchange-2013-Provision-d4ef5719)
    
- [Propriedades nomeadas, cabeçalhos X e você](https://blogs.technet.com/b/exchange/archive/2009/04/06/3407221.aspx)
    
- [Propriedades nomeadas, redondo 2: o que está em frente](https://blogs.technet.com/b/exchange/archive/2009/06/12/3407672.aspx)
    
- [Firewall de cabeçalho](https://technet.microsoft.com/library/bb232136%28v=exchg.150%29.aspx)
    
- [EWS, MIME e os cabeçalhos de mensagem da Internet ausentes](https://msdn.microsoft.com/library/office/hh545614%28v=exchg.140%29.aspx)
    
- [Processar mensagens de email em lotes usando o EWS no Exchange](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    

