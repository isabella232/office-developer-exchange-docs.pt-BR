---
title: Conversation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationAction
api_type:
- schema
ms.assetid: 9ecea41a-3860-4569-8e9b-284b451fc4e0
description: O elemento Conversation contém uma única ação a ser aplicada a uma única conversa.
ms.openlocfilehash: cb7d874f787b105d5185749dfaf1e940d2411d89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529249"
---
# <a name="conversationaction"></a><span data-ttu-id="902d8-103">Conversation</span><span class="sxs-lookup"><span data-stu-id="902d8-103">ConversationAction</span></span>

<span data-ttu-id="902d8-104">O elemento **Conversation** contém uma única ação a ser aplicada a uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="902d8-104">The **ConversationAction** element contains a single action to be applied to a single conversation.</span></span> 
  
[<span data-ttu-id="902d8-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="902d8-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="902d8-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="902d8-106">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="902d8-107">Conversation</span><span class="sxs-lookup"><span data-stu-id="902d8-107">ConversationAction</span></span>](conversationaction.md)
  
```XML
<ConversationAction>
   <Action/>
   <ConversationId/>
   <ContextFolderId/>
   <ConversationLastSyncTime/>
   <ProcessRightAway/>
   <DestinationFolderId/>
   <Categories/>
   <EnableAlwaysDelete/>
   <IsRead/>
   <DeleteType/>
</ConversationAction>
```

 <span data-ttu-id="902d8-108">**ConversationActionType**</span><span class="sxs-lookup"><span data-stu-id="902d8-108">**ConversationActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="902d8-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="902d8-109">Attributes and elements</span></span>

<span data-ttu-id="902d8-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="902d8-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="902d8-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="902d8-111">Attributes</span></span>

<span data-ttu-id="902d8-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="902d8-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="902d8-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="902d8-113">Child elements</span></span>

|<span data-ttu-id="902d8-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="902d8-114">**Element**</span></span>|<span data-ttu-id="902d8-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="902d8-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="902d8-116">Ação (ConversationActionTypeType)</span><span class="sxs-lookup"><span data-stu-id="902d8-116">Action (ConversationActionTypeType)</span></span>](action-conversationactiontypetype.md) <br/> |<span data-ttu-id="902d8-117">Contém a ação a ser executada na conversa especificada pelo elemento [Conversation](conversationid.md) .</span><span class="sxs-lookup"><span data-stu-id="902d8-117">Contains the action to perform on the conversation specified by the [ConversationId](conversationid.md) element.</span></span> <span data-ttu-id="902d8-118">Esse elemento deve estar presente.</span><span class="sxs-lookup"><span data-stu-id="902d8-118">This element must be present.</span></span>  <br/> |
|[<span data-ttu-id="902d8-119">ConversationId</span><span class="sxs-lookup"><span data-stu-id="902d8-119">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="902d8-120">Contém o identificador da conversa que terá a ação especificada pelo elemento [Action (ConversationActionTypeType)](action-conversationactiontypetype.md) aplicada a itens na conversa.</span><span class="sxs-lookup"><span data-stu-id="902d8-120">Contains the identifier of the conversation that will have the action specified by the [Action (ConversationActionTypeType)](action-conversationactiontypetype.md) element applied to items in the conversation.</span></span> <span data-ttu-id="902d8-121">Esse elemento deve estar presente.</span><span class="sxs-lookup"><span data-stu-id="902d8-121">This element must be present.</span></span>  <br/> |
|[<span data-ttu-id="902d8-122">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="902d8-122">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="902d8-123">Indica a pasta que é direcionada para ações que usam pastas.</span><span class="sxs-lookup"><span data-stu-id="902d8-123">Indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="902d8-124">Esse elemento deve estar presente ao copiar, excluir, mover e definir o estado de leitura em itens de conversa em uma pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="902d8-124">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span>  <br/> |
|[<span data-ttu-id="902d8-125">ConversationLastSyncTime</span><span class="sxs-lookup"><span data-stu-id="902d8-125">ConversationLastSyncTime</span></span>](conversationlastsynctime.md) <br/> |<span data-ttu-id="902d8-126">Contém a data e hora em que uma conversa foi sincronizada pela última vez.</span><span class="sxs-lookup"><span data-stu-id="902d8-126">Contains the date and time that a conversation was last synchronized.</span></span> <span data-ttu-id="902d8-127">Esse elemento deve estar presente ao tentar excluir todos os itens em uma conversa que foram recebidos até o momento especificado.</span><span class="sxs-lookup"><span data-stu-id="902d8-127">This element must be present when trying to delete all items in a conversation that were received up to the specified time.</span></span>  <br/> |
|[<span data-ttu-id="902d8-128">ProcessRightAway</span><span class="sxs-lookup"><span data-stu-id="902d8-128">ProcessRightAway</span></span>](processrightaway.md) <br/> |<span data-ttu-id="902d8-129">Indica se a resposta é enviada assim que a ação começa o processamento no servidor ou se a resposta é enviada após a conclusão da ação.</span><span class="sxs-lookup"><span data-stu-id="902d8-129">Indicates whether the response is sent as soon as the action starts processing on the server or whether the response is sent after the action has completed.</span></span> <span data-ttu-id="902d8-130">Esse elemento deve estar presente para que a resposta seja enviada de assíncrono para a ação solicitada.</span><span class="sxs-lookup"><span data-stu-id="902d8-130">This element must be present for the response to be sent asynchronous to the requested action.</span></span>  <br/> |
|[<span data-ttu-id="902d8-131">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="902d8-131">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="902d8-132">Indica a pasta de destino para ações de copiar e mover.</span><span class="sxs-lookup"><span data-stu-id="902d8-132">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="902d8-133">Categorias</span><span class="sxs-lookup"><span data-stu-id="902d8-133">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="902d8-134">Contém uma coleção de cadeias de caracteres que identificam as categorias às quais os itens em uma conversa pertencem.</span><span class="sxs-lookup"><span data-stu-id="902d8-134">Contains a collection of strings that identify the categories to which items in a conversation belong.</span></span>  <br/> |
|[<span data-ttu-id="902d8-135">EnableAlwaysDelete</span><span class="sxs-lookup"><span data-stu-id="902d8-135">EnableAlwaysDelete</span></span>](enablealwaysdelete.md) <br/> |<span data-ttu-id="902d8-136">Especifica um sinalizador que permite a exclusão de todos os novos itens em uma conversa.</span><span class="sxs-lookup"><span data-stu-id="902d8-136">Specifies a flag that enables deletion for all new items in a conversation.</span></span>  <br/> |
|[<span data-ttu-id="902d8-137">IsRead</span><span class="sxs-lookup"><span data-stu-id="902d8-137">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="902d8-138">Indica se uma mensagem foi lida.</span><span class="sxs-lookup"><span data-stu-id="902d8-138">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="902d8-139">DeleteType</span><span class="sxs-lookup"><span data-stu-id="902d8-139">DeleteType</span></span>](deletetype.md) <br/> |<span data-ttu-id="902d8-140">Indica como os itens em uma conversa são excluídos.</span><span class="sxs-lookup"><span data-stu-id="902d8-140">Indicates how items in a conversation are deleted.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="902d8-141">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="902d8-141">Parent elements</span></span>

|<span data-ttu-id="902d8-142">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="902d8-142">**Element**</span></span>|<span data-ttu-id="902d8-143">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="902d8-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="902d8-144">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="902d8-144">ConversationActions</span></span>](conversationactions.md) <br/> |<span data-ttu-id="902d8-145">Contém uma coleção de conversas e as ações a serem aplicadas a elas.</span><span class="sxs-lookup"><span data-stu-id="902d8-145">Contains a collection of conversations and the actions to apply to them.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="902d8-146">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="902d8-146">Text value</span></span>

<span data-ttu-id="902d8-147">**Valores de texto do elemento de conversaaction**</span><span class="sxs-lookup"><span data-stu-id="902d8-147">**ConversationAction element text values**</span></span>

|<span data-ttu-id="902d8-148">**Valor**</span><span class="sxs-lookup"><span data-stu-id="902d8-148">**Value**</span></span>|<span data-ttu-id="902d8-149">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="902d8-149">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="902d8-150">AlwaysCategorize</span><span class="sxs-lookup"><span data-stu-id="902d8-150">AlwaysCategorize</span></span>  <br/> |<span data-ttu-id="902d8-151">Sempre categorizar a conversa.</span><span class="sxs-lookup"><span data-stu-id="902d8-151">Always categorize the conversation.</span></span>  <br/> |
|<span data-ttu-id="902d8-152">AlwaysDelete</span><span class="sxs-lookup"><span data-stu-id="902d8-152">AlwaysDelete</span></span>  <br/> |<span data-ttu-id="902d8-153">Sempre excluir a conversa.</span><span class="sxs-lookup"><span data-stu-id="902d8-153">Always delete the conversation.</span></span>  <br/> |
|<span data-ttu-id="902d8-154">AlwaysMove</span><span class="sxs-lookup"><span data-stu-id="902d8-154">AlwaysMove</span></span>  <br/> |<span data-ttu-id="902d8-155">Sempre mover a conversa.</span><span class="sxs-lookup"><span data-stu-id="902d8-155">Always move the conversation.</span></span>  <br/> |
|<span data-ttu-id="902d8-156">Excluir</span><span class="sxs-lookup"><span data-stu-id="902d8-156">Delete</span></span>  <br/> |<span data-ttu-id="902d8-157">Exclua a conversa.</span><span class="sxs-lookup"><span data-stu-id="902d8-157">Delete the conversation.</span></span>  <br/> |
|<span data-ttu-id="902d8-158">Mover</span><span class="sxs-lookup"><span data-stu-id="902d8-158">Move</span></span>  <br/> |<span data-ttu-id="902d8-159">Mover a conversa.</span><span class="sxs-lookup"><span data-stu-id="902d8-159">Move the conversation.</span></span>  <br/> |
|<span data-ttu-id="902d8-160">Copiar</span><span class="sxs-lookup"><span data-stu-id="902d8-160">Copy</span></span>  <br/> |<span data-ttu-id="902d8-161">Copie a conversa.</span><span class="sxs-lookup"><span data-stu-id="902d8-161">Copy the conversation.</span></span>  <br/> |
|<span data-ttu-id="902d8-162">Setreadstate</span><span class="sxs-lookup"><span data-stu-id="902d8-162">SetReadState</span></span>  <br/> |<span data-ttu-id="902d8-163">Definir o estado de leitura da conversa.</span><span class="sxs-lookup"><span data-stu-id="902d8-163">Set the read state of the conversation.</span></span>  <br/> |
|<span data-ttu-id="902d8-164">SetRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="902d8-164">SetRetentionPolicy</span></span>  <br/> |<span data-ttu-id="902d8-165">Defina a política de retenção da conversa.</span><span class="sxs-lookup"><span data-stu-id="902d8-165">Set the retention policy for the conversation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="902d8-166">Comentários</span><span class="sxs-lookup"><span data-stu-id="902d8-166">Remarks</span></span>

<span data-ttu-id="902d8-167">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="902d8-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="902d8-168">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="902d8-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="902d8-169">Namespace</span><span class="sxs-lookup"><span data-stu-id="902d8-169">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="902d8-170">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="902d8-170">Schema Name</span></span>  <br/> |<span data-ttu-id="902d8-171">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="902d8-171">Types schema</span></span>  <br/> |
|<span data-ttu-id="902d8-172">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="902d8-172">Validation File</span></span>  <br/> |<span data-ttu-id="902d8-173">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="902d8-173">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="902d8-174">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="902d8-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="902d8-175">False</span><span class="sxs-lookup"><span data-stu-id="902d8-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="902d8-176">Confira também</span><span class="sxs-lookup"><span data-stu-id="902d8-176">See also</span></span>



[<span data-ttu-id="902d8-177">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="902d8-177">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="902d8-178">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="902d8-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

