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
description: A operação MoveItem é usada para mover um ou mais itens para uma pasta de destino único.
ms.openlocfilehash: c5619befb02ec20ef0911992484dcc00cc2c5e92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824492"
---
# <a name="moveitem-operation"></a><span data-ttu-id="aa358-103">Operação MoveItem</span><span class="sxs-lookup"><span data-stu-id="aa358-103">MoveItem operation</span></span>

<span data-ttu-id="aa358-104">A operação **MoveItem** é usada para mover um ou mais itens para uma pasta de destino único.</span><span class="sxs-lookup"><span data-stu-id="aa358-104">The **MoveItem** operation is used to move one or more items to a single destination folder.</span></span> 
  
## <a name="moveitem-request-example"></a><span data-ttu-id="aa358-105">Exemplo de solicitação MoveItem</span><span class="sxs-lookup"><span data-stu-id="aa358-105">MoveItem request example</span></span>

### <a name="description"></a><span data-ttu-id="aa358-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa358-106">Description</span></span>

<span data-ttu-id="aa358-107">O exemplo a seguir de uma solicitação de **MoveItem** mostra como mover um item na pasta Rascunhos.</span><span class="sxs-lookup"><span data-stu-id="aa358-107">The following example of a **MoveItem** request shows how to move an item to the Drafts folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="aa358-108">Código</span><span class="sxs-lookup"><span data-stu-id="aa358-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <MoveItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comments"></a><span data-ttu-id="aa358-109">Comments</span><span class="sxs-lookup"><span data-stu-id="aa358-109">Comments</span></span>

<span data-ttu-id="aa358-110">O elemento [ToFolderId](tofolderid.md) Especifica a pasta para a qual os itens serão movidos.</span><span class="sxs-lookup"><span data-stu-id="aa358-110">The [ToFolderId](tofolderid.md) element specifies the folder to which the items will be moved.</span></span> <span data-ttu-id="aa358-111">Observe que todos os itens listados na coleção [ItemIds](itemids.md) terminarão na pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="aa358-111">Note that all items listed in the [ItemIds](itemids.md) collection will end up in the destination folder.</span></span> <span data-ttu-id="aa358-112">Você deve fazer chamadas de **MoveItem** separadas colocar itens em pastas de destino diferente.</span><span class="sxs-lookup"><span data-stu-id="aa358-112">You must make separate **MoveItem** calls to place items in different destination folders.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="aa358-113">O identificador do item e alterar chave foram diminuídas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="aa358-113">The item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="aa358-114">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="aa358-114">Request elements</span></span>

<span data-ttu-id="aa358-115">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="aa358-115">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="aa358-116">MoveItem</span><span class="sxs-lookup"><span data-stu-id="aa358-116">MoveItem</span></span>](moveitem.md)
    
- [<span data-ttu-id="aa358-117">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="aa358-117">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="aa358-118">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="aa358-118">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="aa358-119">ItemIds</span><span class="sxs-lookup"><span data-stu-id="aa358-119">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="aa358-120">ItemId</span><span class="sxs-lookup"><span data-stu-id="aa358-120">ItemId</span></span>](itemid.md)
    
## <a name="moveitem-response-example"></a><span data-ttu-id="aa358-121">Exemplo de resposta MoveItem</span><span class="sxs-lookup"><span data-stu-id="aa358-121">MoveItem response example</span></span>

### <a name="description"></a><span data-ttu-id="aa358-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa358-122">Description</span></span>

<span data-ttu-id="aa358-123">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de **MoveItem** .</span><span class="sxs-lookup"><span data-stu-id="aa358-123">The following example shows a successful response to a **MoveItem** request.</span></span> 
  
<span data-ttu-id="aa358-124">O identificador do item do novo item será retornado na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="aa358-124">The item identifier of the new item is returned in the response message.</span></span> <span data-ttu-id="aa358-125">Identificadores de item não são retornados em respostas em entre caixas de correio ou de caixa de correio para operações de **MoveItem** de pasta pública.</span><span class="sxs-lookup"><span data-stu-id="aa358-125">Item identifiers are not returned in responses for cross-mailbox or mailbox to public folder **MoveItem** operations.</span></span> 
  
### <a name="code"></a><span data-ttu-id="aa358-126">Código</span><span class="sxs-lookup"><span data-stu-id="aa358-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <MoveItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="aa358-127">Comments</span><span class="sxs-lookup"><span data-stu-id="aa358-127">Comments</span></span>

<span data-ttu-id="aa358-128">A operação **MoveItem** indicará êxito se a movimentação não tiver sido bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="aa358-128">The **MoveItem** operation will indicate success if the move was successful.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="aa358-129">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="aa358-129">Successful response elements</span></span>

<span data-ttu-id="aa358-130">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="aa358-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="aa358-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="aa358-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="aa358-132">MoveItemResponse</span><span class="sxs-lookup"><span data-stu-id="aa358-132">MoveItemResponse</span></span>](moveitemresponse.md)
    
- [<span data-ttu-id="aa358-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="aa358-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="aa358-134">MoveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="aa358-134">MoveItemResponseMessage</span></span>](moveitemresponsemessage.md)
    
- [<span data-ttu-id="aa358-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="aa358-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="aa358-136">Items</span><span class="sxs-lookup"><span data-stu-id="aa358-136">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="aa358-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="aa358-137">See also</span></span>



- [<span data-ttu-id="aa358-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="aa358-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

