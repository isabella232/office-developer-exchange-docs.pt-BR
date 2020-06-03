---
title: Email e EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 4d7bdb37-f7f1-409f-9749-f8bcde7dc52a
description: Descubra como trabalhar com mensagens de email, incluindo como criar um email e como realizar outras tarefas relacionadas a email usando a API gerenciada do EWS ou o EWS no Exchange.
localization_priority: Priority
ms.openlocfilehash: 323d9d2cc40aa86044a439ad53e53a4808916783
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455440"
---
# <a name="email-and-ews-in-exchange"></a>Email e EWS no Exchange

Descubra como trabalhar com mensagens de email, incluindo como criar um email e como realizar outras tarefas relacionadas a email usando a API gerenciada do EWS ou o EWS no Exchange.
  

  
Em seu núcleo, o Exchange é sobre email. Mas o que torna um email um email? Bem, as mensagens de email são um dos [itens fortemente tipados](folders-and-items-in-ews-in-exchange.md#bk_item) no Exchange, o que significa que eles contêm um [conjunto específico de propriedades](email-properties-and-elements-in-ews-in-exchange.md), mesmo antes de serem enviados. As mensagens de email são representadas pela classe [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) na API gerenciada do EWS e pelo elemento [Message](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) e seus elementos filhos no EWS. 
  
Na API gerenciada do EWS, o objeto **EmailMessage** deriva do objeto [Item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) . A classe **EmailMessage** estende a classe de **Item** fornecendo propriedades adicionais como [EmailMessage. Sender](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.sender%28v=exchg.80%29.aspx) e [EmailMessage. IsRead](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.isread%28v=exchg.80%29.aspx), que agora são comuns a praticamente todos os cenários de mensagens. Ao obter, atualizar ou excluir uma mensagem de email, na maioria dos casos, você pode fazer isso usando o objeto **EmailMessage** [ou o objeto](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemschema%28v=exchg.80%29.aspx) de item base, dependendo se as propriedades com as quais você está trabalhando estão no [EmailMessageSchema](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessageschema%28v=exchg.80%29.aspx) ou na classe **PostItem** . A criação do item é diferente porque a classe de **Item** não tem um construtor, portanto, quando você estiver criando um email, você usará o [Construtor EmailMessage](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) para criá-lo e os métodos [EmailMessage. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) ou [EmailMessage. SendAndSaveCopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) para salvá-lo ou enviá-lo e salvá-lo. 
  
Da mesma forma, no EWS, use a operação [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) com o elemento [Message](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) para criar uma mensagem de email. Para obter, atualizar ou excluir emails usando o EWS, o fato de que o item que está sendo modificado é uma mensagem de email não é importante, além do fato de que as propriedades adicionais estão disponíveis em mensagens de email. As mesmas operações que são usadas para outros itens com rigidez de tipos também são usadas para mensagens de email. 
  
|**Tarefa**|**Método de API gerenciada do EWS**|**Operação do EWS**|
|:-----|:-----|:-----|
|Criar  <br/> |[EmailMessage. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) <br/> |[CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|Obter  <br/> |[EmailMessage. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|Atualizar  <br/> |[Item. Update](https://msdn.microsoft.com/library/dd635915%28v=exchg.80%29.aspx) <br/> |[UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Excluir  <br/> |[Item. Delete](https://msdn.microsoft.com/library/dd635072%28v=exchg.80%29.aspx) <br/> |[DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
   
Como as mensagens de email são simplesmente [itens fortemente tipados](folders-and-items-in-ews-in-exchange.md#bk_item), em alguns casos, você trabalha com eles da mesma maneira que você [trabalha com itens genéricos](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md). 
  
## <a name="create-an-email-message-by-using-the-ews-managed-api"></a>Criar uma mensagem de email usando a API gerenciada do EWS
<a name="bk_createewsma"> </a>

Você pode criar uma mensagem de email usando o método [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) de API gerenciada do EWS, conforme mostrado no código no exemplo a seguir. Observe que o exemplo salva apenas a mensagem na pasta Rascunhos, ela não envia a mensagem. Para obter informações sobre como enviar a mensagem ou criar e enviar a mensagem em uma única etapa, consulte [enviar mensagens de email usando o EWS no Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md).
  
Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange. 
  
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

Você pode criar uma mensagem de email usando a operação EWS [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) , conforme mostrado no exemplo a seguir. Essa é também a solicitação XML que a API gerenciada do EWS envia quando você [cria uma mensagem de email](#bk_createewsma). Observe que o exemplo a seguir apenas salva a mensagem na pasta Rascunhos, ela não envia a mensagem. Para obter informações sobre como enviar a mensagem ou criar e enviar a mensagem em um Ste, consulte [enviar mensagens de email usando o EWS no Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

O servidor responde à solicitação **CreateItem** com uma mensagem [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que o email foi criado com êxito e o [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) da mensagem recém-criada. 
  
## <a name="get-update-and-delete-an-email-message-by-using-the-ews-managed-api"></a>Obter, atualizar e excluir uma mensagem de email usando a API gerenciada do EWS
<a name="bk_getewsma"> </a>

Você pode usar a API gerenciada do EWS para obter, atualizar ou excluir uma mensagem de email da mesma maneira que executará essas ações em qualquer item genérico do repositório do Exchange. Para obter mais informações, consulte [trabalhar com itens de caixa de correio do Exchange usando o EWS no Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md).
  
Se você estiver atualizando uma mensagem de email, consulte [Propriedades e elementos de email no EWS no Exchange](email-properties-and-elements-in-ews-in-exchange.md) para obter uma lista de propriedades de mensagens de email graváveis. Para enviar uma mensagem de rascunho após tê-la atualizado, confira [Enviar uma mensagem de email de rascunho usando a API gerenciada do EWS](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftewsma).
  
## <a name="get-update-and-delete-an-email-message-by-using-ews"></a>Obter, atualizar e excluir uma mensagem de email usando o EWS
<a name="bk_getews"> </a>

Você pode usar o EWS para obter, atualizar e excluir uma mensagem de email da mesma forma que executa essas ações em qualquer item genérico do repositório do Exchange. Para obter mais informações, consulte [trabalhar com itens de caixa de correio do Exchange usando o EWS no Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md).
  
Se você estiver atualizando uma mensagem de email, consulte [Propriedades e elementos de email no EWS no Exchange](email-properties-and-elements-in-ews-in-exchange.md) para obter uma lista de propriedades de mensagens de email graváveis. Para enviar uma mensagem de rascunho após tê-la atualizado, confira [Enviar uma mensagem de email de rascunho usando EWS](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews).
  
## <a name="in-this-section"></a>Nesta seção
<a name="bk_inthissection"> </a>

- [Propriedades e elementos de email no EWS no Exchange](email-properties-and-elements-in-ews-in-exchange.md)
    
- [Enviar mensagens de email usando o EWS no Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md)
    
- [Responder a mensagens de email usando o EWS no Exchange](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)
    
- [Mover e copiar mensagens de email usando o EWS no Exchange](how-to-move-and-copy-email-messages-by-using-ews-in-exchange.md)
    
- [Trabalhar com conversas usando o EWS no Exchange](how-to-work-with-conversations-by-using-ews-in-exchange.md)
    
- [Extrair uma entidade de uma mensagem de email usando o EWS no Exchange](how-to-extract-an-entity-from-an-email-message-by-using-ews-in-exchange.md)
    
- [Processar mensagens de email em lotes usando o EWS no Exchange](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>Confira também


- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    
- [Pastas e itens no EWS no Exchange](folders-and-items-in-ews-in-exchange.md)
    

