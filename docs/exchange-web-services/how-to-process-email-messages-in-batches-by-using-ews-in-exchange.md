---
title: Processar mensagens de email em lotes usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: 96390f92-cab1-4de6-9ec2-a55678fc20af
description: Saiba como criar, obter, atualizar e excluir lotes de mensagens de email em uma única chamada usando a API gerenciada do EWS ou o EWS no Exchange.
localization_priority: Priority
ms.openlocfilehash: 2592076c9c5b57356d96872f006dd7b0abfc328a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527772"
---
# <a name="process-email-messages-in-batches-by-using-ews-in-exchange"></a>Processar mensagens de email em lotes usando o EWS no Exchange

Saiba como criar, obter, atualizar e excluir lotes de mensagens de email em uma única chamada usando a API gerenciada do EWS ou o EWS no Exchange.

Você pode usar a API gerenciada do EWS ou o EWS para trabalhar com lotes de mensagens de email para reduzir o número de chamadas feitas por um cliente para um servidor Exchange. Ao usar a API gerenciada do EWS para criar, obter, atualizar, excluir e enviar mensagens em lotes, use os métodos de objeto do [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , enquanto quando você trabalha com mensagens de email únicas, usa métodos de objeto do [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) . Se você estiver usando o EWS, use as mesmas operações para trabalhar com um único e lotes de mensagens de email.

**Tabela 1. Métodos da API gerenciada do EWS e operações do EWS para trabalhar com lotes de mensagens de email**

|**Para...**|**Usar este método de API gerenciada do EWS**|**Use esta operação do EWS**|
|:-----|:-----|:-----|
|Criar mensagens de email em lotes  <br/> |[ExchangeService. CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) <br/> |[CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|Obter mensagens de email em lotes  <br/> |[ExchangeService. BindToItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|Atualizar mensagens de email em lotes  <br/> |[ExchangeService. UpdateItems](https://msdn.microsoft.com/library/dd634705%28v=exchg.80%29.aspx) <br/> |[UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Excluir mensagens de email em lotes  <br/> |[ExchangeService. DeleteItems](https://msdn.microsoft.com/library/dd635460%28v=exchg.80%29.aspx) <br/> |[DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |

Neste artigo, você aprenderá a concluir tarefas básicas para lotes de mensagens de email usando a API gerenciada do EWS ou o EWS.

## <a name="create-email-messages-in-batches-by-using-the-ews-managed-api"></a>Criar mensagens de email em lotes usando a API gerenciada do EWS
<a name="bk_createewsma"> </a>

Você pode criar mensagens em lotes usando o método **CreateItems** da API gerenciada do EWS, conforme mostrado no exemplo a seguir. Este exemplo cria três objetos [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) localmente, adiciona cada mensagem a uma coleção e, em seguida, chama o método **CreateItems** na coleção de mensagens.

Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange.

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

Observe que o exemplo salva apenas as mensagens na pasta Rascunhos; Ele não envia as mensagens. Para saber mais sobre como enviar as mensagens, confira [enviar mensagens de email em lotes usando a API gerenciada do EWS](#bk_sendewsma).

## <a name="create-email-messages-in-batches-by-using-ews"></a>Criar mensagens de email em lotes usando o EWS
<a name="bk_createews"> </a>

Você pode criar mensagens de email em lotes usando a operação [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS, conforme mostrado no exemplo de código a seguir. Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa a API gerenciada do EWS para [criar mensagens de email em lotes](#bk_createewsma).

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

O servidor responde à solicitação **CreateItem** com uma mensagem [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR** para cada uma das novas mensagens, o que indica que cada email foi criado e salvo com êxito.

Observe que o exemplo salva apenas as mensagens na pasta Rascunhos; Ele não envia as mensagens. Para saber mais sobre como enviar as mensagens, confira [enviar mensagens de email em lotes usando o EWS](#bk_sendews).

## <a name="send-email-messages-in-batches-by-using-the-ews-managed-api"></a>Enviar mensagens de email em lotes usando a API gerenciada do EWS
<a name="bk_sendewsma"> </a>

Você usa o mesmo código para enviar mensagens de email em lotes que você usa para criar mensagens de email em lotes, exceto pelo fato de que alguns dos parâmetros do método [CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) mudam. Portanto, para enviar mensagens de email usando a API gerenciada do EWS, use o código que você usa para [criar mensagens de email em lotes](#bk_createewsma)e substitua a chamada para o método **CreateItems** com a chamada no exemplo a seguir. Neste exemplo, as mensagens são criadas na pasta Itens enviados e a disposição da mensagem é alterada para [MessageDisposition. SendAndSaveCopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.messagedisposition%28v=exchg.80%29.aspx), para que a mensagem seja enviada e não seja salva localmente.

```cs
// Create and send the batch of email messages on the server.
// This method call results in an CreateItem call to EWS.
ServiceResponseCollection<ServiceResponse> response = service.CreateItems(messageItems, WellKnownFolderName.SentItems, MessageDisposition.SendAndSaveCopy, null);
```

## <a name="send-email-messages-in-batches-by-using-ews"></a>Enviar mensagens de email em lotes usando o EWS
<a name="bk_sendews"> </a>

Você usa o mesmo código para enviar mensagens de email em lotes que você usa para criar mensagens de email em lotes, exceto pelo fato de que alguns dos valores de atributo são alterados para a operação **CreateItem** . Portanto, para enviar mensagens de email usando o EWS, use o código que você usa para [criar mensagens de email em lotes](#bk_createews)e altere o valor de **MessageDisposition** para "SendAndSaveCopy" e altere o [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) para "itens enviados", conforme mostrado no exemplo de código a seguir.

```XML
<m:CreateItem MessageDisposition="SendAndSaveCopy">
  <m:SavedItemFolderId>
    <t:DistinguishedFolderId Id="sentitems" />
  </m:SavedItemFolderId>
```

O servidor responde à solicitação **CreateItem** com uma mensagem [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR** para cada uma das novas mensagens, o que indica que cada email foi criado e enviado com êxito.

## <a name="get-email-messages-in-batches-by-using-the-ews-managed-api"></a>Obter mensagens de email em lotes usando a API gerenciada do EWS
<a name="bk_getewsma"> </a>

Você pode obter mensagens de email em lotes usando o método [BindToItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) da API gerenciada do EWS, conforme mostrado no exemplo a seguir.

Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange.

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

## <a name="get-email-messages-in-batches-by-using-ews"></a>Obter mensagens de email em lotes usando o EWS
<a name="bk_getews"> </a>

Você pode obter mensagens de email em lotes usando a operação do EWS do [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) e o código no exemplo a seguir. Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa a API gerenciada do EWS para [obter mensagens de email em lotes](#bk_getewsma).

Os atributos **ItemId** e **ChangeKey** foram reduzidos para facilitar a leitura.

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

O servidor responde à solicitação **GetItem** com uma mensagem [GetItemResponse](https://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) que inclui as [Propriedades da primeira classe](email-properties-and-elements-in-ews-in-exchange.md) para cada uma das mensagens solicitadas.

## <a name="update-email-messages-in-batches-by-using-the-ews-managed-api"></a>Atualizar mensagens de email em lotes usando a API gerenciada do EWS
<a name="bk_updateewsma"> </a>

Você pode obter mensagens de email em lotes usando o método [UpdateItems](https://msdn.microsoft.com/library/dd634705%28v=exchg.80%29.aspx) da API gerenciada do EWS, conforme mostrado no exemplo a seguir.

Para obter uma lista de propriedades de mensagens de email graváveis, confira [Propriedades e elementos de email no EWS no Exchange](email-properties-and-elements-in-ews-in-exchange.md).

Para obter detalhes sobre como enviar uma mensagem de rascunho após ela ter sido atualizada, consulte [enviando mensagens de email usando a API gerenciada do EWS](#bk_sendewsma).

Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange.

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

## <a name="update-email-messages-in-batches-by-using-ews"></a>Atualizar mensagens de email em lotes usando o EWS
<a name="bk_updateews"> </a>

Você pode atualizar mensagens de email em lotes usando a operação [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) do EWS, conforme mostrado no exemplo de código a seguir. Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa a API gerenciada do EWS para [Atualizar mensagens de email em lotes](#bk_updateewsma).

Para obter uma lista de elementos de mensagem de email graváveis, confira [Propriedades e elementos de email no EWS no Exchange](email-properties-and-elements-in-ews-in-exchange.md).

Para obter detalhes sobre como enviar uma mensagem de rascunho após ela ter sido atualizada, consulte [Enviar uma mensagem de email de rascunho usando EWS](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews).

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

O servidor responde à solicitação **UpdateItem** com uma mensagem [UpdateItemResponse](https://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) que inclui um valor de [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que cada uma das atualizações foi salva com êxito no servidor. Todos os conflitos são relatados no elemento [ConflictResult](https://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) .

## <a name="delete-email-messages-in-batches-by-using-the-ews-managed-api"></a>Excluir mensagens de email em lotes usando a API gerenciada do EWS
<a name="bk_deleteewsma"> </a>

Você pode excluir mensagens em lotes usando o método [DeleteItems](https://msdn.microsoft.com/library/dd635460%28v=exchg.80%29.aspx) da API gerenciada do EWS, conforme mostrado no exemplo a seguir.

Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange.

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

## <a name="delete-email-messages-in-batches-by-using-ews"></a>Excluir mensagens de email em lotes usando EWS
<a name="bk_deleteews"> </a>

Você pode excluir mensagens de email em lotes usando a operação [DeleteItem](../web-service-reference/deleteitem-operation.md) do EWS, conforme mostrado no exemplo de código a seguir. Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa a API gerenciada do EWS para [excluir mensagens de email em lotes](#bk_deleteewsma).

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

O servidor responde à solicitação **DeleteItem** com uma mensagem [DeleteItemResponse](https://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) que inclui um valor de [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR** para cada item que foi removido. Observe que a operação também retorna êxito se a ID do item não foi encontrada.

## <a name="verifying-that-a-batch-process-completed-successfully"></a>Verificar se um processo em lote foi concluído com êxito
<a name="bk_successful"> </a>

Quando uma ou mais mensagens de email em uma solicitação em lote não puderem ser processadas conforme solicitado, um erro será retornado para cada mensagem de email que falhou e o restante dos emails no lote será processado conforme o esperado. As falhas no processamento em lotes podem ocorrer se o item foi excluído e, portanto, não pode ser enviado, recuperado ou atualizado ou quando o item é movido para uma pasta diferente e, portanto, tem uma nova ID de item e não pode ser modificado com a ID de item enviada. As informações desta seção mostram como obter detalhes de erro sobre falhas no processamento em lotes de mensagens de email.

Para verificar o sucesso de um processo em lote usando a API gerenciada do EWS, você pode verificar se a propriedade [OverallResult](https://msdn.microsoft.com/library/dd634515%28v=exchg.80%29.aspx) de [myresponsecollection](https://msdn.microsoft.com/library/dd633715%28v=exchg.80%29.aspx) é igual a [falha. êxito](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx). Em caso afirmativo, todos os emails foram processados com êxito. Se o **OverallResult** não for igual a **pararesult. Success**, um ou mais emails não foram processados com êxito. Cada um dos objetos retornados em **Naresponsecollection** contém as seguintes propriedades:

- [ErrorCode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx)

- [ErrorDetails](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx)

- [ErrorMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx)

- [Errorproperties](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx)

- [Resultado](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx)

Essas propriedades contêm informações sobre o motivo pelo qual as mensagens de email não puderam ser processadas conforme solicitado. Os exemplos neste artigo imprimem o **resultado**, **ErrorCode**e **ErrorMessage** de cada mensagem com falha. Você pode usar esses resultados para investigar o problema.

Para o EWS, para verificar o sucesso de um processo em lote, verifique o atributo [ResponseClass](https://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) para cada item que está sendo processado. Veja a seguir a estrutura básica do **ResponseMessageType**, o tipo base do qual todas as mensagens de resposta são derivadas.

```XML
<ResponseMessage ResponseClass="Success | Warning | Error">
            <MessageText/>
            <ResponseCode/>
            <DescriptiveLinkKey/>
            <MessageXml/>
</ResponseMessage>
```

O atributo **ResponseClass** é definido como **Success** se o email foi processado com êxito ou **erro** se o email não foi processado com êxito. Para mensagens de email, você não encontrará um **aviso** durante o processamento em lotes. Se o **ResponseClass** for **bem-sucedido**, o elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) que segue também é sempre definido como **NOERROR**. Se o **ResponseClass** for **erro**, você precisa verificar os valores dos elementos [MessageText](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **ResponseCode**e [MessageXml](https://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) para determinar o que causou o problema. [DescriptiveLinkKey](https://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) não está sendo usado.

## <a name="see-also"></a>Confira também


- [Email e EWS no Exchange](email-and-ews-in-exchange.md)

- [Enviar mensagens de email usando o EWS no Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md)

- [Responder a mensagens de email usando o EWS no Exchange](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)

- [Mover e copiar mensagens de email usando o EWS no Exchange](how-to-move-and-copy-email-messages-by-using-ews-in-exchange.md)

- [Limitações de limitação para solicitações de lote do EWS](ews-throttling-in-exchange.md#throttling-implications-for-ews-batch-requests)
