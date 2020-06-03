---
title: MovedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MovedEvent
api_type:
- schema
ms.assetid: 572f8b40-dfa8-47bc-b0c1-e1a7138506fd
description: O elemento MovedEvent representa um evento no qual um item ou pasta é movido de uma pasta pai para outra pasta pai.
ms.openlocfilehash: 1f8fb57dba7edb769fe0dd658d89c032dccf8c5f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530405"
---
# <a name="movedevent"></a><span data-ttu-id="c0ed3-103">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="c0ed3-103">MovedEvent</span></span>

<span data-ttu-id="c0ed3-104">O elemento **MovedEvent** representa um evento no qual um item ou pasta é movido de uma pasta pai para outra pasta pai.</span><span class="sxs-lookup"><span data-stu-id="c0ed3-104">The **MovedEvent** element represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span> 
  
```xml
<MovedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
   <OldItemId/>
   <OldParentFolderId/>
</MovedEvent>
```

```xml
<MovedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</MovedEvent>
```


<span data-ttu-id="c0ed3-105">**MovedCopiedEventType**</span><span class="sxs-lookup"><span data-stu-id="c0ed3-105">**MovedCopiedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c0ed3-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c0ed3-106">Attributes and elements</span></span>

<span data-ttu-id="c0ed3-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c0ed3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c0ed3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c0ed3-108">Attributes</span></span>

<span data-ttu-id="c0ed3-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c0ed3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c0ed3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c0ed3-110">Child elements</span></span>

|<span data-ttu-id="c0ed3-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c0ed3-111">**Element**</span></span>|<span data-ttu-id="c0ed3-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c0ed3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0ed3-113">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="c0ed3-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="c0ed3-114">Representa um indicador de eventos na tabela de eventos de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c0ed3-114">Represents an events bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="c0ed3-115">Registra</span><span class="sxs-lookup"><span data-stu-id="c0ed3-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="c0ed3-116">Representa o carimbo de data/hora de um evento de caixa de correio mover item/pasta.</span><span class="sxs-lookup"><span data-stu-id="c0ed3-116">Represents the timestamp of a move item/folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="c0ed3-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="c0ed3-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="c0ed3-118">Representa o identificador da pasta movida.</span><span class="sxs-lookup"><span data-stu-id="c0ed3-118">Represents the identifier of the moved folder.</span></span>  <br/> |
|[<span data-ttu-id="c0ed3-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="c0ed3-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="c0ed3-120">Representa o identificador do item movido.</span><span class="sxs-lookup"><span data-stu-id="c0ed3-120">Represents the identifier of the moved item.</span></span>  <br/> |
|[<span data-ttu-id="c0ed3-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="c0ed3-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="c0ed3-122">Representa o identificador da pasta que contém o item ou a pasta movido.</span><span class="sxs-lookup"><span data-stu-id="c0ed3-122">Represents the identifier of the folder that contains the moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="c0ed3-123">OldFolderId</span><span class="sxs-lookup"><span data-stu-id="c0ed3-123">OldFolderId</span></span>](oldfolderid.md) <br/> |<span data-ttu-id="c0ed3-124">Contém o identificador de pasta da pasta original antes de ela ser movida ou copiada.</span><span class="sxs-lookup"><span data-stu-id="c0ed3-124">Contains the folder identifier of the original folder before it was moved or copied.</span></span>  <br/> |
|[<span data-ttu-id="c0ed3-125">OldItemId</span><span class="sxs-lookup"><span data-stu-id="c0ed3-125">OldItemId</span></span>](olditemid.md) <br/> |<span data-ttu-id="c0ed3-126">Contém o identificador exclusivo do item original antes de ser movido.</span><span class="sxs-lookup"><span data-stu-id="c0ed3-126">Contains the unique identifier of the original item before it was moved.</span></span>  <br/> |
|[<span data-ttu-id="c0ed3-127">OldParentFolderId</span><span class="sxs-lookup"><span data-stu-id="c0ed3-127">OldParentFolderId</span></span>](oldparentfolderid.md) <br/> |<span data-ttu-id="c0ed3-128">Contém o identificador da pasta pai original de um item ou pasta que foi movido.</span><span class="sxs-lookup"><span data-stu-id="c0ed3-128">Contains the identifier of the original parent folder of an item or folder that was moved.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c0ed3-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c0ed3-129">Parent elements</span></span>

|<span data-ttu-id="c0ed3-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c0ed3-130">**Element**</span></span>|<span data-ttu-id="c0ed3-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c0ed3-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0ed3-132">Notificação</span><span class="sxs-lookup"><span data-stu-id="c0ed3-132">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c0ed3-133">Contém informações sobre a assinatura e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="c0ed3-133">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c0ed3-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="c0ed3-134">Remarks</span></span>

<span data-ttu-id="c0ed3-135">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="c0ed3-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c0ed3-136">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c0ed3-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c0ed3-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="c0ed3-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c0ed3-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c0ed3-138">Schema name</span></span>  <br/> |<span data-ttu-id="c0ed3-139">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c0ed3-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="c0ed3-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c0ed3-140">Validation file</span></span>  <br/> |<span data-ttu-id="c0ed3-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c0ed3-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c0ed3-142">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="c0ed3-142">Can be empty</span></span>  <br/> |<span data-ttu-id="c0ed3-143">False</span><span class="sxs-lookup"><span data-stu-id="c0ed3-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c0ed3-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="c0ed3-144">See also</span></span>

- [<span data-ttu-id="c0ed3-145">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="c0ed3-145">Subscribe operation</span></span>](subscribe-operation.md) 
- [<span data-ttu-id="c0ed3-146">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="c0ed3-146">GetEvents operation</span></span>](getevents-operation.md) 
- [<span data-ttu-id="c0ed3-147">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="c0ed3-147">Unsubscribe operation</span></span>](unsubscribe-operation.md)

