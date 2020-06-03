---
title: GetAppMarketplaceUrlResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc3368ec-78c2-4f8d-8394-4891e90dafd2
description: O elemento GetAppMarketplaceUrlResponse especifica a resposta a uma solicitação GetAppMarketplaceUrl.
ms.openlocfilehash: 7ff000908a2f73f41575cae8a7795644dd60565d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530850"
---
# <a name="getappmarketplaceurlresponse"></a><span data-ttu-id="fa313-103">GetAppMarketplaceUrlResponse</span><span class="sxs-lookup"><span data-stu-id="fa313-103">GetAppMarketplaceUrlResponse</span></span>

<span data-ttu-id="fa313-104">O elemento **GetAppMarketplaceUrlResponse** especifica a resposta a uma solicitação **GetAppMarketplaceUrl** .</span><span class="sxs-lookup"><span data-stu-id="fa313-104">The **GetAppMarketplaceUrlResponse** element specifies the response to a **GetAppMarketplaceUrl** request.</span></span> 
  
```XML
<GetAppMarketplaceUrlResponse ResponseClass=" Success | Warning | Error ">
    <AppMarketplaceUrl/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetAppMarketplaceUrlResponse>
```

 <span data-ttu-id="fa313-105">**GetAppMarketplaceUrlResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="fa313-105">**GetAppMarketplaceUrlResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fa313-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="fa313-106">Attributes and elements</span></span>

<span data-ttu-id="fa313-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fa313-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fa313-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="fa313-108">Attributes</span></span>

|<span data-ttu-id="fa313-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="fa313-109">**Attribute**</span></span>|<span data-ttu-id="fa313-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fa313-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fa313-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="fa313-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="fa313-112">Indica a classe da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa313-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="fa313-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="fa313-113">ResponseClass</span></span>

|<span data-ttu-id="fa313-114">**Valor**</span><span class="sxs-lookup"><span data-stu-id="fa313-114">**Value**</span></span>|<span data-ttu-id="fa313-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fa313-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fa313-116">Êxito</span><span class="sxs-lookup"><span data-stu-id="fa313-116">Success</span></span>  <br/> |<span data-ttu-id="fa313-117">Indica êxito.</span><span class="sxs-lookup"><span data-stu-id="fa313-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="fa313-118">Aviso</span><span class="sxs-lookup"><span data-stu-id="fa313-118">Warning</span></span>  <br/> |<span data-ttu-id="fa313-119">Indica um aviso.</span><span class="sxs-lookup"><span data-stu-id="fa313-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="fa313-120">Erro</span><span class="sxs-lookup"><span data-stu-id="fa313-120">Error</span></span>  <br/> |<span data-ttu-id="fa313-121">Indica um erro.</span><span class="sxs-lookup"><span data-stu-id="fa313-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fa313-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fa313-122">Child elements</span></span>

|<span data-ttu-id="fa313-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fa313-123">**Element**</span></span>|<span data-ttu-id="fa313-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fa313-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa313-125">AppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="fa313-125">AppMarketplaceUrl</span></span>](appmarketplaceurl.md) <br/> |<span data-ttu-id="fa313-126">Especifica a URL do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fa313-126">Specifies the URL for the app.</span></span>  <br/> |
|[<span data-ttu-id="fa313-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="fa313-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="fa313-128">Atualmente não usado e reservado para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="fa313-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="fa313-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="fa313-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="fa313-130">Fornece uma descrição de texto do status da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa313-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="fa313-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="fa313-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="fa313-132">Fornece informações adicionais de resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="fa313-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="fa313-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="fa313-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="fa313-134">Fornece informações de status sobre a solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa313-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fa313-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fa313-135">Parent elements</span></span>

|<span data-ttu-id="fa313-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fa313-136">**Element**</span></span>|<span data-ttu-id="fa313-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fa313-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa313-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="fa313-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="fa313-139">Contém as mensagens de resposta para uma solicitação de serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fa313-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fa313-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="fa313-140">Remarks</span></span>

<span data-ttu-id="fa313-141">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="fa313-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fa313-142">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fa313-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fa313-143">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="fa313-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fa313-144">Namespace</span><span class="sxs-lookup"><span data-stu-id="fa313-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fa313-145">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fa313-145">Schema Name</span></span>  <br/> |<span data-ttu-id="fa313-146">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="fa313-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="fa313-147">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fa313-147">Validation File</span></span>  <br/> |<span data-ttu-id="fa313-148">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="fa313-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fa313-149">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="fa313-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="fa313-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="fa313-150">See also</span></span>



- [<span data-ttu-id="fa313-151">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fa313-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

