---
title: Provisionar os headers x usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 45a99a14-a85f-47f8-af48-18eb6c6cc230
description: Saiba como provisionar os headers x para uma caixa de correio usando a API Gerenciada do EWS ou o EWS Exchange.
ms.openlocfilehash: e60092e0d40d5815cdf3fd4ed588e2f74978c245
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521113"
---
# <a name="provision-x-headers-by-using-ews-in-exchange"></a>Provisionar os headers x usando o EWS no Exchange

Saiba como provisionar os headers x para uma caixa de correio usando a API Gerenciada do EWS ou o EWS Exchange.
  
Os headers X são headers não padrão adicionados à coleção de header de um email para comunicar informações. Por exemplo, Exchange carimba mensagens com o header **X-MS-Exchange-Organization-SCL** para indicar o nível de confiança de spam (SCL) atribuído ao email. Clientes de email como Outlook podem usar essas informações para determinar que tipo de ação deve ser tomada no email (por exemplo, Outlook pode impedir que imagens exam, a menos que o usuário tome uma ação). 
  
Exchange adiciona os headers x de entrada ao esquema de caixa de correio como uma propriedade nomeada na primeira vez em que recebe um email com esse header x. O valor de header x não é salvo no primeiro email; no entanto, ele é salvo em todos os emails subsequentes que incluem o header x. Por esse motivo, seu aplicativo deve provisionar os headers x antes de você esperar usá-los. O mapeamento entre uma propriedade nomeada e um header x ocorre na entrega de transporte do email para a caixa de correio. Isso significa que você precisa receber o email por meio de entrega de transporte; você não pode salvar apenas um email que inclui o header x em uma caixa de correio para criar o mapeamento para uma propriedade nomeada.
  
> [!NOTE]
> Se você descobrir que os headers x não [](https://code.msdn.microsoft.com/Exchange-2013-Build-an-32f62f5a) estão sendo salvos, determine se um agente de transporte ou firewall de [header](https://technet.microsoft.com/library/bb232136%28v=exchg.150%29.aspx) está filtrando seus headers x antes de chegar à caixa de correio. r
  
## <a name="provision-an-x-header-by-using-the-ews-managed-api"></a>Provisionar um header x usando a API Gerenciada do EWS
<a name="bk_example1"> </a>

O exemplo de código a seguir mostra como usar o método [EmailMessage.Send](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) da API gerenciada do EWS para provisionar um header x para uma caixa de correio. Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que a caixa de correio de destino não excedeu a [cota de propriedades nomeadas.](https://technet.microsoft.com/library/bb851492%28v=EXCHG.80%29.aspx)
  
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

## <a name="provision-an-x-header-by-using-ews"></a>Provisionar um header x usando o EWS
<a name="bk_example1"> </a>

O exemplo de código a seguir mostra como usar a operação [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) do EWS para criar e enviar um email para provisionar uma caixa de correio com um header x. Esta é a solicitação XML que é enviada pela API Gerenciada do EWS quando você provisiona um header x usando [a API Gerenciada do EWS.](#bk_example1)
  
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

Na primeira vez que você provisionar um header x no Exchange Online, Exchange Online como parte do Office 365 ou uma versão local do Exchange a partir do Exchange Server 2010, o valor de um novo header x personalizado não será gravado na mensagem armazenada. Isso porque o header x deve primeiro ser mapeado para uma propriedade nomeada na caixa de correio do usuário. O mapeamento ocorre na primeira solicitação para adicionar as propriedades nomeadas. Quando ocorre uma solicitação subsequente para criar a propriedade nomeada, a propriedade e o valor são armazenados na mensagem. No Exchange 2007, na primeira vez que um header x é gravado em um banco de dados de caixa de correio, um mapeamento é criado para o header x para uma propriedade nomeada no banco de dados de caixa de correio. Quando ocorre uma solicitação subsequente para criar a propriedade nomeada, o header x é processado e armazenado para qualquer caixa de correio no banco de dados Exchange 2007.
  
## <a name="next-steps"></a>Próximas etapas
<a name="bk_example1"> </a>

Este artigo mostra como provisionar um header x para uma única caixa de correio enviando um email para um usuário. Você também pode provisionar um header x para muitos usuários enviando um email em lote para uma lista de [destinatários](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md) na organização do chamador. 
  
## <a name="see-also"></a>Confira também


- [Propriedades e propriedades estendidas no EWS no Exchange](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Exchange 2013: Provisionar headers X personalizados programaticamente](https://code.msdn.microsoft.com/exchange/Exchange-2013-Provision-d4ef5719)
    
- [Propriedades nomeadas, X-Headers e Você](https://blogs.technet.com/b/exchange/archive/2009/04/06/3407221.aspx)
    
- [Propriedades nomeadas, Round 2: O que está por vir](https://blogs.technet.com/b/exchange/archive/2009/06/12/3407672.aspx)
    
- [Header Firewall](https://technet.microsoft.com/library/bb232136%28v=exchg.150%29.aspx)
    
- [EWS, MIME e os headers de mensagens da Internet ausentes](https://msdn.microsoft.com/library/office/hh545614%28v=exchg.140%29.aspx)
    
- [Processar mensagens de email em lotes usando o EWS em Exchange](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    

