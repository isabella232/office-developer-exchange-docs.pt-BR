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
description: O elemento CopiedEvent representa um evento no qual uma pasta ou um item é copiada.
ms.openlocfilehash: 89ca9fb1fd2f4187efdec0e087d840bfee197a29
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751542"
---
# <a name="copiedevent"></a><span data-ttu-id="73373-103">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="73373-103">CopiedEvent</span></span>

<span data-ttu-id="73373-104">O elemento **CopiedEvent** representa um evento no qual uma pasta ou um item é copiada.</span><span class="sxs-lookup"><span data-stu-id="73373-104">The **CopiedEvent** element represents an event in which an item or folder is copied.</span></span> 
  
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

 <span data-ttu-id="73373-105">**MovedCopiedEventType**</span><span class="sxs-lookup"><span data-stu-id="73373-105">**MovedCopiedEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="73373-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="73373-106">Attributes and elements</span></span>

<span data-ttu-id="73373-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="73373-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="73373-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="73373-108">Attributes</span></span>

<span data-ttu-id="73373-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="73373-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="73373-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="73373-110">Child elements</span></span>

|<span data-ttu-id="73373-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="73373-111">**Element**</span></span>|<span data-ttu-id="73373-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="73373-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="73373-113">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="73373-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="73373-114">Representa um indicador de eventos na tabela de eventos de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="73373-114">Represents an events bookmark in the mailbox events table.</span></span>  <br/> |
|[<span data-ttu-id="73373-115">Carimbo de hora</span><span class="sxs-lookup"><span data-stu-id="73373-115">TimeStamp</span></span>](timestamp.md) <br/> |<span data-ttu-id="73373-116">Representa o carimbo de hora de um evento de caixa de correio de item/pasta de cópia.</span><span class="sxs-lookup"><span data-stu-id="73373-116">Represents the timestamp of a copy item/folder mailbox event.</span></span>  <br/> |
|[<span data-ttu-id="73373-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="73373-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="73373-118">Representa o identificador da pasta.</span><span class="sxs-lookup"><span data-stu-id="73373-118">Represents the identifier of the folder.</span></span>  <br/> |
|[<span data-ttu-id="73373-119">ItemId</span><span class="sxs-lookup"><span data-stu-id="73373-119">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="73373-120">Representa o identificador do item.</span><span class="sxs-lookup"><span data-stu-id="73373-120">Represents the identifier of the item.</span></span>  <br/> |
|[<span data-ttu-id="73373-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="73373-121">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="73373-122">Representa o identificador da pasta que contém a cópia.</span><span class="sxs-lookup"><span data-stu-id="73373-122">Represents the identifier of the folder that contains the copy.</span></span>  <br/> |
|[<span data-ttu-id="73373-123">OldFolderId</span><span class="sxs-lookup"><span data-stu-id="73373-123">OldFolderId</span></span>](oldfolderid.md) <br/> |<span data-ttu-id="73373-124">Representa o identificador de pasta da pasta original antes que ele foi copiado.</span><span class="sxs-lookup"><span data-stu-id="73373-124">Represents the folder identifier of the original folder before it was copied.</span></span>  <br/> |
|[<span data-ttu-id="73373-125">OldItemId</span><span class="sxs-lookup"><span data-stu-id="73373-125">OldItemId</span></span>](olditemid.md) <br/> |<span data-ttu-id="73373-126">Contém o identificador exclusivo do item original antes que ele foi copiado.</span><span class="sxs-lookup"><span data-stu-id="73373-126">Contains the unique identifier of the original item before it was copied.</span></span>  <br/> |
|[<span data-ttu-id="73373-127">OldParentFolderId</span><span class="sxs-lookup"><span data-stu-id="73373-127">OldParentFolderId</span></span>](oldparentfolderid.md) <br/> |<span data-ttu-id="73373-128">Contém o identificador da pasta pai original de um item ou a pasta que foi copiada.</span><span class="sxs-lookup"><span data-stu-id="73373-128">Contains the identifier of the original parent folder of an item or folder that was copied.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="73373-129">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="73373-129">Parent elements</span></span>

|<span data-ttu-id="73373-130">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="73373-130">**Element**</span></span>|<span data-ttu-id="73373-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="73373-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="73373-132">Notificação</span><span class="sxs-lookup"><span data-stu-id="73373-132">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="73373-133">Contém informações sobre a inscrição e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="73373-133">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="73373-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="73373-134">Remarks</span></span>

<span data-ttu-id="73373-135">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="73373-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="73373-136">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="73373-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="73373-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="73373-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="73373-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="73373-138">Schema name</span></span>  <br/> |<span data-ttu-id="73373-139">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="73373-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="73373-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="73373-140">Validation file</span></span>  <br/> |<span data-ttu-id="73373-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="73373-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="73373-142">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="73373-142">Can be empty</span></span>  <br/> |<span data-ttu-id="73373-143">False</span><span class="sxs-lookup"><span data-stu-id="73373-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="73373-144">Ver também</span><span class="sxs-lookup"><span data-stu-id="73373-144">See also</span></span>



[<span data-ttu-id="73373-145">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="73373-145">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="73373-146">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="73373-146">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="73373-147">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="73373-147">Unsubscribe operation</span></span>](unsubscribe-operation.md)


[<span data-ttu-id="73373-148">Usando inscrições de recepção</span><span class="sxs-lookup"><span data-stu-id="73373-148">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[<span data-ttu-id="73373-149">Aplicativo de amostra de notificação de push</span><span class="sxs-lookup"><span data-stu-id="73373-149">Push Notification Sample Application</span></span>](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

