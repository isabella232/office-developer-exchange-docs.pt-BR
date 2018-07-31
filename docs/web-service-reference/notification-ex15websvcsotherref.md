---
title: Notification
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Notification
api_type:
- schema
ms.assetid: c9070936-0930-438e-839c-91127256a6c8
description: O elemento de notificação contém informações sobre a inscrição e os eventos que ocorreram desde a última notificação.
ms.openlocfilehash: 942ec18521fc484a7a3aa1385fb54f480ce9d11f
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354348"
---
# <a name="notification"></a><span data-ttu-id="48301-103">Notification</span><span class="sxs-lookup"><span data-stu-id="48301-103">Notification</span></span>

<span data-ttu-id="48301-104">O elemento de **notificação** contém informações sobre a inscrição e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="48301-104">The **Notification** element contains information about the subscription and the events that have occurred since the last notification.</span></span> 
  
```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <CopiedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <CreatedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <DeletedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <ModifiedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <MovedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <NewMailEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <StatusEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <FreeBusyChangedEvent/>
</Notification>
```

<span data-ttu-id="48301-105">**NotificationType**</span><span class="sxs-lookup"><span data-stu-id="48301-105">**NotificationType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="48301-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="48301-106">Attributes and elements</span></span>

<span data-ttu-id="48301-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="48301-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="48301-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="48301-108">Attributes</span></span>

<span data-ttu-id="48301-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="48301-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="48301-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="48301-110">Child elements</span></span>

|<span data-ttu-id="48301-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="48301-111">**Element**</span></span>|<span data-ttu-id="48301-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="48301-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="48301-113">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="48301-113">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="48301-114">Representa o identificador de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="48301-114">Represents the identifier for a subscription.</span></span>  <br/> |
|[<span data-ttu-id="48301-115">PreviousWatermark</span><span class="sxs-lookup"><span data-stu-id="48301-115">PreviousWatermark</span></span>](previouswatermark.md) <br/> |<span data-ttu-id="48301-116">Representa a marca d'água do evento mais recente que foi comunicada com êxito para o cliente para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="48301-116">Represents the watermark of the latest event that was successfully communicated to the client for the subscription.</span></span>  <br/> |
|[<span data-ttu-id="48301-117">MoreEvents</span><span class="sxs-lookup"><span data-stu-id="48301-117">MoreEvents</span></span>](moreevents.md) <br/> |<span data-ttu-id="48301-118">Indica se há mais eventos na fila sejam entregues ao cliente.</span><span class="sxs-lookup"><span data-stu-id="48301-118">Indicates whether there are more events in the queue to be delivered to the client.</span></span>  <br/> |
|[<span data-ttu-id="48301-119">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="48301-119">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="48301-120">Representa um evento no qual uma pasta ou um item é copiada.</span><span class="sxs-lookup"><span data-stu-id="48301-120">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="48301-121">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="48301-121">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="48301-122">Representa um evento no qual uma pasta ou um item é criada.</span><span class="sxs-lookup"><span data-stu-id="48301-122">Represents an event in which an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="48301-123">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="48301-123">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="48301-124">Representa um evento no qual uma pasta ou um item é excluída.</span><span class="sxs-lookup"><span data-stu-id="48301-124">Represents an event in which an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="48301-125">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="48301-125">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="48301-126">Representa um evento no qual um item ou pasta é modificada.</span><span class="sxs-lookup"><span data-stu-id="48301-126">Represents an event in which an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="48301-127">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="48301-127">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="48301-128">Representa um evento na qual um item ou pasta é movida de uma pasta pai para outra pasta pai.</span><span class="sxs-lookup"><span data-stu-id="48301-128">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="48301-129">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="48301-129">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="48301-130">Representa um evento que é disparado por um novo item de email em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="48301-130">Represents an event that is triggered by a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="48301-131">StatusEvent</span><span class="sxs-lookup"><span data-stu-id="48301-131">StatusEvent</span></span>](statusevent.md) <br/> |<span data-ttu-id="48301-132">Representa uma notificação que nenhuma nova atividade ocorreu na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="48301-132">Represents a notification that no new activity has occurred in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="48301-133">FreeBusyChangedEvent</span><span class="sxs-lookup"><span data-stu-id="48301-133">FreeBusyChangedEvent</span></span>](freebusychangedevent.md) <br/> |<span data-ttu-id="48301-134">Representa um evento no qual o tempo de disponibilidade de um item foi alterada.</span><span class="sxs-lookup"><span data-stu-id="48301-134">Represents an event in which an item's free/busy time has changed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="48301-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="48301-135">Parent elements</span></span>

|<span data-ttu-id="48301-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="48301-136">**Element**</span></span>|<span data-ttu-id="48301-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="48301-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="48301-138">GetEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="48301-138">GetEventsResponseMessage</span></span>](geteventsresponsemessage.md) <br/> |<span data-ttu-id="48301-139">Contém o status e o resultado de uma única solicitação GetEvents.</span><span class="sxs-lookup"><span data-stu-id="48301-139">Contains the status and result of a single GetEvents request.</span></span>  <br/> |
|[<span data-ttu-id="48301-140">SendNotificationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="48301-140">SendNotificationResponseMessage</span></span>](sendnotificationresponsemessage.md) <br/> |<span data-ttu-id="48301-141">Contém o status e o resultado de uma única solicitação SendNotification.</span><span class="sxs-lookup"><span data-stu-id="48301-141">Contains the status and result of a single SendNotification request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="48301-142">Text value</span><span class="sxs-lookup"><span data-stu-id="48301-142">Text value</span></span>

<span data-ttu-id="48301-143">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="48301-143">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="48301-144">Comentários</span><span class="sxs-lookup"><span data-stu-id="48301-144">Remarks</span></span>

<span data-ttu-id="48301-145">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="48301-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="48301-146">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="48301-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="48301-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="48301-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="48301-148">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="48301-148">Schema Name</span></span>  <br/> |<span data-ttu-id="48301-149">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="48301-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="48301-150">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="48301-150">Validation File</span></span>  <br/> |<span data-ttu-id="48301-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="48301-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="48301-152">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="48301-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="48301-153">False</span><span class="sxs-lookup"><span data-stu-id="48301-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="48301-154">Ver também</span><span class="sxs-lookup"><span data-stu-id="48301-154">See also</span></span>

- [<span data-ttu-id="48301-155">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="48301-155">Subscribe operation</span></span>](subscribe-operation.md) 
- [<span data-ttu-id="48301-156">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="48301-156">GetEvents operation</span></span>](getevents-operation.md) 
- [<span data-ttu-id="48301-157">Operação GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="48301-157">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md) 
- [<span data-ttu-id="48301-158">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="48301-158">Unsubscribe operation</span></span>](unsubscribe-operation.md)

