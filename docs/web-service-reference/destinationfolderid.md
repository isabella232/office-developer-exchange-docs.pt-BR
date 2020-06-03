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
description: O elemento DestinationFolderId indica a pasta de destino para ações de copiar e mover.
ms.openlocfilehash: dbfd25084dbd4ea9d5f4ddf98b256d02e71139d3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526911"
---
# <a name="destinationfolderid"></a><span data-ttu-id="e3f28-103">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="e3f28-103">DestinationFolderId</span></span>

<span data-ttu-id="e3f28-104">O elemento **DestinationFolderId** indica a pasta de destino para ações de copiar e mover.</span><span class="sxs-lookup"><span data-stu-id="e3f28-104">The **DestinationFolderId** element indicates the destination folder for copy and move actions.</span></span> 
  
- [<span data-ttu-id="e3f28-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="e3f28-105">ApplyConversationAction</span></span>](applyconversationaction.md)  
- [<span data-ttu-id="e3f28-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="e3f28-106">ConversationActions</span></span>](conversationactions.md) 
- [<span data-ttu-id="e3f28-107">Conversation</span><span class="sxs-lookup"><span data-stu-id="e3f28-107">ConversationAction</span></span>](conversationaction.md)  
- [<span data-ttu-id="e3f28-108">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="e3f28-108">DestinationFolderId</span></span>](destinationfolderid.md)
  
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

<span data-ttu-id="e3f28-109">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="e3f28-109">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e3f28-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e3f28-110">Attributes and elements</span></span>

<span data-ttu-id="e3f28-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e3f28-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e3f28-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="e3f28-112">Attributes</span></span>

<span data-ttu-id="e3f28-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e3f28-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e3f28-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e3f28-114">Child elements</span></span>

|<span data-ttu-id="e3f28-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e3f28-115">**Element**</span></span>|<span data-ttu-id="e3f28-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e3f28-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3f28-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="e3f28-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="e3f28-118">Contém o identificador e a chave de alteração da pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="e3f28-118">Contains the identifier and change key of the destination folder.</span></span>  <br/> |
|[<span data-ttu-id="e3f28-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="e3f28-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="e3f28-120">Identifica pastas que podem ser referenciadas por nome.</span><span class="sxs-lookup"><span data-stu-id="e3f28-120">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e3f28-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e3f28-121">Parent elements</span></span>

|<span data-ttu-id="e3f28-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e3f28-122">**Element**</span></span>|<span data-ttu-id="e3f28-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e3f28-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3f28-124">Conversation</span><span class="sxs-lookup"><span data-stu-id="e3f28-124">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="e3f28-125">Contém uma única ação a ser aplicada a uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="e3f28-125">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e3f28-126">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="e3f28-126">Text value</span></span>

<span data-ttu-id="e3f28-127">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e3f28-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e3f28-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="e3f28-128">Remarks</span></span>

<span data-ttu-id="e3f28-129">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e3f28-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e3f28-130">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e3f28-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e3f28-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="e3f28-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e3f28-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e3f28-132">Schema Name</span></span>  <br/> |<span data-ttu-id="e3f28-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e3f28-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="e3f28-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e3f28-134">Validation File</span></span>  <br/> |<span data-ttu-id="e3f28-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e3f28-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e3f28-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e3f28-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="e3f28-137">False</span><span class="sxs-lookup"><span data-stu-id="e3f28-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e3f28-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="e3f28-138">See also</span></span>

- [<span data-ttu-id="e3f28-139">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="e3f28-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

