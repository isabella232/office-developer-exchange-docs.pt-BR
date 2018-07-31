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
ms.openlocfilehash: 791b8af87c0cc8ae7f07850e3a6fedd9975a251e
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353172"
---
# <a name="createdevent"></a><span data-ttu-id="9afbd-103">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="9afbd-103">CreatedEvent</span></span>

<span data-ttu-id="9afbd-104">O elemento **CreatedEvent** representa um evento no qual uma pasta ou um item é criada.</span><span class="sxs-lookup"><span data-stu-id="9afbd-104">The **CreatedEvent** element represents an event in which an item or folder is created.</span></span> 
  
```xml
<CreatedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
</CreatedEvent>
```

```xml
<CreatedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
</CreatedEvent>
```

<span data-ttu-id="9afbd-105">**BaseObjectChangedEventType**</span><span class="sxs-lookup"><span data-stu-id="9afbd-105">**BaseObjectChangedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9afbd-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9afbd-106">Attributes and elements</span></span>

<span data-ttu-id="9afbd-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9afbd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9afbd-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9afbd-108">Attributes</span></span>

<span data-ttu-id="9afbd-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9afbd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9afbd-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9afbd-110">Child elements</span></span>

|<span data-ttu-id="9afbd-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9afbd-111">**Element**</span></span>|<span data-ttu-id="9afbd-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9afbd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9afbd-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="9afbd-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="9afbd-114">Representa um indicador de evento na tabela de eventos de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="9afbd-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="9afbd-115">TimeStamp</span><span class="sxs-lookup"><span data-stu-id="9afbd-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="9afbd-116">Representa o carimbo de hora de um evento de caixa de correio de item ou pasta criado.</span><span class="sxs-lookup"><span data-stu-id="9afbd-116">Represents the timestamp of a created item or folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="9afbd-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="9afbd-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="9afbd-118">Representa o identificador da pasta criada.</span><span class="sxs-lookup"><span data-stu-id="9afbd-118">Represents the identifier of the created folder.</span></span>  <br/> |
|[<span data-ttu-id="9afbd-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="9afbd-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="9afbd-120">Representa o identificador do item criado.</span><span class="sxs-lookup"><span data-stu-id="9afbd-120">Represents the identifier of the created item.</span></span>  <br/> |
|[<span data-ttu-id="9afbd-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="9afbd-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="9afbd-122">Representa o identificador da pasta pai da pasta ou item criado.</span><span class="sxs-lookup"><span data-stu-id="9afbd-122">Represents the identifier of the parent folder of the created item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9afbd-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9afbd-123">Parent elements</span></span>

|<span data-ttu-id="9afbd-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9afbd-124">**Element**</span></span>|<span data-ttu-id="9afbd-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9afbd-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9afbd-126">Notificação</span><span class="sxs-lookup"><span data-stu-id="9afbd-126">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9afbd-127">Contém informações sobre a inscrição e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="9afbd-127">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9afbd-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="9afbd-128">Remarks</span></span>

<span data-ttu-id="9afbd-129">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="9afbd-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9afbd-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9afbd-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9afbd-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="9afbd-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9afbd-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9afbd-132">Schema name</span></span>  <br/> |<span data-ttu-id="9afbd-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9afbd-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="9afbd-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9afbd-134">Validation file</span></span>  <br/> |<span data-ttu-id="9afbd-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9afbd-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9afbd-136">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="9afbd-136">Can be empty</span></span>  <br/> |<span data-ttu-id="9afbd-137">False</span><span class="sxs-lookup"><span data-stu-id="9afbd-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9afbd-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="9afbd-138">See also</span></span>

- [<span data-ttu-id="9afbd-139">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="9afbd-139">Subscribe operation</span></span>](subscribe-operation.md)  
- [<span data-ttu-id="9afbd-140">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="9afbd-140">GetEvents operation</span></span>](getevents-operation.md)  
- [<span data-ttu-id="9afbd-141">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="9afbd-141">Unsubscribe operation</span></span>](unsubscribe-operation.md)
- [<span data-ttu-id="9afbd-142">Usando inscrições de recepção</span><span class="sxs-lookup"><span data-stu-id="9afbd-142">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx) 
- [<span data-ttu-id="9afbd-143">Notificações de eventos no EWS</span><span class="sxs-lookup"><span data-stu-id="9afbd-143">Event notifications in EWS</span></span>](http://msdn.microsoft.com/library/4fd4b351-d35c-4ccc-9ed9-878932ab9d50%28Office.15%29.aspx)

