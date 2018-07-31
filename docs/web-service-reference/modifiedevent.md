---
title: ModifiedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ModifiedEvent
api_type:
- schema
ms.assetid: ca1309f4-2df7-4289-811c-75c3db0e7072
description: O elemento ModifiedEvent representa um evento no qual um item ou pasta é modificada.
ms.openlocfilehash: 2e9fb870396d49efb5cdf307a502b4111c2e507e
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353809"
---
# <a name="modifiedevent"></a><span data-ttu-id="3d9d9-103">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="3d9d9-103">ModifiedEvent</span></span>

<span data-ttu-id="3d9d9-104">O elemento **ModifiedEvent** representa um evento no qual um item ou pasta é modificada.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-104">The **ModifiedEvent** element represents an event in which an item or folder is modified.</span></span> 
  
```xml
<ModifiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <UnreadCount/>
</ModifiedEvent>
```

```xml
<ModifiedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/> 
   <ParentFolderId/>
   <UnreadCount/>
</ModifiedEvent>
```

<span data-ttu-id="3d9d9-105">**ModifiedEventType**</span><span class="sxs-lookup"><span data-stu-id="3d9d9-105">**ModifiedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="3d9d9-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3d9d9-106">Attributes and elements</span></span>

<span data-ttu-id="3d9d9-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3d9d9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3d9d9-108">Attributes</span></span>

<span data-ttu-id="3d9d9-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3d9d9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3d9d9-110">Child elements</span></span>

|<span data-ttu-id="3d9d9-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3d9d9-111">**Element**</span></span>|<span data-ttu-id="3d9d9-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3d9d9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3d9d9-113">Watermark</span><span class="sxs-lookup"><span data-stu-id="3d9d9-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="3d9d9-114">Representa um indicador de evento na tabela de eventos de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="3d9d9-115">TimeStamp</span><span class="sxs-lookup"><span data-stu-id="3d9d9-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="3d9d9-116">Representa o carimbo de hora de um evento de caixa de correio de item ou pasta modificado.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-116">Represents the timestamp of a modified item or folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="3d9d9-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="3d9d9-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="3d9d9-118">Representa o identificador da pasta modificada.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-118">Represents the identifier of the modified folder.</span></span>  <br/> |
|[<span data-ttu-id="3d9d9-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="3d9d9-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="3d9d9-120">Representa o identificador do item modificado.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-120">Represents the identifier of the modified item.</span></span>  <br/> |
|[<span data-ttu-id="3d9d9-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="3d9d9-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="3d9d9-122">Representa o identificador da pasta pai da pasta ou item modificado.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-122">Represents the identifier of the parent folder of the modified item or folder.</span></span>  <br/> |
|[<span data-ttu-id="3d9d9-123">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="3d9d9-123">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="3d9d9-124">Representa a contagem de itens não lidos dentro de uma determinada pasta.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-124">Represents the count of unread items within a given folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3d9d9-125">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3d9d9-125">Parent elements</span></span>

|<span data-ttu-id="3d9d9-126">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3d9d9-126">**Element**</span></span>|<span data-ttu-id="3d9d9-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3d9d9-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3d9d9-128">Notificação</span><span class="sxs-lookup"><span data-stu-id="3d9d9-128">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="3d9d9-129">Contém informações sobre a inscrição e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-129">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3d9d9-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="3d9d9-130">Remarks</span></span>

<span data-ttu-id="3d9d9-131">Dois eventos modificados são gerados para cada modificação de um item em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-131">Two modified events are generated for each modification of an item in a folder.</span></span> <span data-ttu-id="3d9d9-132">Um evento é relevante para o item que foi alterado.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-132">One event is relevant to the item that changed.</span></span> <span data-ttu-id="3d9d9-133">O evento outro é relevante para a pasta pai do item.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-133">The other event is relevant to the parent folder of the item.</span></span> <span data-ttu-id="3d9d9-134">Esta é a mesma pasta que a assinatura foi criada contra.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-134">This is the same folder that the subscription was created against.</span></span> <span data-ttu-id="3d9d9-135">O evento que está associado à pasta é usado para se comunicar uma alteração possível para a propriedade [UnreadCount](unreadcount.md) na pasta.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-135">The event that is associated with the folder is used to communicate a potential change to the [UnreadCount](unreadcount.md) property on the folder.</span></span> 
  
<span data-ttu-id="3d9d9-136">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="3d9d9-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3d9d9-137">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3d9d9-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3d9d9-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="3d9d9-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3d9d9-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3d9d9-139">Schema name</span></span>  <br/> |<span data-ttu-id="3d9d9-140">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3d9d9-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="3d9d9-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3d9d9-141">Validation file</span></span>  <br/> |<span data-ttu-id="3d9d9-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3d9d9-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3d9d9-143">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="3d9d9-143">Can be empty</span></span>  <br/> |<span data-ttu-id="3d9d9-144">False</span><span class="sxs-lookup"><span data-stu-id="3d9d9-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3d9d9-145">Ver também</span><span class="sxs-lookup"><span data-stu-id="3d9d9-145">See also</span></span>

- [<span data-ttu-id="3d9d9-146">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="3d9d9-146">Subscribe operation</span></span>](subscribe-operation.md)  
- [<span data-ttu-id="3d9d9-147">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="3d9d9-147">GetEvents operation</span></span>](getevents-operation.md)  
- [<span data-ttu-id="3d9d9-148">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="3d9d9-148">Unsubscribe operation</span></span>](unsubscribe-operation.md)

