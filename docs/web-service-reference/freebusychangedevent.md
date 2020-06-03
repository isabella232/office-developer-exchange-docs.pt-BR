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
description: O elemento FreeBusyChangedEvent representa um evento no qual o horário de disponibilidade de um item foi alterado.
ms.openlocfilehash: d9ea8bc210ab503c4e9f606bcb66317cefe15de1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456476"
---
# <a name="freebusychangedevent"></a><span data-ttu-id="88833-103">FreeBusyChangedEvent</span><span class="sxs-lookup"><span data-stu-id="88833-103">FreeBusyChangedEvent</span></span>

<span data-ttu-id="88833-104">O elemento **FreeBusyChangedEvent** representa um evento no qual o horário de disponibilidade de um item foi alterado.</span><span class="sxs-lookup"><span data-stu-id="88833-104">The **FreeBusyChangedEvent** element represents an event in which an item's free/busy time has changed.</span></span> 
  
```xml
<CreatedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</CreatedEvent>
```

 <span data-ttu-id="88833-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="88833-105">**BaseObjectChangedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88833-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="88833-106">Attributes and elements</span></span>

<span data-ttu-id="88833-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="88833-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88833-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="88833-108">Attributes</span></span>

<span data-ttu-id="88833-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="88833-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="88833-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="88833-110">Child elements</span></span>

|<span data-ttu-id="88833-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="88833-111">**Element**</span></span>|<span data-ttu-id="88833-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="88833-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88833-113">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="88833-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="88833-114">Representa um indicador de evento na tabela de eventos de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="88833-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="88833-115">Registra</span><span class="sxs-lookup"><span data-stu-id="88833-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="88833-116">Representa o carimbo de data/hora de um evento de caixa de correio de item de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="88833-116">Represents the timestamp of a free/busy item mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="88833-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="88833-117">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="88833-118">Representa o identificador do item de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="88833-118">Represents the identifier of the free/busy item.</span></span>  <br/> |
|[<span data-ttu-id="88833-119">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="88833-119">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="88833-120">Representa o identificador da pasta pai do item de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="88833-120">Represents the identifier of the parent folder of the free/busy item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="88833-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="88833-121">Parent elements</span></span>

|<span data-ttu-id="88833-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="88833-122">**Element**</span></span>|<span data-ttu-id="88833-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="88833-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88833-124">Notificação</span><span class="sxs-lookup"><span data-stu-id="88833-124">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="88833-125">Contém informações sobre a assinatura e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="88833-125">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="88833-126">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="88833-126">Text value</span></span>

<span data-ttu-id="88833-127">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="88833-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="88833-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="88833-128">Remarks</span></span>

<span data-ttu-id="88833-129">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="88833-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="88833-130">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="88833-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88833-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="88833-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="88833-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="88833-132">Schema name</span></span>  <br/> |<span data-ttu-id="88833-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="88833-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="88833-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="88833-134">Validation file</span></span>  <br/> |<span data-ttu-id="88833-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="88833-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="88833-136">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="88833-136">Can be empty</span></span>  <br/> |<span data-ttu-id="88833-137">False</span><span class="sxs-lookup"><span data-stu-id="88833-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="88833-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="88833-138">See also</span></span>



[<span data-ttu-id="88833-139">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="88833-139">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="88833-140">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="88833-140">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="88833-141">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="88833-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)


[<span data-ttu-id="88833-142">Usando assinaturas pull</span><span class="sxs-lookup"><span data-stu-id="88833-142">Using Pull Subscriptions</span></span>](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[<span data-ttu-id="88833-143">Notificações de eventos no EWS</span><span class="sxs-lookup"><span data-stu-id="88833-143">Event notifications in EWS</span></span>](https://msdn.microsoft.com/library/4fd4b351-d35c-4ccc-9ed9-878932ab9d50%28Office.15%29.aspx)

