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
description: O elemento Action contém a ação a ser executada na conversa especificada pelo elemento CONVERSATION.
ms.openlocfilehash: f97b04b98cdc29bee9aff5fa1fc6f37400b8314c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527541"
---
# <a name="action-conversationactiontypetype"></a><span data-ttu-id="58163-103">Ação (ConversationActionTypeType)</span><span class="sxs-lookup"><span data-stu-id="58163-103">Action (ConversationActionTypeType)</span></span>

<span data-ttu-id="58163-104">O elemento **Action** contém a ação a ser executada na conversa especificada pelo elemento [Conversation](conversationid.md) .</span><span class="sxs-lookup"><span data-stu-id="58163-104">The **Action** element contains the action to perform on the conversation specified by the [ConversationId](conversationid.md) element.</span></span> 
  
- [<span data-ttu-id="58163-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="58163-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
- [<span data-ttu-id="58163-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="58163-106">ConversationActions</span></span>](conversationactions.md)
  
- [<span data-ttu-id="58163-107">Conversation</span><span class="sxs-lookup"><span data-stu-id="58163-107">ConversationAction</span></span>](conversationaction.md)
  
- [<span data-ttu-id="58163-108">Ação (ConversationActionTypeType)</span><span class="sxs-lookup"><span data-stu-id="58163-108">Action (ConversationActionTypeType)</span></span>](action-conversationactiontypetype.md)
  
```XML
<Action> AlwaysCategorize | AlwaysDelete | AlwaysMove | Delete | Move | Copy | SetReadState </Action>
```

 <span data-ttu-id="58163-109">**ConversationActionTypeType**</span><span class="sxs-lookup"><span data-stu-id="58163-109">**ConversationActionTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="58163-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="58163-110">Attributes and elements</span></span>

<span data-ttu-id="58163-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="58163-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="58163-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="58163-112">Attributes</span></span>

<span data-ttu-id="58163-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="58163-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="58163-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="58163-114">Child elements</span></span>

<span data-ttu-id="58163-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="58163-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="58163-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="58163-116">Parent elements</span></span>

|<span data-ttu-id="58163-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="58163-117">**Element**</span></span>|<span data-ttu-id="58163-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="58163-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="58163-119">Conversation</span><span class="sxs-lookup"><span data-stu-id="58163-119">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="58163-120">Contém uma única ação a ser aplicada a uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="58163-120">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="58163-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="58163-121">Text value</span></span>

<span data-ttu-id="58163-122">O valor de texto do elemento **Action** indica qual ação será executada em uma conversa.</span><span class="sxs-lookup"><span data-stu-id="58163-122">The text value of the **Action** element indicates which action will be performed on a conversation.</span></span> <span data-ttu-id="58163-123">Estes são os valores de texto possíveis e as ações correspondentes:</span><span class="sxs-lookup"><span data-stu-id="58163-123">The following are the possible text values and the corresponding actions:</span></span> 
  
- <span data-ttu-id="58163-124">**AlwaysCategorize** -os itens atuais e novos itens na conversa serão automaticamente definidos com as categorias identificadas no elemento [Categories](categories-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="58163-124">**AlwaysCategorize** - The current items and new items in the conversation will automatically be set with the categories identified in the [Categories](categories-ex15websvcsotherref.md) element.</span></span> 
    
- <span data-ttu-id="58163-125">**AlwaysDelete** -os itens atuais e novos itens na conversa serão excluídos automaticamente.</span><span class="sxs-lookup"><span data-stu-id="58163-125">**AlwaysDelete** - The current items and new items in the conversation will automatically be deleted.</span></span> <span data-ttu-id="58163-126">O modo de exclusão é definido pelo elemento [DeleteType](deletetype.md) .</span><span class="sxs-lookup"><span data-stu-id="58163-126">The deletion mode is set by the [DeleteType](deletetype.md) element.</span></span> 
    
- <span data-ttu-id="58163-127">**AlwaysMove** -os itens atuais e os novos itens da conversa serão movidos automaticamente para a pasta identificada pelo elemento [DestinationFolderId](destinationfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="58163-127">**AlwaysMove** - The current items and new items in the conversation will automatically be moved to the folder identified by the [DestinationFolderId](destinationfolderid.md) element.</span></span> 
    
- <span data-ttu-id="58163-128">**Excluir** -os itens atuais da conversa serão excluídos.</span><span class="sxs-lookup"><span data-stu-id="58163-128">**Delete** - The current items in the conversation will be deleted.</span></span> <span data-ttu-id="58163-129">Os itens subsequentes na conversa não serão excluídos.</span><span class="sxs-lookup"><span data-stu-id="58163-129">Subsequent items in the conversation will not be deleted.</span></span> <span data-ttu-id="58163-130">O modo de exclusão é definido pelo elemento [DeleteType](deletetype.md) .</span><span class="sxs-lookup"><span data-stu-id="58163-130">The deletion mode is set by the [DeleteType](deletetype.md) element.</span></span> 
    
- <span data-ttu-id="58163-131">**Move** -os itens atuais na conversa serão movidos para a pasta identificada pelo elemento [DestinationFolderId](destinationfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="58163-131">**Move** - The current items in the conversation will be moved to the folder identified by the [DestinationFolderId](destinationfolderid.md) element.</span></span> <span data-ttu-id="58163-132">Os itens subsequentes na conversa não serão movidos.</span><span class="sxs-lookup"><span data-stu-id="58163-132">Subsequent items in the conversation will not be moved.</span></span> 
    
- <span data-ttu-id="58163-133">**Copy** – os itens atuais na conversa serão copiados para a pasta identificada pelo elemento [DestinationFolderId](destinationfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="58163-133">**Copy** - The current items in the conversation will be copied to the folder identified by the [DestinationFolderId](destinationfolderid.md) element.</span></span> <span data-ttu-id="58163-134">Os itens subsequentes na conversa não serão copiados.</span><span class="sxs-lookup"><span data-stu-id="58163-134">Subsequent items in the conversation will not be copied.</span></span> 
    
- <span data-ttu-id="58163-135">**Setreadstate** -os itens atuais na conversa terão o estado de leitura definido.</span><span class="sxs-lookup"><span data-stu-id="58163-135">**SetReadState** - The current items in the conversation will have their read state set.</span></span> <span data-ttu-id="58163-136">O estado de leitura é definido pelo elemento [IsRead](isread.md) .</span><span class="sxs-lookup"><span data-stu-id="58163-136">The read state is set by the [IsRead](isread.md) element.</span></span> 
    
- <span data-ttu-id="58163-137">**Flag** -os itens atuais na conversa terão um sinalizador definido conforme definido pelo elemento [Flag](flag.md) .</span><span class="sxs-lookup"><span data-stu-id="58163-137">**Flag** - The current items in the conversation will have a flag set as defined by the [Flag](flag.md) element.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="58163-138">Comentários</span><span class="sxs-lookup"><span data-stu-id="58163-138">Remarks</span></span>

<span data-ttu-id="58163-139">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="58163-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="58163-140">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="58163-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="58163-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="58163-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="58163-142">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="58163-142">Schema Name</span></span>  <br/> |<span data-ttu-id="58163-143">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="58163-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="58163-144">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="58163-144">Validation File</span></span>  <br/> |<span data-ttu-id="58163-145">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="58163-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="58163-146">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="58163-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="58163-147">False</span><span class="sxs-lookup"><span data-stu-id="58163-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="58163-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="58163-148">See also</span></span>

- [<span data-ttu-id="58163-149">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="58163-149">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="58163-150">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="58163-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

