---
title: DestinationFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DestinationFolderId
api_type:
- schema
ms.assetid: 77d2d222-320b-4aab-88e4-934ef177f55c
description: O elemento DestinationFolderId indica a pasta de destino para cópia e move ações.
ms.openlocfilehash: bfbacb9c82a681c7963ab5164c43cbb648e726cd
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353375"
---
# <a name="destinationfolderid"></a><span data-ttu-id="b0f26-103">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="b0f26-103">DestinationFolderId</span></span>

<span data-ttu-id="b0f26-104">O elemento **DestinationFolderId** indica a pasta de destino para cópia e move ações.</span><span class="sxs-lookup"><span data-stu-id="b0f26-104">The **DestinationFolderId** element indicates the destination folder for copy and move actions.</span></span> 
  
- [<span data-ttu-id="b0f26-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="b0f26-105">ApplyConversationAction</span></span>](applyconversationaction.md)  
- [<span data-ttu-id="b0f26-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="b0f26-106">ConversationActions</span></span>](conversationactions.md) 
- [<span data-ttu-id="b0f26-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="b0f26-107">ConversationAction</span></span>](conversationaction.md)  
- [<span data-ttu-id="b0f26-108">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="b0f26-108">DestinationFolderId</span></span>](destinationfolderid.md)
  
```XML
<DestinationFolderId>
   <FolderId/>
</DestinationFolderId>
```

```XML
<DestinationFolderId>
   <DistinguishedFolderId/>
</DestinationFolderId>
```

<span data-ttu-id="b0f26-109">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="b0f26-109">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b0f26-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b0f26-110">Attributes and elements</span></span>

<span data-ttu-id="b0f26-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b0f26-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0f26-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="b0f26-112">Attributes</span></span>

<span data-ttu-id="b0f26-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b0f26-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b0f26-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b0f26-114">Child elements</span></span>

|<span data-ttu-id="b0f26-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b0f26-115">**Element**</span></span>|<span data-ttu-id="b0f26-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b0f26-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0f26-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="b0f26-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="b0f26-118">Contém o identificador e alterar a chave da pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="b0f26-118">Contains the identifier and change key of the destination folder.</span></span>  <br/> |
|[<span data-ttu-id="b0f26-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="b0f26-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="b0f26-120">Identifica as pastas que podem ser referidas por nome.</span><span class="sxs-lookup"><span data-stu-id="b0f26-120">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b0f26-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b0f26-121">Parent elements</span></span>

|<span data-ttu-id="b0f26-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b0f26-122">**Element**</span></span>|<span data-ttu-id="b0f26-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b0f26-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0f26-124">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="b0f26-124">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="b0f26-125">Contém uma única ação a ser aplicado a uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="b0f26-125">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b0f26-126">Text value</span><span class="sxs-lookup"><span data-stu-id="b0f26-126">Text value</span></span>

<span data-ttu-id="b0f26-127">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b0f26-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b0f26-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="b0f26-128">Remarks</span></span>

<span data-ttu-id="b0f26-129">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="b0f26-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b0f26-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b0f26-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0f26-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="b0f26-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b0f26-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b0f26-132">Schema Name</span></span>  <br/> |<span data-ttu-id="b0f26-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b0f26-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="b0f26-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b0f26-134">Validation File</span></span>  <br/> |<span data-ttu-id="b0f26-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b0f26-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b0f26-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b0f26-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="b0f26-137">False</span><span class="sxs-lookup"><span data-stu-id="b0f26-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b0f26-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="b0f26-138">See also</span></span>

- [<span data-ttu-id="b0f26-139">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="b0f26-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

