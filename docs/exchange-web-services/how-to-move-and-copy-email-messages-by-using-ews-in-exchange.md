---
title: Mover e copiar mensagens de email usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 4771668f-5623-4397-a5c0-b75a7ba01698
description: Aprenda a mover e copiar mensagens de email usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: 16f0604a16785c34dd04bdabedeedd331668a479
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750792"
---
# <a name="move-and-copy-email-messages-by-using-ews-in-exchange"></a><span data-ttu-id="25b32-103">Mover e copiar mensagens de email usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="25b32-103">Move and copy email messages by using EWS in Exchange</span></span>

<span data-ttu-id="25b32-104">Aprenda a mover e copiar mensagens de email usando a API gerenciada de EWS ou EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="25b32-104">Learn how to move and copy email messages by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="25b32-105">Você pode usar a API gerenciada de EWS ou EWS mover e copiar mensagens de email em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="25b32-105">You can use the EWS Managed API or EWS to move and copy email messages in a mailbox.</span></span>
  
<span data-ttu-id="25b32-106">**Tabela 1. Métodos de API gerenciada de EWS e operações de EWS para mover e copiar mensagens de email**</span><span class="sxs-lookup"><span data-stu-id="25b32-106">**Table 1. EWS Managed API methods and EWS operations for moving and copying email messages**</span></span>

|<span data-ttu-id="25b32-107">**Task**</span><span class="sxs-lookup"><span data-stu-id="25b32-107">**Task**</span></span>|<span data-ttu-id="25b32-108">**Método API gerenciada de EWS**</span><span class="sxs-lookup"><span data-stu-id="25b32-108">**EWS Managed API method**</span></span>|<span data-ttu-id="25b32-109">**Operação do EWS**</span><span class="sxs-lookup"><span data-stu-id="25b32-109">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="25b32-110">Mover uma mensagem de email</span><span class="sxs-lookup"><span data-stu-id="25b32-110">Move an email message</span></span>  <br/> |[<span data-ttu-id="25b32-111">EmailMessage.Move</span><span class="sxs-lookup"><span data-stu-id="25b32-111">EmailMessage.Move</span></span>](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="25b32-112">MoveItem</span><span class="sxs-lookup"><span data-stu-id="25b32-112">MoveItem</span></span>](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="25b32-113">Copiar uma mensagem de email</span><span class="sxs-lookup"><span data-stu-id="25b32-113">Copy an email message</span></span>  <br/> |[<span data-ttu-id="25b32-114">EmailMessage.Copy</span><span class="sxs-lookup"><span data-stu-id="25b32-114">EmailMessage.Copy</span></span>](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="25b32-115">CopyItem</span><span class="sxs-lookup"><span data-stu-id="25b32-115">CopyItem</span></span>](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="25b32-116">É importante observar que, quando você move ou copia uma mensagem de email em uma pasta diferente, um novo item for criado na nova pasta com uma ID exclusiva de item, e a mensagem original é excluída.</span><span class="sxs-lookup"><span data-stu-id="25b32-116">It's important to note that when you move or copy an email message into a different folder, a new item is created in the new folder with a unique item ID, and the original message is deleted.</span></span> <span data-ttu-id="25b32-117">Se você estiver movendo ou copiando uma mensagem de email entre as duas pastas na mesma caixa de correio, o novo item será retornado na resposta, que fornece acesso a ID do item novo.</span><span class="sxs-lookup"><span data-stu-id="25b32-117">If you're moving or copying an email message between two folders in the same mailbox, the new item is returned in the response, which gives you access to the new item ID.</span></span> <span data-ttu-id="25b32-118">No entanto, se você estiver movendo ou copiando uma mensagem de email entre duas caixas de correio ou entre uma caixa de correio e uma pasta pública, o novo item não será retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="25b32-118">However, if you're moving or copying an email message between two mailboxes or between a mailbox and a public folder, the new item is not returned in the response.</span></span> <span data-ttu-id="25b32-119">Para acessar a mensagem movida nesse cenário, use o método de API gerenciada de EWS [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) ou a operação de EWS [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , [criar uma definição de propriedade estendida](properties-and-extended-properties-in-ews-in-exchange.md) para a propriedade [PidTagSearchKey](http://msdn.microsoft.com/en-us/library/cc839918.aspx) (0x300B0102), ou como criar e configurar um sinalizador estendido propriedade e, em seguida, procure a propriedade estendida personalizada na nova pasta.</span><span class="sxs-lookup"><span data-stu-id="25b32-119">To access the moved message in that scenario, use the EWS Managed API [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) method or EWS [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation, [create an extended property definition](properties-and-extended-properties-in-ews-in-exchange.md) for the [PidTagSearchKey](http://msdn.microsoft.com/en-us/library/cc839918.aspx) (0x300B0102) property, or create and set a custom extended property and then search for the custom extended property in the new folder.</span></span> 
  
<span data-ttu-id="25b32-120">Excluir uma mensagem de email é diferente de mover um item para a pasta Itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="25b32-120">Deleting an email message is different than moving an item to the Deleted Items folder.</span></span> <span data-ttu-id="25b32-121">Se você usar o método de API gerenciada de EWS [item](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) ou a operação de EWS [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) , o item especificado na solicitação é removido da pasta original e uma cópia é colocada na pasta Itens excluídos com uma nova ID de item.</span><span class="sxs-lookup"><span data-stu-id="25b32-121">If you use the EWS Managed API [Item.Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) method or the EWS [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) operation, the item specified in the request is removed from the original folder, and a copy is placed in the Deleted Items folder with a new item ID.</span></span> <span data-ttu-id="25b32-122">Ao contrário de quando você move ou copia qualquer item, o novo item não será retornado o método **Delete** ou a resposta de operação **DeleteItem** .</span><span class="sxs-lookup"><span data-stu-id="25b32-122">Unlike when you move or copy any item, the new item is not returned in the **Delete** method or the **DeleteItem** operation response.</span></span> <span data-ttu-id="25b32-123">As etapas envolvidas na [exclusão de um email usando a API gerenciada de EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) ou [EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) são os mesmos para excluir qualquer item genérica do armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="25b32-123">The steps involved in [deleting an email by using the EWS Managed API](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) or [EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) are the same as those for deleting any generic item from the Exchange store.</span></span> 
  
## <a name="move-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="25b32-124">Mover uma mensagem de email usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="25b32-124">Move an email message by using the EWS Managed API</span></span>
<span data-ttu-id="25b32-125"><a name="bk_moveewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="25b32-125"></span></span>

<span data-ttu-id="25b32-126">O exemplo de código a seguir mostra como usar o método [EmailMessage.Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) para mover uma mensagem de email existentes de uma pasta para outro.</span><span class="sxs-lookup"><span data-stu-id="25b32-126">The following code example shows how to use the [EmailMessage.Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) method to move an existing email message from one folder to another.</span></span> 
  
<span data-ttu-id="25b32-127">Este exemplo pressupõe que o **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , e esse **ItemId** é a [Id](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) da mensagem de email para mover ou copiar.</span><span class="sxs-lookup"><span data-stu-id="25b32-127">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that **ItemId** is the [Id](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the email message to move or copy.</span></span> 
  
```cs
// As a best practice, limit the properties returned by the Bind method to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, EmailMessageSchema.Subject, EmailMessageSchema.ParentFolderId);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage beforeMessage = EmailMessage.Bind(service, ItemId, propSet);
// Move the specified mail to the JunkEmail folder and store the returned item.
Item item = beforeMessage.Move(WellKnownFolderName.JunkEmail);
// Check that the item was moved by binding to the moved email message 
// and retrieving the new ParentFolderId.
// This method call results in a GetItem call to EWS.
EmailMessage movedMessage = EmailMessage.Bind(service, item.Id, propSet);
Console.WriteLine("An email message with the subject '" + beforeMessage.Subject + "' has been moved from the '" + beforeMessage.ParentFolderId + "' folder to the '" + movedMessage.ParentFolderId + "' folder.");
```

## <a name="move-an-email-message-by-using-ews"></a><span data-ttu-id="25b32-128">Mover uma mensagem de email usando o EWS</span><span class="sxs-lookup"><span data-stu-id="25b32-128">Move an email message by using EWS</span></span>
<span data-ttu-id="25b32-129"><a name="bk_moveews"> </a></span><span class="sxs-lookup"><span data-stu-id="25b32-129"></span></span>

<span data-ttu-id="25b32-130">O exemplo de código a seguir mostra como usar a operação [MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) para mover uma mensagem de email para a pasta Lixo eletrônico.</span><span class="sxs-lookup"><span data-stu-id="25b32-130">The following code example shows how to use the [MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) operation to move an email message to the Junk Email folder.</span></span> 
  
<span data-ttu-id="25b32-131">Isso também é a solicitação XML que é enviada pelo EWS Managed API ao chamar o método [Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="25b32-131">This is also the XML request that is sent by the EWS Managed API when calling the [Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="25b32-132">Os valores de alguns atributos e elementos foram diminuídos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="25b32-132">The values of some attributes and elements have been shortened for readability.</span></span> 
  
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
    <m:MoveItem>
      <m:ToFolderId>
        <t:DistinguishedFolderId Id="junkemail" />
      </m:ToFolderId>
      <m:ItemIds>
        <t:ItemId Id="AfwDoAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF25sM1" />
      </m:ItemIds>
    </m:MoveItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="25b32-133">O servidor responde à solicitação **MoveItem** com uma mensagem de [MoveItemResponse](http://msdn.microsoft.com/library/77be5104-1e09-4d50-abec-4fadb3a230e5%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que a mensagem de email foi movida com êxito.</span><span class="sxs-lookup"><span data-stu-id="25b32-133">The server responds to the **MoveItem** request with a [MoveItemResponse](http://msdn.microsoft.com/library/77be5104-1e09-4d50-abec-4fadb3a230e5%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email message was moved successfully.</span></span> <span data-ttu-id="25b32-134">A resposta também inclui o **ItemId** da mensagem de email na nova pasta, que é importante para armazenar porque o **ItemId** é diferente na nova pasta.</span><span class="sxs-lookup"><span data-stu-id="25b32-134">The response also includes the **ItemId** for the email message in the new folder, which is important to store because the **ItemId** is different in the new folder.</span></span> 
  
## <a name="copy-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="25b32-135">Copiar uma mensagem de email usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="25b32-135">Copy an email message by using the EWS Managed API</span></span>
<span data-ttu-id="25b32-136"><a name="bk_copyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="25b32-136"></span></span>

<span data-ttu-id="25b32-137">O exemplo de código a seguir mostra como usar o método [EmailMessage.Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) para copiar uma mensagem de email existentes de uma pasta para outro.</span><span class="sxs-lookup"><span data-stu-id="25b32-137">The following code example shows how to use the [EmailMessage.Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) method to copy an existing email message from one folder to another.</span></span> 
  
<span data-ttu-id="25b32-138">Este exemplo pressupõe que o **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , e esse **ItemId** é a [Id](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) da mensagem de email para copiar.</span><span class="sxs-lookup"><span data-stu-id="25b32-138">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that **ItemId** is the [Id](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the email message to copy.</span></span> <span data-ttu-id="25b32-139">Os valores de alguns parâmetros foram diminuídos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="25b32-139">The values of some parameters have been shortened for readability.</span></span> 
  
```cs
// As a best practice, limit the properties returned by the Bind method to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, EmailMessageSchema.Subject, EmailMessageSchema.ParentFolderId);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage originalMessage = EmailMessage.Bind(service, ItemId, propSet);
// Copy the orignal message into another folder in the mailbox and store the returned item.
Item item = originalMessage.Copy("epQ/3AAA=");
// Check that the item was copied by binding to the copied email message 
// and retrieving the new ParentFolderId.
// This method call results in a GetItem call to EWS.
EmailMessage copiedMessage = EmailMessage.Bind(service, item.Id, propSet);
Console.WriteLine("An email message with the subject '" + originalMessage.Subject + "' has been copied from the '" + originalMessage.ParentFolderId + "' folder to the '" + copiedMessage.ParentFolderId + "' folder.");
```

## <a name="copy-an-email-message-by-using-ews"></a><span data-ttu-id="25b32-140">Copiar uma mensagem de email usando o EWS</span><span class="sxs-lookup"><span data-stu-id="25b32-140">Copy an email message by using EWS</span></span>
<span data-ttu-id="25b32-141"><a name="bk_copyews"> </a></span><span class="sxs-lookup"><span data-stu-id="25b32-141"></span></span>

<span data-ttu-id="25b32-142">O exemplo de código a seguir mostra como usar a operação [CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) para copiar uma mensagem de email para uma pasta diferente na caixa de correio mesma enviando o [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) da mensagem de email para mover e especificando a pasta de destino no [ToFolderId ](http://msdn.microsoft.com/library/bd6a4265-ad40-43f6-bcc4-0bf5df4e984c%28Office.15%29.aspx)elemento.</span><span class="sxs-lookup"><span data-stu-id="25b32-142">The following code example shows how to use the [CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) operation to copy an email message to different folder in the same mailbox by sending the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the email message to move, and specifying the destination folder in the [ToFolderId](http://msdn.microsoft.com/library/bd6a4265-ad40-43f6-bcc4-0bf5df4e984c%28Office.15%29.aspx) element.</span></span> 
  
<span data-ttu-id="25b32-143">Isso também é a solicitação XML que é enviada pelo EWS Managed API ao chamar o método [Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="25b32-143">This is also the XML request that is sent by the EWS Managed API when calling the [Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="25b32-144">Os valores de alguns atributos e elementos foram diminuídos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="25b32-144">The values of some attributes and elements have been shortened for readability.</span></span> 
  
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
    <m:CopyItem>
      <m:ToFolderId>
        <t:FolderId Id="pQ/3AAA=" />
      </m:ToFolderId>
      <m:ItemIds>
        <t:ItemId Id="2TSeSAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF2d+3+" />
      </m:ItemIds>
    </m:CopyItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="25b32-145">O servidor responde à solicitação **CopyItem** com uma mensagem de [CopyItemResponse](http://msdn.microsoft.com/library/ae402bc1-4589-45e0-a929-f368c916a7e4%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError**, que indica que a mensagem de email foi copiada com êxito.</span><span class="sxs-lookup"><span data-stu-id="25b32-145">The server responds to the **CopyItem** request with a [CopyItemResponse](http://msdn.microsoft.com/library/ae402bc1-4589-45e0-a929-f368c916a7e4%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email message was copied successfully.</span></span> <span data-ttu-id="25b32-146">A resposta também inclui o **ItemId** da mensagem de email na nova pasta, que é importante para armazenar porque o **ItemId** é diferente na nova pasta.</span><span class="sxs-lookup"><span data-stu-id="25b32-146">The response also includes the **ItemId** for the email message in the new folder, which is important to store because the **ItemId** is different in the new folder.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="25b32-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="25b32-147">See also</span></span>


- [<span data-ttu-id="25b32-148">Email e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="25b32-148">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
    
- [<span data-ttu-id="25b32-149">Enviar mensagens de email usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="25b32-149">Send email messages by using EWS in Exchange</span></span>](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

