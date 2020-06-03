---
title: EventType
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
description: O elemento EventTypes contém uma coleção de tipos de notificação de eventos que são usados para criar uma assinatura.
ms.openlocfilehash: 45ce1ed0699c8140029ae3fb7f667a5132f4731e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530625"
---
# <a name="eventtypes"></a><span data-ttu-id="a34f5-103">EventType</span><span class="sxs-lookup"><span data-stu-id="a34f5-103">EventTypes</span></span>

<span data-ttu-id="a34f5-104">O elemento **EventTypes** contém uma coleção de tipos de notificação de eventos que são usados para criar uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="a34f5-104">The **EventTypes** element contains a collection of event notification types that are used to create a subscription.</span></span> 
  
```xml
<EventTypes>
   <EventType/>
</EventTypes>
```

 <span data-ttu-id="a34f5-105">**NonEmptyArrayOfNotificationEventTypesType**</span><span class="sxs-lookup"><span data-stu-id="a34f5-105">**NonEmptyArrayOfNotificationEventTypesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a34f5-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a34f5-106">Attributes and elements</span></span>

<span data-ttu-id="a34f5-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a34f5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a34f5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a34f5-108">Attributes</span></span>

<span data-ttu-id="a34f5-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a34f5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a34f5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a34f5-110">Child elements</span></span>

|<span data-ttu-id="a34f5-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a34f5-111">**Element**</span></span>|<span data-ttu-id="a34f5-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a34f5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a34f5-113">EventType</span><span class="sxs-lookup"><span data-stu-id="a34f5-113">EventType</span></span>](eventtype.md) <br/> |<span data-ttu-id="a34f5-114">Representa um tipo de notificação de evento solicitado que é usado para criar uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="a34f5-114">Represents a requested event notification type that is used to create a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a34f5-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a34f5-115">Parent elements</span></span>

|<span data-ttu-id="a34f5-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a34f5-116">**Element**</span></span>|<span data-ttu-id="a34f5-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a34f5-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a34f5-118">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="a34f5-118">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="a34f5-119">Representa uma assinatura para uma assinatura de notificação de eventos baseada em pull.</span><span class="sxs-lookup"><span data-stu-id="a34f5-119">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="a34f5-120">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="a34f5-120">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="a34f5-121">Representa uma assinatura para uma assinatura de notificação de eventos baseada em push.</span><span class="sxs-lookup"><span data-stu-id="a34f5-121">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="a34f5-122">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="a34f5-122">StreamingSubscriptionRequest</span></span>](streamingsubscriptionrequest.md) <br/> |<span data-ttu-id="a34f5-123">Representa uma assinatura para uma assinatura de notificação de eventos de streaming.</span><span class="sxs-lookup"><span data-stu-id="a34f5-123">Represents a subscription to a streaming event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a34f5-124">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="a34f5-124">Text value</span></span>

<span data-ttu-id="a34f5-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a34f5-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a34f5-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="a34f5-126">Remarks</span></span>

<span data-ttu-id="a34f5-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a34f5-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a34f5-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a34f5-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a34f5-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="a34f5-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a34f5-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a34f5-130">Schema Name</span></span>  <br/> |<span data-ttu-id="a34f5-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a34f5-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="a34f5-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a34f5-132">Validation File</span></span>  <br/> |<span data-ttu-id="a34f5-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a34f5-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a34f5-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a34f5-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="a34f5-135">False</span><span class="sxs-lookup"><span data-stu-id="a34f5-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a34f5-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="a34f5-136">See also</span></span>



[<span data-ttu-id="a34f5-137">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="a34f5-137">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="a34f5-138">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="a34f5-138">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="a34f5-139">Operação GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="a34f5-139">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="a34f5-140">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="a34f5-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)

