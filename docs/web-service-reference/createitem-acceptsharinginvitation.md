---
title: CreateItem (AcceptSharingInvitation)
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
ms.assetid: 710c893a-3037-4f04-b336-aefedd36c406
description: A operação CreateItem é usada para aceitar um convite para compartilhar os dados do calendário ou contatos de outro usuário.
ms.openlocfilehash: eda846b72f42fe886497b355d9cddade7c5f4044
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457512"
---
# <a name="createitem-acceptsharinginvitation"></a><span data-ttu-id="37b9e-103">CreateItem (AcceptSharingInvitation)</span><span class="sxs-lookup"><span data-stu-id="37b9e-103">CreateItem (AcceptSharingInvitation)</span></span>

<span data-ttu-id="37b9e-104">A operação **CreateItem** é usada para aceitar um convite para compartilhar os dados do calendário ou contatos de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="37b9e-104">The **CreateItem** operation is used to accept an invitation to share another user's calendar or contacts data.</span></span> 
  
## <a name="accept-sharing-invitation-request-example"></a><span data-ttu-id="37b9e-105">Exemplo de solicitação de convite de compartilhamento de aceitação</span><span class="sxs-lookup"><span data-stu-id="37b9e-105">Accept Sharing Invitation request example</span></span>

### <a name="description"></a><span data-ttu-id="37b9e-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="37b9e-106">Description</span></span>

<span data-ttu-id="37b9e-107">O exemplo a seguir mostra como aceitar um convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="37b9e-107">The following example shows how to accept a sharing invitation.</span></span>
  
### <a name="code"></a><span data-ttu-id="37b9e-108">Código</span><span class="sxs-lookup"><span data-stu-id="37b9e-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Items xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <AcceptSharingInvitation xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <ReferenceItemId Id="AAAlAFVzZ" ChangeKey="CwAAABYAA" />
        </AcceptSharingInvitation>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="37b9e-109">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="37b9e-109">Request elements</span></span>

<span data-ttu-id="37b9e-110">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="37b9e-110">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="37b9e-111">CreateItem</span><span class="sxs-lookup"><span data-stu-id="37b9e-111">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="37b9e-112">Itens</span><span class="sxs-lookup"><span data-stu-id="37b9e-112">Items</span></span>](items.md)
    
- [<span data-ttu-id="37b9e-113">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="37b9e-113">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md)
    
- [<span data-ttu-id="37b9e-114">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="37b9e-114">ReferenceItemId</span></span>](referenceitemid.md)
    
### <a name="comments"></a><span data-ttu-id="37b9e-115">Comentários</span><span class="sxs-lookup"><span data-stu-id="37b9e-115">Comments</span></span>

<span data-ttu-id="37b9e-116">O identificador de item e a chave de alteração foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="37b9e-116">The item identifier and change key have been shortened to preserve readability.</span></span>
  
## <a name="successful-accept-sharing-invitation-response-example"></a><span data-ttu-id="37b9e-117">Exemplo de resposta de convite para aceitar compartilhamento bem-sucedido</span><span class="sxs-lookup"><span data-stu-id="37b9e-117">Successful Accept Sharing Invitation response example</span></span>

### <a name="description"></a><span data-ttu-id="37b9e-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="37b9e-118">Description</span></span>

<span data-ttu-id="37b9e-119">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação **CreateItem** .</span><span class="sxs-lookup"><span data-stu-id="37b9e-119">The following example shows a successful response to a **CreateItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="37b9e-120">Código</span><span class="sxs-lookup"><span data-stu-id="37b9e-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
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

### <a name="successful-response-elements"></a><span data-ttu-id="37b9e-121">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="37b9e-121">Successful response elements</span></span>

<span data-ttu-id="37b9e-122">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="37b9e-122">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="37b9e-123">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="37b9e-123">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="37b9e-124">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="37b9e-124">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="37b9e-125">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="37b9e-125">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="37b9e-126">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="37b9e-126">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="37b9e-127">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="37b9e-127">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="37b9e-128">Itens</span><span class="sxs-lookup"><span data-stu-id="37b9e-128">Items</span></span>](items.md)
    
## <a name="accept-sharing-invitation-error-response-example"></a><span data-ttu-id="37b9e-129">Exemplo de resposta de erro de convite de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="37b9e-129">Accept Sharing Invitation Error response example</span></span>

### <a name="description"></a><span data-ttu-id="37b9e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="37b9e-130">Description</span></span>

<span data-ttu-id="37b9e-131">O exemplo a seguir mostra uma resposta de erro a uma solicitação **CreateItem** .</span><span class="sxs-lookup"><span data-stu-id="37b9e-131">The following example shows an error response to a **CreateItem** request.</span></span> <span data-ttu-id="37b9e-132">O erro é causado por uma tentativa de aceitar um convite de compartilhamento que não pode ser encontrado no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="37b9e-132">The error is caused by an attempt to accept a sharing invitation that cannot be found in the Exchange store.</span></span> 
  
### <a name="code"></a><span data-ttu-id="37b9e-133">Código</span><span class="sxs-lookup"><span data-stu-id="37b9e-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
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

### <a name="error-response-elements"></a><span data-ttu-id="37b9e-134">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="37b9e-134">Error response elements</span></span>

<span data-ttu-id="37b9e-135">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="37b9e-135">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="37b9e-136">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="37b9e-136">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="37b9e-137">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="37b9e-137">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="37b9e-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="37b9e-138">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="37b9e-139">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="37b9e-139">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="37b9e-140">MessageText</span><span class="sxs-lookup"><span data-stu-id="37b9e-140">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="37b9e-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="37b9e-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="37b9e-142">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="37b9e-142">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="37b9e-143">Itens</span><span class="sxs-lookup"><span data-stu-id="37b9e-143">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="37b9e-144">Também consulte</span><span class="sxs-lookup"><span data-stu-id="37b9e-144">See also</span></span>



[<span data-ttu-id="37b9e-145">Operação CreateItem</span><span class="sxs-lookup"><span data-stu-id="37b9e-145">CreateItem operation</span></span>](createitem-operation.md)

