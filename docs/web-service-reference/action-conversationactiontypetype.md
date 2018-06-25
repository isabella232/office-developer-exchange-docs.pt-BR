---
title: Ação (ConversationActionTypeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Action
api_type:
- schema
ms.assetid: 8bbc12f2-76c5-4fda-828f-56b2086a0454
description: O elemento Action contém a ação a ser executada a conversa especificada pelo elemento ConversationId.
ms.openlocfilehash: b468eeaf0c2509bfa53cbd83f497f0bae20a7f68
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751033"
---
# <a name="action-conversationactiontypetype"></a><span data-ttu-id="cc3f6-103">Ação (ConversationActionTypeType)</span><span class="sxs-lookup"><span data-stu-id="cc3f6-103">Action (ConversationActionTypeType)</span></span>

<span data-ttu-id="cc3f6-104">O elemento **Action** contém a ação a ser executada a conversa especificada pelo elemento [ConversationId](conversationid.md) .</span><span class="sxs-lookup"><span data-stu-id="cc3f6-104">The **Action** element contains the action to perform on the conversation specified by the [ConversationId](conversationid.md) element.</span></span> 
  
- [<span data-ttu-id="cc3f6-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="cc3f6-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
- [<span data-ttu-id="cc3f6-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="cc3f6-106">ConversationActions</span></span>](conversationactions.md)
  
- [<span data-ttu-id="cc3f6-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="cc3f6-107">ConversationAction</span></span>](conversationaction.md)
  
- [<span data-ttu-id="cc3f6-108">Ação (ConversationActionTypeType)</span><span class="sxs-lookup"><span data-stu-id="cc3f6-108">Action (ConversationActionTypeType)</span></span>](action-conversationactiontypetype.md)
  
```XML
<Action> AlwaysCategorize | AlwaysDelete | AlwaysMove | Delete | Move | Copy | SetReadState </Action>
```

 <span data-ttu-id="cc3f6-109">**ConversationActionTypeType**</span><span class="sxs-lookup"><span data-stu-id="cc3f6-109">**ConversationActionTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cc3f6-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="cc3f6-110">Attributes and elements</span></span>

<span data-ttu-id="cc3f6-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cc3f6-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cc3f6-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="cc3f6-112">Attributes</span></span>

<span data-ttu-id="cc3f6-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cc3f6-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cc3f6-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cc3f6-114">Child elements</span></span>

<span data-ttu-id="cc3f6-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cc3f6-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cc3f6-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cc3f6-116">Parent elements</span></span>

|<span data-ttu-id="cc3f6-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cc3f6-117">**Element**</span></span>|<span data-ttu-id="cc3f6-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cc3f6-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc3f6-119">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="cc3f6-119">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="cc3f6-120">Contém uma única ação a ser aplicado a uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="cc3f6-120">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cc3f6-121">Text value</span><span class="sxs-lookup"><span data-stu-id="cc3f6-121">Text value</span></span>

<span data-ttu-id="cc3f6-122">O valor de texto do elemento **Action** indica a ação que será executada em uma conversa.</span><span class="sxs-lookup"><span data-stu-id="cc3f6-122">The text value of the **Action** element indicates which action will be performed on a conversation.</span></span> <span data-ttu-id="cc3f6-123">Estes são os valores de texto possíveis e as ações correspondentes:</span><span class="sxs-lookup"><span data-stu-id="cc3f6-123">The following are the possible text values and the corresponding actions:</span></span> 
  
- <span data-ttu-id="cc3f6-124">**AlwaysCategorize** - os itens atuais e novos itens da conversa serão definidas automaticamente com as categorias identificadas no elemento [categorias](categories-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="cc3f6-124">**AlwaysCategorize** - The current items and new items in the conversation will automatically be set with the categories identified in the [Categories](categories-ex15websvcsotherref.md) element.</span></span> 
    
- <span data-ttu-id="cc3f6-125">**AlwaysDelete** - os itens atuais e novos itens da conversa serão excluídas automaticamente.</span><span class="sxs-lookup"><span data-stu-id="cc3f6-125">**AlwaysDelete** - The current items and new items in the conversation will automatically be deleted.</span></span> <span data-ttu-id="cc3f6-126">O modo de exclusão é definido pelo elemento [DeleteType](deletetype.md) .</span><span class="sxs-lookup"><span data-stu-id="cc3f6-126">The deletion mode is set by the [DeleteType](deletetype.md) element.</span></span> 
    
- <span data-ttu-id="cc3f6-127">**AlwaysMove** - os itens atuais e novos itens da conversa serão movidas automaticamente para a pasta identificada pelo elemento [DestinationFolderId](destinationfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="cc3f6-127">**AlwaysMove** - The current items and new items in the conversation will automatically be moved to the folder identified by the [DestinationFolderId](destinationfolderid.md) element.</span></span> 
    
- <span data-ttu-id="cc3f6-128">**Excluir** - os itens da conversa atuais será excluído.</span><span class="sxs-lookup"><span data-stu-id="cc3f6-128">**Delete** - The current items in the conversation will be deleted.</span></span> <span data-ttu-id="cc3f6-129">Os itens na conversa subsequentes não serão excluídos.</span><span class="sxs-lookup"><span data-stu-id="cc3f6-129">Subsequent items in the conversation will not be deleted.</span></span> <span data-ttu-id="cc3f6-130">O modo de exclusão é definido pelo elemento [DeleteType](deletetype.md) .</span><span class="sxs-lookup"><span data-stu-id="cc3f6-130">The deletion mode is set by the [DeleteType](deletetype.md) element.</span></span> 
    
- <span data-ttu-id="cc3f6-131">**Mova** - os itens atuais na conversa serão movidas para a pasta identificada pelo elemento [DestinationFolderId](destinationfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="cc3f6-131">**Move** - The current items in the conversation will be moved to the folder identified by the [DestinationFolderId](destinationfolderid.md) element.</span></span> <span data-ttu-id="cc3f6-132">Os itens na conversa subsequentes não serão movidos.</span><span class="sxs-lookup"><span data-stu-id="cc3f6-132">Subsequent items in the conversation will not be moved.</span></span> 
    
- <span data-ttu-id="cc3f6-133">**Copy** - os itens da conversa atuais serão copiadas para a pasta identificada pelo elemento [DestinationFolderId](destinationfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="cc3f6-133">**Copy** - The current items in the conversation will be copied to the folder identified by the [DestinationFolderId](destinationfolderid.md) element.</span></span> <span data-ttu-id="cc3f6-134">Os itens na conversa subsequentes não serão copiados.</span><span class="sxs-lookup"><span data-stu-id="cc3f6-134">Subsequent items in the conversation will not be copied.</span></span> 
    
- <span data-ttu-id="cc3f6-135">**SetReadState** - os itens da conversa atuais terá seu estado de leitura definido.</span><span class="sxs-lookup"><span data-stu-id="cc3f6-135">**SetReadState** - The current items in the conversation will have their read state set.</span></span> <span data-ttu-id="cc3f6-136">O estado lido é definido pelo elemento [foi lido](isread.md) .</span><span class="sxs-lookup"><span data-stu-id="cc3f6-136">The read state is set by the [IsRead](isread.md) element.</span></span> 
    
- <span data-ttu-id="cc3f6-137">**Sinalizador** - os itens da conversa atuais terão um sinalizador definido como determinado pelo elemento [sinalizador](flag.md) .</span><span class="sxs-lookup"><span data-stu-id="cc3f6-137">**Flag** - The current items in the conversation will have a flag set as defined by the [Flag](flag.md) element.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="cc3f6-138">Comentários</span><span class="sxs-lookup"><span data-stu-id="cc3f6-138">Remarks</span></span>

<span data-ttu-id="cc3f6-139">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="cc3f6-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cc3f6-140">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="cc3f6-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cc3f6-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="cc3f6-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cc3f6-142">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cc3f6-142">Schema Name</span></span>  <br/> |<span data-ttu-id="cc3f6-143">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="cc3f6-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="cc3f6-144">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cc3f6-144">Validation File</span></span>  <br/> |<span data-ttu-id="cc3f6-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cc3f6-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cc3f6-146">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="cc3f6-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="cc3f6-147">False</span><span class="sxs-lookup"><span data-stu-id="cc3f6-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cc3f6-148">Ver também</span><span class="sxs-lookup"><span data-stu-id="cc3f6-148">See also</span></span>

- [<span data-ttu-id="cc3f6-149">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="cc3f6-149">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="cc3f6-150">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="cc3f6-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

