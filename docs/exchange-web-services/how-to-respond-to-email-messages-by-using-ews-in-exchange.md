---
title: Responder às mensagens de email usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9d584991-4d67-4d36-ae2f-99970af8488f
description: Saiba como responder às mensagens de email usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: 2f1428251084a7f2bf8d589a788c143f34b64d5c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750820"
---
# <a name="respond-to-email-messages-by-using-ews-in-exchange"></a><span data-ttu-id="03b70-103">Responder às mensagens de email usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="03b70-103">Respond to email messages by using EWS in Exchange</span></span>

<span data-ttu-id="03b70-104">Saiba como responder às mensagens de email usando a API gerenciada de EWS ou EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="03b70-104">Learn how to respond to email messages by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="03b70-105">Você pode usar a API gerenciada de EWS ou EWS responder às mensagens por responder a eles ou encaminhá-los aos destinatários.</span><span class="sxs-lookup"><span data-stu-id="03b70-105">You can use the EWS Managed API or EWS to respond to messages by replying to them or forwarding them to recipients.</span></span>
  
<span data-ttu-id="03b70-106">**Tabela 1. Operações de EWS para responder a emails e métodos de API gerenciada de EWS**</span><span class="sxs-lookup"><span data-stu-id="03b70-106">**Table 1. EWS Managed API methods and EWS operations for responding to email messages**</span></span>

|<span data-ttu-id="03b70-107">**Task**</span><span class="sxs-lookup"><span data-stu-id="03b70-107">**Task**</span></span>|<span data-ttu-id="03b70-108">**Método API gerenciada de EWS**</span><span class="sxs-lookup"><span data-stu-id="03b70-108">**EWS Managed API method**</span></span>|<span data-ttu-id="03b70-109">**Operação do EWS**</span><span class="sxs-lookup"><span data-stu-id="03b70-109">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="03b70-110">Responder a uma mensagem de email</span><span class="sxs-lookup"><span data-stu-id="03b70-110">Reply to an email message</span></span>  <br/> |[<span data-ttu-id="03b70-111">EmailMessage.Reply</span><span class="sxs-lookup"><span data-stu-id="03b70-111">EmailMessage.Reply</span></span>](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="03b70-112">EmailMessage.CreateReply</span><span class="sxs-lookup"><span data-stu-id="03b70-112">EmailMessage.CreateReply</span></span>](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.createreply%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="03b70-113">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx), onde o elemento [Items](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) tem um elemento filho do [ReplyToItem](http://msdn.microsoft.com/library/35ee751a-41c0-4216-ad8b-78f7ada43a2f%28Office.15%29.aspx) ou [ReplyAllToItem](http://msdn.microsoft.com/library/8ca970ca-ca73-40db-9233-7b271cc5f44f%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="03b70-113">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx), where the [Items](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) element has a child element of either [ReplyToItem](http://msdn.microsoft.com/library/35ee751a-41c0-4216-ad8b-78f7ada43a2f%28Office.15%29.aspx) or [ReplyAllToItem](http://msdn.microsoft.com/library/8ca970ca-ca73-40db-9233-7b271cc5f44f%28Office.15%29.aspx).</span></span>  <br/> |
|<span data-ttu-id="03b70-114">Encaminhar uma mensagem de email</span><span class="sxs-lookup"><span data-stu-id="03b70-114">Forward an email message</span></span>  <br/> |[<span data-ttu-id="03b70-115">EmailMessage.Forward</span><span class="sxs-lookup"><span data-stu-id="03b70-115">EmailMessage.Forward</span></span>](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.forward%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="03b70-116">EmailMessage.CreateForward</span><span class="sxs-lookup"><span data-stu-id="03b70-116">EmailMessage.CreateForward</span></span>](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.createforward%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="03b70-117">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx), onde o elemento [Items](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) tem um elemento filho do [ForwardItem](http://msdn.microsoft.com/library/97786086-8b91-4471-8af8-d21e8d66de87%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="03b70-117">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx), where the [Items](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) element has a child element of [ForwardItem](http://msdn.microsoft.com/library/97786086-8b91-4471-8af8-d21e8d66de87%28Office.15%29.aspx).</span></span>  <br/> |
   
## <a name="reply-to-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="03b70-118">Responder a uma mensagem de email usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="03b70-118">Reply to an email message by using the EWS Managed API</span></span>
<span data-ttu-id="03b70-119"><a name="bk_replyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="03b70-119"></span></span>

<span data-ttu-id="03b70-120">A API gerenciada de EWS fornece dois métodos que você pode usar para responder a mensagens: [responder](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) e [CreateReply](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.createreply%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="03b70-120">The EWS Managed API provides two methods that you can use to respond to messages: [Reply](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) and [CreateReply](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.createreply%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="03b70-121">O método **Reply** leva apenas dois parâmetros: a mensagem de resposta para preceder o corpo existente e um valor **Boolean** que indica se a resposta deve ir para todos os destinatários (true) ou apenas o remetente (false).</span><span class="sxs-lookup"><span data-stu-id="03b70-121">The **Reply** method only takes two parameters: the response message to prepend to the existing body, and a **Boolean** value that indicates whether the response should go to all recipients (true) or just the sender (false).</span></span> <span data-ttu-id="03b70-122">Se você precisa adicionar destinatários adicionais a uma mensagem, definir propriedades adicionais em uma resposta ou adicionar um anexo, use o método **CreateReply** , que permite que você defina todas as [Propriedades de primeira classe](email-properties-and-elements-in-ews-in-exchange.md) que estão disponíveis em uma [EmailMessage ](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx)objeto.</span><span class="sxs-lookup"><span data-stu-id="03b70-122">If you need to add additional recipients to a message, set additional properties on a response, or add an attachment, use the **CreateReply** method, which enables you to set all the [first-class properties](email-properties-and-elements-in-ews-in-exchange.md) that are available on an [EmailMessage](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object.</span></span> 
  
<span data-ttu-id="03b70-123">O exemplo de código a seguir mostra como usar o método **Reply** para responder a uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="03b70-123">The following code example shows how to use the **Reply** method to respond to an email message.</span></span> 
  
<span data-ttu-id="03b70-124">Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="03b70-124">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="03b70-125">A variável local *ItemId* é a [Id](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) do item para responder aos.</span><span class="sxs-lookup"><span data-stu-id="03b70-125">The local variable  *ItemId*  is the [Id](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to respond to.</span></span> <span data-ttu-id="03b70-126">O exemplo chama o [método FindRecentlySent](#bk_findlast) para verificar se a mensagem foi marcada como respondido.</span><span class="sxs-lookup"><span data-stu-id="03b70-126">The example calls the [FindRecentlySent method](#bk_findlast) to verify that the message was marked as replied to.</span></span> 
  
```cs
// As a best practice, limit the properties returned by the Bind method to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, ItemSchema.LastModifiedTime);
// Bind to the email message to reply to by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage message = EmailMessage.Bind(service, ItemId, propSet);
string myReply = "This is the message body of the email reply.";
bool replyToAll = false;
// Send the response message.
// This method call results in a CreateItem call to EWS.
message.Reply(myReply, replyToAll);
// Verify that the response was sent by calling FindRecentlySent.
FindRecentlySent(message);
```

<span data-ttu-id="03b70-127">O exemplo de código a seguir mostra como usar o método **CreateReply** para responder a uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="03b70-127">The following code example shows how to use the **CreateReply** method to respond to an email message.</span></span> 
  
```cs
// Bind to the email message to reply to by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage message = EmailMessage.Bind(service, ItemId, BasePropertySet.IdOnly);
// Create the reply response message from the original email message.
// Indicate whether the message is a reply or reply all type of reply.
bool replyToAll = true;
ResponseMessage responseMessage = message.CreateReply(replyToAll);
// Prepend the reply to the message body. 
string myReply = "This is the message body of the email reply.";
responseMessage.BodyPrefix = myReply;
// Send the response message.
// This method call results in a CreateItem call to EWS.
responseMessage.SendAndSaveCopy();
// Check that the response was sent by calling FindRecentlySent.
FindRecentlySent(message);
```

<span data-ttu-id="03b70-128">Se você precisar adicionar um anexo à mensagem de resposta, substitua a chamada para o método **SendAndSaveCopy** o código a seguir.</span><span class="sxs-lookup"><span data-stu-id="03b70-128">If you need to add an attachment to the response message, replace the call to the **SendAndSaveCopy** method with the following code.</span></span> 
  
```cs
EmailMessage reply = responseMessage.Save();
reply.Attachments.AddFileAttachment("attachmentname.txt");
reply.Update(ConflictResolutionMode.AutoResolve);
reply.SendAndSaveCopy();
```

## <a name="reply-to-an-email-message-by-using-ews"></a><span data-ttu-id="03b70-129">Responder a uma mensagem de email usando o EWS</span><span class="sxs-lookup"><span data-stu-id="03b70-129">Reply to an email message by using EWS</span></span>
<span data-ttu-id="03b70-130"><a name="bk_replyews"> </a></span><span class="sxs-lookup"><span data-stu-id="03b70-130"></span></span>

<span data-ttu-id="03b70-131">O exemplo de código a seguir mostra como responder a uma mensagem usando o EWS.</span><span class="sxs-lookup"><span data-stu-id="03b70-131">The following code example shows how to reply to a message by using EWS.</span></span> <span data-ttu-id="03b70-132">Use a operação [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) com o atributo **MessageDisposition** definido como **SendAndSaveCopy** para enviar a mensagem e salvar a resposta na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="03b70-132">Use the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation with the **MessageDisposition** attribute set to **SendAndSaveCopy** to send the message and save the response in the Sent Items folder.</span></span> <span data-ttu-id="03b70-133">Incluir elemento [ReplyAllToItem](http://msdn.microsoft.com/library/8ca970ca-ca73-40db-9233-7b271cc5f44f%28Office.15%29.aspx) como um filho do elemento de [itens](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) para responder a todos no thread da mensagem, ou incluir o elemento [ReplyToItem](http://msdn.microsoft.com/library/35ee751a-41c0-4216-ad8b-78f7ada43a2f%28Office.15%29.aspx) para responder somente ao remetente.</span><span class="sxs-lookup"><span data-stu-id="03b70-133">Include either the [ReplyAllToItem](http://msdn.microsoft.com/library/8ca970ca-ca73-40db-9233-7b271cc5f44f%28Office.15%29.aspx) element as a child of the [Items](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) element to reply to everyone on the message thread, or include the [ReplyToItem](http://msdn.microsoft.com/library/35ee751a-41c0-4216-ad8b-78f7ada43a2f%28Office.15%29.aspx) element to reply only to the sender.</span></span> 
  
<span data-ttu-id="03b70-134">Isso também é a solicitação XML que o EWS Managed API envia ao chamar o método [CreateReply](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.createreply%28v=exchg.80%29.aspx) ou a [resposta](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="03b70-134">This is also the XML request that the EWS Managed API sends when calling either the [Reply](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) or the [CreateReply](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.createreply%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version=" Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:Items>
        <t:ReplyAllToItem>
          <t:ReferenceItemId Id="AAMkADE4="
                             ChangeKey="CQAAABYA" />
          <t:NewBodyContent BodyType="HTML">This is the message body of the email reply.</t:NewBodyContent>
        </t:ReplyAllToItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="03b70-135">O servidor responde à solicitação **CreateItem** com uma mensagem de [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que a resposta foi criada e enviada com êxito.</span><span class="sxs-lookup"><span data-stu-id="03b70-135">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the reply was created and sent successfully.</span></span>
  
<span data-ttu-id="03b70-136">Se você precisar adicionar um anexo a sua mensagem de resposta, chamar a operação **CreateItem** conforme especificado acima, mas altere o **MessageDisposition** para **SaveOnly**.</span><span class="sxs-lookup"><span data-stu-id="03b70-136">If you need to add an attachment to your response message, call the **CreateItem** operation as specified above, but change the **MessageDisposition** to **SaveOnly**.</span></span> <span data-ttu-id="03b70-137">Ligar para a operação [CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) , seguida da operação [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="03b70-137">Then call the [CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) operation, followed by the [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation.</span></span> 
  
## <a name="forward-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="03b70-138">Encaminhar uma mensagem de email usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="03b70-138">Forward an email message by using the EWS Managed API</span></span>
<span data-ttu-id="03b70-139"><a name="bk_forwardewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="03b70-139"></span></span>

<span data-ttu-id="03b70-140">A API gerenciada de EWS fornece dois métodos que você pode usar para encaminhar mensagens: [Encaminhar](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.forward%28v=exchg.80%29.aspx) e [CreateForward](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.createforward%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="03b70-140">The EWS Managed API provides two methods that you can use to forward messages: [Forward](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.forward%28v=exchg.80%29.aspx) and [CreateForward](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.createforward%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="03b70-141">O método **Forward** leva apenas dois parâmetros: a mensagem preceder o corpo existente e uma matriz ou coleção de destinatários, dependendo da sobrecarga você optar por usar.</span><span class="sxs-lookup"><span data-stu-id="03b70-141">The **Forward** method only takes two parameters: the message to prepend to the existing body, and an array or collection of recipients, depending on the overload you choose to use.</span></span> <span data-ttu-id="03b70-142">Se você precisar adicionar um anexo à mensagem você está encaminhamento, ou definir propriedades adicionais sobre a nova mensagem, use o método **CreateForward** , que permite que você defina todas as propriedades que estão disponíveis em um objeto [EmailMessage](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="03b70-142">If you need to add an attachment to the message you're forwarding, or set additional properties on the new message, use the **CreateForward** method, which enables you to set all the properties that are available on an [EmailMessage](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object.</span></span> 
  
<span data-ttu-id="03b70-143">O exemplo de código a seguir mostra como usar o método **Forward** para encaminhar uma mensagem de email para um destinatário.</span><span class="sxs-lookup"><span data-stu-id="03b70-143">The following code example shows how to use the **Forward** method to forward an email message to one recipient.</span></span> 
  
<span data-ttu-id="03b70-144">Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="03b70-144">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="03b70-145">A variável local *ItemId* é a [Id](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) do item para encaminhar.</span><span class="sxs-lookup"><span data-stu-id="03b70-145">The local variable  *ItemId*  is the [Id](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to forward.</span></span> <span data-ttu-id="03b70-146">O exemplo chama o [método FindRecentlySent](#bk_findlast) para verificar se a mensagem foi marcada como encaminhadas.</span><span class="sxs-lookup"><span data-stu-id="03b70-146">The example calls the [FindRecentlySent method](#bk_findlast) to verify that the message was marked as forwarded.</span></span> 
  
```cs
// Bind to the email message to reply to by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage message = EmailMessage.Bind(service, ItemId, BasePropertySet.IdOnly);
string myForward = "This is the message body of the forwarded email.";
// Send the response message.
// This method call results in a CreateItem call to EWS.
message.Forward(myForward, "sadie@contoso.com");
// Verify that the forwarded response was sent by calling FindRecentlySent.
FindRecentlySent(message);
```

<span data-ttu-id="03b70-147">O exemplo de código a seguir mostra como usar o método **CreateForward** para encaminhar uma mensagem de email para um destinatário.</span><span class="sxs-lookup"><span data-stu-id="03b70-147">The following code example shows how to use the **CreateForward** method to forward an email message to one recipient.</span></span> 
  
```cs
// Bind to the email message to reply to by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage message = EmailMessage.Bind(service, ItemId, BasePropertySet.IdOnly);
// Create the reply response message from the original email message.
// Indicate whether the message is a reply or reply all type of reply.
ResponseMessage forwardMessage = message.CreateForward();
// Set properties on the email message.
forwardMessage.ToRecipients.Add("sadie@contoso.com");
forwardMessage.Body = "Sadie,<br><br>I thought you'd be interested in this thread.<br><br>-Mack";
// Send and save a copy of the replied email message in the default Sent Items folder. 
forwardMessage.SendAndSaveCopy();
// Verify that the forwarded message was sent by calling FindRecentlySent.
FindRecentlySent(message);
```

<span data-ttu-id="03b70-148">Se você precisar adicionar um anexo à mensagem encaminhada, substitua a chamada para o método **SendAndSaveCopy** o código a seguir.</span><span class="sxs-lookup"><span data-stu-id="03b70-148">If you need to add an attachment to the forwarded message, replace the call to the **SendAndSaveCopy** method with the following code.</span></span> 
  
```cs
EmailMessage forward = forwardMessage.Save();
forward.Attachments.AddFileAttachment("attachmentname.txt");
forward.Update(ConflictResolutionMode.AutoResolve);
forward.SendAndSaveCopy();
```

## <a name="forward-an-email-message-by-using-ews"></a><span data-ttu-id="03b70-149">Encaminhar uma mensagem de email usando o EWS</span><span class="sxs-lookup"><span data-stu-id="03b70-149">Forward an email message by using EWS</span></span>
<span data-ttu-id="03b70-150"><a name="bk_forwardews"> </a></span><span class="sxs-lookup"><span data-stu-id="03b70-150"></span></span>

<span data-ttu-id="03b70-151">O exemplo de código a seguir mostra como encaminhar uma mensagem usando o EWS.</span><span class="sxs-lookup"><span data-stu-id="03b70-151">The following code example shows how to forward a message by using EWS.</span></span> <span data-ttu-id="03b70-152">Use a operação [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) com o atributo **MessageDisposition** definido como **SendAndSaveCopy** para enviar a mensagem e salvar a resposta na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="03b70-152">Use the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation with the **MessageDisposition** attribute set to **SendAndSaveCopy** to send the message and save the response in the Sent Items folder.</span></span> <span data-ttu-id="03b70-153">O elemento [ForwardItem](http://msdn.microsoft.com/library/97786086-8b91-4471-8af8-d21e8d66de87%28Office.15%29.aspx) indica que o item é uma mensagem encaminhada.</span><span class="sxs-lookup"><span data-stu-id="03b70-153">The [ForwardItem](http://msdn.microsoft.com/library/97786086-8b91-4471-8af8-d21e8d66de87%28Office.15%29.aspx) element indicates that the item is a forwarded message.</span></span> 
  
<span data-ttu-id="03b70-154">Isso também é a solicitação XML que o EWS Managed API envia ao chamar o [Encaminhar](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.forward%28v=exchg.80%29.aspx) ou o método [CreateForward](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.createforward%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="03b70-154">This is also the XML request that the EWS Managed API sends when calling either the [Forward](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.forward%28v=exchg.80%29.aspx) or the [CreateForward](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.createforward%28v=exchg.80%29.aspx) method.</span></span> 
  
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
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:Items>
        <t:ForwardItem>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
          <t:ReferenceItemId Id="AAAMkADE="
                             ChangeKey="CQAAABYA" />
          <t:NewBodyContent BodyType="HTML">This is the message body of the forwarded email.</t:NewBodyContent>
        </t:ForwardItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="03b70-155">O servidor responde à solicitação **CreateItem** com uma mensagem de [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor do elemento de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que a mensagem encaminhada foi criada e enviada com êxito.</span><span class="sxs-lookup"><span data-stu-id="03b70-155">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the forwarded message was created and sent successfully.</span></span>
  
<span data-ttu-id="03b70-156">Se você precisar adicionar um anexo a sua mensagem de resposta, chamar a operação **CreateItem** , mas altere o **MessageDisposition** para **SaveOnly**.</span><span class="sxs-lookup"><span data-stu-id="03b70-156">If you need to add an attachment to your response message, call the **CreateItem** operation, but change the **MessageDisposition** to **SaveOnly**.</span></span> <span data-ttu-id="03b70-157">Ligar para a operação [CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) , seguida da operação [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="03b70-157">Then call the [CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) operation, followed by the [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation.</span></span> 
  
## <a name="find-the-message-last-replied-to-or-forwarded-by-using-the-ews-managed-api"></a><span data-ttu-id="03b70-158">Encontre a mensagem última respondida ou encaminhada usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="03b70-158">Find the message last replied to or forwarded by using the EWS Managed API</span></span>
<span data-ttu-id="03b70-159"><a name="bk_findlast"> </a></span><span class="sxs-lookup"><span data-stu-id="03b70-159"></span></span>

<span data-ttu-id="03b70-160">O exemplo de código a seguir mostra como localizar o último verbo executado e a hora do último verbo tiver sido executado no item especificado.</span><span class="sxs-lookup"><span data-stu-id="03b70-160">The following code example shows how to find the last verb executed and the time the last verb was executed on the item specified.</span></span> <span data-ttu-id="03b70-161">Este método é chamado a partir de outros exemplos de código do API gerenciada de EWS neste tópico para verificar se os itens que você respondeu ou encaminhou foram marcados como respondida ou encaminhados na caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="03b70-161">This method is called from other EWS Managed API code examples in this topic to verify that the items you replied to or forwarded were marked as replied to or forwarded in your Inbox.</span></span> 
  
<span data-ttu-id="03b70-162">O exemplo usa a propriedade de [PidTagLastVerbExecuted](http://msdn.microsoft.com/pt-br/library/cc841968.aspx) (0x10820003) estendido para determinar se a mensagem foi uma resposta, uma resposta a todos ou um encaminhamento e [PidTagLastVerbExecutionTime](http://msdn.microsoft.com/pt-br/library/cc839918.aspx) (0x10820040) estendido de propriedade para determinar quando o responder ou encaminhar foi enviada.</span><span class="sxs-lookup"><span data-stu-id="03b70-162">The example uses the [PidTagLastVerbExecuted](http://msdn.microsoft.com/pt-br/library/cc841968.aspx) (0x10820003) extended property to determine whether the message was a reply, a reply all, or a forward, and the [PidTagLastVerbExecutionTime](http://msdn.microsoft.com/pt-br/library/cc839918.aspx) (0x10820040) extended property to determine when the reply or forward was sent.</span></span> 
  
```cs
public static void FindRecentlySent(EmailMessage messageToCheck)
{
    // Create extended property definitions for PidTagLastVerbExecuted and PidTagLastVerbExecutionTime.
    ExtendedPropertyDefinition PidTagLastVerbExecuted = new ExtendedPropertyDefinition(0x1081, MapiPropertyType.Integer);
    ExtendedPropertyDefinition PidTagLastVerbExecutionTime = new ExtendedPropertyDefinition(0x1082, MapiPropertyType.SystemTime);
    PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, EmailMessageSchema.Subject, PidTagLastVerbExecutionTime, PidTagLastVerbExecuted);
    messageToCheck = EmailMessage.Bind(service, messageToCheck.Id, propSet);
    // Determine the last verb executed on the message and display output.
    object responseType;
    if (messageToCheck.TryGetProperty(PidTagLastVerbExecuted, out responseType))
    {
        object ReplyTime = null;
        switch (((Int32)responseType))
        {
            case 102: Console.WriteLine("A reply was sent to the '" + messageToCheck.Subject.ToString() + "' email message at");
                break;
            case 103: Console.WriteLine("A reply all was sent to the '" + messageToCheck.Subject.ToString() + "' email message at");
                break;
            case 104: Console.WriteLine("The '" + messageToCheck.Subject.ToString() + "' email message was forwarded at");
                break;
        }
        if (messageToCheck.TryGetProperty(PidTagLastVerbExecutionTime, out ReplyTime))
        {
            Console.WriteLine(((DateTime)ReplyTime).ToString() + ".");
        }
    }
    else
    {
        Console.WriteLine("No changes were made to  '" + messageToCheck.Subject.ToString() + "'.");
    }
}
```

## <a name="see-also"></a><span data-ttu-id="03b70-163">Confira também</span><span class="sxs-lookup"><span data-stu-id="03b70-163">See also</span></span>


- [<span data-ttu-id="03b70-164">Email e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="03b70-164">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
    
- [<span data-ttu-id="03b70-165">Enviar mensagens de email usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="03b70-165">Send email messages by using EWS in Exchange</span></span>](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

