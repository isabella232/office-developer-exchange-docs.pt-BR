---
title: Assinar
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Subscribe
api_type:
- schema
ms.assetid: 6c2ee57d-e216-4a94-92db-faa3cb0e244a
description: O elemento Subscribe contém as propriedades usadas para criar assinaturas.
ms.openlocfilehash: f60e67654fb6af76e8081036a3463f5be401862d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530955"
---
# <a name="subscribe"></a><span data-ttu-id="e0bbb-103">Assinar</span><span class="sxs-lookup"><span data-stu-id="e0bbb-103">Subscribe</span></span>

<span data-ttu-id="e0bbb-104">O elemento **Subscribe** contém as propriedades usadas para criar assinaturas.</span><span class="sxs-lookup"><span data-stu-id="e0bbb-104">The **Subscribe** element contains the properties used to create subscriptions.</span></span> 
  
```XML
<Subscribe>
   <PullSubscriptionRequest/>
   <PushSubscriptionRequest/>
   <StreamingSubscriptionRequest/>
</Subscribe>
```

 <span data-ttu-id="e0bbb-105">**SubscribeType**</span><span class="sxs-lookup"><span data-stu-id="e0bbb-105">**SubscribeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e0bbb-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e0bbb-106">Attributes and elements</span></span>

<span data-ttu-id="e0bbb-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e0bbb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e0bbb-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e0bbb-108">Attributes</span></span>

<span data-ttu-id="e0bbb-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e0bbb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e0bbb-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e0bbb-110">Child elements</span></span>

|<span data-ttu-id="e0bbb-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e0bbb-111">**Element**</span></span>|<span data-ttu-id="e0bbb-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e0bbb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e0bbb-113">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="e0bbb-113">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="e0bbb-114">Representa uma assinatura para uma notificação de evento baseado em pull.</span><span class="sxs-lookup"><span data-stu-id="e0bbb-114">Represents a subscription to a pull-based event notification.</span></span>  <br/> |
|[<span data-ttu-id="e0bbb-115">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="e0bbb-115">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="e0bbb-116">Representa uma assinatura para uma notificação de evento baseado em push.</span><span class="sxs-lookup"><span data-stu-id="e0bbb-116">Represents a subscription to a push-based event notification.</span></span>  <br/> |
|[<span data-ttu-id="e0bbb-117">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="e0bbb-117">StreamingSubscriptionRequest</span></span>](streamingsubscriptionrequest.md) <br/> |<span data-ttu-id="e0bbb-118">Representa uma assinatura para uma notificação de evento de streaming.</span><span class="sxs-lookup"><span data-stu-id="e0bbb-118">Represents a subscription to a streaming event notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e0bbb-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e0bbb-119">Parent elements</span></span>

<span data-ttu-id="e0bbb-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e0bbb-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e0bbb-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="e0bbb-121">Remarks</span></span>

<span data-ttu-id="e0bbb-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e0bbb-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e0bbb-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e0bbb-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e0bbb-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="e0bbb-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e0bbb-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e0bbb-125">Schema name</span></span>  <br/> |<span data-ttu-id="e0bbb-126">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e0bbb-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e0bbb-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e0bbb-127">Validation file</span></span>  <br/> |<span data-ttu-id="e0bbb-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e0bbb-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e0bbb-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="e0bbb-129">Can be empty</span></span>  <br/> |<span data-ttu-id="e0bbb-130">False</span><span class="sxs-lookup"><span data-stu-id="e0bbb-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e0bbb-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="e0bbb-131">See also</span></span>



[<span data-ttu-id="e0bbb-132">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="e0bbb-132">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="e0bbb-133">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="e0bbb-133">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="e0bbb-134">Operação GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="e0bbb-134">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="e0bbb-135">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="e0bbb-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)

