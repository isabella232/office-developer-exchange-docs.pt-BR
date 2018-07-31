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
ms.openlocfilehash: 94428a079be6da8873c777556771579a7110fb62
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354278"
---
# <a name="contextfolderid"></a><span data-ttu-id="96a59-104">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="96a59-104">ContextFolderId</span></span>

<span data-ttu-id="96a59-105">O elemento **ContextFolderId** indica a pasta que está programada para ações que usam pastas.</span><span class="sxs-lookup"><span data-stu-id="96a59-105">The **ContextFolderId** element indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="96a59-106">Este elemento deve estar presente quando copiar, excluir, mover e definindo o estado lido em itens da conversa em uma pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="96a59-106">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span> 
  
- [<span data-ttu-id="96a59-107">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="96a59-107">ApplyConversationAction</span></span>](applyconversationaction.md) 
- [<span data-ttu-id="96a59-108">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="96a59-108">ConversationActions</span></span>](conversationactions.md)
- [<span data-ttu-id="96a59-109">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="96a59-109">ConversationAction</span></span>](conversationaction.md)
- [<span data-ttu-id="96a59-110">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="96a59-110">ContextFolderId</span></span>](contextfolderid.md)
  
```XML
<ContextFolderId>
   <FolderId/>
</ContextFolderId>
```

```XML
<ContextFolderId>
   <DistinguishedFolderId/>
</ContextFolderId>
```


<span data-ttu-id="96a59-111">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="96a59-111">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="96a59-112">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="96a59-112">Attributes and elements</span></span>

<span data-ttu-id="96a59-113">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="96a59-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96a59-114">Atributos</span><span class="sxs-lookup"><span data-stu-id="96a59-114">Attributes</span></span>

<span data-ttu-id="96a59-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="96a59-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="96a59-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="96a59-116">Child elements</span></span>

|<span data-ttu-id="96a59-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="96a59-117">**Element**</span></span>|<span data-ttu-id="96a59-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="96a59-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96a59-119">FolderId</span><span class="sxs-lookup"><span data-stu-id="96a59-119">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="96a59-120">Contém o identificador e alterar a chave da pasta de contexto.</span><span class="sxs-lookup"><span data-stu-id="96a59-120">Contains the identifier and change key of the context folder.</span></span>  <br/> |
|[<span data-ttu-id="96a59-121">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="96a59-121">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="96a59-122">Identifica as pastas que podem ser referidas por nome.</span><span class="sxs-lookup"><span data-stu-id="96a59-122">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="96a59-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="96a59-123">Parent elements</span></span>

|<span data-ttu-id="96a59-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="96a59-124">**Element**</span></span>|<span data-ttu-id="96a59-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="96a59-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96a59-126">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="96a59-126">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="96a59-127">Contém uma única ação a ser aplicado a uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="96a59-127">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="96a59-128">Text value</span><span class="sxs-lookup"><span data-stu-id="96a59-128">Text value</span></span>

<span data-ttu-id="96a59-129">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="96a59-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="96a59-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="96a59-130">Remarks</span></span>

<span data-ttu-id="96a59-131">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="96a59-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="96a59-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="96a59-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96a59-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="96a59-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="96a59-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="96a59-134">Schema Name</span></span>  <br/> |<span data-ttu-id="96a59-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="96a59-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="96a59-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="96a59-136">Validation File</span></span>  <br/> |<span data-ttu-id="96a59-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="96a59-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="96a59-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="96a59-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="96a59-139">False</span><span class="sxs-lookup"><span data-stu-id="96a59-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="96a59-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="96a59-140">See also</span></span>

- [<span data-ttu-id="96a59-141">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="96a59-141">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

