---
title: Operação CreateItem (solicitação de reunião)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: fe136881-a804-456a-8552-8a1bea5eb9c8
description: A operação CreateItem é usada para responder às solicitações de reunião.
ms.openlocfilehash: f9e6bd1742e6a30d08736ea67c0ff80b7a18e88a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457106"
---
# <a name="createitem-operation-meeting-request"></a><span data-ttu-id="3e022-103">Operação CreateItem (solicitação de reunião)</span><span class="sxs-lookup"><span data-stu-id="3e022-103">CreateItem operation (meeting request)</span></span>

<span data-ttu-id="3e022-104">A operação CreateItem é usada para responder às solicitações de reunião.</span><span class="sxs-lookup"><span data-stu-id="3e022-104">The CreateItem operation is used to respond to meeting requests.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3e022-105">Comentários</span><span class="sxs-lookup"><span data-stu-id="3e022-105">Remarks</span></span>

<span data-ttu-id="3e022-106">A operação CreateItem fornece três opções para responder a uma solicitação de reunião: aceitar, aceitar provisoriamente ou recusar.</span><span class="sxs-lookup"><span data-stu-id="3e022-106">The CreateItem operation provides three options for responding to a meeting request: accept, tentatively accept, or decline.</span></span> 
  
## <a name="accept-meeting-request-example"></a><span data-ttu-id="3e022-107">Exemplo de aceitação de solicitação de reunião</span><span class="sxs-lookup"><span data-stu-id="3e022-107">Accept Meeting request example</span></span>

### <a name="description"></a><span data-ttu-id="3e022-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e022-108">Description</span></span>

<span data-ttu-id="3e022-109">O exemplo a seguir mostra como aceitar um convite de solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="3e022-109">The following example shows how to accept a meeting request invitation.</span></span>
  
### <a name="code"></a><span data-ttu-id="3e022-110">Código</span><span class="sxs-lookup"><span data-stu-id="3e022-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                MessageDisposition="SendAndSaveCopy">
      <Items>
        <AcceptItem xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <ReferenceItemId Id="AAAlAFVzZ"
                           ChangeKey="CwAAABYAA"/>
        </AcceptItem>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="3e022-111">Comentários</span><span class="sxs-lookup"><span data-stu-id="3e022-111">Comments</span></span>

<span data-ttu-id="3e022-112">Para aceitar provisoriamente ou recusar a solicitação de reunião, use os elementos [TentativelyAcceptItem](tentativelyacceptitem.md) ou [DeclineItem](declineitem.md) no lugar do elemento [AcceptItem](acceptitem.md) .</span><span class="sxs-lookup"><span data-stu-id="3e022-112">To tentatively accept or to decline the meeting request, use the [TentativelyAcceptItem](tentativelyacceptitem.md) or [DeclineItem](declineitem.md) elements in place of the [AcceptItem](acceptitem.md) element.</span></span> 
  
<span data-ttu-id="3e022-113">O identificador de item e a chave de alteração foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3e022-113">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="accepting-meeting-request-elements"></a><span data-ttu-id="3e022-114">Aceitar elementos de solicitação de reunião</span><span class="sxs-lookup"><span data-stu-id="3e022-114">Accepting Meeting Request Elements</span></span>

<span data-ttu-id="3e022-115">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="3e022-115">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="3e022-116">CreateItem</span><span class="sxs-lookup"><span data-stu-id="3e022-116">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="3e022-117">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="3e022-117">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="3e022-118">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="3e022-118">AcceptItem</span></span>](acceptitem.md)
    
- [<span data-ttu-id="3e022-119">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="3e022-119">ReferenceItemId</span></span>](referenceitemid.md)
    
## <a name="successful-accept-meeting-response-example"></a><span data-ttu-id="3e022-120">Exemplo de resposta de reunião de aceitação bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="3e022-120">Successful Accept Meeting response example</span></span>

### <a name="description"></a><span data-ttu-id="3e022-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e022-121">Description</span></span>

<span data-ttu-id="3e022-122">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação CreateItem.</span><span class="sxs-lookup"><span data-stu-id="3e022-122">The following example shows a successful response to the CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="3e022-123">Código</span><span class="sxs-lookup"><span data-stu-id="3e022-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="3e022-124">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="3e022-124">Successful response elements</span></span>

<span data-ttu-id="3e022-125">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="3e022-125">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="3e022-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="3e022-126">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="3e022-127">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="3e022-127">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="3e022-128">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="3e022-128">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="3e022-129">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="3e022-129">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="3e022-130">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3e022-130">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="3e022-131">Itens</span><span class="sxs-lookup"><span data-stu-id="3e022-131">Items</span></span>](items.md)
    
## <a name="accept-meeting-error-response-example"></a><span data-ttu-id="3e022-132">Exemplo de resposta de erro de reunião</span><span class="sxs-lookup"><span data-stu-id="3e022-132">Accept Meeting Error response example</span></span>

### <a name="description"></a><span data-ttu-id="3e022-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e022-133">Description</span></span>

<span data-ttu-id="3e022-134">O exemplo a seguir mostra uma resposta de erro para CreateItem.</span><span class="sxs-lookup"><span data-stu-id="3e022-134">The following example shows an error response to CreateItem request.</span></span> <span data-ttu-id="3e022-135">O erro é causado por uma tentativa de aceitar uma solicitação de reunião que não pode ser encontrada no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3e022-135">The error is caused by an attempt to accept a meeting request that cannot be found in the Exchange store.</span></span>
  
### <a name="code"></a><span data-ttu-id="3e022-136">Código</span><span class="sxs-lookup"><span data-stu-id="3e022-136">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
  xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="3e022-137">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="3e022-137">Error response elements</span></span>

<span data-ttu-id="3e022-138">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="3e022-138">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="3e022-139">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="3e022-139">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="3e022-140">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="3e022-140">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="3e022-141">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="3e022-141">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="3e022-142">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="3e022-142">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="3e022-143">MessageText</span><span class="sxs-lookup"><span data-stu-id="3e022-143">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="3e022-144">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3e022-144">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="3e022-145">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="3e022-145">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="3e022-146">Itens</span><span class="sxs-lookup"><span data-stu-id="3e022-146">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="3e022-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="3e022-147">See also</span></span>



[<span data-ttu-id="3e022-148">Operação CreateItem</span><span class="sxs-lookup"><span data-stu-id="3e022-148">CreateItem operation</span></span>](createitem-operation.md)
  
[<span data-ttu-id="3e022-149">Operação CreateItem (item de calendário)</span><span class="sxs-lookup"><span data-stu-id="3e022-149">CreateItem operation (calendar item)</span></span>](createitem-operation-calendar-item.md)

