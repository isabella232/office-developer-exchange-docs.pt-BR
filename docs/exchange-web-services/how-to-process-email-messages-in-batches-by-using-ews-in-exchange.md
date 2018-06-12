---
title: Processar as mensagens de email em lotes, usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 96390f92-cab1-4de6-9ec2-a55678fc20af
description: Saiba como criar, obter, atualizar e excluir os lotes de mensagens de email em uma única chamada usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: 30ebbdf4c92111df629c7662987e301d167336e2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750831"
---
# <a name="process-email-messages-in-batches-by-using-ews-in-exchange"></a>Processar as mensagens de email em lotes, usando o EWS no Exchange

Saiba como criar, obter, atualizar e excluir os lotes de mensagens de email em uma única chamada usando a API gerenciada de EWS ou EWS no Exchange.
  
Você pode usar a API gerenciada de EWS ou torna o EWS para trabalhar com lotes de mensagens de email para reduzir o número de chamadas de um cliente com um servidor Exchange. Quando você usa o EWS Managed API para criar, obter, atualizar, excluir e enviar mensagens em lotes, você usar métodos do objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , enquanto que quando você trabalha com mensagens de email único, você usar os métodos do objeto [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) . Se você estiver usando o EWS, use as mesmas operações para trabalhar com único e de lotes de mensagens de email. 
  
**Tabela 1. Métodos de API gerenciada de EWS e operações de EWS para trabalhar com os lotes de mensagens de email**

|**Para...**|**Use este método API gerenciada de EWS**|**Use esta operação EWS**|
|:-----|:-----|:-----|
|Criar mensagens de email em lotes  <br/> |[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) <br/> |[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|Obter mensagens de email em lotes  <br/> |[ExchangeService.BindToItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|Mensagens de email de atualização em lotes  <br/> |[ExchangeService.UpdateItems](http://msdn.microsoft.com/en-us/library/dd634705%28v=exchg.80%29.aspx) <br/> |[UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Excluir mensagens de email em lotes  <br/> |[ExchangeService.DeleteItems](http://msdn.microsoft.com/en-us/library/dd635460%28v=exchg.80%29.aspx) <br/> |[DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
   
Neste artigo, você aprenderá como concluir as tarefas básicas para lotes de mensagens de email usando o EWS Managed API ou o EWS.
  
## <a name="create-email-messages-in-batches-by-using-the-ews-managed-api"></a>Criar mensagens de email em lotes, usando a API gerenciada de EWS
<a name="bk_createewsma"> </a>

Você pode criar mensagens em lotes, usando o método API gerenciada de EWS **CreateItems** , conforme mostrado no exemplo a seguir. Este exemplo cria três objetos [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) localmente, adiciona a cada mensagem a uma coleção e chama o método **CreateItems** na coleção de mensagens. 
  
Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange. 
  
```cs
public static Collection<ItemId> CreateDraftEmailInBatch(ExchangeService service)
{
    // These are unsaved local instances of an EmailMessage object.
    // Despite the required parameter of an ExchangeService object (service), no call
    // to an Exchange server is made when the objects are instantiated.
    // A call to the Exchange server is made when the service.CreateItems() method is called.
    EmailMessage message1 = new EmailMessage(service);
    EmailMessage message2 = new EmailMessage(service);
    EmailMessage message3 = new EmailMessage(service);
    // Set the properties on the first message.
    message1.Subject = "Project priorities";
    message1.Body = "(1) Buy pizza, (2) Eat pizza";
    message1.ToRecipients.Add("sadie@contoso.com");
    // Set the properties on the second message.
    message2.Subject = "Company Soccer Team";
    message2.Body = "Are you interested in joining?";
    message2.ToRecipients.Add("magdalena@contoso.com");
    // Set the properties on the third message.
    message3.Subject = "Code Blast";
    message3.Body = "Are you interested in getting together to finish the methods for the ContosoLive project?";
    message3.ToRecipients.Add("mack@contoso.com");
    // Add the EmailMessage objects to a collection.
    Collection<EmailMessage> messageItems = new Collection<EmailMessage>() { message1, message2, message3 };
    // Create the batch of email messages on the server.
    // This method call results in an CreateItem call to EWS.
    ServiceResponseCollection<ServiceResponse> response = service.CreateItems(messageItems, WellKnownFolderName.Drafts, MessageDisposition.SaveOnly, null);
    // Instantiate a collection of item IDs to populate from the values that are returned by the Exchange server.
    Collection<ItemId> itemIds = new Collection<ItemId>();
    // Collect the item IDs from the created email messages.
    foreach (EmailMessage message in messageItems)
    {
        try
        {
            itemIds.Add(message.Id);
            Console.WriteLine("Email message '{0}' created successfully.", message.Subject);
        }
        catch (Exception ex)
        {
            // Print out the exception and the last eight characters of the item ID.
            Console.WriteLine("Exception while creating message {0}: {1}", message.Id.ToString().Substring(144), ex.Message);
        }
    }
    // Check for success of the CreateItems method call.
    if (response.OverallResult == ServiceResult.Success)
    {
            Console.WriteLine("All locally created messages were successfully saved to the Drafts folder.");
            Console.WriteLine("\r\n");
    }
   
    // If the method did not return success, print the result message for each email.
    else
    {
        int counter = 1;
        foreach (ServiceResponse resp in response)
        {
            // Print out the result and the last eight characters of the item ID.
            Console.WriteLine("Result (message {0}), id {1}: {2}", counter, itemIds[counter - 1].ToString().Substring(144), resp.Result);
            Console.WriteLine("Error Code: {0}", resp.ErrorCode);
            Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
            Console.WriteLine("\r\n");
            counter++;
        }
    }
    return itemIds;
}
```

Observe que o exemplo a salvará somente as mensagens na pasta Rascunhos; ele não envia as mensagens. Para obter mais informações sobre como enviar as mensagens, consulte [Enviar mensagens de email em lotes, usando a API gerenciada de EWS](#bk_sendewsma).
  
## <a name="create-email-messages-in-batches-by-using-ews"></a>Criar mensagens de email em lotes, usando o EWS
<a name="bk_createews"> </a>

Você pode criar mensagens de email em lotes, usando a operação [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS, conforme mostrado no exemplo de código a seguir. Isso também é a solicitação XML que o EWS Managed API envia quando você usar a API gerenciada de EWS para [criar mensagens de email em lotes](#bk_createewsma). 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
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
              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
        <t:Message>
          <t:Subject>Company Soccer Team</t:Subject>
          <t:Body BodyType="HTML">Are you interested in joining?</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>magdalena@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
        <t:Message>
          <t:Subject>Code Blast</t:Subject>
          <t:Body BodyType="HTML">Are you interested in getting together to finish the methods for the ContosoLive project?</t:Body>
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

O servidor responde à solicitação **CreateItem** com uma mensagem de [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError** para cada uma das novas mensagens, que indica que cada email foi criada e salva com êxito . 
  
Observe que o exemplo a salvará somente as mensagens na pasta Rascunhos; ele não envia as mensagens. Para obter mais informações sobre como enviar as mensagens, consulte [Enviar mensagens de email em lotes, usando o EWS](#bk_sendews).
  
## <a name="send-email-messages-in-batches-by-using-the-ews-managed-api"></a>Enviar mensagens de email em lotes, usando a API gerenciada de EWS
<a name="bk_sendewsma"> </a>

Você pode usar o mesmo código para enviar emails em lotes que você usa para criar mensagens de email em lotes, exceto pelo fato de alguns dos parâmetros do método [CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) alterar. Assim, para enviar mensagens de email usando a API gerenciada de EWS, use o código que você usa para [criar mensagens de email em lotes](#bk_createewsma)e substitua a chamada para o método **CreateItems** a chamada no exemplo a seguir. Neste exemplo, as mensagens são criadas na pasta Itens enviados, e a disposição de mensagem é alterada para [MessageDisposition.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.messagedisposition%28v=exchg.80%29.aspx), para que a mensagem é enviada e não apenas salvo localmente.
  
```cs
// Create and send the batch of email messages on the server.
// This method call results in an CreateItem call to EWS.
ServiceResponseCollection<ServiceResponse> response = service.CreateItems(messageItems, WellKnownFolderName.SentItems, MessageDisposition.SendAndSaveCopy, null);
```

## <a name="send-email-messages-in-batches-by-using-ews"></a>Enviar mensagens de email em lotes, usando o EWS
<a name="bk_sendews"> </a>

Você pode usar o mesmo código para enviar emails em lotes que você use para criar mensagens de email em lotes, exceto pelo fato de alguns dos valores de atributo alterar para a operação **CreateItem** . Assim, para enviar mensagens de email usando o EWS, use o código que você usa para [criar a mensagem de email em lotes](#bk_createews)e altere o valor de **MessageDisposition** para "SendAndSaveCopy" e altere o [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) para "itens enviados", conforme mostrado no exemplo de código a seguir. 
  
```XML
<m:CreateItem MessageDisposition="SendAndSaveCopy">
  <m:SavedItemFolderId>
    <t:DistinguishedFolderId Id="sentitems" />
  </m:SavedItemFolderId>
```

O servidor responde à solicitação **CreateItem** com uma mensagem de [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError** para cada uma das novas mensagens, que indica que cada email foi criado e enviado com êxito. 
  
## <a name="get-email-messages-in-batches-by-using-the-ews-managed-api"></a>Obter mensagens de email em lotes, usando a API gerenciada de EWS
<a name="bk_getewsma"> </a>

Você pode obter mensagens de email em lotes, usando o método API gerenciada de EWS [BindToItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) , conforme mostrado no exemplo a seguir. 
  
Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange. 
  
```cs
public static Collection<EmailMessage> BatchGetEmailItems(ExchangeService service, Collection<ItemId> itemIds)
{
    // Create a property set that limits the properties returned by the Bind method to only those that are required.
    PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, EmailMessageSchema.Subject, EmailMessageSchema.ToRecipients);
    // Get the items from the server.
    // This method call results in a GetItem call to EWS.
    ServiceResponseCollection<GetItemResponse> response = service.BindToItems(itemIds, propSet);
           
    // Instantiate a collection of EmailMessage objects to populate from the values that are returned by the Exchange server.
    Collection<EmailMessage> messageItems = new Collection<EmailMessage>();
    foreach (GetItemResponse getItemResponse in response)
    {
        try
        {
            Item item = getItemResponse.Item;
            EmailMessage message = (EmailMessage)item;
            messageItems.Add(message);
            // Print out confirmation and the last eight characters of the item ID.
            Console.WriteLine("Found item {0}.", message.Id.ToString().Substring(144));
        }
        catch (Exception ex)
        {
           Console.WriteLine("Exception while getting a message: {0}", ex.Message);
        }
    }
    // Check for success of the BindToItems method call.
    if (response.OverallResult == ServiceResult.Success)
    {
        Console.WriteLine("All email messages retrieved successfully.");
        Console.WriteLine("\r\n");
    }
        return messageItems;
}
```

## <a name="get-email-messages-in-batches-by-using-ews"></a>Obter mensagens de email em lotes, usando o EWS
<a name="bk_getews"> </a>

Você pode obter mensagens de email em lotes, usando a operação de EWS [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) e o código no exemplo a seguir. Isso também é a solicitação XML que o EWS Managed API envia quando você usar a API gerenciada de EWS para [obter as mensagens de email em lotes](#bk_getewsma). 
  
Os atributos **ItemId** e **ChangeKey** foram diminuídos para melhorar a legibilidade. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="message:ToRecipients" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="m4NxAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKB0" />
        <t:ItemId Id="m4NyAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKB1" />
        <t:ItemId Id="m4NzAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKB2" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **GetItem** com uma mensagem de [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) que inclui as [Propriedades de primeira classe](email-properties-and-elements-in-ews-in-exchange.md) para cada uma das mensagens solicitadas. 
  
## <a name="update-email-messages-in-batches-by-using-the-ews-managed-api"></a>Mensagens de email de atualização em lotes, usando a API gerenciada de EWS
<a name="bk_updateewsma"> </a>

Você pode obter mensagens de email em lotes, usando o método API gerenciada de EWS [UpdateItems](http://msdn.microsoft.com/en-us/library/dd634705%28v=exchg.80%29.aspx) , conforme mostrado no exemplo a seguir. 
  
Para obter uma lista das propriedades de mensagem de email gravável, consulte [Email propriedades e os elementos no EWS no Exchange](email-properties-and-elements-in-ews-in-exchange.md).
  
Para obter detalhes sobre como enviar uma mensagem de rascunho após ele ser atualizado, consulte o [envio de mensagens de email usando a API gerenciada de EWS](#bk_sendewsma).
  
Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange. 
  
```cs
public static Collection<EmailMessage> BatchUpdateEmailItems(ExchangeService service, Collection<EmailMessage> messageItems)
{
    // Update the subject of each message locally.
    foreach (EmailMessage message in messageItems)
    {
        // Update the Subject of the email.
        message.Subject = "Updated subject at " + DateTime.Now;
        // Print out confirmation with the last eight characters of the item ID and the email subject.
        Console.WriteLine("Updated local email message {0} with the subject '{1}'.", message.Id.ToString().Substring(144), message.Subject);
    }
    // Send the item updates to the server.
    // This method call results in an UpdateItem call to EWS.
    ServiceResponseCollection<UpdateItemResponse> response = service.UpdateItems(messageItems, WellKnownFolderName.Drafts, ConflictResolutionMode.AutoResolve, MessageDisposition.SaveOnly, null);
    // Check for success of the UpdateItems method call.
    if (response.OverallResult == ServiceResult.Success)
    {
        Console.WriteLine("All email messages updated successfully.\r\n");
    }
    // If the method did not return success, print the result message for each email.
    else
    {
        Console.WriteLine("All emails were not successfully saved on the server.\r\n");
        int counter = 1;
        foreach (ServiceResponse resp in response)
        {
            Console.WriteLine("Result for (message {0}): {1}", counter, resp.Result);
            Console.WriteLine("Error Code: {0}", resp.ErrorCode);
            Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
            counter++;
        }
    }
    return messageItems;
}    
```

## <a name="update-email-messages-in-batches-by-using-ews"></a>Mensagens de email de atualização em lotes, usando o EWS
<a name="bk_updateews"> </a>

Você pode atualizar as mensagens de email em lotes, usando a operação [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS, conforme mostrado no exemplo de código a seguir. Isso também é a solicitação XML que o EWS Managed API envia quando você usar a API gerenciada de EWS para [atualizar as mensagens de email em lotes](#bk_updateewsma).
  
Para obter uma lista de elementos de mensagem de email gravável, consulte [Email propriedades e os elementos no EWS no Exchange](email-properties-and-elements-in-ews-in-exchange.md).
  
Para obter detalhes sobre como enviar uma mensagem de rascunho após ele ser atualizado, consulte [Enviar uma mensagem de email usando o EWS rascunho](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateItem MessageDisposition="SaveOnly"
                  ConflictResolution="AutoResolve">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts" />
      </m:SavedItemFolderId>
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="m4OVAAA="
                    ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKCy" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:Message>
                <t:Subject>Updated subject at 1/17/2014 2:58:09 PM</t:Subject>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
        <t:ItemChange>
          <t:ItemId Id="m4OWAAA="
                    ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKCz" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:Message>
                <t:Subject>Updated subject at 1/17/2014 2:58:09 PM</t:Subject>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
        <t:ItemChange>
          <t:ItemId Id="m4OXAAA="
                    ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKC0" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:Message>
                <t:Subject>Updated subject at 1/17/2014 2:58:09 PM</t:Subject>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **UpdateItem** com uma mensagem de [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que cada uma das atualizações foi salvo com êxito no servidor. Todos os conflitos são relatados no elemento [ConflictResult](http://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) . 
  
## <a name="delete-email-messages-in-batches-by-using-the-ews-managed-api"></a>Excluir mensagens de email em lotes usando a API gerenciada de EWS
<a name="bk_deleteewsma"> </a>

Você pode excluir mensagens em lotes, usando o método API gerenciada de EWS [DeleteItems](http://msdn.microsoft.com/en-us/library/dd635460%28v=exchg.80%29.aspx) , conforme mostrado no exemplo a seguir. 
  
Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange. 
  
```cs
public static void BatchDeleteEmailItems(ExchangeService service, Collection<ItemId> itemIds)
{
    // Delete the batch of email message objects.
    // This method call results in an DeleteItem call to EWS.
    ServiceResponseCollection<ServiceResponse> response = service.DeleteItems(itemIds, DeleteMode.SoftDelete, null, AffectedTaskOccurrence.AllOccurrences);
    
    // Check for success of the DeleteItems method call.
    // DeleteItems returns success even if it does not find all the item IDs.
    if (response.OverallResult == ServiceResult.Success)
    {
        Console.WriteLine("Email messages deleted successfully.\r\n");
    }
    // If the method did not return success, print a message.
    else
    {
        Console.WriteLine("Not all email messages deleted successfully.\r\n");
    }
}
```

## <a name="delete-email-messages-in-batches-by-using-ews"></a>Excluir mensagens de email em lotes, usando o EWS
<a name="bk_deleteews"> </a>

Você pode excluir mensagens de email em lotes, usando a operação [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) EWS, conforme mostrado no exemplo de código a seguir. Isso também é a solicitação XML que o EWS Managed API envia quando você usar a API gerenciada de EWS para [Excluir mensagens de email em lotes](#bk_deleteewsma).
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:DeleteItem DeleteType="SoftDelete"
                  AffectedTaskOccurrences="AllOccurrences">
      <m:ItemIds>
        <t:ItemId Id="m4OkAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKDE" />
        <t:ItemId Id="m4OlAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKDF" />
        <t:ItemId Id="m4OmAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKDG" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **DeleteItem** com uma mensagem de [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError** para cada item que foi removido. Observe que a operação também retorna sucesso se a ID do item não pôde ser encontrada. 
  
## <a name="verifying-that-a-batch-process-completed-successfully"></a>Verificando se um processo em lote foi concluída com êxito
<a name="bk_successful"> </a>

Quando uma ou mais mensagens de email em uma solicitação de lote não podem ser processadas, conforme solicitado, um erro será retornado para cada mensagem de email que falharam e o restante de emails no lote são processadas conforme o esperado. Falhas no processamento em lotes podem ocorrer se o item foi excluído e, portanto, não pode ser enviado, recuperado ou atualizado, ou se o item movido para uma pasta diferente e, portanto, tem uma nova ID de item e não pode ser modificado com a ID de item enviada. As informações nesta seção mostram como obter os detalhes de erro sobre falhas no processamento em lotes da mensagem de email.
  
Para verificar o sucesso de um processo em lote usando a API gerenciada de EWS, você pode verificar se a propriedade [OverallResult](http://msdn.microsoft.com/en-us/library/dd634515%28v=exchg.80%29.aspx) do [ServiceResponseCollection](http://msdn.microsoft.com/en-us/library/dd633715%28v=exchg.80%29.aspx) for igual a [ServiceResult.Success](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx). Nesse caso, todos os emails foram processados com êxito. Se o **OverallResult** não for igual a **ServiceResult.Success**, um ou mais os emails existentes não foram processadas com êxito. Cada um dos objetos retornados no **ServiceResponseCollection** contém as seguintes propriedades: 
  
- [ErrorCode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx)
    
- [ErrorDetails](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx)
    
- [ErrorMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx)
    
- [ErrorProperties](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx)
    
- [Resultado](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx)
    
Essas propriedades contêm informações sobre por que as mensagens de email não pôde ser processadas conforme solicitado. Os exemplos neste artigo imprimam o **resultado**, **ErrorCode**e **ErrorMessage** para cada mensagem com falha. Você pode usar estes resultados para investigar o problema. 
  
Para o EWS, para verificar o sucesso de um processo em lote, verifique o atributo [ResponseClass](http://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) para cada item que estão sendo processada. Veja a seguir a estrutura básica do **ResponseMessageType**, o tipo de base da resposta que todas as mensagens são derivadas. 
  
```XML
<ResponseMessage ResponseClass="Success | Warning | Error">
            <MessageText/>
            <ResponseCode/>
            <DescriptiveLinkKey/>
            <MessageXml/>
</ResponseMessage>
```

O atributo **ResponseClass** é definido como **sucesso** se o email foi processado com êxito, ou **erro** se o email não foi processado com êxito. Para mensagens de email, você não encontrará um **Aviso** durante o processamento em lotes. Se o **ResponseClass** for **sucesso**, o elemento [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) que segue também sempre é definido como **NoError**. Se a **ResponseClass** **erro**, você precisará verificar os valores dos elementos [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **ResponseCode**e [MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) para determinar o que causou o problema. [DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) não é usada no momento. 
  
## <a name="see-also"></a>Confira também


- [Email e EWS no Exchange](email-and-ews-in-exchange.md)
    
- [Enviar mensagens de email usando o EWS no Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md)
    
- [Responder às mensagens de email usando o EWS no Exchange](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)
    
- [Mover e copiar mensagens de email usando o EWS no Exchange](how-to-move-and-copy-email-messages-by-using-ews-in-exchange.md)
    
- [Limitação implicações para solicitações de lote EWS](ews-throttling-in-exchange.md#bk_ThrottlingBatch)
    

