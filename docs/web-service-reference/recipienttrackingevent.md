---
title: RecipientTrackingEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientTrackingEvent
api_type:
- schema
ms.assetid: 2bffdac7-c2f5-4805-ae7e-bd865301acb6
description: O elemento RecipientTrackingEvent contém informações para um único evento de um destinatário.
ms.openlocfilehash: c5488ba105f9a853a490d6f0f4ff9ff15b537e23
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824989"
---
# <a name="recipienttrackingevent"></a><span data-ttu-id="065fd-103">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="065fd-103">RecipientTrackingEvent</span></span>

<span data-ttu-id="065fd-104">O elemento **RecipientTrackingEvent** contém informações para um único evento de um destinatário.</span><span class="sxs-lookup"><span data-stu-id="065fd-104">The **RecipientTrackingEvent** element contains information for a single event for a recipient.</span></span> 
  
```XML
<RecipientTrackingEvent>
   <Date/>
   <Recipient/>
   <DeliveryStatus/>
   <EventDescription/>
   <EventData/>
   <Server/>
   <InternalId/>
   <BccRecipient/>
   <HiddenRecipient/>
   <UniquePathId/>
   <RootAddress/>
   <Properties/>
</RecipientTrackingEvent>
```

 <span data-ttu-id="065fd-105">**RecipientTrackingEventType**</span><span class="sxs-lookup"><span data-stu-id="065fd-105">**RecipientTrackingEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="065fd-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="065fd-106">Attributes and elements</span></span>

<span data-ttu-id="065fd-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="065fd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="065fd-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="065fd-108">Attributes</span></span>

<span data-ttu-id="065fd-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="065fd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="065fd-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="065fd-110">Child elements</span></span>

|<span data-ttu-id="065fd-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="065fd-111">**Element**</span></span>|<span data-ttu-id="065fd-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="065fd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="065fd-113">Data (MessageTracking)</span><span class="sxs-lookup"><span data-stu-id="065fd-113">Date (MessageTracking)</span></span>](date-messagetracking.md) <br/> |<span data-ttu-id="065fd-114">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="065fd-114">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="065fd-115">Recipient</span><span class="sxs-lookup"><span data-stu-id="065fd-115">Recipient</span></span>](recipient.md) <br/> |<span data-ttu-id="065fd-116">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="065fd-116">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="065fd-117">DeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="065fd-117">DeliveryStatus</span></span>](deliverystatus.md) <br/> |<span data-ttu-id="065fd-118">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="065fd-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="065fd-119">EventDescription</span><span class="sxs-lookup"><span data-stu-id="065fd-119">EventDescription</span></span>](eventdescription.md) <br/> |<span data-ttu-id="065fd-120">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="065fd-120">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="065fd-121">EventData</span><span class="sxs-lookup"><span data-stu-id="065fd-121">EventData</span></span>](eventdata.md) <br/> |<span data-ttu-id="065fd-122">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="065fd-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="065fd-123">Servidor (MessageTracking)</span><span class="sxs-lookup"><span data-stu-id="065fd-123">Server (MessageTracking)</span></span>](server-messagetracking.md) <br/> |<span data-ttu-id="065fd-124">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="065fd-124">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="065fd-125">InternalId</span><span class="sxs-lookup"><span data-stu-id="065fd-125">InternalId</span></span>](internalid.md) <br/> |<span data-ttu-id="065fd-126">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="065fd-126">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="065fd-127">BccRecipient</span><span class="sxs-lookup"><span data-stu-id="065fd-127">BccRecipient</span></span>](bccrecipient.md) <br/> |<span data-ttu-id="065fd-128">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="065fd-128">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="065fd-129">HiddenRecipient</span><span class="sxs-lookup"><span data-stu-id="065fd-129">HiddenRecipient</span></span>](hiddenrecipient.md) <br/> |<span data-ttu-id="065fd-130">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="065fd-130">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="065fd-131">UniquePathId</span><span class="sxs-lookup"><span data-stu-id="065fd-131">UniquePathId</span></span>](uniquepathid.md) <br/> |<span data-ttu-id="065fd-132">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="065fd-132">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="065fd-133">RootAddress</span><span class="sxs-lookup"><span data-stu-id="065fd-133">RootAddress</span></span>](rootaddress.md) <br/> |<span data-ttu-id="065fd-134">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="065fd-134">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="065fd-135">Propriedades (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="065fd-135">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="065fd-136">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="065fd-136">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="065fd-137">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="065fd-137">Parent elements</span></span>

|<span data-ttu-id="065fd-138">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="065fd-138">**Element**</span></span>|<span data-ttu-id="065fd-139">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="065fd-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="065fd-140">RecipientTrackingEvents</span><span class="sxs-lookup"><span data-stu-id="065fd-140">RecipientTrackingEvents</span></span>](recipienttrackingevents.md) <br/> |<span data-ttu-id="065fd-141">Contém uma lista de um ou mais eventos de rastreamento para um destinatário.</span><span class="sxs-lookup"><span data-stu-id="065fd-141">Contains a list of one or more tracking events for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="065fd-142">Text value</span><span class="sxs-lookup"><span data-stu-id="065fd-142">Text value</span></span>

<span data-ttu-id="065fd-143">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="065fd-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="065fd-144">Comentários</span><span class="sxs-lookup"><span data-stu-id="065fd-144">Remarks</span></span>

<span data-ttu-id="065fd-145">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="065fd-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="065fd-146">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="065fd-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="065fd-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="065fd-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="065fd-148">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="065fd-148">Schema Name</span></span>  <br/> |<span data-ttu-id="065fd-149">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="065fd-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="065fd-150">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="065fd-150">Validation File</span></span>  <br/> |<span data-ttu-id="065fd-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="065fd-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="065fd-152">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="065fd-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="065fd-153">False</span><span class="sxs-lookup"><span data-stu-id="065fd-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="065fd-154">Ver também</span><span class="sxs-lookup"><span data-stu-id="065fd-154">See also</span></span>



[<span data-ttu-id="065fd-155">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="065fd-155">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="065fd-156">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="065fd-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

