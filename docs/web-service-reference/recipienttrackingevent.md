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
description: O elemento RecipientTrackingEvent contém informações de um único evento para um destinatário.
ms.openlocfilehash: e9a014cdfac122f112205cfa5032535a770f9d82
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465482"
---
# <a name="recipienttrackingevent"></a><span data-ttu-id="dd3bb-103">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="dd3bb-103">RecipientTrackingEvent</span></span>

<span data-ttu-id="dd3bb-104">O elemento **RecipientTrackingEvent** contém informações de um único evento para um destinatário.</span><span class="sxs-lookup"><span data-stu-id="dd3bb-104">The **RecipientTrackingEvent** element contains information for a single event for a recipient.</span></span> 
  
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

 <span data-ttu-id="dd3bb-105">**RecipientTrackingEventType**</span><span class="sxs-lookup"><span data-stu-id="dd3bb-105">**RecipientTrackingEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dd3bb-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="dd3bb-106">Attributes and elements</span></span>

<span data-ttu-id="dd3bb-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="dd3bb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd3bb-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="dd3bb-108">Attributes</span></span>

<span data-ttu-id="dd3bb-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dd3bb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dd3bb-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="dd3bb-110">Child elements</span></span>

|<span data-ttu-id="dd3bb-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dd3bb-111">**Element**</span></span>|<span data-ttu-id="dd3bb-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dd3bb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd3bb-113">Data (MessageTracking)</span><span class="sxs-lookup"><span data-stu-id="dd3bb-113">Date (MessageTracking)</span></span>](date-messagetracking.md) <br/> |<span data-ttu-id="dd3bb-114">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd3bb-114">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="dd3bb-115">Recipiente</span><span class="sxs-lookup"><span data-stu-id="dd3bb-115">Recipient</span></span>](recipient.md) <br/> |<span data-ttu-id="dd3bb-116">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd3bb-116">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="dd3bb-117">DeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="dd3bb-117">DeliveryStatus</span></span>](deliverystatus.md) <br/> |<span data-ttu-id="dd3bb-118">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd3bb-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="dd3bb-119">EventDescription</span><span class="sxs-lookup"><span data-stu-id="dd3bb-119">EventDescription</span></span>](eventdescription.md) <br/> |<span data-ttu-id="dd3bb-120">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd3bb-120">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="dd3bb-121">EventData</span><span class="sxs-lookup"><span data-stu-id="dd3bb-121">EventData</span></span>](eventdata.md) <br/> |<span data-ttu-id="dd3bb-122">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="dd3bb-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="dd3bb-123">Servidor (MessageTracking)</span><span class="sxs-lookup"><span data-stu-id="dd3bb-123">Server (MessageTracking)</span></span>](server-messagetracking.md) <br/> |<span data-ttu-id="dd3bb-124">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd3bb-124">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="dd3bb-125">InternalId</span><span class="sxs-lookup"><span data-stu-id="dd3bb-125">InternalId</span></span>](internalid.md) <br/> |<span data-ttu-id="dd3bb-126">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="dd3bb-126">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="dd3bb-127">BccRecipient</span><span class="sxs-lookup"><span data-stu-id="dd3bb-127">BccRecipient</span></span>](bccrecipient.md) <br/> |<span data-ttu-id="dd3bb-128">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="dd3bb-128">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="dd3bb-129">HiddenRecipient</span><span class="sxs-lookup"><span data-stu-id="dd3bb-129">HiddenRecipient</span></span>](hiddenrecipient.md) <br/> |<span data-ttu-id="dd3bb-130">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="dd3bb-130">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="dd3bb-131">UniquePathId</span><span class="sxs-lookup"><span data-stu-id="dd3bb-131">UniquePathId</span></span>](uniquepathid.md) <br/> |<span data-ttu-id="dd3bb-132">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="dd3bb-132">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="dd3bb-133">RootAddress</span><span class="sxs-lookup"><span data-stu-id="dd3bb-133">RootAddress</span></span>](rootaddress.md) <br/> |<span data-ttu-id="dd3bb-134">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="dd3bb-134">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="dd3bb-135">Propriedades (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="dd3bb-135">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="dd3bb-136">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="dd3bb-136">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dd3bb-137">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="dd3bb-137">Parent elements</span></span>

|<span data-ttu-id="dd3bb-138">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dd3bb-138">**Element**</span></span>|<span data-ttu-id="dd3bb-139">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dd3bb-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd3bb-140">RecipientTrackingEvents</span><span class="sxs-lookup"><span data-stu-id="dd3bb-140">RecipientTrackingEvents</span></span>](recipienttrackingevents.md) <br/> |<span data-ttu-id="dd3bb-141">Contém uma lista de um ou mais eventos de controle de um destinatário.</span><span class="sxs-lookup"><span data-stu-id="dd3bb-141">Contains a list of one or more tracking events for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dd3bb-142">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="dd3bb-142">Text value</span></span>

<span data-ttu-id="dd3bb-143">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="dd3bb-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dd3bb-144">Comentários</span><span class="sxs-lookup"><span data-stu-id="dd3bb-144">Remarks</span></span>

<span data-ttu-id="dd3bb-145">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="dd3bb-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dd3bb-146">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="dd3bb-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dd3bb-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="dd3bb-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dd3bb-148">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="dd3bb-148">Schema Name</span></span>  <br/> |<span data-ttu-id="dd3bb-149">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="dd3bb-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="dd3bb-150">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="dd3bb-150">Validation File</span></span>  <br/> |<span data-ttu-id="dd3bb-151">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="dd3bb-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dd3bb-152">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="dd3bb-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="dd3bb-153">False</span><span class="sxs-lookup"><span data-stu-id="dd3bb-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dd3bb-154">Confira também</span><span class="sxs-lookup"><span data-stu-id="dd3bb-154">See also</span></span>



[<span data-ttu-id="dd3bb-155">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="dd3bb-155">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="dd3bb-156">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="dd3bb-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

