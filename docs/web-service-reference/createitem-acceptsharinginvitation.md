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
description: A operação CreateItem é usada para aceitar um convite para compartilhar o calendário de outro usuário ou de dados de contatos.
ms.openlocfilehash: 993ef0402e624af69f632af5bdce4c02bd9d41f3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751596"
---
# <a name="createitem-acceptsharinginvitation"></a><span data-ttu-id="f88f5-103">CreateItem (AcceptSharingInvitation)</span><span class="sxs-lookup"><span data-stu-id="f88f5-103">CreateItem (AcceptSharingInvitation)</span></span>

<span data-ttu-id="f88f5-104">A operação **CreateItem** é usada para aceitar um convite para compartilhar o calendário de outro usuário ou de dados de contatos.</span><span class="sxs-lookup"><span data-stu-id="f88f5-104">The **CreateItem** operation is used to accept an invitation to share another user's calendar or contacts data.</span></span> 
  
## <a name="accept-sharing-invitation-request-example"></a><span data-ttu-id="f88f5-105">Aceitar um exemplo de solicitação de convite de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="f88f5-105">Accept Sharing Invitation request example</span></span>

### <a name="description"></a><span data-ttu-id="f88f5-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="f88f5-106">Description</span></span>

<span data-ttu-id="f88f5-107">O exemplo a seguir mostra como aceitar um convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="f88f5-107">The following example shows how to accept a sharing invitation.</span></span>
  
### <a name="code"></a><span data-ttu-id="f88f5-108">Código</span><span class="sxs-lookup"><span data-stu-id="f88f5-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Items xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <AcceptSharingInvitation xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <ReferenceItemId Id="AAAlAFVzZ" ChangeKey="CwAAABYAA" />
        </AcceptSharingInvitation>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="f88f5-109">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f88f5-109">Request elements</span></span>

<span data-ttu-id="f88f5-110">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="f88f5-110">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="f88f5-111">CreateItem</span><span class="sxs-lookup"><span data-stu-id="f88f5-111">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="f88f5-112">Items</span><span class="sxs-lookup"><span data-stu-id="f88f5-112">Items</span></span>](items.md)
    
- [<span data-ttu-id="f88f5-113">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="f88f5-113">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md)
    
- [<span data-ttu-id="f88f5-114">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="f88f5-114">ReferenceItemId</span></span>](referenceitemid.md)
    
### <a name="comments"></a><span data-ttu-id="f88f5-115">Comments</span><span class="sxs-lookup"><span data-stu-id="f88f5-115">Comments</span></span>

<span data-ttu-id="f88f5-116">O identificador do item e alterar chave foram diminuídas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f88f5-116">The item identifier and change key have been shortened to preserve readability.</span></span>
  
## <a name="successful-accept-sharing-invitation-response-example"></a><span data-ttu-id="f88f5-117">Exemplo de resposta bem-sucedida aceitar o convite de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="f88f5-117">Successful Accept Sharing Invitation response example</span></span>

### <a name="description"></a><span data-ttu-id="f88f5-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="f88f5-118">Description</span></span>

<span data-ttu-id="f88f5-119">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de **CreateItem** .</span><span class="sxs-lookup"><span data-stu-id="f88f5-119">The following example shows a successful response to a **CreateItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f88f5-120">Código</span><span class="sxs-lookup"><span data-stu-id="f88f5-120">Code</span></span>

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
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a><span data-ttu-id="f88f5-121">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="f88f5-121">Successful response elements</span></span>

<span data-ttu-id="f88f5-122">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="f88f5-122">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="f88f5-123">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f88f5-123">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="f88f5-124">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="f88f5-124">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="f88f5-125">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f88f5-125">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="f88f5-126">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f88f5-126">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="f88f5-127">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f88f5-127">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f88f5-128">Items</span><span class="sxs-lookup"><span data-stu-id="f88f5-128">Items</span></span>](items.md)
    
## <a name="accept-sharing-invitation-error-response-example"></a><span data-ttu-id="f88f5-129">Aceitar um exemplo de resposta de erro de convite de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="f88f5-129">Accept Sharing Invitation Error response example</span></span>

### <a name="description"></a><span data-ttu-id="f88f5-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="f88f5-130">Description</span></span>

<span data-ttu-id="f88f5-131">O exemplo a seguir mostra uma resposta de erro a uma solicitação de **CreateItem** .</span><span class="sxs-lookup"><span data-stu-id="f88f5-131">The following example shows an error response to a **CreateItem** request.</span></span> <span data-ttu-id="f88f5-132">O erro é gerado por uma tentativa de aceitar um convite de compartilhamento que não pode ser encontrado no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f88f5-132">The error is caused by an attempt to accept a sharing invitation that cannot be found in the Exchange store.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f88f5-133">Código</span><span class="sxs-lookup"><span data-stu-id="f88f5-133">Code</span></span>

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
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="f88f5-134">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="f88f5-134">Error response elements</span></span>

<span data-ttu-id="f88f5-135">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="f88f5-135">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="f88f5-136">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f88f5-136">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="f88f5-137">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="f88f5-137">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="f88f5-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f88f5-138">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="f88f5-139">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f88f5-139">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="f88f5-140">MessageText</span><span class="sxs-lookup"><span data-stu-id="f88f5-140">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="f88f5-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f88f5-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f88f5-142">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f88f5-142">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="f88f5-143">Items</span><span class="sxs-lookup"><span data-stu-id="f88f5-143">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="f88f5-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="f88f5-144">See also</span></span>



[<span data-ttu-id="f88f5-145">Operação CreateItem</span><span class="sxs-lookup"><span data-stu-id="f88f5-145">CreateItem operation</span></span>](createitem-operation.md)

