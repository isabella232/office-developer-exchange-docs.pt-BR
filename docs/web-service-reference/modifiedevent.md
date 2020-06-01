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
description: O elemento ModifiedEvent representa um evento no qual um item ou pasta é modificado.
ms.openlocfilehash: 1a798773601a0857b9064c7fa6a532a7a36517ab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468548"
---
# <a name="modifiedevent"></a><span data-ttu-id="2033d-103">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="2033d-103">ModifiedEvent</span></span>

<span data-ttu-id="2033d-104">O elemento **ModifiedEvent** representa um evento no qual um item ou pasta é modificado.</span><span class="sxs-lookup"><span data-stu-id="2033d-104">The **ModifiedEvent** element represents an event in which an item or folder is modified.</span></span> 
  
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

<span data-ttu-id="2033d-105">**ModifiedEventType**</span><span class="sxs-lookup"><span data-stu-id="2033d-105">**ModifiedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2033d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="2033d-106">Attributes and elements</span></span>

<span data-ttu-id="2033d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2033d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2033d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2033d-108">Attributes</span></span>

<span data-ttu-id="2033d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2033d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2033d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2033d-110">Child elements</span></span>

|<span data-ttu-id="2033d-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2033d-111">**Element**</span></span>|<span data-ttu-id="2033d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2033d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2033d-113">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="2033d-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="2033d-114">Representa um indicador de evento na tabela de eventos de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2033d-114">Represents an event bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="2033d-115">Registra</span><span class="sxs-lookup"><span data-stu-id="2033d-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="2033d-116">Representa o carimbo de data/hora de um evento de caixa de correio de pasta ou item modificado.</span><span class="sxs-lookup"><span data-stu-id="2033d-116">Represents the timestamp of a modified item or folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="2033d-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="2033d-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="2033d-118">Representa o identificador da pasta modificada.</span><span class="sxs-lookup"><span data-stu-id="2033d-118">Represents the identifier of the modified folder.</span></span>  <br/> |
|[<span data-ttu-id="2033d-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="2033d-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="2033d-120">Representa o identificador do item modificado.</span><span class="sxs-lookup"><span data-stu-id="2033d-120">Represents the identifier of the modified item.</span></span>  <br/> |
|[<span data-ttu-id="2033d-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="2033d-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="2033d-122">Representa o identificador da pasta pai do item ou pasta modificada.</span><span class="sxs-lookup"><span data-stu-id="2033d-122">Represents the identifier of the parent folder of the modified item or folder.</span></span>  <br/> |
|[<span data-ttu-id="2033d-123">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="2033d-123">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="2033d-124">Representa a contagem de itens não lidos em uma determinada pasta.</span><span class="sxs-lookup"><span data-stu-id="2033d-124">Represents the count of unread items within a given folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2033d-125">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2033d-125">Parent elements</span></span>

|<span data-ttu-id="2033d-126">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2033d-126">**Element**</span></span>|<span data-ttu-id="2033d-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2033d-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2033d-128">Notificação</span><span class="sxs-lookup"><span data-stu-id="2033d-128">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2033d-129">Contém informações sobre a assinatura e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="2033d-129">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2033d-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="2033d-130">Remarks</span></span>

<span data-ttu-id="2033d-131">Dois eventos modificados são gerados para cada modificação de um item em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="2033d-131">Two modified events are generated for each modification of an item in a folder.</span></span> <span data-ttu-id="2033d-132">Um evento é relevante para o item que foi alterado.</span><span class="sxs-lookup"><span data-stu-id="2033d-132">One event is relevant to the item that changed.</span></span> <span data-ttu-id="2033d-133">O outro evento é relevante para a pasta pai do item.</span><span class="sxs-lookup"><span data-stu-id="2033d-133">The other event is relevant to the parent folder of the item.</span></span> <span data-ttu-id="2033d-134">Esta é a mesma pasta em que a assinatura foi criada.</span><span class="sxs-lookup"><span data-stu-id="2033d-134">This is the same folder that the subscription was created against.</span></span> <span data-ttu-id="2033d-135">O evento associado à pasta é usado para comunicar uma possível alteração à propriedade [UnreadCount](unreadcount.md) na pasta.</span><span class="sxs-lookup"><span data-stu-id="2033d-135">The event that is associated with the folder is used to communicate a potential change to the [UnreadCount](unreadcount.md) property on the folder.</span></span> 
  
<span data-ttu-id="2033d-136">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="2033d-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2033d-137">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="2033d-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2033d-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="2033d-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2033d-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2033d-139">Schema name</span></span>  <br/> |<span data-ttu-id="2033d-140">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="2033d-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="2033d-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2033d-141">Validation file</span></span>  <br/> |<span data-ttu-id="2033d-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2033d-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2033d-143">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="2033d-143">Can be empty</span></span>  <br/> |<span data-ttu-id="2033d-144">False</span><span class="sxs-lookup"><span data-stu-id="2033d-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2033d-145">Confira também</span><span class="sxs-lookup"><span data-stu-id="2033d-145">See also</span></span>

- [<span data-ttu-id="2033d-146">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="2033d-146">Subscribe operation</span></span>](subscribe-operation.md)  
- [<span data-ttu-id="2033d-147">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="2033d-147">GetEvents operation</span></span>](getevents-operation.md)  
- [<span data-ttu-id="2033d-148">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="2033d-148">Unsubscribe operation</span></span>](unsubscribe-operation.md)

