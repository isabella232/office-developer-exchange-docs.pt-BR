---
title: Operação MoveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveItem
api_type:
- schema
ms.assetid: dcf40fa7-7796-4a5c-bf5b-7a509a18d208
description: A operação MoveItem é usada para mover um ou mais itens para uma única pasta de destino.
ms.openlocfilehash: 6a455e483ad2e5c84b91cfaa7562f4f1ec46a112
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465678"
---
# <a name="moveitem-operation"></a><span data-ttu-id="ec4d0-103">Operação MoveItem</span><span class="sxs-lookup"><span data-stu-id="ec4d0-103">MoveItem operation</span></span>

<span data-ttu-id="ec4d0-104">A operação **MoveItem** é usada para mover um ou mais itens para uma única pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="ec4d0-104">The **MoveItem** operation is used to move one or more items to a single destination folder.</span></span> 
  
## <a name="moveitem-request-example"></a><span data-ttu-id="ec4d0-105">Exemplo de solicitação MoveItem</span><span class="sxs-lookup"><span data-stu-id="ec4d0-105">MoveItem request example</span></span>

### <a name="description"></a><span data-ttu-id="ec4d0-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec4d0-106">Description</span></span>

<span data-ttu-id="ec4d0-107">O exemplo a seguir de uma solicitação **MoveItem** mostra como mover um item para a pasta Rascunhos.</span><span class="sxs-lookup"><span data-stu-id="ec4d0-107">The following example of a **MoveItem** request shows how to move an item to the Drafts folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ec4d0-108">Código</span><span class="sxs-lookup"><span data-stu-id="ec4d0-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <MoveItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <ToFolderId>
        <t:DistinguishedFolderId Id="drafts"/>
      </ToFolderId>
      <ItemIds>
        <t:ItemId Id="AAAtAEF/swbAAA=" ChangeKey="EwAAABYA/s4b"/>
      </ItemIds>
    </MoveItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="ec4d0-109">Comentários</span><span class="sxs-lookup"><span data-stu-id="ec4d0-109">Comments</span></span>

<span data-ttu-id="ec4d0-110">O elemento [ToFolderId](tofolderid.md) especifica a pasta para a qual os itens serão movidos.</span><span class="sxs-lookup"><span data-stu-id="ec4d0-110">The [ToFolderId](tofolderid.md) element specifies the folder to which the items will be moved.</span></span> <span data-ttu-id="ec4d0-111">Observe que todos os itens listados na coleção [ItemIds](itemids.md) terminarão na pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="ec4d0-111">Note that all items listed in the [ItemIds](itemids.md) collection will end up in the destination folder.</span></span> <span data-ttu-id="ec4d0-112">Você deve fazer chamadas **MoveItem** separadas para colocar itens em pastas de destino diferentes.</span><span class="sxs-lookup"><span data-stu-id="ec4d0-112">You must make separate **MoveItem** calls to place items in different destination folders.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="ec4d0-113">O identificador de item e a chave de alteração foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ec4d0-113">The item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="ec4d0-114">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="ec4d0-114">Request elements</span></span>

<span data-ttu-id="ec4d0-115">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="ec4d0-115">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="ec4d0-116">MoveItem</span><span class="sxs-lookup"><span data-stu-id="ec4d0-116">MoveItem</span></span>](moveitem.md)
    
- [<span data-ttu-id="ec4d0-117">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="ec4d0-117">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="ec4d0-118">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="ec4d0-118">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="ec4d0-119">ItemIds</span><span class="sxs-lookup"><span data-stu-id="ec4d0-119">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="ec4d0-120">ItemId</span><span class="sxs-lookup"><span data-stu-id="ec4d0-120">ItemId</span></span>](itemid.md)
    
## <a name="moveitem-response-example"></a><span data-ttu-id="ec4d0-121">Exemplo de resposta MoveItem</span><span class="sxs-lookup"><span data-stu-id="ec4d0-121">MoveItem response example</span></span>

### <a name="description"></a><span data-ttu-id="ec4d0-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec4d0-122">Description</span></span>

<span data-ttu-id="ec4d0-123">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação **MoveItem** .</span><span class="sxs-lookup"><span data-stu-id="ec4d0-123">The following example shows a successful response to a **MoveItem** request.</span></span> 
  
<span data-ttu-id="ec4d0-124">O identificador de item do novo item é retornado na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="ec4d0-124">The item identifier of the new item is returned in the response message.</span></span> <span data-ttu-id="ec4d0-125">Os identificadores de item não são retornados em respostas para as operações de **MoveItem** de caixa de correio ou de caixa de correio de pasta pública.</span><span class="sxs-lookup"><span data-stu-id="ec4d0-125">Item identifiers are not returned in responses for cross-mailbox or mailbox to public folder **MoveItem** operations.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ec4d0-126">Código</span><span class="sxs-lookup"><span data-stu-id="ec4d0-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <MoveItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:MoveItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemID Id="AAMkAd" ChangeKey="FwAAABY" />
            </t:Message>
          </m:Items>
        </m:MoveItemResponseMessage>
      </m:ResponseMessages>
    </MoveItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="ec4d0-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="ec4d0-127">Comments</span></span>

<span data-ttu-id="ec4d0-128">A operação **MoveItem** indicará êxito se a movimentação tiver sido bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="ec4d0-128">The **MoveItem** operation will indicate success if the move was successful.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="ec4d0-129">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="ec4d0-129">Successful response elements</span></span>

<span data-ttu-id="ec4d0-130">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="ec4d0-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="ec4d0-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ec4d0-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ec4d0-132">MoveItemResponse</span><span class="sxs-lookup"><span data-stu-id="ec4d0-132">MoveItemResponse</span></span>](moveitemresponse.md)
    
- [<span data-ttu-id="ec4d0-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ec4d0-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ec4d0-134">MoveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ec4d0-134">MoveItemResponseMessage</span></span>](moveitemresponsemessage.md)
    
- [<span data-ttu-id="ec4d0-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ec4d0-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ec4d0-136">Itens</span><span class="sxs-lookup"><span data-stu-id="ec4d0-136">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="ec4d0-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="ec4d0-137">See also</span></span>



- [<span data-ttu-id="ec4d0-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ec4d0-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

