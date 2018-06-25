---
title: ContextFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContextFolderId
api_type:
- schema
ms.assetid: 48de92aa-e124-42b5-89bc-cdce5e93d78b
description: O elemento ContextFolderId indica a pasta que está programada para ações que usam pastas. Este elemento deve estar presente quando copiar, excluir, mover e definindo o estado lido em itens da conversa em uma pasta de destino.
ms.openlocfilehash: bd863d0395b9b9d7b437833acfb656fec4580985
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751510"
---
# <a name="contextfolderid"></a><span data-ttu-id="8389c-104">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="8389c-104">ContextFolderId</span></span>

<span data-ttu-id="8389c-105">O elemento **ContextFolderId** indica a pasta que está programada para ações que usam pastas.</span><span class="sxs-lookup"><span data-stu-id="8389c-105">The **ContextFolderId** element indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="8389c-106">Este elemento deve estar presente quando copiar, excluir, mover e definindo o estado lido em itens da conversa em uma pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="8389c-106">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span> 
  
[<span data-ttu-id="8389c-107">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="8389c-107">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="8389c-108">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="8389c-108">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="8389c-109">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="8389c-109">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="8389c-110">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="8389c-110">ContextFolderId</span></span>](contextfolderid.md)
  
```XML
<ContextFolderId>
   <FolderId/>
</ContextFolderId>
```

 <span data-ttu-id="8389c-111">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="8389c-111">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8389c-112">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8389c-112">Attributes and elements</span></span>

<span data-ttu-id="8389c-113">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8389c-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8389c-114">Atributos</span><span class="sxs-lookup"><span data-stu-id="8389c-114">Attributes</span></span>

<span data-ttu-id="8389c-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8389c-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8389c-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8389c-116">Child elements</span></span>

|<span data-ttu-id="8389c-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8389c-117">**Element**</span></span>|<span data-ttu-id="8389c-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8389c-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8389c-119">FolderId</span><span class="sxs-lookup"><span data-stu-id="8389c-119">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="8389c-120">Contém o identificador e alterar a chave da pasta de contexto.</span><span class="sxs-lookup"><span data-stu-id="8389c-120">Contains the identifier and change key of the context folder.</span></span>  <br/> |
|[<span data-ttu-id="8389c-121">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="8389c-121">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="8389c-122">Identifica as pastas que podem ser referidas por nome.</span><span class="sxs-lookup"><span data-stu-id="8389c-122">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8389c-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8389c-123">Parent elements</span></span>

|<span data-ttu-id="8389c-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8389c-124">**Element**</span></span>|<span data-ttu-id="8389c-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8389c-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8389c-126">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="8389c-126">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="8389c-127">Contém uma única ação a ser aplicado a uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="8389c-127">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8389c-128">Text value</span><span class="sxs-lookup"><span data-stu-id="8389c-128">Text value</span></span>

<span data-ttu-id="8389c-129">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8389c-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8389c-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="8389c-130">Remarks</span></span>

<span data-ttu-id="8389c-131">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="8389c-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8389c-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8389c-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8389c-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="8389c-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8389c-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8389c-134">Schema Name</span></span>  <br/> |<span data-ttu-id="8389c-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8389c-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="8389c-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8389c-136">Validation File</span></span>  <br/> |<span data-ttu-id="8389c-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8389c-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8389c-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8389c-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="8389c-139">False</span><span class="sxs-lookup"><span data-stu-id="8389c-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8389c-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="8389c-140">See also</span></span>



[<span data-ttu-id="8389c-141">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="8389c-141">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

