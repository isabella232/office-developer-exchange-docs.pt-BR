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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465482"
---
# <a name="recipienttrackingevent"></a><span data-ttu-id="6f7ac-103">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="6f7ac-103">RecipientTrackingEvent</span></span>

<span data-ttu-id="6f7ac-104">O elemento **RecipientTrackingEvent** contém informações de um único evento para um destinatário.</span><span class="sxs-lookup"><span data-stu-id="6f7ac-104">The **RecipientTrackingEvent** element contains information for a single event for a recipient.</span></span> 
  
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

 <span data-ttu-id="6f7ac-105">**RecipientTrackingEventType**</span><span class="sxs-lookup"><span data-stu-id="6f7ac-105">**RecipientTrackingEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6f7ac-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6f7ac-106">Attributes and elements</span></span>

<span data-ttu-id="6f7ac-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6f7ac-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6f7ac-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6f7ac-108">Attributes</span></span>

<span data-ttu-id="6f7ac-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6f7ac-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6f7ac-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6f7ac-110">Child elements</span></span>

|<span data-ttu-id="6f7ac-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6f7ac-111">**Element**</span></span>|<span data-ttu-id="6f7ac-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6f7ac-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f7ac-113">Data (MessageTracking)</span><span class="sxs-lookup"><span data-stu-id="6f7ac-113">Date (MessageTracking)</span></span>](date-messagetracking.md) <br/> |<span data-ttu-id="6f7ac-114">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f7ac-114">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="6f7ac-115">Recipiente</span><span class="sxs-lookup"><span data-stu-id="6f7ac-115">Recipient</span></span>](recipient.md) <br/> |<span data-ttu-id="6f7ac-116">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f7ac-116">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="6f7ac-117">DeliveryStatus</span><span class="sxs-lookup"><span data-stu-id="6f7ac-117">DeliveryStatus</span></span>](deliverystatus.md) <br/> |<span data-ttu-id="6f7ac-118">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f7ac-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="6f7ac-119">EventDescription</span><span class="sxs-lookup"><span data-stu-id="6f7ac-119">EventDescription</span></span>](eventdescription.md) <br/> |<span data-ttu-id="6f7ac-120">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f7ac-120">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="6f7ac-121">EventData</span><span class="sxs-lookup"><span data-stu-id="6f7ac-121">EventData</span></span>](eventdata.md) <br/> |<span data-ttu-id="6f7ac-122">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="6f7ac-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="6f7ac-123">Servidor (MessageTracking)</span><span class="sxs-lookup"><span data-stu-id="6f7ac-123">Server (MessageTracking)</span></span>](server-messagetracking.md) <br/> |<span data-ttu-id="6f7ac-124">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f7ac-124">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="6f7ac-125">InternalId</span><span class="sxs-lookup"><span data-stu-id="6f7ac-125">InternalId</span></span>](internalid.md) <br/> |<span data-ttu-id="6f7ac-126">Este elemento é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f7ac-126">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="6f7ac-127">BccRecipient</span><span class="sxs-lookup"><span data-stu-id="6f7ac-127">BccRecipient</span></span>](bccrecipient.md) <br/> |<span data-ttu-id="6f7ac-128">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="6f7ac-128">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="6f7ac-129">HiddenRecipient</span><span class="sxs-lookup"><span data-stu-id="6f7ac-129">HiddenRecipient</span></span>](hiddenrecipient.md) <br/> |<span data-ttu-id="6f7ac-130">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="6f7ac-130">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="6f7ac-131">UniquePathId</span><span class="sxs-lookup"><span data-stu-id="6f7ac-131">UniquePathId</span></span>](uniquepathid.md) <br/> |<span data-ttu-id="6f7ac-132">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="6f7ac-132">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="6f7ac-133">RootAddress</span><span class="sxs-lookup"><span data-stu-id="6f7ac-133">RootAddress</span></span>](rootaddress.md) <br/> |<span data-ttu-id="6f7ac-134">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="6f7ac-134">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="6f7ac-135">Propriedades (ArrayOfTrackingPropertiesType)</span><span class="sxs-lookup"><span data-stu-id="6f7ac-135">Properties (ArrayOfTrackingPropertiesType)</span></span>](properties-arrayoftrackingpropertiestype.md) <br/> |<span data-ttu-id="6f7ac-136">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="6f7ac-136">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6f7ac-137">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6f7ac-137">Parent elements</span></span>

|<span data-ttu-id="6f7ac-138">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6f7ac-138">**Element**</span></span>|<span data-ttu-id="6f7ac-139">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6f7ac-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f7ac-140">RecipientTrackingEvents</span><span class="sxs-lookup"><span data-stu-id="6f7ac-140">RecipientTrackingEvents</span></span>](recipienttrackingevents.md) <br/> |<span data-ttu-id="6f7ac-141">Contém uma lista de um ou mais eventos de controle de um destinatário.</span><span class="sxs-lookup"><span data-stu-id="6f7ac-141">Contains a list of one or more tracking events for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6f7ac-142">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="6f7ac-142">Text value</span></span>

<span data-ttu-id="6f7ac-143">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6f7ac-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6f7ac-144">Comentários</span><span class="sxs-lookup"><span data-stu-id="6f7ac-144">Remarks</span></span>

<span data-ttu-id="6f7ac-145">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6f7ac-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6f7ac-146">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6f7ac-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6f7ac-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="6f7ac-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6f7ac-148">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6f7ac-148">Schema Name</span></span>  <br/> |<span data-ttu-id="6f7ac-149">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="6f7ac-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="6f7ac-150">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6f7ac-150">Validation File</span></span>  <br/> |<span data-ttu-id="6f7ac-151">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6f7ac-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6f7ac-152">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6f7ac-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="6f7ac-153">False</span><span class="sxs-lookup"><span data-stu-id="6f7ac-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6f7ac-154">Confira também</span><span class="sxs-lookup"><span data-stu-id="6f7ac-154">See also</span></span>



[<span data-ttu-id="6f7ac-155">Operação GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="6f7ac-155">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="6f7ac-156">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6f7ac-156">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

