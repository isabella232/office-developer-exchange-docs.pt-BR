---
title: CreatedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreatedEvent
api_type:
- schema
ms.assetid: f0e53a53-c352-42a5-8280-cd808b0e961b
description: O elemento CreatedEvent representa um evento no qual uma pasta ou um item é criada.
ms.openlocfilehash: f52516090d0789b4dd9fc1ced824786ce000e885
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751574"
---
# <a name="createdevent"></a><span data-ttu-id="b1583-103">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="b1583-103">CreatedEvent</span></span>

<span data-ttu-id="b1583-104">O elemento **CreatedEvent** representa um evento no qual uma pasta ou um item é criada.</span><span class="sxs-lookup"><span data-stu-id="b1583-104">The **CreatedEvent** element represents an event in which an item or folder is created.</span></span> 
  
```xml
<CreatedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</CreatedEvent>
```

 <span data-ttu-id="b1583-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="b1583-105">**BaseObjectChangedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b1583-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b1583-106">Attributes and elements</span></span>

<span data-ttu-id="b1583-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b1583-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b1583-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b1583-108">Attributes</span></span>

<span data-ttu-id="b1583-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b1583-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b1583-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b1583-110">Child elements</span></span>

|<span data-ttu-id="b1583-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b1583-111">**Element**</span></span>|<span data-ttu-id="b1583-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b1583-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b1583-113">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="b1583-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="b1583-114">Representa um indicador de evento na tabela de eventos de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b1583-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="b1583-115">Carimbo de hora</span><span class="sxs-lookup"><span data-stu-id="b1583-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="b1583-116">Representa o carimbo de hora de um evento de caixa de correio de item ou pasta criado.</span><span class="sxs-lookup"><span data-stu-id="b1583-116">Represents the timestamp of a created item or folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="b1583-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="b1583-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="b1583-118">Representa o identificador da pasta criada.</span><span class="sxs-lookup"><span data-stu-id="b1583-118">Represents the identifier of the created folder.</span></span>  <br/> |
|[<span data-ttu-id="b1583-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="b1583-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="b1583-120">Representa o identificador do item criado.</span><span class="sxs-lookup"><span data-stu-id="b1583-120">Represents the identifier of the created item.</span></span>  <br/> |
|[<span data-ttu-id="b1583-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="b1583-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="b1583-122">Representa o identificador da pasta pai da pasta ou item criado.</span><span class="sxs-lookup"><span data-stu-id="b1583-122">Represents the identifier of the parent folder of the created item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b1583-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b1583-123">Parent elements</span></span>

|<span data-ttu-id="b1583-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b1583-124">**Element**</span></span>|<span data-ttu-id="b1583-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b1583-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b1583-126">Notificação</span><span class="sxs-lookup"><span data-stu-id="b1583-126">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b1583-127">Contém informações sobre a inscrição e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="b1583-127">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b1583-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="b1583-128">Remarks</span></span>

<span data-ttu-id="b1583-129">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="b1583-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b1583-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b1583-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b1583-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="b1583-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b1583-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b1583-132">Schema name</span></span>  <br/> |<span data-ttu-id="b1583-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b1583-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="b1583-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b1583-134">Validation file</span></span>  <br/> |<span data-ttu-id="b1583-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b1583-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b1583-136">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b1583-136">Can be empty</span></span>  <br/> |<span data-ttu-id="b1583-137">False</span><span class="sxs-lookup"><span data-stu-id="b1583-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b1583-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="b1583-138">See also</span></span>



[<span data-ttu-id="b1583-139">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="b1583-139">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="b1583-140">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="b1583-140">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="b1583-141">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="b1583-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)


[<span data-ttu-id="b1583-142">Usando inscrições de recepção</span><span class="sxs-lookup"><span data-stu-id="b1583-142">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[<span data-ttu-id="b1583-143">Notificações de eventos no EWS</span><span class="sxs-lookup"><span data-stu-id="b1583-143">Event notifications in EWS</span></span>](http://msdn.microsoft.com/library/4fd4b351-d35c-4ccc-9ed9-878932ab9d50%28Office.15%29.aspx)

