---
title: Mover e copiar mensagens de email usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 4771668f-5623-4397-a5c0-b75a7ba01698
description: Saiba como mover e copiar mensagens de email usando a API gerenciada do EWS ou o EWS no Exchange.
localization_priority: Priority
ms.openlocfilehash: d13e84648f194dd4f431cf128396daf016addb22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527933"
---
# <a name="move-and-copy-email-messages-by-using-ews-in-exchange"></a><span data-ttu-id="77727-103">Mover e copiar mensagens de email usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="77727-103">Move and copy email messages by using EWS in Exchange</span></span>

<span data-ttu-id="77727-104">Saiba como mover e copiar mensagens de email usando a API gerenciada do EWS ou o EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="77727-104">Learn how to move and copy email messages by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="77727-105">Você pode usar a API gerenciada do EWS ou o EWS para mover e copiar mensagens de email em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="77727-105">You can use the EWS Managed API or EWS to move and copy email messages in a mailbox.</span></span>
  
<span data-ttu-id="77727-106">**Tabela 1. Métodos da API gerenciada do EWS e operações do EWS para mover e copiar mensagens de email**</span><span class="sxs-lookup"><span data-stu-id="77727-106">**Table 1. EWS Managed API methods and EWS operations for moving and copying email messages**</span></span>

|<span data-ttu-id="77727-107">**Tarefa**</span><span class="sxs-lookup"><span data-stu-id="77727-107">**Task**</span></span>|<span data-ttu-id="77727-108">**Método de API gerenciada do EWS**</span><span class="sxs-lookup"><span data-stu-id="77727-108">**EWS Managed API method**</span></span>|<span data-ttu-id="77727-109">**Operação do EWS**</span><span class="sxs-lookup"><span data-stu-id="77727-109">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="77727-110">Mover uma mensagem de email</span><span class="sxs-lookup"><span data-stu-id="77727-110">Move an email message</span></span>  <br/> |[<span data-ttu-id="77727-111">EmailMessage. move</span><span class="sxs-lookup"><span data-stu-id="77727-111">EmailMessage.Move</span></span>](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="77727-112">MoveItem</span><span class="sxs-lookup"><span data-stu-id="77727-112">MoveItem</span></span>](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="77727-113">Copiar uma mensagem de email</span><span class="sxs-lookup"><span data-stu-id="77727-113">Copy an email message</span></span>  <br/> |[<span data-ttu-id="77727-114">EmailMessage. Copy</span><span class="sxs-lookup"><span data-stu-id="77727-114">EmailMessage.Copy</span></span>](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="77727-115">CopyItem</span><span class="sxs-lookup"><span data-stu-id="77727-115">CopyItem</span></span>](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="77727-116">É importante observar que quando você move ou copia uma mensagem de email em uma pasta diferente, um novo item é criado na nova pasta com uma ID de item exclusivo e a mensagem original é excluída.</span><span class="sxs-lookup"><span data-stu-id="77727-116">It's important to note that when you move or copy an email message into a different folder, a new item is created in the new folder with a unique item ID, and the original message is deleted.</span></span> <span data-ttu-id="77727-117">Se você estiver movendo ou copiando uma mensagem de email entre duas pastas na mesma caixa de correio, o novo item será retornado na resposta, o que fornece acesso à nova ID de item.</span><span class="sxs-lookup"><span data-stu-id="77727-117">If you're moving or copying an email message between two folders in the same mailbox, the new item is returned in the response, which gives you access to the new item ID.</span></span> <span data-ttu-id="77727-118">No entanto, se você estiver movendo ou copiando uma mensagem de email entre duas caixas de correio ou entre uma caixa de correio e uma pasta pública, o novo item não será retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="77727-118">However, if you're moving or copying an email message between two mailboxes or between a mailbox and a public folder, the new item is not returned in the response.</span></span> <span data-ttu-id="77727-119">Para acessar a mensagem movida nesse cenário, use o método [FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) da API gerenciada do EWS ou a operação do EWS [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , [crie uma definição de propriedade estendida](properties-and-extended-properties-in-ews-in-exchange.md) para a propriedade [PidTagSearchKey](https://msdn.microsoft.com/library/cc839918.aspx) (0x300B0102), ou crie e defina uma propriedade estendida personalizada e, em seguida, procure a propriedade estendida personalizada na nova pasta.</span><span class="sxs-lookup"><span data-stu-id="77727-119">To access the moved message in that scenario, use the EWS Managed API [FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) method or EWS [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation, [create an extended property definition](properties-and-extended-properties-in-ews-in-exchange.md) for the [PidTagSearchKey](https://msdn.microsoft.com/library/cc839918.aspx) (0x300B0102) property, or create and set a custom extended property and then search for the custom extended property in the new folder.</span></span> 
  
<span data-ttu-id="77727-120">Excluir uma mensagem de email é diferente de mover um item para a pasta itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="77727-120">Deleting an email message is different than moving an item to the Deleted Items folder.</span></span> <span data-ttu-id="77727-121">Se você usar o item da API gerenciada do EWS [. Delete](https://msdn.microsoft.com/library/office/dd635072%28v=exchg.80%29.aspx) ou a operação do EWS [DeleteItem](../web-service-reference/deleteitem-operation.md) , o item especificado na solicitação será removido da pasta original e uma cópia será colocada na pasta itens excluídos com uma nova ID de item.</span><span class="sxs-lookup"><span data-stu-id="77727-121">If you use the EWS Managed API [Item.Delete](https://msdn.microsoft.com/library/office/dd635072%28v=exchg.80%29.aspx) method or the EWS [DeleteItem](../web-service-reference/deleteitem-operation.md) operation, the item specified in the request is removed from the original folder, and a copy is placed in the Deleted Items folder with a new item ID.</span></span> <span data-ttu-id="77727-122">Diferentemente de quando você move ou copia qualquer item, o novo item não é retornado no método **delete** ou a resposta da operação **DeleteItem** .</span><span class="sxs-lookup"><span data-stu-id="77727-122">Unlike when you move or copy any item, the new item is not returned in the **Delete** method or the **DeleteItem** operation response.</span></span> <span data-ttu-id="77727-123">As etapas envolvidas na [exclusão de um email usando a API gerenciada do EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) ou [EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) são as mesmas que as para excluir qualquer item genérico do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="77727-123">The steps involved in [deleting an email by using the EWS Managed API](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) or [EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) are the same as those for deleting any generic item from the Exchange store.</span></span> 
  
## <a name="move-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="77727-124">Mover uma mensagem de email usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="77727-124">Move an email message by using the EWS Managed API</span></span>
<span data-ttu-id="77727-125"><a name="bk_moveewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="77727-125"><a name="bk_moveewsma"> </a></span></span>

<span data-ttu-id="77727-126">O exemplo de código a seguir mostra como usar o método [EmailMessage. move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) para mover uma mensagem de email existente de uma pasta para outra.</span><span class="sxs-lookup"><span data-stu-id="77727-126">The following code example shows how to use the [EmailMessage.Move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) method to move an existing email message from one folder to another.</span></span> 
  
<span data-ttu-id="77727-127">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que **ItemId** é a [ID](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) da mensagem de email a ser movida ou copiada.</span><span class="sxs-lookup"><span data-stu-id="77727-127">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that **ItemId** is the [Id](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the email message to move or copy.</span></span> 
  
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

## <a name="move-an-email-message-by-using-ews"></a><span data-ttu-id="77727-128">Mover uma mensagem de email usando o EWS</span><span class="sxs-lookup"><span data-stu-id="77727-128">Move an email message by using EWS</span></span>
<span data-ttu-id="77727-129"><a name="bk_moveews"> </a></span><span class="sxs-lookup"><span data-stu-id="77727-129"><a name="bk_moveews"> </a></span></span>

<span data-ttu-id="77727-130">O exemplo de código a seguir mostra como usar a operação [MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) para mover uma mensagem de email para a pasta lixo eletrônico.</span><span class="sxs-lookup"><span data-stu-id="77727-130">The following code example shows how to use the [MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) operation to move an email message to the Junk Email folder.</span></span> 
  
<span data-ttu-id="77727-131">Essa é também a solicitação XML que é enviada pela API gerenciada do EWS ao chamar o método [move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="77727-131">This is also the XML request that is sent by the EWS Managed API when calling the [Move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="77727-132">Os valores de alguns atributos e elementos foram reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="77727-132">The values of some attributes and elements have been shortened for readability.</span></span> 
  
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

<span data-ttu-id="77727-133">O servidor responde à solicitação **MoveItem** com uma mensagem [MoveItemResponse](https://msdn.microsoft.com/library/77be5104-1e09-4d50-abec-4fadb3a230e5%28Office.15%29.aspx) que inclui um valor de [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que a mensagem de email foi movida com êxito.</span><span class="sxs-lookup"><span data-stu-id="77727-133">The server responds to the **MoveItem** request with a [MoveItemResponse](https://msdn.microsoft.com/library/77be5104-1e09-4d50-abec-4fadb3a230e5%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email message was moved successfully.</span></span> <span data-ttu-id="77727-134">A resposta também inclui o **ItemId** para a mensagem de email na nova pasta, o que é importante armazenar porque **ItemId** é diferente na nova pasta.</span><span class="sxs-lookup"><span data-stu-id="77727-134">The response also includes the **ItemId** for the email message in the new folder, which is important to store because the **ItemId** is different in the new folder.</span></span> 
  
## <a name="copy-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="77727-135">Copiar uma mensagem de email usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="77727-135">Copy an email message by using the EWS Managed API</span></span>
<span data-ttu-id="77727-136"><a name="bk_copyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="77727-136"><a name="bk_copyewsma"> </a></span></span>

<span data-ttu-id="77727-137">O exemplo de código a seguir mostra como usar o método [EmailMessage. Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) para copiar uma mensagem de email existente de uma pasta para outra.</span><span class="sxs-lookup"><span data-stu-id="77727-137">The following code example shows how to use the [EmailMessage.Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) method to copy an existing email message from one folder to another.</span></span> 
  
<span data-ttu-id="77727-138">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que **ItemId** é a [ID](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) da mensagem de email a ser copiada.</span><span class="sxs-lookup"><span data-stu-id="77727-138">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that **ItemId** is the [Id](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the email message to copy.</span></span> <span data-ttu-id="77727-139">Os valores de alguns parâmetros foram reduzidos para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="77727-139">The values of some parameters have been shortened for readability.</span></span> 
  
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

## <a name="copy-an-email-message-by-using-ews"></a><span data-ttu-id="77727-140">Copiar uma mensagem de email usando EWS</span><span class="sxs-lookup"><span data-stu-id="77727-140">Copy an email message by using EWS</span></span>
<span data-ttu-id="77727-141"><a name="bk_copyews"> </a></span><span class="sxs-lookup"><span data-stu-id="77727-141"><a name="bk_copyews"> </a></span></span>

<span data-ttu-id="77727-142">O exemplo de código a seguir mostra como usar a operação [CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) para copiar uma mensagem de email para uma pasta diferente na mesma caixa de correio enviando o [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) da mensagem de email a ser movida e especificando a pasta de destino no elemento [ToFolderId](https://msdn.microsoft.com/library/bd6a4265-ad40-43f6-bcc4-0bf5df4e984c%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="77727-142">The following code example shows how to use the [CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) operation to copy an email message to different folder in the same mailbox by sending the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the email message to move, and specifying the destination folder in the [ToFolderId](https://msdn.microsoft.com/library/bd6a4265-ad40-43f6-bcc4-0bf5df4e984c%28Office.15%29.aspx) element.</span></span> 
  
<span data-ttu-id="77727-143">Essa é também a solicitação XML que é enviada pela API gerenciada do EWS ao chamar o método [Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="77727-143">This is also the XML request that is sent by the EWS Managed API when calling the [Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="77727-144">Os valores de alguns atributos e elementos foram reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="77727-144">The values of some attributes and elements have been shortened for readability.</span></span> 
  
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

<span data-ttu-id="77727-145">O servidor responde à solicitação **CopyItem** com uma mensagem [CopyItemResponse](https://msdn.microsoft.com/library/ae402bc1-4589-45e0-a929-f368c916a7e4%28Office.15%29.aspx) que inclui um valor de [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica que a mensagem de email foi copiada com êxito.</span><span class="sxs-lookup"><span data-stu-id="77727-145">The server responds to the **CopyItem** request with a [CopyItemResponse](https://msdn.microsoft.com/library/ae402bc1-4589-45e0-a929-f368c916a7e4%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email message was copied successfully.</span></span> <span data-ttu-id="77727-146">A resposta também inclui o **ItemId** para a mensagem de email na nova pasta, o que é importante armazenar porque **ItemId** é diferente na nova pasta.</span><span class="sxs-lookup"><span data-stu-id="77727-146">The response also includes the **ItemId** for the email message in the new folder, which is important to store because the **ItemId** is different in the new folder.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="77727-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="77727-147">See also</span></span>


- [<span data-ttu-id="77727-148">Email e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="77727-148">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
    
- [<span data-ttu-id="77727-149">Enviar mensagens de email usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="77727-149">Send email messages by using EWS in Exchange</span></span>](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

