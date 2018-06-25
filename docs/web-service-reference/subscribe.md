---
title: Inscrever-se
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
description: O elemento de Subscribe contém as propriedades usadas para criar inscrições.
ms.openlocfilehash: 9f23f566f9105c655b289ed9b434c5e7b917207f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825618"
---
# <a name="subscribe"></a><span data-ttu-id="d53a5-103">Inscrever-se</span><span class="sxs-lookup"><span data-stu-id="d53a5-103">Subscribe</span></span>

<span data-ttu-id="d53a5-104">O elemento de **Subscribe** contém as propriedades usadas para criar inscrições.</span><span class="sxs-lookup"><span data-stu-id="d53a5-104">The **Subscribe** element contains the properties used to create subscriptions.</span></span> 
  
```XML
<Subscribe>
   <PullSubscriptionRequest/>
   <PushSubscriptionRequest/>
   <StreamingSubscriptionRequest/>
</Subscribe>
```

 <span data-ttu-id="d53a5-105">**SubscribeType**</span><span class="sxs-lookup"><span data-stu-id="d53a5-105">**SubscribeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d53a5-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d53a5-106">Attributes and elements</span></span>

<span data-ttu-id="d53a5-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d53a5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d53a5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d53a5-108">Attributes</span></span>

<span data-ttu-id="d53a5-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d53a5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d53a5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d53a5-110">Child elements</span></span>

|<span data-ttu-id="d53a5-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d53a5-111">**Element**</span></span>|<span data-ttu-id="d53a5-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d53a5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d53a5-113">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="d53a5-113">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="d53a5-114">Representa uma assinatura de uma notificação de evento baseado em extração.</span><span class="sxs-lookup"><span data-stu-id="d53a5-114">Represents a subscription to a pull-based event notification.</span></span>  <br/> |
|[<span data-ttu-id="d53a5-115">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="d53a5-115">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="d53a5-116">Representa uma assinatura de uma notificação de push com base no evento.</span><span class="sxs-lookup"><span data-stu-id="d53a5-116">Represents a subscription to a push-based event notification.</span></span>  <br/> |
|[<span data-ttu-id="d53a5-117">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="d53a5-117">StreamingSubscriptionRequest</span></span>](streamingsubscriptionrequest.md) <br/> |<span data-ttu-id="d53a5-118">Representa uma assinatura de uma notificação de evento streaming.</span><span class="sxs-lookup"><span data-stu-id="d53a5-118">Represents a subscription to a streaming event notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d53a5-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d53a5-119">Parent elements</span></span>

<span data-ttu-id="d53a5-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d53a5-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d53a5-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="d53a5-121">Remarks</span></span>

<span data-ttu-id="d53a5-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d53a5-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d53a5-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d53a5-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d53a5-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="d53a5-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d53a5-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d53a5-125">Schema name</span></span>  <br/> |<span data-ttu-id="d53a5-126">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d53a5-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d53a5-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d53a5-127">Validation file</span></span>  <br/> |<span data-ttu-id="d53a5-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d53a5-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d53a5-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d53a5-129">Can be empty</span></span>  <br/> |<span data-ttu-id="d53a5-130">False</span><span class="sxs-lookup"><span data-stu-id="d53a5-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d53a5-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="d53a5-131">See also</span></span>



[<span data-ttu-id="d53a5-132">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="d53a5-132">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="d53a5-133">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="d53a5-133">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="d53a5-134">Operação GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="d53a5-134">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="d53a5-135">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="d53a5-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)

