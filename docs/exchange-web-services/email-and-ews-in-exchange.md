---
title: Email e EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 4d7bdb37-f7f1-409f-9749-f8bcde7dc52a
description: Descubra como trabalhar com mensagens de email, incluindo como criar um email e como executar outras tarefas relacionadas ao email usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: 2cd4613635bd2a5ecc061b50b0aecbdde1d32d46
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353669"
---
# <a name="email-and-ews-in-exchange"></a>Email e EWS no Exchange

Descubra como trabalhar com mensagens de email, incluindo como criar um email e como executar outras tarefas relacionadas ao email usando a API gerenciada de EWS ou EWS no Exchange.
  

  
Essencialmente, o Exchange é sobre email. Mas o que torna um email um email? Bem, mensagens de email são um do [fortemente tipadas itens](folders-and-items-in-ews-in-exchange.md#bk_item) no Exchange, que significa que eles contenham um determinado [conjunto de propriedades](email-properties-and-elements-in-ews-in-exchange.md), mesmo antes que eles enviados. Mensagens de email são representadas pela classe [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) na API gerenciada do EWS e o elemento de [mensagem](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) e seus elementos filhos no EWS. 
  
Na API gerenciada do EWS, o objeto **EmailMessage** deriva o objeto de [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) . A classe **EmailMessage** estende a classe de **Item** , fornecendo propriedades adicionais, como [EmailMessage.Sender](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sender%28v=exchg.80%29.aspx) e [EmailMessage.IsRead](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.isread%28v=exchg.80%29.aspx), que agora são comuns a quase todos os cenários de mensagens. Quando você obtiver, atualizem ou excluam uma mensagem de email, na maioria dos casos, que você pode fazer isso usando o objeto **EmailMessage** ou o objeto de **Item** base, dependendo se as propriedades que você está trabalhando no [EmailMessageSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessageschema%28v=exchg.80%29.aspx) ou o [ ItemSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemschema%28v=exchg.80%29.aspx) classe. Criação de item é diferente porque a classe de **Item** não tem um construtor, portanto quando você estiver criando um email, você usará o [Construtor de EmailMessage](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) para criar a ele e o [EmailMessage.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) ou [EmailMessage.SendAndSaveCopy ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx)métodos salvá-lo, ou enviá-la e salvá-lo. 
  
Da mesma forma, no EWS, use a operação [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) com o elemento de [mensagem](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) para criar uma mensagem de email. Para obter, atualizar ou excluir emails usando o EWS, o fato de que o item que está sendo modificado é uma mensagem de email não é importante, com exceção do fato de que as propriedades adicionais estão disponíveis em mensagens de email. As mesmas operações que são usadas para outros itens fortemente tipados também são usadas para mensagens de email. 
  
|**Task**|**Método API gerenciada de EWS**|**Operação do EWS**|
|:-----|:-----|:-----|
|Criar  <br/> |[EmailMessage.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) <br/> |[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|Get  <br/> |[EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|Atualizar  <br/> |[Item.Update](http://msdn.microsoft.com/en-us/library/dd635915%28v=exchg.80%29.aspx) <br/> |[UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Delete  <br/> |[Item](http://msdn.microsoft.com/en-us/library/dd635072%28v=exchg.80%29.aspx) <br/> |[DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
   
Como mensagens de email são simplesmente [fortemente tipadas itens](folders-and-items-in-ews-in-exchange.md#bk_item), em alguns casos você trabalhar com eles da mesma maneira que você [trabalhar com itens genéricos](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md). 
  
## <a name="create-an-email-message-by-using-the-ews-managed-api"></a>Criar uma mensagem de email usando a API gerenciada de EWS
<a name="bk_createewsma"> </a>

Você pode criar uma mensagem de email usando o método EWS Managed API [Salvar](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) , conforme mostrado no código no exemplo a seguir. Observe que o exemplo salva apenas a mensagem na pasta Rascunhos, ele não enviará a mensagem. Para obter informações sobre como enviar a mensagem ou como criar e enviar a mensagem em uma única etapa, consulte [Enviar mensagens de email usando o EWS no Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md).
  
Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange. 
  
```cs
// Create a new email message.
EmailMessage message = new EmailMessage(service);
// Set properties on the email message.
message.ToRecipients.Add("mack@contoso.com");
message.Subject = "Project priorities";
message.Body = "(1) Buy pizza, (2) Eat pizza";
// Save the email message to the Drafts folder (where it can be retrieved, updated, and sent at a later time).
// This method call results in a CreateItem call to EWS.
message.Save(WellKnownFolderName.Drafts);
Console.WriteLine("A draft email message with the subject '" + message.Subject + "' has been saved to the Drafts folder.");
```

## <a name="create-an-email-message-by-using-ews"></a>Criar uma mensagem de email usando o EWS
<a name="bk_createews"> </a>

Você pode criar uma mensagem de email usando a operação de EWS [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) , conforme mostrado no exemplo a seguir. Isso também é a solicitação XML que o EWS Managed API envia quando você [criar uma mensagem de email](#bk_createewsma). Observe que o exemplo a seguir salva apenas a mensagem na pasta Rascunhos, ele não enviará a mensagem. Para obter informações sobre como enviar a mensagem ou como criar e enviar a mensagem em um colar, consulte [Enviar mensagens de email usando o EWS no Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP2" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Project priorities</t:Subject>
          <t:Body BodyType="HTML">(1) Buy pizza, (2) Eat pizza</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>mack@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

O servidor responde à solicitação **CreateItem** com uma mensagem de [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica se o email foi criado com êxito e o [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) do recentemente mensagem criada. 
  
## <a name="get-update-and-delete-an-email-message-by-using-the-ews-managed-api"></a>Obter, atualizar e excluir uma mensagem de email usando a API gerenciada de EWS
<a name="bk_getewsma"> </a>

Você pode usar a API gerenciada de EWS para obter, atualizar ou excluir uma mensagem de email da mesma maneira que você executa essas ações em qualquer item genérica do armazenamento do Exchange. Para obter mais informações, consulte [trabalhar com itens de caixa de correio do Exchange usando o EWS no Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md).
  
Se você estiver atualizando uma mensagem de email, consulte [Email propriedades e os elementos no EWS no Exchange](email-properties-and-elements-in-ews-in-exchange.md) para obter uma lista das propriedades de mensagem de email gravável. Para enviar uma mensagem de rascunho depois que você atualizou-lo, consulte [Enviar uma mensagem de email de rascunho usando a API gerenciada de EWS](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftewsma).
  
## <a name="get-update-and-delete-an-email-message-by-using-ews"></a>Obter, atualizar e excluir uma mensagem de email usando o EWS
<a name="bk_getews"> </a>

Você pode usar o EWS para obter, atualizar e excluir uma mensagem de email da mesma maneira que você executa essas ações em qualquer item genérica do armazenamento do Exchange. Para obter mais informações, consulte [trabalhar com itens de caixa de correio do Exchange usando o EWS no Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md).
  
Se você estiver atualizando uma mensagem de email, consulte [Email propriedades e os elementos no EWS no Exchange](email-properties-and-elements-in-ews-in-exchange.md) para obter uma lista das propriedades de mensagem de email gravável. Para enviar uma mensagem de rascunho depois que você atualizou-lo, consulte [Enviar uma mensagem de email usando o EWS rascunho](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews).
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_inthissection"> </a>

- [Email propriedades e os elementos no EWS no Exchange](email-properties-and-elements-in-ews-in-exchange.md)
    
- [Enviar mensagens de email usando o EWS no Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md)
    
- [Responder às mensagens de email usando o EWS no Exchange](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)
    
- [Mover e copiar mensagens de email usando o EWS no Exchange](how-to-move-and-copy-email-messages-by-using-ews-in-exchange.md)
    
- [Trabalhar com conversas usando o EWS no Exchange](how-to-work-with-conversations-by-using-ews-in-exchange.md)
    
- [Extrair uma entidade de uma mensagem de email usando o EWS no Exchange](how-to-extract-an-entity-from-an-email-message-by-using-ews-in-exchange.md)
    
- [Processar as mensagens de email em lotes, usando o EWS no Exchange](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também


- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Pastas e itens no EWS no Exchange](folders-and-items-in-ews-in-exchange.md)
    

