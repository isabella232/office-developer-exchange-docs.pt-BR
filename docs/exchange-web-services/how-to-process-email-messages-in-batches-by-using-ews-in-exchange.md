---
title: Processar as mensagens de email em lotes, usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 96390f92-cab1-4de6-9ec2-a55678fc20af
description: Saiba como criar, obter, atualizar e excluir os lotes de mensagens de email em uma única chamada usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: b7dcc8f0961a34061b0476e2136193bf21731d99
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354040"
---
# <a name="process-email-messages-in-batches-by-using-ews-in-exchange"></a><span data-ttu-id="be893-103">Processar as mensagens de email em lotes, usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="be893-103">Process email messages in batches by using EWS in Exchange</span></span>

<span data-ttu-id="be893-104">Saiba como criar, obter, atualizar e excluir os lotes de mensagens de email em uma única chamada usando a API gerenciada de EWS ou EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="be893-104">Learn how to create, get, update, and delete batches of email messages in a single call by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="be893-105">Você pode usar a API gerenciada de EWS ou torna o EWS para trabalhar com lotes de mensagens de email para reduzir o número de chamadas de um cliente com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="be893-105">You can use the EWS Managed API or EWS to work with batches of email messages to reduce the number of calls a client makes to an Exchange server.</span></span> <span data-ttu-id="be893-106">Quando você usa o EWS Managed API para criar, obter, atualizar, excluir e enviar mensagens em lotes, você usar métodos do objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , enquanto que quando você trabalha com mensagens de email único, você usar os métodos do objeto [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="be893-106">When you use the EWS Managed API to create, get, update, delete, and send messages in batches, you use [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object methods, whereas when you work with single email messages, you use [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object methods.</span></span> <span data-ttu-id="be893-107">Se você estiver usando o EWS, use as mesmas operações para trabalhar com único e de lotes de mensagens de email.</span><span class="sxs-lookup"><span data-stu-id="be893-107">If you are using EWS, you use the same operations to work with both single and batches of email messages.</span></span> 
  
<span data-ttu-id="be893-108">**Tabela 1. Métodos de API gerenciada de EWS e operações de EWS para trabalhar com os lotes de mensagens de email**</span><span class="sxs-lookup"><span data-stu-id="be893-108">**Table 1. EWS Managed API methods and EWS operations for working with batches of email messages**</span></span>

|<span data-ttu-id="be893-109">**Para...**</span><span class="sxs-lookup"><span data-stu-id="be893-109">**In order to…**</span></span>|<span data-ttu-id="be893-110">**Use este método API gerenciada de EWS**</span><span class="sxs-lookup"><span data-stu-id="be893-110">**Use this EWS Managed API method**</span></span>|<span data-ttu-id="be893-111">**Use esta operação EWS**</span><span class="sxs-lookup"><span data-stu-id="be893-111">**Use this EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="be893-112">Criar mensagens de email em lotes</span><span class="sxs-lookup"><span data-stu-id="be893-112">Create email messages in batches</span></span>  <br/> |[<span data-ttu-id="be893-113">ExchangeService.CreateItems</span><span class="sxs-lookup"><span data-stu-id="be893-113">ExchangeService.CreateItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="be893-114">CreateItem</span><span class="sxs-lookup"><span data-stu-id="be893-114">CreateItem</span></span>](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="be893-115">Obter mensagens de email em lotes</span><span class="sxs-lookup"><span data-stu-id="be893-115">Get email messages in batches</span></span>  <br/> |[<span data-ttu-id="be893-116">ExchangeService.BindToItems</span><span class="sxs-lookup"><span data-stu-id="be893-116">ExchangeService.BindToItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="be893-117">GetItem</span><span class="sxs-lookup"><span data-stu-id="be893-117">GetItem</span></span>](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="be893-118">Mensagens de email de atualização em lotes</span><span class="sxs-lookup"><span data-stu-id="be893-118">Update email messages in batches</span></span>  <br/> |[<span data-ttu-id="be893-119">ExchangeService.UpdateItems</span><span class="sxs-lookup"><span data-stu-id="be893-119">ExchangeService.UpdateItems</span></span>](http://msdn.microsoft.com/en-us/library/dd634705%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="be893-120">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="be893-120">UpdateItem</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="be893-121">Excluir mensagens de email em lotes</span><span class="sxs-lookup"><span data-stu-id="be893-121">Delete email messages in batches</span></span>  <br/> |[<span data-ttu-id="be893-122">ExchangeService.DeleteItems</span><span class="sxs-lookup"><span data-stu-id="be893-122">ExchangeService.DeleteItems</span></span>](http://msdn.microsoft.com/en-us/library/dd635460%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="be893-123">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="be893-123">DeleteItem</span></span>](../web-service-reference/deleteitem-operation.md) <br/> |
   
<span data-ttu-id="be893-124">Neste artigo, você aprenderá como concluir as tarefas básicas para lotes de mensagens de email usando o EWS Managed API ou o EWS.</span><span class="sxs-lookup"><span data-stu-id="be893-124">In this article, you'll learn how to complete basic tasks for batches of email messages by using the EWS Managed API or EWS.</span></span>
  
## <a name="create-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="be893-125">Criar mensagens de email em lotes, usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="be893-125">Create email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="be893-126"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="be893-126"></span></span>

<span data-ttu-id="be893-127">Você pode criar mensagens em lotes, usando o método API gerenciada de EWS **CreateItems** , conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="be893-127">You can create messages in batches by using the EWS Managed API **CreateItems** method, as shown in the following example.</span></span> <span data-ttu-id="be893-128">Este exemplo cria três objetos [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) localmente, adiciona a cada mensagem a uma coleção e chama o método **CreateItems** na coleção de mensagens.</span><span class="sxs-lookup"><span data-stu-id="be893-128">This example creates three [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) objects locally, adds each message to a collection, then calls the **CreateItems** method on the collection of messages.</span></span> 
  
<span data-ttu-id="be893-129">Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="be893-129">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

<span data-ttu-id="be893-130">Observe que o exemplo a salvará somente as mensagens na pasta Rascunhos; ele não envia as mensagens.</span><span class="sxs-lookup"><span data-stu-id="be893-130">Note that the example only saves the messages in the Drafts folder; it does not send the messages.</span></span> <span data-ttu-id="be893-131">Para obter mais informações sobre como enviar as mensagens, consulte [Enviar mensagens de email em lotes, usando a API gerenciada de EWS](#bk_sendewsma).</span><span class="sxs-lookup"><span data-stu-id="be893-131">For more about how to send the messages, see [Send email messages in batches by using the EWS Managed API](#bk_sendewsma).</span></span>
  
## <a name="create-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="be893-132">Criar mensagens de email em lotes, usando o EWS</span><span class="sxs-lookup"><span data-stu-id="be893-132">Create email messages in batches by using EWS</span></span>
<span data-ttu-id="be893-133"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="be893-133"></span></span>

<span data-ttu-id="be893-134">Você pode criar mensagens de email em lotes, usando a operação [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS, conforme mostrado no exemplo de código a seguir.</span><span class="sxs-lookup"><span data-stu-id="be893-134">You can create email messages in batches by using the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS operation, as shown in the following code example.</span></span> <span data-ttu-id="be893-135">Isso também é a solicitação XML que o EWS Managed API envia quando você usar a API gerenciada de EWS para [criar mensagens de email em lotes](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="be893-135">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [create email messages in batches](#bk_createewsma).</span></span> 
  
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

<span data-ttu-id="be893-136">O servidor responde à solicitação **CreateItem** com uma mensagem de [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError** para cada uma das novas mensagens, que indica que cada email foi criada e salva com êxito .</span><span class="sxs-lookup"><span data-stu-id="be893-136">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each of the new messages, which indicates that each email was created and saved successfully.</span></span> 
  
<span data-ttu-id="be893-137">Observe que o exemplo a salvará somente as mensagens na pasta Rascunhos; ele não envia as mensagens.</span><span class="sxs-lookup"><span data-stu-id="be893-137">Note that the example only saves the messages in the Drafts folder; it does not send the messages.</span></span> <span data-ttu-id="be893-138">Para obter mais informações sobre como enviar as mensagens, consulte [Enviar mensagens de email em lotes, usando o EWS](#bk_sendews).</span><span class="sxs-lookup"><span data-stu-id="be893-138">For more about how to send the messages, see [Send email messages in batches by using EWS](#bk_sendews).</span></span>
  
## <a name="send-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="be893-139">Enviar mensagens de email em lotes, usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="be893-139">Send email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="be893-140"><a name="bk_sendewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="be893-140"></span></span>

<span data-ttu-id="be893-141">Você pode usar o mesmo código para enviar emails em lotes que você usa para criar mensagens de email em lotes, exceto pelo fato de alguns dos parâmetros do método [CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) alterar.</span><span class="sxs-lookup"><span data-stu-id="be893-141">You use the same code to send email messages in batches that you use to create email messages in batches, except that a few of the [CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) method parameters change.</span></span> <span data-ttu-id="be893-142">Assim, para enviar mensagens de email usando a API gerenciada de EWS, use o código que você usa para [criar mensagens de email em lotes](#bk_createewsma)e substitua a chamada para o método **CreateItems** a chamada no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="be893-142">So, to send email messages by using the EWS Managed API, use the code you use to [create email messages in batches](#bk_createewsma), and replace the call to the **CreateItems** method with the call in the following example.</span></span> <span data-ttu-id="be893-143">Neste exemplo, as mensagens são criadas na pasta Itens enviados, e a disposição de mensagem é alterada para [MessageDisposition.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.messagedisposition%28v=exchg.80%29.aspx), para que a mensagem é enviada e não apenas salvo localmente.</span><span class="sxs-lookup"><span data-stu-id="be893-143">In this example, the messages are created in the Sent Items folder, and the message disposition is changed to [MessageDisposition.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.messagedisposition%28v=exchg.80%29.aspx), so that the message is sent, and not just saved locally.</span></span>
  
```cs
// Create and send the batch of email messages on the server.
// This method call results in an CreateItem call to EWS.
ServiceResponseCollection<ServiceResponse> response = service.CreateItems(messageItems, WellKnownFolderName.SentItems, MessageDisposition.SendAndSaveCopy, null);
```

## <a name="send-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="be893-144">Enviar mensagens de email em lotes, usando o EWS</span><span class="sxs-lookup"><span data-stu-id="be893-144">Send email messages in batches by using EWS</span></span>
<span data-ttu-id="be893-145"><a name="bk_sendews"> </a></span><span class="sxs-lookup"><span data-stu-id="be893-145"></span></span>

<span data-ttu-id="be893-146">Você pode usar o mesmo código para enviar emails em lotes que você use para criar mensagens de email em lotes, exceto pelo fato de alguns dos valores de atributo alterar para a operação **CreateItem** .</span><span class="sxs-lookup"><span data-stu-id="be893-146">You use the same code to send email messages in batches that you use to create email messages in batches, except that a few of the attribute values change for the **CreateItem** operation.</span></span> <span data-ttu-id="be893-147">Assim, para enviar mensagens de email usando o EWS, use o código que você usa para [criar a mensagem de email em lotes](#bk_createews)e altere o valor de **MessageDisposition** para "SendAndSaveCopy" e altere o [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) para "itens enviados", conforme mostrado no exemplo de código a seguir.</span><span class="sxs-lookup"><span data-stu-id="be893-147">So, to send email messages by using EWS, use the code you use to [create email message in batches](#bk_createews), and change the **MessageDisposition** value to "SendAndSaveCopy", and change the [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) to "sentitems", as shown in the following code example.</span></span> 
  
```XML
<m:CreateItem MessageDisposition="SendAndSaveCopy">
  <m:SavedItemFolderId>
    <t:DistinguishedFolderId Id="sentitems" />
  </m:SavedItemFolderId>
```

<span data-ttu-id="be893-148">O servidor responde à solicitação **CreateItem** com uma mensagem de [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError** para cada uma das novas mensagens, que indica que cada email foi criado e enviado com êxito.</span><span class="sxs-lookup"><span data-stu-id="be893-148">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each of the new messages, which indicates that each email was created and sent successfully.</span></span> 
  
## <a name="get-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="be893-149">Obter mensagens de email em lotes, usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="be893-149">Get email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="be893-150"><a name="bk_getewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="be893-150"></span></span>

<span data-ttu-id="be893-151">Você pode obter mensagens de email em lotes, usando o método API gerenciada de EWS [BindToItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) , conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="be893-151">You can get email messages in batches by using the EWS Managed API [BindToItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span> 
  
<span data-ttu-id="be893-152">Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="be893-152">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="get-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="be893-153">Obter mensagens de email em lotes, usando o EWS</span><span class="sxs-lookup"><span data-stu-id="be893-153">Get email messages in batches by using EWS</span></span>
<span data-ttu-id="be893-154"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="be893-154"></span></span>

<span data-ttu-id="be893-155">Você pode obter mensagens de email em lotes, usando a operação de EWS [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) e o código no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="be893-155">You can get email messages in batches by using the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS operation and the code in the following example.</span></span> <span data-ttu-id="be893-156">Isso também é a solicitação XML que o EWS Managed API envia quando você usar a API gerenciada de EWS para [obter as mensagens de email em lotes](#bk_getewsma).</span><span class="sxs-lookup"><span data-stu-id="be893-156">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [get email messages in batches](#bk_getewsma).</span></span> 
  
<span data-ttu-id="be893-157">Os atributos **ItemId** e **ChangeKey** foram diminuídos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="be893-157">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span> 
  
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

<span data-ttu-id="be893-158">O servidor responde à solicitação **GetItem** com uma mensagem de [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) que inclui as [Propriedades de primeira classe](email-properties-and-elements-in-ews-in-exchange.md) para cada uma das mensagens solicitadas.</span><span class="sxs-lookup"><span data-stu-id="be893-158">The server responds to the **GetItem** request with a [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes the [first class properties](email-properties-and-elements-in-ews-in-exchange.md) for each of the requested messages.</span></span> 
  
## <a name="update-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="be893-159">Mensagens de email de atualização em lotes, usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="be893-159">Update email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="be893-160"><a name="bk_updateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="be893-160"></span></span>

<span data-ttu-id="be893-161">Você pode obter mensagens de email em lotes, usando o método API gerenciada de EWS [UpdateItems](http://msdn.microsoft.com/en-us/library/dd634705%28v=exchg.80%29.aspx) , conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="be893-161">You can get email messages in batches by using the EWS Managed API [UpdateItems](http://msdn.microsoft.com/en-us/library/dd634705%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span> 
  
<span data-ttu-id="be893-162">Para obter uma lista das propriedades de mensagem de email gravável, consulte [Email propriedades e os elementos no EWS no Exchange](email-properties-and-elements-in-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="be893-162">For a list of writable email message properties, see [Email properties and elements in EWS in Exchange](email-properties-and-elements-in-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="be893-163">Para obter detalhes sobre como enviar uma mensagem de rascunho após ele ser atualizado, consulte o [envio de mensagens de email usando a API gerenciada de EWS](#bk_sendewsma).</span><span class="sxs-lookup"><span data-stu-id="be893-163">For details about how to send a draft message after it's been updated, see [Sending email messages by using the EWS Managed API](#bk_sendewsma).</span></span>
  
<span data-ttu-id="be893-164">Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="be893-164">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="update-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="be893-165">Mensagens de email de atualização em lotes, usando o EWS</span><span class="sxs-lookup"><span data-stu-id="be893-165">Update email messages in batches by using EWS</span></span>
<span data-ttu-id="be893-166"><a name="bk_updateews"> </a></span><span class="sxs-lookup"><span data-stu-id="be893-166"></span></span>

<span data-ttu-id="be893-167">Você pode atualizar as mensagens de email em lotes, usando a operação [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS, conforme mostrado no exemplo de código a seguir.</span><span class="sxs-lookup"><span data-stu-id="be893-167">You can update email messages in batches by using the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS operation, as shown in following code example.</span></span> <span data-ttu-id="be893-168">Isso também é a solicitação XML que o EWS Managed API envia quando você usar a API gerenciada de EWS para [atualizar as mensagens de email em lotes](#bk_updateewsma).</span><span class="sxs-lookup"><span data-stu-id="be893-168">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [update email messages in batches](#bk_updateewsma).</span></span>
  
<span data-ttu-id="be893-169">Para obter uma lista de elementos de mensagem de email gravável, consulte [Email propriedades e os elementos no EWS no Exchange](email-properties-and-elements-in-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="be893-169">For a list of writable email message elements, see [Email properties and elements in EWS in Exchange](email-properties-and-elements-in-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="be893-170">Para obter detalhes sobre como enviar uma mensagem de rascunho após ele ser atualizado, consulte [Enviar uma mensagem de email usando o EWS rascunho](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews).</span><span class="sxs-lookup"><span data-stu-id="be893-170">For details about how to send a draft message after it's been updated, see [Send a draft email message by using EWS](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews).</span></span>
  
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

<span data-ttu-id="be893-171">O servidor responde à solicitação **UpdateItem** com uma mensagem de [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que cada uma das atualizações foi salvo com êxito no servidor.</span><span class="sxs-lookup"><span data-stu-id="be893-171">The server responds to the **UpdateItem** request with an [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that each of the updates was saved successfully on the server.</span></span> <span data-ttu-id="be893-172">Todos os conflitos são relatados no elemento [ConflictResult](http://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="be893-172">Any conflicts are reported in the [ConflictResult](http://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) element.</span></span> 
  
## <a name="delete-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="be893-173">Excluir mensagens de email em lotes usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="be893-173">Delete email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="be893-174"><a name="bk_deleteewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="be893-174"></span></span>

<span data-ttu-id="be893-175">Você pode excluir mensagens em lotes, usando o método API gerenciada de EWS [DeleteItems](http://msdn.microsoft.com/en-us/library/dd635460%28v=exchg.80%29.aspx) , conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="be893-175">You can delete messages in batches by using the EWS Managed API [DeleteItems](http://msdn.microsoft.com/en-us/library/dd635460%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span> 
  
<span data-ttu-id="be893-176">Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="be893-176">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="delete-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="be893-177">Excluir mensagens de email em lotes, usando o EWS</span><span class="sxs-lookup"><span data-stu-id="be893-177">Delete email messages in batches by using EWS</span></span>
<span data-ttu-id="be893-178"><a name="bk_deleteews"> </a></span><span class="sxs-lookup"><span data-stu-id="be893-178"></span></span>

<span data-ttu-id="be893-179">Você pode excluir mensagens de email em lotes, usando a operação [DeleteItem](../web-service-reference/deleteitem-operation.md) EWS, conforme mostrado no exemplo de código a seguir.</span><span class="sxs-lookup"><span data-stu-id="be893-179">You can delete email messages in batches by using the [DeleteItem](../web-service-reference/deleteitem-operation.md) EWS operation, as shown in the following code example.</span></span> <span data-ttu-id="be893-180">Isso também é a solicitação XML que o EWS Managed API envia quando você usar a API gerenciada de EWS para [Excluir mensagens de email em lotes](#bk_deleteewsma).</span><span class="sxs-lookup"><span data-stu-id="be893-180">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [delete email messages in batches](#bk_deleteewsma).</span></span>
  
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

<span data-ttu-id="be893-181">O servidor responde à solicitação **DeleteItem** com uma mensagem de [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError** para cada item que foi removido.</span><span class="sxs-lookup"><span data-stu-id="be893-181">The server responds to the **DeleteItem** request with a [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each item that was removed.</span></span> <span data-ttu-id="be893-182">Observe que a operação também retorna sucesso se a ID do item não pôde ser encontrada.</span><span class="sxs-lookup"><span data-stu-id="be893-182">Note that the operation also returns success if the item ID could not be found.</span></span> 
  
## <a name="verifying-that-a-batch-process-completed-successfully"></a><span data-ttu-id="be893-183">Verificando se um processo em lote foi concluída com êxito</span><span class="sxs-lookup"><span data-stu-id="be893-183">Verifying that a batch process completed successfully</span></span>
<span data-ttu-id="be893-184"><a name="bk_successful"> </a></span><span class="sxs-lookup"><span data-stu-id="be893-184"></span></span>

<span data-ttu-id="be893-185">Quando uma ou mais mensagens de email em uma solicitação de lote não podem ser processadas, conforme solicitado, um erro será retornado para cada mensagem de email que falharam e o restante de emails no lote são processadas conforme o esperado.</span><span class="sxs-lookup"><span data-stu-id="be893-185">When one or more email messages in a batched request can't be processed as requested, an error is returned for each email message that failed, and the rest of the emails in the batch are processed as expected.</span></span> <span data-ttu-id="be893-186">Falhas no processamento em lotes podem ocorrer se o item foi excluído e, portanto, não pode ser enviado, recuperado ou atualizado, ou se o item movido para uma pasta diferente e, portanto, tem uma nova ID de item e não pode ser modificado com a ID de item enviada.</span><span class="sxs-lookup"><span data-stu-id="be893-186">Failures in batch processing can occur if the item was deleted, and therefore can't be sent, retrieved, or updated, or if the item moved to a different folder, and therefore has a new item ID, and cannot be modified with the item ID sent.</span></span> <span data-ttu-id="be893-187">As informações nesta seção mostram como obter os detalhes de erro sobre falhas no processamento em lotes da mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="be893-187">The information in this section shows how to get error details about failures in batch processing of email message.</span></span>
  
<span data-ttu-id="be893-188">Para verificar o sucesso de um processo em lote usando a API gerenciada de EWS, você pode verificar se a propriedade [OverallResult](http://msdn.microsoft.com/en-us/library/dd634515%28v=exchg.80%29.aspx) do [ServiceResponseCollection](http://msdn.microsoft.com/en-us/library/dd633715%28v=exchg.80%29.aspx) for igual a [ServiceResult.Success](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="be893-188">To verify the success of a batch process by using the EWS Managed API, you can check that the [OverallResult](http://msdn.microsoft.com/en-us/library/dd634515%28v=exchg.80%29.aspx) property of the [ServiceResponseCollection](http://msdn.microsoft.com/en-us/library/dd633715%28v=exchg.80%29.aspx) is equal to [ServiceResult.Success](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="be893-189">Nesse caso, todos os emails foram processados com êxito.</span><span class="sxs-lookup"><span data-stu-id="be893-189">If so, all the emails were processed successfully.</span></span> <span data-ttu-id="be893-190">Se o **OverallResult** não for igual a **ServiceResult.Success**, um ou mais os emails existentes não foram processadas com êxito.</span><span class="sxs-lookup"><span data-stu-id="be893-190">If the **OverallResult** is not equal to **ServiceResult.Success**, one or more of the emails were not processed successfully.</span></span> <span data-ttu-id="be893-191">Cada um dos objetos retornados no **ServiceResponseCollection** contém as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="be893-191">Each of the objects returned in the **ServiceResponseCollection** contains the following properties:</span></span> 
  
- [<span data-ttu-id="be893-192">ErrorCode</span><span class="sxs-lookup"><span data-stu-id="be893-192">ErrorCode</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="be893-193">ErrorDetails</span><span class="sxs-lookup"><span data-stu-id="be893-193">ErrorDetails</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="be893-194">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="be893-194">ErrorMessage</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="be893-195">ErrorProperties</span><span class="sxs-lookup"><span data-stu-id="be893-195">ErrorProperties</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="be893-196">Resultado</span><span class="sxs-lookup"><span data-stu-id="be893-196">Result</span></span>](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx)
    
<span data-ttu-id="be893-197">Essas propriedades contêm informações sobre por que as mensagens de email não pôde ser processadas conforme solicitado.</span><span class="sxs-lookup"><span data-stu-id="be893-197">These properties contain information about why the email messages could not be processed as requested.</span></span> <span data-ttu-id="be893-198">Os exemplos neste artigo imprimam o **resultado**, **ErrorCode**e **ErrorMessage** para cada mensagem com falha.</span><span class="sxs-lookup"><span data-stu-id="be893-198">The examples in this article print out the **Result**, **ErrorCode**, and **ErrorMessage** for each failed message.</span></span> <span data-ttu-id="be893-199">Você pode usar estes resultados para investigar o problema.</span><span class="sxs-lookup"><span data-stu-id="be893-199">You can use these results to investigate the issue.</span></span> 
  
<span data-ttu-id="be893-200">Para o EWS, para verificar o sucesso de um processo em lote, verifique o atributo [ResponseClass](http://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) para cada item que estão sendo processada.</span><span class="sxs-lookup"><span data-stu-id="be893-200">For EWS, to verify the success of a batched process, check the [ResponseClass](http://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) attribute for each item being processed.</span></span> <span data-ttu-id="be893-201">Veja a seguir a estrutura básica do **ResponseMessageType**, o tipo de base da resposta que todas as mensagens são derivadas.</span><span class="sxs-lookup"><span data-stu-id="be893-201">The following is the basic structure of the **ResponseMessageType**, the base type from which all response messages are derived.</span></span> 
  
```XML
<ResponseMessage ResponseClass="Success | Warning | Error">
            <MessageText/>
            <ResponseCode/>
            <DescriptiveLinkKey/>
            <MessageXml/>
</ResponseMessage>
```

<span data-ttu-id="be893-202">O atributo **ResponseClass** é definido como **sucesso** se o email foi processado com êxito, ou **erro** se o email não foi processado com êxito.</span><span class="sxs-lookup"><span data-stu-id="be893-202">The **ResponseClass** attribute is set to **Success** if the email was processed successfully, or **Error** if the email was not processed successfully.</span></span> <span data-ttu-id="be893-203">Para mensagens de email, você não encontrará um **Aviso** durante o processamento em lotes.</span><span class="sxs-lookup"><span data-stu-id="be893-203">For email messages, you will not encounter a **Warning** during batch processing.</span></span> <span data-ttu-id="be893-204">Se o **ResponseClass** for **sucesso**, o elemento [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) que segue também sempre é definido como **NoError**.</span><span class="sxs-lookup"><span data-stu-id="be893-204">If the **ResponseClass** is **Success**, the [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element that follows is also always set to **NoError**.</span></span> <span data-ttu-id="be893-205">Se a **ResponseClass** **erro**, você precisará verificar os valores dos elementos [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **ResponseCode**e [MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) para determinar o que causou o problema.</span><span class="sxs-lookup"><span data-stu-id="be893-205">If the **ResponseClass** is **Error**, you need to check the values of the [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **ResponseCode**, and [MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) elements to determine what caused the problem.</span></span> <span data-ttu-id="be893-206">[DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) não é usada no momento.</span><span class="sxs-lookup"><span data-stu-id="be893-206">[DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) is currently unused.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="be893-207">Confira também</span><span class="sxs-lookup"><span data-stu-id="be893-207">See also</span></span>


- [<span data-ttu-id="be893-208">Email e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="be893-208">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
    
- [<span data-ttu-id="be893-209">Enviar mensagens de email usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="be893-209">Send email messages by using EWS in Exchange</span></span>](how-to-send-email-messages-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="be893-210">Responder às mensagens de email usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="be893-210">Respond to email messages by using EWS in Exchange</span></span>](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="be893-211">Mover e copiar mensagens de email usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="be893-211">Move and copy email messages by using EWS in Exchange</span></span>](how-to-move-and-copy-email-messages-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="be893-212">Limitação implicações para solicitações de lote EWS</span><span class="sxs-lookup"><span data-stu-id="be893-212">Throttling implications for EWS batch requests</span></span>](ews-throttling-in-exchange.md#bk_ThrottlingBatch)
    

