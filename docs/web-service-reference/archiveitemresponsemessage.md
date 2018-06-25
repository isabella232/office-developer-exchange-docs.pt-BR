---
title: ArchiveItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2ac58d6f-e019-4352-b82f-8ac67a171e63
description: O elemento ArchiveItemResponseMessage Especifica a mensagem de resposta a uma solicitação ArchiveItem.
ms.openlocfilehash: a7832e2cb4ec91a0871de5979fd1b418c0626aa6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751202"
---
# <a name="archiveitemresponsemessage"></a><span data-ttu-id="c92a6-103">ArchiveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c92a6-103">ArchiveItemResponseMessage</span></span>

<span data-ttu-id="c92a6-104">O elemento **ArchiveItemResponseMessage** Especifica a mensagem de resposta a uma solicitação **ArchiveItem** .</span><span class="sxs-lookup"><span data-stu-id="c92a6-104">The **ArchiveItemResponseMessage** element specifies the response message to an **ArchiveItem** request.</span></span> 
  
```XML
<ArchiveItemResponseMessage ResponseClass="">
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
    <Items></Items>
</ArchiveItemResponseMessage>
```

 <span data-ttu-id="c92a6-105">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="c92a6-105">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c92a6-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c92a6-106">Attributes and elements</span></span>

<span data-ttu-id="c92a6-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c92a6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c92a6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c92a6-108">Attributes</span></span>

|<span data-ttu-id="c92a6-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="c92a6-109">**Attribute**</span></span>|<span data-ttu-id="c92a6-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c92a6-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c92a6-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="c92a6-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="c92a6-112">Indica a classe da resposta.</span><span class="sxs-lookup"><span data-stu-id="c92a6-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="c92a6-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="c92a6-113">ResponseClass</span></span>

|<span data-ttu-id="c92a6-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="c92a6-114">**Value**</span></span>|<span data-ttu-id="c92a6-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c92a6-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c92a6-116">Êxito</span><span class="sxs-lookup"><span data-stu-id="c92a6-116">Success</span></span>  <br/> |<span data-ttu-id="c92a6-117">Indica o sucesso.</span><span class="sxs-lookup"><span data-stu-id="c92a6-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="c92a6-118">Aviso</span><span class="sxs-lookup"><span data-stu-id="c92a6-118">Warning</span></span>  <br/> |<span data-ttu-id="c92a6-119">Indica um aviso.</span><span class="sxs-lookup"><span data-stu-id="c92a6-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="c92a6-120">Erro</span><span class="sxs-lookup"><span data-stu-id="c92a6-120">Error</span></span>  <br/> |<span data-ttu-id="c92a6-121">Indica um erro.</span><span class="sxs-lookup"><span data-stu-id="c92a6-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c92a6-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c92a6-122">Child elements</span></span>

|<span data-ttu-id="c92a6-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c92a6-123">**Element**</span></span>|<span data-ttu-id="c92a6-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c92a6-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c92a6-125">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c92a6-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="c92a6-126">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="c92a6-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="c92a6-127">Items</span><span class="sxs-lookup"><span data-stu-id="c92a6-127">Items</span></span>](items.md) <br/> |<span data-ttu-id="c92a6-128">Contém uma matriz de itens.</span><span class="sxs-lookup"><span data-stu-id="c92a6-128">Contains an array of items.</span></span>  <br/> |
|[<span data-ttu-id="c92a6-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="c92a6-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="c92a6-130">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="c92a6-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="c92a6-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="c92a6-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="c92a6-132">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="c92a6-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="c92a6-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c92a6-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="c92a6-134">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="c92a6-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c92a6-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c92a6-135">Parent elements</span></span>

|<span data-ttu-id="c92a6-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c92a6-136">**Element**</span></span>|<span data-ttu-id="c92a6-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c92a6-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c92a6-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c92a6-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="c92a6-139">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c92a6-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c92a6-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="c92a6-140">Remarks</span></span>

<span data-ttu-id="c92a6-141">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c92a6-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c92a6-142">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c92a6-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c92a6-143">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c92a6-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c92a6-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="c92a6-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c92a6-145">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c92a6-145">Schema Name</span></span>  <br/> |<span data-ttu-id="c92a6-146">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="c92a6-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="c92a6-147">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c92a6-147">Validation File</span></span>  <br/> |<span data-ttu-id="c92a6-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c92a6-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c92a6-149">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="c92a6-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c92a6-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="c92a6-150">See also</span></span>

- [<span data-ttu-id="c92a6-151">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c92a6-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

