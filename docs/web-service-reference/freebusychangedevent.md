---
title: FreeBusyChangedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyChangedEvent
api_type:
- schema
ms.assetid: 63abbfc5-c29f-4110-a922-6b1247187f28
description: O elemento FreeBusyChangedEvent representa um evento no qual o tempo de disponibilidade de um item foi alterada.
ms.openlocfilehash: 7271d375526e7614d0150594c2b988666a59eb8d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752369"
---
# <a name="freebusychangedevent"></a><span data-ttu-id="0bcc5-103">FreeBusyChangedEvent</span><span class="sxs-lookup"><span data-stu-id="0bcc5-103">FreeBusyChangedEvent</span></span>

<span data-ttu-id="0bcc5-104">O elemento **FreeBusyChangedEvent** representa um evento no qual o tempo de disponibilidade de um item foi alterada.</span><span class="sxs-lookup"><span data-stu-id="0bcc5-104">The **FreeBusyChangedEvent** element represents an event in which an item's free/busy time has changed.</span></span> 
  
```xml
<CreatedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</CreatedEvent>
```

 <span data-ttu-id="0bcc5-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="0bcc5-105">**BaseObjectChangedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0bcc5-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0bcc5-106">Attributes and elements</span></span>

<span data-ttu-id="0bcc5-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0bcc5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0bcc5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0bcc5-108">Attributes</span></span>

<span data-ttu-id="0bcc5-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0bcc5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0bcc5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0bcc5-110">Child elements</span></span>

|<span data-ttu-id="0bcc5-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0bcc5-111">**Element**</span></span>|<span data-ttu-id="0bcc5-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0bcc5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0bcc5-113">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="0bcc5-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="0bcc5-114">Representa um indicador de evento na tabela de eventos de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0bcc5-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="0bcc5-115">Carimbo de hora</span><span class="sxs-lookup"><span data-stu-id="0bcc5-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="0bcc5-116">Representa o carimbo de hora de um evento de caixa de correio do item de livre/ocupado.</span><span class="sxs-lookup"><span data-stu-id="0bcc5-116">Represents the timestamp of a free/busy item mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="0bcc5-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="0bcc5-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="0bcc5-118">Representa o identificador do item livre/ocupado.</span><span class="sxs-lookup"><span data-stu-id="0bcc5-118">Represents the identifier of the free/busy item.</span></span>  <br/> |
|[<span data-ttu-id="0bcc5-119">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="0bcc5-119">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="0bcc5-120">Representa o identificador da pasta pai do item livre/ocupado.</span><span class="sxs-lookup"><span data-stu-id="0bcc5-120">Represents the identifier of the parent folder of the free/busy item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0bcc5-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0bcc5-121">Parent elements</span></span>

|<span data-ttu-id="0bcc5-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0bcc5-122">**Element**</span></span>|<span data-ttu-id="0bcc5-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0bcc5-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0bcc5-124">Notificação</span><span class="sxs-lookup"><span data-stu-id="0bcc5-124">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="0bcc5-125">Contém informações sobre a inscrição e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="0bcc5-125">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0bcc5-126">Text value</span><span class="sxs-lookup"><span data-stu-id="0bcc5-126">Text value</span></span>

<span data-ttu-id="0bcc5-127">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0bcc5-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0bcc5-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="0bcc5-128">Remarks</span></span>

<span data-ttu-id="0bcc5-129">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0bcc5-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0bcc5-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0bcc5-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0bcc5-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="0bcc5-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0bcc5-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0bcc5-132">Schema name</span></span>  <br/> |<span data-ttu-id="0bcc5-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0bcc5-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="0bcc5-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0bcc5-134">Validation file</span></span>  <br/> |<span data-ttu-id="0bcc5-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0bcc5-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0bcc5-136">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="0bcc5-136">Can be empty</span></span>  <br/> |<span data-ttu-id="0bcc5-137">False</span><span class="sxs-lookup"><span data-stu-id="0bcc5-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0bcc5-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="0bcc5-138">See also</span></span>



[<span data-ttu-id="0bcc5-139">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="0bcc5-139">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="0bcc5-140">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="0bcc5-140">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="0bcc5-141">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="0bcc5-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)


[<span data-ttu-id="0bcc5-142">Usando inscrições de recepção</span><span class="sxs-lookup"><span data-stu-id="0bcc5-142">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[<span data-ttu-id="0bcc5-143">Notificações de eventos no EWS</span><span class="sxs-lookup"><span data-stu-id="0bcc5-143">Event notifications in EWS</span></span>](http://msdn.microsoft.com/library/4fd4b351-d35c-4ccc-9ed9-878932ab9d50%28Office.15%29.aspx)

