---
title: GetAppMarketplaceUrlResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc3368ec-78c2-4f8d-8394-4891e90dafd2
description: O elemento GetAppMarketplaceUrlResponse Especifica a resposta a uma solicitação GetAppMarketplaceUrl.
ms.openlocfilehash: 553ebfc4615280c77d4a1ef9e5db3e5d10a0f2a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752402"
---
# <a name="getappmarketplaceurlresponse"></a><span data-ttu-id="5d98f-103">GetAppMarketplaceUrlResponse</span><span class="sxs-lookup"><span data-stu-id="5d98f-103">GetAppMarketplaceUrlResponse</span></span>

<span data-ttu-id="5d98f-104">O elemento **GetAppMarketplaceUrlResponse** Especifica a resposta a uma solicitação **GetAppMarketplaceUrl** .</span><span class="sxs-lookup"><span data-stu-id="5d98f-104">The **GetAppMarketplaceUrlResponse** element specifies the response to a **GetAppMarketplaceUrl** request.</span></span> 
  
```XML
<GetAppMarketplaceUrlResponse ResponseClass=" Success | Warning | Error ">
    <AppMarketplaceUrl/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetAppMarketplaceUrlResponse>
```

 <span data-ttu-id="5d98f-105">**GetAppMarketplaceUrlResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="5d98f-105">**GetAppMarketplaceUrlResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5d98f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5d98f-106">Attributes and elements</span></span>

<span data-ttu-id="5d98f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5d98f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5d98f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5d98f-108">Attributes</span></span>

|<span data-ttu-id="5d98f-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="5d98f-109">**Attribute**</span></span>|<span data-ttu-id="5d98f-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5d98f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5d98f-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="5d98f-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="5d98f-112">Indica a classe da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d98f-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="5d98f-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="5d98f-113">ResponseClass</span></span>

|<span data-ttu-id="5d98f-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="5d98f-114">**Value**</span></span>|<span data-ttu-id="5d98f-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5d98f-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5d98f-116">Êxito</span><span class="sxs-lookup"><span data-stu-id="5d98f-116">Success</span></span>  <br/> |<span data-ttu-id="5d98f-117">Indica o sucesso.</span><span class="sxs-lookup"><span data-stu-id="5d98f-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="5d98f-118">Aviso</span><span class="sxs-lookup"><span data-stu-id="5d98f-118">Warning</span></span>  <br/> |<span data-ttu-id="5d98f-119">Indica um aviso.</span><span class="sxs-lookup"><span data-stu-id="5d98f-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="5d98f-120">Erro</span><span class="sxs-lookup"><span data-stu-id="5d98f-120">Error</span></span>  <br/> |<span data-ttu-id="5d98f-121">Indica um erro.</span><span class="sxs-lookup"><span data-stu-id="5d98f-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5d98f-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5d98f-122">Child elements</span></span>

|<span data-ttu-id="5d98f-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5d98f-123">**Element**</span></span>|<span data-ttu-id="5d98f-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5d98f-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d98f-125">AppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="5d98f-125">AppMarketplaceUrl</span></span>](appmarketplaceurl.md) <br/> |<span data-ttu-id="5d98f-126">Especifica a URL para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5d98f-126">Specifies the URL for the app.</span></span>  <br/> |
|[<span data-ttu-id="5d98f-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5d98f-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="5d98f-128">No momento não utilizados e reservada para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="5d98f-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="5d98f-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="5d98f-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="5d98f-130">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="5d98f-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="5d98f-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="5d98f-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="5d98f-132">Fornece informações de resposta de erro adicionais.</span><span class="sxs-lookup"><span data-stu-id="5d98f-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="5d98f-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5d98f-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="5d98f-134">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="5d98f-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5d98f-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5d98f-135">Parent elements</span></span>

|<span data-ttu-id="5d98f-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5d98f-136">**Element**</span></span>|<span data-ttu-id="5d98f-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5d98f-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d98f-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5d98f-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="5d98f-139">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d98f-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5d98f-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="5d98f-140">Remarks</span></span>

<span data-ttu-id="5d98f-141">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5d98f-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5d98f-142">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d98f-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5d98f-143">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5d98f-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5d98f-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="5d98f-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5d98f-145">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5d98f-145">Schema Name</span></span>  <br/> |<span data-ttu-id="5d98f-146">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="5d98f-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="5d98f-147">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5d98f-147">Validation File</span></span>  <br/> |<span data-ttu-id="5d98f-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5d98f-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5d98f-149">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="5d98f-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="5d98f-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="5d98f-150">See also</span></span>



- [<span data-ttu-id="5d98f-151">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5d98f-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

