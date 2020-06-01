---
title: ArchiveItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2ac58d6f-e019-4352-b82f-8ac67a171e63
description: O elemento ArchiveItemResponseMessage especifica a mensagem de resposta para uma solicitação ArchiveItem.
ms.openlocfilehash: 24d09d63cab6805194e35031d8590290573de0a9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463388"
---
# <a name="archiveitemresponsemessage"></a><span data-ttu-id="8701d-103">ArchiveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8701d-103">ArchiveItemResponseMessage</span></span>

<span data-ttu-id="8701d-104">O elemento **ArchiveItemResponseMessage** especifica a mensagem de resposta para uma solicitação **ArchiveItem** .</span><span class="sxs-lookup"><span data-stu-id="8701d-104">The **ArchiveItemResponseMessage** element specifies the response message to an **ArchiveItem** request.</span></span> 
  
```XML
<ArchiveItemResponseMessage ResponseClass="">
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
    <Items></Items>
</ArchiveItemResponseMessage>
```

 <span data-ttu-id="8701d-105">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="8701d-105">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8701d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8701d-106">Attributes and elements</span></span>

<span data-ttu-id="8701d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8701d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8701d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8701d-108">Attributes</span></span>

|<span data-ttu-id="8701d-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="8701d-109">**Attribute**</span></span>|<span data-ttu-id="8701d-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8701d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8701d-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="8701d-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="8701d-112">Indica a classe da resposta.</span><span class="sxs-lookup"><span data-stu-id="8701d-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="8701d-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="8701d-113">ResponseClass</span></span>

|<span data-ttu-id="8701d-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="8701d-114">**Value**</span></span>|<span data-ttu-id="8701d-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8701d-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8701d-116">Êxito</span><span class="sxs-lookup"><span data-stu-id="8701d-116">Success</span></span>  <br/> |<span data-ttu-id="8701d-117">Indica êxito.</span><span class="sxs-lookup"><span data-stu-id="8701d-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="8701d-118">Aviso</span><span class="sxs-lookup"><span data-stu-id="8701d-118">Warning</span></span>  <br/> |<span data-ttu-id="8701d-119">Indica um aviso.</span><span class="sxs-lookup"><span data-stu-id="8701d-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="8701d-120">Erro</span><span class="sxs-lookup"><span data-stu-id="8701d-120">Error</span></span>  <br/> |<span data-ttu-id="8701d-121">Indica um erro.</span><span class="sxs-lookup"><span data-stu-id="8701d-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8701d-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8701d-122">Child elements</span></span>

|<span data-ttu-id="8701d-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8701d-123">**Element**</span></span>|<span data-ttu-id="8701d-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8701d-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8701d-125">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="8701d-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="8701d-126">Atualmente não usado e reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="8701d-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="8701d-127">Itens</span><span class="sxs-lookup"><span data-stu-id="8701d-127">Items</span></span>](items.md) <br/> |<span data-ttu-id="8701d-128">Contém uma matriz de itens.</span><span class="sxs-lookup"><span data-stu-id="8701d-128">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="8701d-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="8701d-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="8701d-130">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="8701d-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="8701d-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="8701d-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="8701d-132">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="8701d-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="8701d-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8701d-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="8701d-134">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="8701d-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8701d-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8701d-135">Parent elements</span></span>

|<span data-ttu-id="8701d-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8701d-136">**Element**</span></span>|<span data-ttu-id="8701d-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8701d-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8701d-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8701d-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="8701d-139">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8701d-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8701d-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="8701d-140">Remarks</span></span>

<span data-ttu-id="8701d-141">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8701d-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8701d-142">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8701d-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8701d-143">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="8701d-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8701d-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="8701d-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8701d-145">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8701d-145">Schema Name</span></span>  <br/> |<span data-ttu-id="8701d-146">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="8701d-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="8701d-147">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8701d-147">Validation File</span></span>  <br/> |<span data-ttu-id="8701d-148">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="8701d-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8701d-149">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="8701d-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="8701d-150">Também consulte</span><span class="sxs-lookup"><span data-stu-id="8701d-150">See also</span></span>

- [<span data-ttu-id="8701d-151">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8701d-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

