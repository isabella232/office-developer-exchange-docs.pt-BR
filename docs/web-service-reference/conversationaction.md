---
title: ConversationAction
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
description: O elemento ConversationAction contém uma única ação a ser aplicado a uma única conversa.
ms.openlocfilehash: 45cd6df3aba94062bd5aa0ddf9367e8cf118dc6b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751521"
---
# <a name="conversationaction"></a><span data-ttu-id="9be20-103">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="9be20-103">ConversationAction</span></span>

<span data-ttu-id="9be20-104">O elemento **ConversationAction** contém uma única ação a ser aplicado a uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="9be20-104">The **ConversationAction** element contains a single action to be applied to a single conversation.</span></span> 
  
[<span data-ttu-id="9be20-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="9be20-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="9be20-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="9be20-106">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="9be20-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="9be20-107">ConversationAction</span></span>](conversationaction.md)
  
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

 <span data-ttu-id="9be20-108">**ConversationActionType**</span><span class="sxs-lookup"><span data-stu-id="9be20-108">**ConversationActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9be20-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9be20-109">Attributes and elements</span></span>

<span data-ttu-id="9be20-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9be20-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9be20-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="9be20-111">Attributes</span></span>

<span data-ttu-id="9be20-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9be20-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9be20-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9be20-113">Child elements</span></span>

|<span data-ttu-id="9be20-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9be20-114">**Element**</span></span>|<span data-ttu-id="9be20-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9be20-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9be20-116">Ação (ConversationActionTypeType)</span><span class="sxs-lookup"><span data-stu-id="9be20-116">Action (ConversationActionTypeType)</span></span>](action-conversationactiontypetype.md) <br/> |<span data-ttu-id="9be20-117">Contém a ação a ser executada a conversa especificada pelo elemento [ConversationId](conversationid.md) .</span><span class="sxs-lookup"><span data-stu-id="9be20-117">Contains the action to perform on the conversation specified by the [ConversationId](conversationid.md) element.</span></span> <span data-ttu-id="9be20-118">Este elemento deve estar presente.</span><span class="sxs-lookup"><span data-stu-id="9be20-118">This element must be present.</span></span>  <br/> |
|[<span data-ttu-id="9be20-119">ConversationId</span><span class="sxs-lookup"><span data-stu-id="9be20-119">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="9be20-120">Contém o identificador da conversa que terá a ação especificada pelo elemento [Action (ConversationActionTypeType)](action-conversationactiontypetype.md) aplicado aos itens da conversa.</span><span class="sxs-lookup"><span data-stu-id="9be20-120">Contains the identifier of the conversation that will have the action specified by the [Action (ConversationActionTypeType)](action-conversationactiontypetype.md) element applied to items in the conversation.</span></span> <span data-ttu-id="9be20-121">Este elemento deve estar presente.</span><span class="sxs-lookup"><span data-stu-id="9be20-121">This element must be present.</span></span>  <br/> |
|[<span data-ttu-id="9be20-122">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="9be20-122">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="9be20-123">Indica a pasta que está programada para ações que usam pastas.</span><span class="sxs-lookup"><span data-stu-id="9be20-123">Indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="9be20-124">Este elemento deve estar presente quando copiar, excluir, mover e definindo o estado lido em itens da conversa em uma pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="9be20-124">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span>  <br/> |
|[<span data-ttu-id="9be20-125">ConversationLastSyncTime</span><span class="sxs-lookup"><span data-stu-id="9be20-125">ConversationLastSyncTime</span></span>](conversationlastsynctime.md) <br/> |<span data-ttu-id="9be20-126">Contém a data e hora da última sincronização uma conversa.</span><span class="sxs-lookup"><span data-stu-id="9be20-126">Contains the date and time that a conversation was last synchronized.</span></span> <span data-ttu-id="9be20-127">Este elemento deve estar presente durante a tentativa de excluir todos os itens em uma conversa que foram recebidos do período especificado.</span><span class="sxs-lookup"><span data-stu-id="9be20-127">This element must be present when trying to delete all items in a conversation that were received up to the specified time.</span></span>  <br/> |
|[<span data-ttu-id="9be20-128">ProcessRightAway</span><span class="sxs-lookup"><span data-stu-id="9be20-128">ProcessRightAway</span></span>](processrightaway.md) <br/> |<span data-ttu-id="9be20-129">Indica se a resposta é enviada assim que a ação inicia o processamento no servidor ou se a resposta é enviada depois que a ação foi concluída.</span><span class="sxs-lookup"><span data-stu-id="9be20-129">Indicates whether the response is sent as soon as the action starts processing on the server or whether the response is sent after the action has completed.</span></span> <span data-ttu-id="9be20-130">Este elemento deve estar presente para a resposta a ser enviado assíncrona para a ação solicitada.</span><span class="sxs-lookup"><span data-stu-id="9be20-130">This element must be present for the response to be sent asynchronous to the requested action.</span></span>  <br/> |
|[<span data-ttu-id="9be20-131">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="9be20-131">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="9be20-132">Indica a pasta de destino para cópia e mover ações.</span><span class="sxs-lookup"><span data-stu-id="9be20-132">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="9be20-133">Categorias</span><span class="sxs-lookup"><span data-stu-id="9be20-133">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9be20-134">Contém uma coleção de cadeias de caracteres que identificam as categorias às quais os itens em uma conversa pertencem.</span><span class="sxs-lookup"><span data-stu-id="9be20-134">Contains a collection of strings that identify the categories to which items in a conversation belong.</span></span>  <br/> |
|[<span data-ttu-id="9be20-135">EnableAlwaysDelete</span><span class="sxs-lookup"><span data-stu-id="9be20-135">EnableAlwaysDelete</span></span>](enablealwaysdelete.md) <br/> |<span data-ttu-id="9be20-136">Especifica um sinalizador que permite a exclusão de todos os novos itens em uma conversa.</span><span class="sxs-lookup"><span data-stu-id="9be20-136">Specifies a flag that enables deletion for all new items in a conversation.</span></span>  <br/> |
|[<span data-ttu-id="9be20-137">Foi lido</span><span class="sxs-lookup"><span data-stu-id="9be20-137">IsRead</span></span>](isread.md) <br/> |<span data-ttu-id="9be20-138">Indica se uma mensagem foi lido.</span><span class="sxs-lookup"><span data-stu-id="9be20-138">Indicates whether a message has been read.</span></span>  <br/> |
|[<span data-ttu-id="9be20-139">DeleteType</span><span class="sxs-lookup"><span data-stu-id="9be20-139">DeleteType</span></span>](deletetype.md) <br/> |<span data-ttu-id="9be20-140">Indica como os itens em uma conversa são excluídos.</span><span class="sxs-lookup"><span data-stu-id="9be20-140">Indicates how items in a conversation are deleted.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9be20-141">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9be20-141">Parent elements</span></span>

|<span data-ttu-id="9be20-142">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9be20-142">**Element**</span></span>|<span data-ttu-id="9be20-143">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9be20-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9be20-144">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="9be20-144">ConversationActions</span></span>](conversationactions.md) <br/> |<span data-ttu-id="9be20-145">Contém uma coleção de conversas e as ações a serem aplicadas a eles.</span><span class="sxs-lookup"><span data-stu-id="9be20-145">Contains a collection of conversations and the actions to apply to them.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9be20-146">Text value</span><span class="sxs-lookup"><span data-stu-id="9be20-146">Text value</span></span>

<span data-ttu-id="9be20-147">**Valores de texto do elemento ConversationAction**</span><span class="sxs-lookup"><span data-stu-id="9be20-147">**ConversationAction element text values**</span></span>

|<span data-ttu-id="9be20-148">**Valor**</span><span class="sxs-lookup"><span data-stu-id="9be20-148">**Value**</span></span>|<span data-ttu-id="9be20-149">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9be20-149">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9be20-150">AlwaysCategorize</span><span class="sxs-lookup"><span data-stu-id="9be20-150">AlwaysCategorize</span></span>  <br/> |<span data-ttu-id="9be20-151">Sempre categorize a conversa.</span><span class="sxs-lookup"><span data-stu-id="9be20-151">Always categorize the conversation.</span></span>  <br/> |
|<span data-ttu-id="9be20-152">AlwaysDelete</span><span class="sxs-lookup"><span data-stu-id="9be20-152">AlwaysDelete</span></span>  <br/> |<span data-ttu-id="9be20-153">Exclua sempre a conversa.</span><span class="sxs-lookup"><span data-stu-id="9be20-153">Always delete the conversation.</span></span>  <br/> |
|<span data-ttu-id="9be20-154">AlwaysMove</span><span class="sxs-lookup"><span data-stu-id="9be20-154">AlwaysMove</span></span>  <br/> |<span data-ttu-id="9be20-155">Sempre mover a conversa.</span><span class="sxs-lookup"><span data-stu-id="9be20-155">Always move the conversation.</span></span>  <br/> |
|<span data-ttu-id="9be20-156">Excluir</span><span class="sxs-lookup"><span data-stu-id="9be20-156">Delete</span></span>  <br/> |<span data-ttu-id="9be20-157">Exclua a conversa.</span><span class="sxs-lookup"><span data-stu-id="9be20-157">Delete the conversation.</span></span>  <br/> |
|<span data-ttu-id="9be20-158">Mover</span><span class="sxs-lookup"><span data-stu-id="9be20-158">Move</span></span>  <br/> |<span data-ttu-id="9be20-159">Mova a conversa.</span><span class="sxs-lookup"><span data-stu-id="9be20-159">Move the conversation.</span></span>  <br/> |
|<span data-ttu-id="9be20-160">Cópia</span><span class="sxs-lookup"><span data-stu-id="9be20-160">Copy</span></span>  <br/> |<span data-ttu-id="9be20-161">Copie a conversa.</span><span class="sxs-lookup"><span data-stu-id="9be20-161">Copy the conversation.</span></span>  <br/> |
|<span data-ttu-id="9be20-162">SetReadState</span><span class="sxs-lookup"><span data-stu-id="9be20-162">SetReadState</span></span>  <br/> |<span data-ttu-id="9be20-163">Defina o estado de leitura da conversa.</span><span class="sxs-lookup"><span data-stu-id="9be20-163">Set the read state of the conversation.</span></span>  <br/> |
|<span data-ttu-id="9be20-164">SetRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="9be20-164">SetRetentionPolicy</span></span>  <br/> |<span data-ttu-id="9be20-165">Defina a política de retenção para a conversa.</span><span class="sxs-lookup"><span data-stu-id="9be20-165">Set the retention policy for the conversation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9be20-166">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="9be20-166">Remarks</span></span>

<span data-ttu-id="9be20-167">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="9be20-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9be20-168">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9be20-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9be20-169">Namespace</span><span class="sxs-lookup"><span data-stu-id="9be20-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9be20-170">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9be20-170">Schema Name</span></span>  <br/> |<span data-ttu-id="9be20-171">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9be20-171">Types schema</span></span>  <br/> |
|<span data-ttu-id="9be20-172">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9be20-172">Validation File</span></span>  <br/> |<span data-ttu-id="9be20-173">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9be20-173">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9be20-174">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9be20-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="9be20-175">False</span><span class="sxs-lookup"><span data-stu-id="9be20-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9be20-176">Ver também</span><span class="sxs-lookup"><span data-stu-id="9be20-176">See also</span></span>



[<span data-ttu-id="9be20-177">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="9be20-177">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="9be20-178">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9be20-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

