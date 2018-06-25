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
description: O elemento MovedEvent representa um evento na qual um item ou pasta é movida de uma pasta pai para outra pasta pai.
ms.openlocfilehash: a375f421ca9159103e47b515729316b21149c68a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824479"
---
# <a name="movedevent"></a><span data-ttu-id="8b17e-103">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="8b17e-103">MovedEvent</span></span>

<span data-ttu-id="8b17e-104">O elemento **MovedEvent** representa um evento na qual um item ou pasta é movida de uma pasta pai para outra pasta pai.</span><span class="sxs-lookup"><span data-stu-id="8b17e-104">The **MovedEvent** element represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span> 
  
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

 <span data-ttu-id="8b17e-105">**MovedCopiedEventType**</span><span class="sxs-lookup"><span data-stu-id="8b17e-105">**MovedCopiedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8b17e-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8b17e-106">Attributes and elements</span></span>

<span data-ttu-id="8b17e-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8b17e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8b17e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8b17e-108">Attributes</span></span>

<span data-ttu-id="8b17e-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8b17e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8b17e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8b17e-110">Child elements</span></span>

|<span data-ttu-id="8b17e-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8b17e-111">**Element**</span></span>|<span data-ttu-id="8b17e-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8b17e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b17e-113">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="8b17e-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="8b17e-114">Representa um indicador de eventos na tabela de eventos de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="8b17e-114">Represents an events bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="8b17e-115">Carimbo de hora</span><span class="sxs-lookup"><span data-stu-id="8b17e-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="8b17e-116">Representa o carimbo de hora de um evento de caixa de correio de item/pasta de movimentação.</span><span class="sxs-lookup"><span data-stu-id="8b17e-116">Represents the timestamp of a move item/folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="8b17e-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="8b17e-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="8b17e-118">Representa o identificador da pasta movido.</span><span class="sxs-lookup"><span data-stu-id="8b17e-118">Represents the identifier of the moved folder.</span></span>  <br/> |
|[<span data-ttu-id="8b17e-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="8b17e-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="8b17e-120">Representa o identificador do item movido.</span><span class="sxs-lookup"><span data-stu-id="8b17e-120">Represents the identifier of the moved item.</span></span>  <br/> |
|[<span data-ttu-id="8b17e-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="8b17e-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="8b17e-122">Representa o identificador da pasta que contém o item movido ou pasta.</span><span class="sxs-lookup"><span data-stu-id="8b17e-122">Represents the identifier of the folder that contains the moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="8b17e-123">OldFolderId</span><span class="sxs-lookup"><span data-stu-id="8b17e-123">OldFolderId</span></span>](oldfolderid.md) <br/> |<span data-ttu-id="8b17e-124">Contém o identificador de pasta da pasta original antes que ele foi movido ou copiado.</span><span class="sxs-lookup"><span data-stu-id="8b17e-124">Contains the folder identifier of the original folder before it was moved or copied.</span></span>  <br/> |
|[<span data-ttu-id="8b17e-125">OldItemId</span><span class="sxs-lookup"><span data-stu-id="8b17e-125">OldItemId</span></span>](olditemid.md) <br/> |<span data-ttu-id="8b17e-126">Contém o identificador exclusivo do item original antes de ser movida.</span><span class="sxs-lookup"><span data-stu-id="8b17e-126">Contains the unique identifier of the original item before it was moved.</span></span>  <br/> |
|[<span data-ttu-id="8b17e-127">OldParentFolderId</span><span class="sxs-lookup"><span data-stu-id="8b17e-127">OldParentFolderId</span></span>](oldparentfolderid.md) <br/> |<span data-ttu-id="8b17e-128">Contém o identificador da pasta pai original de um item ou a pasta que foi movida.</span><span class="sxs-lookup"><span data-stu-id="8b17e-128">Contains the identifier of the original parent folder of an item or folder that was moved.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8b17e-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8b17e-129">Parent elements</span></span>

|<span data-ttu-id="8b17e-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8b17e-130">**Element**</span></span>|<span data-ttu-id="8b17e-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8b17e-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b17e-132">Notificação</span><span class="sxs-lookup"><span data-stu-id="8b17e-132">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="8b17e-133">Contém informações sobre a inscrição e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="8b17e-133">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8b17e-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="8b17e-134">Remarks</span></span>

<span data-ttu-id="8b17e-135">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="8b17e-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8b17e-136">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8b17e-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8b17e-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="8b17e-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8b17e-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8b17e-138">Schema name</span></span>  <br/> |<span data-ttu-id="8b17e-139">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8b17e-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="8b17e-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8b17e-140">Validation file</span></span>  <br/> |<span data-ttu-id="8b17e-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8b17e-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8b17e-142">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="8b17e-142">Can be empty</span></span>  <br/> |<span data-ttu-id="8b17e-143">False</span><span class="sxs-lookup"><span data-stu-id="8b17e-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8b17e-144">Ver também</span><span class="sxs-lookup"><span data-stu-id="8b17e-144">See also</span></span>



[<span data-ttu-id="8b17e-145">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="8b17e-145">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="8b17e-146">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="8b17e-146">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="8b17e-147">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="8b17e-147">Unsubscribe operation</span></span>](unsubscribe-operation.md)

