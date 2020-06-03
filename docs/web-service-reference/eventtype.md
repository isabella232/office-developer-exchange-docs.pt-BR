---
title: EventType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EventType
api_type:
- schema
ms.assetid: 04b70f9e-c226-4130-958e-0db0275cf58b
description: O elemento EventType é usado para criar uma assinatura e identifica um tipo de evento a ser relatado em uma notificação.
ms.openlocfilehash: 58c7ce571434b6fb8ac0b1dc2a3f8cd4fd56ff17
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526169"
---
# <a name="eventtype"></a><span data-ttu-id="0f2a8-103">EventType</span><span class="sxs-lookup"><span data-stu-id="0f2a8-103">EventType</span></span>

<span data-ttu-id="0f2a8-104">O elemento **EventType** é usado para criar uma assinatura e identifica um tipo de evento a ser relatado em uma notificação.</span><span class="sxs-lookup"><span data-stu-id="0f2a8-104">The **EventType** element is used to create a subscription and identifies an event type to be reported in a notification.</span></span> 
  
```xml
<EventType/>
```

 <span data-ttu-id="0f2a8-105">**NotificationEventTypeType**</span><span class="sxs-lookup"><span data-stu-id="0f2a8-105">**NotificationEventTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0f2a8-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0f2a8-106">Attributes and elements</span></span>

<span data-ttu-id="0f2a8-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0f2a8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0f2a8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0f2a8-108">Attributes</span></span>

<span data-ttu-id="0f2a8-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0f2a8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0f2a8-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0f2a8-110">Child elements</span></span>

<span data-ttu-id="0f2a8-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0f2a8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0f2a8-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0f2a8-112">Parent elements</span></span>

|<span data-ttu-id="0f2a8-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0f2a8-113">**Element**</span></span>|<span data-ttu-id="0f2a8-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0f2a8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f2a8-115">EventType</span><span class="sxs-lookup"><span data-stu-id="0f2a8-115">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="0f2a8-116">Contém uma coleção de tipos de eventos de notificação de eventos que são usados para criar uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="0f2a8-116">Contains a collection of event notification event types that are used to create a subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0f2a8-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="0f2a8-117">Text value</span></span>

<span data-ttu-id="0f2a8-118">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0f2a8-118">A text value is required.</span></span> <span data-ttu-id="0f2a8-119">Veja a seguir os valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="0f2a8-119">The following are the possible values:</span></span>
  
- <span data-ttu-id="0f2a8-120">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="0f2a8-120">CopiedEvent</span></span>
    
- <span data-ttu-id="0f2a8-121">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="0f2a8-121">CreatedEvent</span></span>
    
- <span data-ttu-id="0f2a8-122">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="0f2a8-122">DeletedEvent</span></span>
    
- <span data-ttu-id="0f2a8-123">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="0f2a8-123">ModifiedEvent</span></span>
    
- <span data-ttu-id="0f2a8-124">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="0f2a8-124">MovedEvent</span></span>
    
- <span data-ttu-id="0f2a8-125">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="0f2a8-125">NewMailEvent</span></span>
    
- <span data-ttu-id="0f2a8-126">FreeBusyChangedEvent</span><span class="sxs-lookup"><span data-stu-id="0f2a8-126">FreeBusyChangedEvent</span></span>
    
## <a name="remarks"></a><span data-ttu-id="0f2a8-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="0f2a8-127">Remarks</span></span>

<span data-ttu-id="0f2a8-128">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0f2a8-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0f2a8-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0f2a8-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0f2a8-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="0f2a8-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0f2a8-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0f2a8-131">Schema Name</span></span>  <br/> |<span data-ttu-id="0f2a8-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0f2a8-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="0f2a8-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0f2a8-133">Validation File</span></span>  <br/> |<span data-ttu-id="0f2a8-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0f2a8-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0f2a8-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0f2a8-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="0f2a8-136">False</span><span class="sxs-lookup"><span data-stu-id="0f2a8-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0f2a8-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="0f2a8-137">See also</span></span>



[<span data-ttu-id="0f2a8-138">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="0f2a8-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="0f2a8-139">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="0f2a8-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="0f2a8-140">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="0f2a8-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)

