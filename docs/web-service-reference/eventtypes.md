---
title: EventTypes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EventTypes
api_type:
- schema
ms.assetid: 29ded9e5-f191-4aa3-bc3e-500de2fc8818
description: O elemento EventTypes contém uma coleção dos tipos de notificação de evento que são usados para criar uma assinatura.
ms.openlocfilehash: f4c622376f6b607ed390511d7bb5f0f723889420
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752106"
---
# <a name="eventtypes"></a><span data-ttu-id="89f8e-103">EventTypes</span><span class="sxs-lookup"><span data-stu-id="89f8e-103">EventTypes</span></span>

<span data-ttu-id="89f8e-104">O elemento **EventTypes** contém uma coleção dos tipos de notificação de evento que são usados para criar uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="89f8e-104">The **EventTypes** element contains a collection of event notification types that are used to create a subscription.</span></span> 
  
```xml
<EventTypes>
   <EventType/>
</EventTypes>
```

 <span data-ttu-id="89f8e-105">**NonEmptyArrayOfNotificationEventTypesType**</span><span class="sxs-lookup"><span data-stu-id="89f8e-105">**NonEmptyArrayOfNotificationEventTypesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="89f8e-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="89f8e-106">Attributes and elements</span></span>

<span data-ttu-id="89f8e-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="89f8e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89f8e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="89f8e-108">Attributes</span></span>

<span data-ttu-id="89f8e-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="89f8e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="89f8e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="89f8e-110">Child elements</span></span>

|<span data-ttu-id="89f8e-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="89f8e-111">**Element**</span></span>|<span data-ttu-id="89f8e-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="89f8e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89f8e-113">EventType</span><span class="sxs-lookup"><span data-stu-id="89f8e-113">EventType</span></span>](eventtype.md) <br/> |<span data-ttu-id="89f8e-114">Representa um tipo de notificação de evento solicitado que é usado para criar uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="89f8e-114">Represents a requested event notification type that is used to create a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="89f8e-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="89f8e-115">Parent elements</span></span>

|<span data-ttu-id="89f8e-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="89f8e-116">**Element**</span></span>|<span data-ttu-id="89f8e-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="89f8e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89f8e-118">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="89f8e-118">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="89f8e-119">Representa uma assinatura para uma inscrição de notificação de evento baseado em extração.</span><span class="sxs-lookup"><span data-stu-id="89f8e-119">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="89f8e-120">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="89f8e-120">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="89f8e-121">Representa uma assinatura para uma inscrição de notificação de push com base no evento.</span><span class="sxs-lookup"><span data-stu-id="89f8e-121">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="89f8e-122">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="89f8e-122">StreamingSubscriptionRequest</span></span>](streamingsubscriptionrequest.md) <br/> |<span data-ttu-id="89f8e-123">Representa uma assinatura para uma inscrição de notificação de evento streaming.</span><span class="sxs-lookup"><span data-stu-id="89f8e-123">Represents a subscription to a streaming event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="89f8e-124">Text value</span><span class="sxs-lookup"><span data-stu-id="89f8e-124">Text value</span></span>

<span data-ttu-id="89f8e-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="89f8e-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="89f8e-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="89f8e-126">Remarks</span></span>

<span data-ttu-id="89f8e-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="89f8e-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89f8e-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="89f8e-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89f8e-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="89f8e-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="89f8e-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="89f8e-130">Schema Name</span></span>  <br/> |<span data-ttu-id="89f8e-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="89f8e-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="89f8e-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="89f8e-132">Validation File</span></span>  <br/> |<span data-ttu-id="89f8e-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="89f8e-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="89f8e-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="89f8e-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="89f8e-135">False</span><span class="sxs-lookup"><span data-stu-id="89f8e-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="89f8e-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="89f8e-136">See also</span></span>



[<span data-ttu-id="89f8e-137">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="89f8e-137">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="89f8e-138">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="89f8e-138">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="89f8e-139">Operação GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="89f8e-139">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="89f8e-140">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="89f8e-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)

