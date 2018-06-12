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
ms.openlocfilehash: fb54c9e042f105d10e68cb0e9b48feae7ed8bf7b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752104"
---
# <a name="eventtype"></a><span data-ttu-id="c2095-103">EventType</span><span class="sxs-lookup"><span data-stu-id="c2095-103">EventType</span></span>

<span data-ttu-id="c2095-104">O elemento **EventType** é usado para criar uma assinatura e identifica um tipo de evento a ser relatado em uma notificação.</span><span class="sxs-lookup"><span data-stu-id="c2095-104">The **EventType** element is used to create a subscription and identifies an event type to be reported in a notification.</span></span> 
  
```xml
<EventType/>
```

 <span data-ttu-id="c2095-105">**NotificationEventTypeType**</span><span class="sxs-lookup"><span data-stu-id="c2095-105">**NotificationEventTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c2095-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c2095-106">Attributes and elements</span></span>

<span data-ttu-id="c2095-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c2095-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2095-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c2095-108">Attributes</span></span>

<span data-ttu-id="c2095-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c2095-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c2095-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c2095-110">Child elements</span></span>

<span data-ttu-id="c2095-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c2095-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c2095-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c2095-112">Parent elements</span></span>

|<span data-ttu-id="c2095-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c2095-113">**Element**</span></span>|<span data-ttu-id="c2095-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c2095-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2095-115">EventTypes</span><span class="sxs-lookup"><span data-stu-id="c2095-115">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="c2095-116">Contém uma coleção dos tipos de evento de notificação de evento que são usados para criar uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="c2095-116">Contains a collection of event notification event types that are used to create a subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c2095-117">Text value</span><span class="sxs-lookup"><span data-stu-id="c2095-117">Text value</span></span>

<span data-ttu-id="c2095-118">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="c2095-118">A text value is required.</span></span> <span data-ttu-id="c2095-119">Veja a seguir os valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="c2095-119">The following are the possible values:</span></span>
  
- <span data-ttu-id="c2095-120">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="c2095-120">CopiedEvent</span></span>
    
- <span data-ttu-id="c2095-121">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="c2095-121">CreatedEvent</span></span>
    
- <span data-ttu-id="c2095-122">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="c2095-122">DeletedEvent</span></span>
    
- <span data-ttu-id="c2095-123">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="c2095-123">ModifiedEvent</span></span>
    
- <span data-ttu-id="c2095-124">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="c2095-124">MovedEvent</span></span>
    
- <span data-ttu-id="c2095-125">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="c2095-125">NewMailEvent</span></span>
    
- <span data-ttu-id="c2095-126">FreeBusyChangedEvent</span><span class="sxs-lookup"><span data-stu-id="c2095-126">FreeBusyChangedEvent</span></span>
    
## <a name="remarks"></a><span data-ttu-id="c2095-127">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="c2095-127">Remarks</span></span>

<span data-ttu-id="c2095-128">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="c2095-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2095-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c2095-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2095-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="c2095-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c2095-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c2095-131">Schema Name</span></span>  <br/> |<span data-ttu-id="c2095-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c2095-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="c2095-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c2095-133">Validation File</span></span>  <br/> |<span data-ttu-id="c2095-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c2095-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c2095-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c2095-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="c2095-136">False</span><span class="sxs-lookup"><span data-stu-id="c2095-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c2095-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="c2095-137">See also</span></span>



[<span data-ttu-id="c2095-138">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="c2095-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="c2095-139">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="c2095-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="c2095-140">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="c2095-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)

