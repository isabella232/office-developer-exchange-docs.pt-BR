---
title: Excluir anexos usando o EWS no Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 71871ac7-ee1a-4f93-9e81-77f312d432f4
description: Aprenda a excluir anexos de itens usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: 458331f81493283efc20d24c7e2bebe0e74bbdbd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750714"
---
# <a name="delete-attachments-by-using-ews-in-exchange"></a><span data-ttu-id="4ebd3-103">Excluir anexos usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4ebd3-103">Delete attachments by using EWS in Exchange</span></span>

<span data-ttu-id="4ebd3-104">Aprenda a excluir anexos de itens usando a API gerenciada de EWS ou EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-104">Learn how to delete attachments from items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="4ebd3-105">Você tem várias opções quando se trata de excluir o arquivo e anexos de item de itens usando a API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-105">You have a number of options when it comes to deleting file and item attachments from items by using the EWS Managed API.</span></span> <span data-ttu-id="4ebd3-106">Você pode excluir todos os anexos da mensagem, exclua um nome de arquivo ou excluir por posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-106">You can delete all the attachments from the message, delete by a file name, or delete by position in the collection.</span></span> <span data-ttu-id="4ebd3-107">Para cada uma dessas opções, há um método [AttachmentCollection](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.attachmentcollection%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4ebd3-107">For each of these options, there is an [AttachmentCollection](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.attachmentcollection%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="4ebd3-108">Por outro lado, com EWS, não importa se você estiver excluindo todos os anexos de um item ou apenas um deles, a sequência de operações é mesma.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-108">Conversely, with EWS, no matter whether you're deleting all attachments from an item or just one, the sequence of operations is same.</span></span> <span data-ttu-id="4ebd3-109">Diferentemente da API gerenciada de EWS, EWS não inclui operações separadas para excluir com base no nome ou a posição na matriz anexos.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-109">Unlike the EWS Managed API, EWS does not include separate operations to delete based on name or position in the attachments array.</span></span>
  
<span data-ttu-id="4ebd3-110">**Tabela 1. Métodos de API gerenciada de EWS e operações de EWS para excluir anexos**</span><span class="sxs-lookup"><span data-stu-id="4ebd3-110">**Table 1. EWS Managed API methods and EWS operations for deleting attachments**</span></span>

|<span data-ttu-id="4ebd3-111">**Task**</span><span class="sxs-lookup"><span data-stu-id="4ebd3-111">**Task**</span></span>|<span data-ttu-id="4ebd3-112">**Método API gerenciada de EWS**</span><span class="sxs-lookup"><span data-stu-id="4ebd3-112">**EWS Managed API method**</span></span>|<span data-ttu-id="4ebd3-113">**Operação do EWS**</span><span class="sxs-lookup"><span data-stu-id="4ebd3-113">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4ebd3-114">Exclua todos os anexos de um item.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-114">Delete all attachments from an item.</span></span>  <br/> |<span data-ttu-id="4ebd3-115">[Item.Bind](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), seguido por [AttachmentCollection.Clear](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.attachmentcollection.clear%28v=exchg.80%29.aspx), seguido por [EmailMessage.Update](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="4ebd3-115">[Item.Bind](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), followed by [AttachmentCollection.Clear](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.attachmentcollection.clear%28v=exchg.80%29.aspx), followed by [EmailMessage.Update](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="4ebd3-116">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) seguido [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="4ebd3-116">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) followed by [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="4ebd3-117">Exclua um anexo de um item pelo nome.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-117">Delete an attachment from an item by name.</span></span>  <br/> |<span data-ttu-id="4ebd3-118">[Item.Bind](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), seguido por [AttachmentCollection.Remove](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx), seguido por [EmailMessage.Update](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="4ebd3-118">[Item.Bind](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), followed by [AttachmentCollection.Remove](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx), followed by [EmailMessage.Update](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="4ebd3-119">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) seguido [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="4ebd3-119">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) followed by [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="4ebd3-120">Exclua um anexo de um item por posição na coleção.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-120">Delete an attachment from an item by position in the collection.</span></span>  <br/> |<span data-ttu-id="4ebd3-121">[Item.Bind](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), seguido por [AttachmentCollection.RemoveAt](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.attachmentcollection.removeat%28v=exchg.80%29.aspx), seguido por [EmailMessage.Update](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="4ebd3-121">[Item.Bind](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), followed by [AttachmentCollection.RemoveAt](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.attachmentcollection.removeat%28v=exchg.80%29.aspx), followed by [EmailMessage.Update](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="4ebd3-122">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) seguido [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="4ebd3-122">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) followed by [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)</span></span> <br/> |
   
## <a name="delete-all-attachments-from-an-email-by-using-the-ews-managed-api"></a><span data-ttu-id="4ebd3-123">Excluir todos os anexos de um email usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="4ebd3-123">Delete all attachments from an email by using the EWS Managed API</span></span>
<span data-ttu-id="4ebd3-124"><a name="bk_deleteattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="4ebd3-124"></span></span>

<span data-ttu-id="4ebd3-125">O exemplo de código a seguir mostra como excluir todos os anexos de um email por:</span><span class="sxs-lookup"><span data-stu-id="4ebd3-125">The following code example shows how to delete all attachments from an email by:</span></span>
  
1. <span data-ttu-id="4ebd3-126">Usando o método [EmailMessage.Bind](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) para vincular a uma mensagem de email existente e recuperar a coleção de [anexos](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="4ebd3-126">Using the [EmailMessage.Bind](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method to bind to an existing email message and retrieve the collection of [Attachments](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx).</span></span>
    
2. <span data-ttu-id="4ebd3-127">Usando o método [AttachmentCollection.Clear](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.attachmentcollection.clear%28v=exchg.80%29.aspx) para excluir todos os anexos de email.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-127">Using the [AttachmentCollection.Clear](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.attachmentcollection.clear%28v=exchg.80%29.aspx) method to delete all the attachments from the email.</span></span> 
    
3. <span data-ttu-id="4ebd3-128">Usando o método [EmailMessage.Update](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) para salvar as alterações.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-128">Using the [EmailMessage.Update](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) method to save the changes.</span></span> 
    
<span data-ttu-id="4ebd3-129">Este exemplo pressupõe que o **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , **itemId** é o [ItemId](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) da mensagem do qual anexos serão excluídos e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-129">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, **itemId** is the [ItemId](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) of the message from which attachments will be deleted, and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static void DeleteAllAttachments(ExchangeService service, ItemId itemId)
{
    // Bind to an existing message by using its item ID and requesting its attachments collection.
    // This method results in a GetItem call to EWS.
    EmailMessage message = EmailMessage.Bind(service, itemId, new PropertySet(ItemSchema.Attachments));
    // Delete all attachments from the message.
    message.Attachments.Clear();
    // Save the updated message.
    // This method results in an DeleteAttachment call to EWS.
    message.Update(ConflictResolutionMode.AlwaysOverwrite);
}
```

## <a name="delete-an-attachment-by-name-from-an-email-by-using-the-ews-managed-api"></a><span data-ttu-id="4ebd3-130">Excluir um anexo pelo nome a partir de um email, usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="4ebd3-130">Delete an attachment by name from an email by using the EWS Managed API</span></span>
<span data-ttu-id="4ebd3-131"><a name="bk_deleteattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="4ebd3-131"></span></span>

<span data-ttu-id="4ebd3-132">O exemplo de código a seguir mostra como excluir um anexo pelo nome por:</span><span class="sxs-lookup"><span data-stu-id="4ebd3-132">The following code example shows how delete an attachment by name by:</span></span>
  
1. <span data-ttu-id="4ebd3-133">Usando o método [EmailMessage.Bind](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) para vincular a uma mensagem de email existente e recuperar a coleção de [anexos](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="4ebd3-133">Using the [EmailMessage.Bind](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method to bind to an existing email message and retrieve the collection of [Attachments](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx).</span></span>
    
2. <span data-ttu-id="4ebd3-134">Usando o método [AttachmentCollection.Remove](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx) para excluir um anexo denominado FileAttachment.txt.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-134">Using the [AttachmentCollection.Remove](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx) method to delete an attachment named FileAttachment.txt.</span></span> 
    
3. <span data-ttu-id="4ebd3-135">Usando o método [EmailMessage.Update](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) para salvar as alterações.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-135">Using the [EmailMessage.Update](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) method to save the changes.</span></span> 
    
<span data-ttu-id="4ebd3-136">Este exemplo pressupõe que o **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , **itemId** é o [ItemId](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) da mensagem do qual o anexo será excluído e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-136">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, **itemId** is the [ItemId](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) of the message from which the attachment will be deleted, and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static void DeleteNamedAttachments(ExchangeService service, ItemId itemId)
{
    // Bind to an existing message by using its item ID and requesting its attachments collection.
    // This method results in a GetItem call to EWS.
    EmailMessage message = EmailMessage.Bind(service, itemId, new PropertySet(ItemSchema.Attachments));
    // Iterate through the attachments collection and delete the attachment named "FileAttachment.txt," if it exists.
    foreach (Attachment attachment in message.Attachments)
    {
        if (attachment.Name == "FileAttachment.txt")
        {
            message.Attachments.Remove(attachment);
            break;
        }
    }
    // Save the updated message.
    // This method results in an DeleteAttachment call to EWS.
    message.Update(ConflictResolutionMode.AlwaysOverwrite);
}
```

## <a name="delete-attachments-by-position-by-using-the-ews-managed-api"></a><span data-ttu-id="4ebd3-137">Excluir anexos por posição usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="4ebd3-137">Delete attachments by position by using the EWS Managed API</span></span>
<span data-ttu-id="4ebd3-138"><a name="bk_deleteattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="4ebd3-138"></span></span>

<span data-ttu-id="4ebd3-139">O exemplo de código a seguir mostra como excluir um anexo por posição por:</span><span class="sxs-lookup"><span data-stu-id="4ebd3-139">The following code example shows how to delete an attachment by position by:</span></span>
  
1. <span data-ttu-id="4ebd3-140">Usando o método [EmailMessage.Bind](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) para vincular a uma mensagem de email existente e recuperar a coleção de [anexos](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx) e a propriedade [EmailMessage.HasAttachments](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4ebd3-140">Using the [EmailMessage.Bind](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method to bind to an existing email message and retrieve the collection of [Attachments](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx) and the [EmailMessage.HasAttachments](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) property.</span></span> 
    
2. <span data-ttu-id="4ebd3-141">Usando o método [AttachmentCollection.Remove](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx) para excluir o primeiro anexo na coleção.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-141">Using the [AttachmentCollection.Remove](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx) method to delete the first attachment in the collection.</span></span> 
    
3. <span data-ttu-id="4ebd3-142">Usando o método [EmailMessage.Update](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) para salvar as alterações.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-142">Using the [EmailMessage.Update](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) method to save the changes.</span></span> 
    
<span data-ttu-id="4ebd3-143">Este exemplo pressupõe que o **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , **itemId** é o [ItemId](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) da mensagem do qual o anexo será excluído e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-143">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, **itemId** is the [ItemId](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) of the message from which the attachment will be deleted, and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static void DeleteAttachmentByPosition(ExchangeService service, ItemId itemId)
{
    // Bind to an existing message by using its item ID and requesting the HasAttachments property and the attachments collection.
    // This method results in a GetItem call to EWS.
    EmailMessage message = EmailMessage.Bind(service, itemId, new PropertySet(EmailMessageSchema.HasAttachments, ItemSchema.Attachments));
    // Remove attachments using the zero-based index position of the attachment in the attachments collection.
    if (message.HasAttachments)
    {
        message.Attachments.RemoveAt(0);
    }
    // Save the updated message.
    // This method results in an DeleteAttachment call to EWS.
    message.Update(ConflictResolutionMode.AlwaysOverwrite);
}
```

## <a name="delete-attachments-from-an-item-by-using-ews"></a><span data-ttu-id="4ebd3-144">Excluir anexos de um item usando o EWS</span><span class="sxs-lookup"><span data-stu-id="4ebd3-144">Delete attachments from an item by using EWS</span></span>
<span data-ttu-id="4ebd3-145"><a name="bk_deleteattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="4ebd3-145"></span></span>

<span data-ttu-id="4ebd3-146">Para excluir anexos usando o EWS, primeiro é necessário recuperar a mensagem e a coleção de anexos para determinar o [AttachmentId (GetAttachment e DeleteAttachment)](http://msdn.microsoft.com/library/4bea1cb5-0a0f-4e14-9b09-f91af8cf9899%28Office.15%29.aspx) do anexo para excluir.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-146">To delete attachments by using EWS, you first need to retrieve the message and the attachment collection to determine the [AttachmentId (GetAttachment and DeleteAttachment)](http://msdn.microsoft.com/library/4bea1cb5-0a0f-4e14-9b09-f91af8cf9899%28Office.15%29.aspx) of the attachment to delete.</span></span> <span data-ttu-id="4ebd3-147">Depois que um ou mais valores **AttachmentId** para excluir, chame a operação [DeleteAttachment](http://msdn.microsoft.com/library/4d48e595-b98c-48e7-bbeb-cacf91d12a78%28Office.15%29.aspx) para remover os anexos especificados da mensagem.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-147">After you have one or more **AttachmentId** values to delete, call the [DeleteAttachment](http://msdn.microsoft.com/library/4d48e595-b98c-48e7-bbeb-cacf91d12a78%28Office.15%29.aspx) operation to remove the specified attachments from the message.</span></span> 
  
<span data-ttu-id="4ebd3-148">O exemplo de código a seguir mostra como usar a operação [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) para obter uma mensagem de email e a coleção de anexos da mensagem.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-148">The following code example shows how to use the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) operation to get an email message and the collection of attachments on the message.</span></span> <span data-ttu-id="4ebd3-149">Isso também é a primeira solicitação XML que o EWS Managed API envia quando você usar a API gerenciada de EWS para [Excluir todos os anexos de um email](#bk_deleteattachewsma).</span><span class="sxs-lookup"><span data-stu-id="4ebd3-149">This is also the first XML request that the EWS Managed API sends when you use the EWS Managed API to [delete all attachments from an email](#bk_deleteattachewsma).</span></span> <span data-ttu-id="4ebd3-150">Os valores de alguns atributos são reduzidos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-150">The values of some attributes are shortened for readability.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Central Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Attachments" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="uqE1AAA=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="4ebd3-151">O servidor responde à solicitação **GetItem** com uma mensagem de [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/pt-br/library/aa580757%28v=exchg.150%29.aspx) de **NoError**, que indica que o email foi recuperado com êxito e os valores de [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) das os anexos existentes.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-151">The server responds to the **GetItem** request with a [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/pt-br/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was retrieved successfully, and the [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) values of the existing attachments.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="939"
                         MinorBuildNumber="12"
                         Version="V2_11"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="uqE1AAA="
                        ChangeKey="CQAAABYAAAAFI5DJmZv+TLtyLOLIF1S5AAAXulcd" />
              <t:Attachments>
                <t:FileAttachment>
                  <t:AttachmentId Id="IpHLObE=" />
                  <t:Name>FileAttachment.txt</t:Name>
                </t:FileAttachment>
                <t:FileAttachment>
                  <t:AttachmentId Id="QuHSSmY=" />
                  <t:Name>SecondAttachment.txt</t:Name>
                </t:FileAttachment>
                <t:FileAttachment>
                  <t:AttachmentId Id="qf2KoPo=" />
                  <t:Name>ThirdAttachment.jpg</t:Name>
                </t:FileAttachment>
                <t:FileAttachment>
                  <t:AttachmentId Id="NFQMnMc=" />
                  <t:Name>FourthAttachment.txt</t:Name>
                </t:FileAttachment>
                <t:ItemAttachment>
                  <t:AttachmentId Id="jJvbLXQ=" />
                  <t:Name>Attached Message Item</t:Name>
                </t:ItemAttachment>
              </t:Attachments>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="4ebd3-152">Depois que você determine qual anexo a excluir, chamar a operação [DeleteAttachment](http://msdn.microsoft.com/library/4d48e595-b98c-48e7-bbeb-cacf91d12a78%28Office.15%29.aspx) e incluir os valores de **AttachmentId** os anexos para excluir.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-152">After you determine which attachment to delete, call the [DeleteAttachment](http://msdn.microsoft.com/library/4d48e595-b98c-48e7-bbeb-cacf91d12a78%28Office.15%29.aspx) operation and include the **AttachmentId** values of the attachments to delete.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Central Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:DeleteAttachment>
      <m:AttachmentIds>
        <t:AttachmentId Id="IpHLObE=" />
        <t:AttachmentId Id="QuHSSmY=" />
        <t:AttachmentId Id="qf2KoPo=" />
        <t:AttachmentId Id="NFQMnMc=" />
        <t:AttachmentId Id="jJvbLXQ=" />
      </m:AttachmentIds>
    </m:DeleteAttachment>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **DeleteAttachment** com uma mensagem de [DeleteAttachmentResponse](http://msdn.microsoft.com/library/24099a88-4ab6-4bf3-8ed5-efec8e07b9b9%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/pt-br/library/aa580757%28v=exchg.150%29.aspx) de **NoError** para cada [DeleteAttachmentResponseMessage](http://msdn.microsoft.com/library/1edb085f-1674-48e5-8ec3-42351adeac7d%28Office.15%29.aspx), que indica que cada anexo foi excluído com êxito. <span data-ttu-id="4ebd3-154">Os valores de alguns atributos são reduzidos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="4ebd3-154">The values of some attributes are shortened for readability.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="939"
                         MinorBuildNumber="12"
                         Version="V2_11"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:DeleteAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:DeleteAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="uqE1AAA=" RootItemChangeKey="AAAXulck" />
        </m:DeleteAttachmentResponseMessage>
        <m:DeleteAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="uqE1AAA=" RootItemChangeKey="AAAXulck" />
        </m:DeleteAttachmentResponseMessage>
        <m:DeleteAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="uqE1AAA=" RootItemChangeKey="AAAXulck" />
        </m:DeleteAttachmentResponseMessage>
        <m:DeleteAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="uqE1AAA=" RootItemChangeKey="AAAXulck" />
        </m:DeleteAttachmentResponseMessage>
        <m:DeleteAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="uqE1AAA=" RootItemChangeKey="AAAXulck" />
        </m:DeleteAttachmentResponseMessage>
      </m:ResponseMessages>
    </m:DeleteAttachmentResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="4ebd3-155">Confira também</span><span class="sxs-lookup"><span data-stu-id="4ebd3-155">See also</span></span>


- [<span data-ttu-id="4ebd3-156">EWS no Exchange e anexos</span><span class="sxs-lookup"><span data-stu-id="4ebd3-156">Attachments and EWS in Exchange</span></span>](attachments-and-ews-in-exchange.md)
    
- [<span data-ttu-id="4ebd3-157">Adicionar anexos usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4ebd3-157">Add attachments by using EWS in Exchange</span></span>](how-to-add-attachments-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="4ebd3-158">Obter anexos usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4ebd3-158">Get attachments by using EWS in Exchange</span></span>](how-to-get-attachments-by-using-ews-in-exchange.md)
    

