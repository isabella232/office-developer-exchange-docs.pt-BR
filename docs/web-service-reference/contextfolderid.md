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
description: O elemento ContextFolderId indica a pasta que é direcionada para ações que usam pastas. Esse elemento deve estar presente ao copiar, excluir, mover e definir o estado de leitura em itens de conversa em uma pasta de destino.
ms.openlocfilehash: 60f1eaf3b45eee83632c7da6f453a1d09f54d9fd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529256"
---
# <a name="contextfolderid"></a><span data-ttu-id="eaa80-104">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="eaa80-104">ContextFolderId</span></span>

<span data-ttu-id="eaa80-105">O elemento **ContextFolderId** indica a pasta que é direcionada para ações que usam pastas.</span><span class="sxs-lookup"><span data-stu-id="eaa80-105">The **ContextFolderId** element indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="eaa80-106">Esse elemento deve estar presente ao copiar, excluir, mover e definir o estado de leitura em itens de conversa em uma pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="eaa80-106">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span> 
  
- [<span data-ttu-id="eaa80-107">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="eaa80-107">ApplyConversationAction</span></span>](applyconversationaction.md) 
- [<span data-ttu-id="eaa80-108">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="eaa80-108">ConversationActions</span></span>](conversationactions.md)
- [<span data-ttu-id="eaa80-109">Conversation</span><span class="sxs-lookup"><span data-stu-id="eaa80-109">ConversationAction</span></span>](conversationaction.md)
- [<span data-ttu-id="eaa80-110">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="eaa80-110">ContextFolderId</span></span>](contextfolderid.md)
  
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


<span data-ttu-id="eaa80-111">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="eaa80-111">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="eaa80-112">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="eaa80-112">Attributes and elements</span></span>

<span data-ttu-id="eaa80-113">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="eaa80-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eaa80-114">Atributos</span><span class="sxs-lookup"><span data-stu-id="eaa80-114">Attributes</span></span>

<span data-ttu-id="eaa80-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eaa80-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eaa80-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="eaa80-116">Child elements</span></span>

|<span data-ttu-id="eaa80-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="eaa80-117">**Element**</span></span>|<span data-ttu-id="eaa80-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="eaa80-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eaa80-119">FolderId</span><span class="sxs-lookup"><span data-stu-id="eaa80-119">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="eaa80-120">Contém o identificador e a chave de alteração da pasta de contexto.</span><span class="sxs-lookup"><span data-stu-id="eaa80-120">Contains the identifier and change key of the context folder.</span></span>  <br/> |
|[<span data-ttu-id="eaa80-121">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="eaa80-121">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="eaa80-122">Identifica pastas que podem ser referenciadas por nome.</span><span class="sxs-lookup"><span data-stu-id="eaa80-122">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eaa80-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="eaa80-123">Parent elements</span></span>

|<span data-ttu-id="eaa80-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="eaa80-124">**Element**</span></span>|<span data-ttu-id="eaa80-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="eaa80-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eaa80-126">Conversation</span><span class="sxs-lookup"><span data-stu-id="eaa80-126">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="eaa80-127">Contém uma única ação a ser aplicada a uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="eaa80-127">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="eaa80-128">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="eaa80-128">Text value</span></span>

<span data-ttu-id="eaa80-129">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="eaa80-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="eaa80-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="eaa80-130">Remarks</span></span>

<span data-ttu-id="eaa80-131">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="eaa80-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eaa80-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="eaa80-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eaa80-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="eaa80-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eaa80-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="eaa80-134">Schema Name</span></span>  <br/> |<span data-ttu-id="eaa80-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="eaa80-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="eaa80-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="eaa80-136">Validation File</span></span>  <br/> |<span data-ttu-id="eaa80-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="eaa80-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="eaa80-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="eaa80-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="eaa80-139">False</span><span class="sxs-lookup"><span data-stu-id="eaa80-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eaa80-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="eaa80-140">See also</span></span>

- [<span data-ttu-id="eaa80-141">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="eaa80-141">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

