---
title: CopiedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopiedEvent
api_type:
- schema
ms.assetid: 82f2fcac-deaa-4ff8-801f-4fe28d8a19f5
description: O elemento CopiedEvent representa um evento no qual um item ou pasta é copiado.
ms.openlocfilehash: 928910ddbe0bf1e48549d1665ab373f7382366d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529242"
---
# <a name="copiedevent"></a><span data-ttu-id="76fff-103">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="76fff-103">CopiedEvent</span></span>

<span data-ttu-id="76fff-104">O elemento **CopiedEvent** representa um evento no qual um item ou pasta é copiado.</span><span class="sxs-lookup"><span data-stu-id="76fff-104">The **CopiedEvent** element represents an event in which an item or folder is copied.</span></span> 
  
```xml
<CopiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</CopiedEvent>
```

```xml
<CopiedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</CopiedEvent>
```

<span data-ttu-id="76fff-105">**MovedCopiedEventType**</span><span class="sxs-lookup"><span data-stu-id="76fff-105">**MovedCopiedEventType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="76fff-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="76fff-106">Attributes and elements</span></span>

<span data-ttu-id="76fff-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="76fff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="76fff-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="76fff-108">Attributes</span></span>

<span data-ttu-id="76fff-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="76fff-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="76fff-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="76fff-110">Child elements</span></span>

|<span data-ttu-id="76fff-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="76fff-111">**Element**</span></span>|<span data-ttu-id="76fff-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="76fff-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76fff-113">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="76fff-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="76fff-114">Representa um indicador de eventos na tabela de eventos de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="76fff-114">Represents an events bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="76fff-115">Registra</span><span class="sxs-lookup"><span data-stu-id="76fff-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="76fff-116">Representa o carimbo de data/hora de um evento Copiar item/pasta de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="76fff-116">Represents the timestamp of a copy item/folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="76fff-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="76fff-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="76fff-118">Representa o identificador da pasta.</span><span class="sxs-lookup"><span data-stu-id="76fff-118">Represents the identifier of the folder.</span></span>  <br/> |
|[<span data-ttu-id="76fff-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="76fff-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="76fff-120">Representa o identificador do item.</span><span class="sxs-lookup"><span data-stu-id="76fff-120">Represents the identifier of the item.</span></span>  <br/> |
|[<span data-ttu-id="76fff-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="76fff-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="76fff-122">Representa o identificador da pasta que contém a cópia.</span><span class="sxs-lookup"><span data-stu-id="76fff-122">Represents the identifier of the folder that contains the copy.</span></span>  <br/> |
|[<span data-ttu-id="76fff-123">OldFolderId</span><span class="sxs-lookup"><span data-stu-id="76fff-123">OldFolderId</span></span>](oldfolderid.md) <br/> |<span data-ttu-id="76fff-124">Representa o identificador de pasta da pasta original antes de ela ser copiada.</span><span class="sxs-lookup"><span data-stu-id="76fff-124">Represents the folder identifier of the original folder before it was copied.</span></span>  <br/> |
|[<span data-ttu-id="76fff-125">OldItemId</span><span class="sxs-lookup"><span data-stu-id="76fff-125">OldItemId</span></span>](olditemid.md) <br/> |<span data-ttu-id="76fff-126">Contém o identificador exclusivo do item original antes de ser copiado.</span><span class="sxs-lookup"><span data-stu-id="76fff-126">Contains the unique identifier of the original item before it was copied.</span></span>  <br/> |
|[<span data-ttu-id="76fff-127">OldParentFolderId</span><span class="sxs-lookup"><span data-stu-id="76fff-127">OldParentFolderId</span></span>](oldparentfolderid.md) <br/> |<span data-ttu-id="76fff-128">Contém o identificador da pasta pai original de um item ou pasta que foi copiado.</span><span class="sxs-lookup"><span data-stu-id="76fff-128">Contains the identifier of the original parent folder of an item or folder that was copied.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="76fff-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="76fff-129">Parent elements</span></span>

|<span data-ttu-id="76fff-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="76fff-130">**Element**</span></span>|<span data-ttu-id="76fff-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="76fff-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76fff-132">Notificação</span><span class="sxs-lookup"><span data-stu-id="76fff-132">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="76fff-133">Contém informações sobre a assinatura e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="76fff-133">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="76fff-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="76fff-134">Remarks</span></span>

<span data-ttu-id="76fff-135">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="76fff-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="76fff-136">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="76fff-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="76fff-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="76fff-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="76fff-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="76fff-138">Schema name</span></span>  <br/> |<span data-ttu-id="76fff-139">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="76fff-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="76fff-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="76fff-140">Validation file</span></span>  <br/> |<span data-ttu-id="76fff-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="76fff-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="76fff-142">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="76fff-142">Can be empty</span></span>  <br/> |<span data-ttu-id="76fff-143">False</span><span class="sxs-lookup"><span data-stu-id="76fff-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="76fff-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="76fff-144">See also</span></span>

- [<span data-ttu-id="76fff-145">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="76fff-145">Subscribe operation</span></span>](subscribe-operation.md) 
- [<span data-ttu-id="76fff-146">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="76fff-146">GetEvents operation</span></span>](getevents-operation.md) 
- [<span data-ttu-id="76fff-147">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="76fff-147">Unsubscribe operation</span></span>](unsubscribe-operation.md)
- [<span data-ttu-id="76fff-148">Usando assinaturas pull</span><span class="sxs-lookup"><span data-stu-id="76fff-148">Using Pull Subscriptions</span></span>](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx) 
- [<span data-ttu-id="76fff-149">Aplicativo de amostra de notificação por push</span><span class="sxs-lookup"><span data-stu-id="76fff-149">Push Notification Sample Application</span></span>](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

