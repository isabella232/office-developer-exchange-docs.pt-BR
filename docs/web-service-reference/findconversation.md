---
title: FindConversation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindConversation
api_type:
- schema
ms.assetid: 94b7083c-60cf-478b-a9af-a88f7acb30fb
description: O elemento de FindConversation define uma solicitação para localizar conversas em uma caixa de correio.
ms.openlocfilehash: 990e15f468f836d51977329c524acb439014da95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752265"
---
# <a name="findconversation"></a><span data-ttu-id="52c8e-103">FindConversation</span><span class="sxs-lookup"><span data-stu-id="52c8e-103">FindConversation</span></span>

<span data-ttu-id="52c8e-104">O elemento de **FindConversation** define uma solicitação para localizar conversas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="52c8e-104">The **FindConversation** element defines a request to find conversations in a mailbox.</span></span> 
  
[<span data-ttu-id="52c8e-105">FindConversation</span><span class="sxs-lookup"><span data-stu-id="52c8e-105">FindConversation</span></span>](findconversation.md)
  
```XML
<FindConversation Traversal="" ViewFilter="">
   <IndexedPageItemView/>
   <SeekToConditionPageItemView/>
   <SortOrder/>
   <ParentFolderId/>
   <MailboxScope/>
   <QueryString/>
   <ConversationShape/>
</FindConversation>
```

 <span data-ttu-id="52c8e-106">**FindConversationType**</span><span class="sxs-lookup"><span data-stu-id="52c8e-106">**FindConversationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="52c8e-107">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="52c8e-107">Attributes and elements</span></span>

<span data-ttu-id="52c8e-108">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="52c8e-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="52c8e-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="52c8e-109">Attributes</span></span>

****

|<span data-ttu-id="52c8e-110">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="52c8e-110">**Attribute**</span></span>|<span data-ttu-id="52c8e-111">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="52c8e-111">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="52c8e-112">Passagem</span><span class="sxs-lookup"><span data-stu-id="52c8e-112">Traversal</span></span>  <br/> |<span data-ttu-id="52c8e-113">Identifica os tipos de passagem subárvore.</span><span class="sxs-lookup"><span data-stu-id="52c8e-113">Identifies the types of sub-tree traversal.</span></span> <span data-ttu-id="52c8e-114">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="52c8e-114">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="52c8e-115">ViewFilter</span><span class="sxs-lookup"><span data-stu-id="52c8e-115">ViewFilter</span></span>  <br/> |<span data-ttu-id="52c8e-116">Identifica os filtros de exibição de tipos.</span><span class="sxs-lookup"><span data-stu-id="52c8e-116">Identifies the types view filters.</span></span> <span data-ttu-id="52c8e-117">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="52c8e-117">This attribute is optional.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="52c8e-118">Valores de atributos de passagem</span><span class="sxs-lookup"><span data-stu-id="52c8e-118">Traversal attribute values</span></span>

****

|<span data-ttu-id="52c8e-119">**Valor**</span><span class="sxs-lookup"><span data-stu-id="52c8e-119">**Value**</span></span>|<span data-ttu-id="52c8e-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="52c8e-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="52c8e-121">Raso</span><span class="sxs-lookup"><span data-stu-id="52c8e-121">Shallow</span></span>  <br/> |<span data-ttu-id="52c8e-122">Indica uma passagem superficial.</span><span class="sxs-lookup"><span data-stu-id="52c8e-122">Indicates a shallow traversal.</span></span>  <br/> |
|<span data-ttu-id="52c8e-123">Profundo</span><span class="sxs-lookup"><span data-stu-id="52c8e-123">Deep</span></span>  <br/> |<span data-ttu-id="52c8e-124">Indica um percurso profundo.</span><span class="sxs-lookup"><span data-stu-id="52c8e-124">Indicates a deep traversal.</span></span>  <br/> |
   
#### <a name="viewfilter-attribute-values"></a><span data-ttu-id="52c8e-125">Valores de atributo ViewFilter</span><span class="sxs-lookup"><span data-stu-id="52c8e-125">ViewFilter attribute values</span></span>

****

|<span data-ttu-id="52c8e-126">**Valor**</span><span class="sxs-lookup"><span data-stu-id="52c8e-126">**Value**</span></span>|<span data-ttu-id="52c8e-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="52c8e-127">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="52c8e-128">Todos</span><span class="sxs-lookup"><span data-stu-id="52c8e-128">All</span></span>  <br/> |<span data-ttu-id="52c8e-129">Encontre todas as conversas.</span><span class="sxs-lookup"><span data-stu-id="52c8e-129">Find all conversations.</span></span>  <br/> |
|<span data-ttu-id="52c8e-130">Sinalizado</span><span class="sxs-lookup"><span data-stu-id="52c8e-130">Flagged</span></span>  <br/> |<span data-ttu-id="52c8e-131">Localize conversas sinalizadas.</span><span class="sxs-lookup"><span data-stu-id="52c8e-131">Find flagged conversations.</span></span>  <br/> |
|<span data-ttu-id="52c8e-132">HasAttachment</span><span class="sxs-lookup"><span data-stu-id="52c8e-132">HasAttachment</span></span>  <br/> |<span data-ttu-id="52c8e-133">Localize conversas com anexos.</span><span class="sxs-lookup"><span data-stu-id="52c8e-133">Find conversations with attachments.</span></span>  <br/> |
|<span data-ttu-id="52c8e-134">ToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="52c8e-134">ToOrCcMe</span></span>  <br/> |<span data-ttu-id="52c8e-135">Localize conversas endereçada ou cc seria para mim.</span><span class="sxs-lookup"><span data-stu-id="52c8e-135">Find conversations addressed or cc'd to me.</span></span>  <br/> |
|<span data-ttu-id="52c8e-136">Não lidas</span><span class="sxs-lookup"><span data-stu-id="52c8e-136">Unread</span></span>  <br/> |<span data-ttu-id="52c8e-137">Localize conversas não lidas.</span><span class="sxs-lookup"><span data-stu-id="52c8e-137">Find unread conversations.</span></span>  <br/> |
|<span data-ttu-id="52c8e-138">TaskActive</span><span class="sxs-lookup"><span data-stu-id="52c8e-138">TaskActive</span></span>  <br/> |<span data-ttu-id="52c8e-139">Encontre as tarefas ativas.</span><span class="sxs-lookup"><span data-stu-id="52c8e-139">Find active tasks.</span></span>  <br/> |
|<span data-ttu-id="52c8e-140">TaskOverdue</span><span class="sxs-lookup"><span data-stu-id="52c8e-140">TaskOverdue</span></span>  <br/> |<span data-ttu-id="52c8e-141">Encontre tarefas atrasadas.</span><span class="sxs-lookup"><span data-stu-id="52c8e-141">Find overdue tasks.</span></span>  <br/> |
|<span data-ttu-id="52c8e-142">TaskCompleted</span><span class="sxs-lookup"><span data-stu-id="52c8e-142">TaskCompleted</span></span>  <br/> |<span data-ttu-id="52c8e-143">Encontre tarefas concluídas.</span><span class="sxs-lookup"><span data-stu-id="52c8e-143">Find completed tasks.</span></span>  <br/> |
|<span data-ttu-id="52c8e-144">NoClutter</span><span class="sxs-lookup"><span data-stu-id="52c8e-144">NoClutter</span></span>  <br/> |<span data-ttu-id="52c8e-145">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="52c8e-145">For internal use only.</span></span>  <br/> |
|<span data-ttu-id="52c8e-146">Desorganização</span><span class="sxs-lookup"><span data-stu-id="52c8e-146">Clutter</span></span>  <br/> |<span data-ttu-id="52c8e-147">Apenas para uso interno.</span><span class="sxs-lookup"><span data-stu-id="52c8e-147">For internal use only.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="52c8e-148">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="52c8e-148">Child elements</span></span>

|<span data-ttu-id="52c8e-149">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="52c8e-149">**Element**</span></span>|<span data-ttu-id="52c8e-150">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="52c8e-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="52c8e-151">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="52c8e-151">IndexedPageItemView</span></span>](indexedpageitemview.md) <br/> |<span data-ttu-id="52c8e-152">Descreve como paginada conversa a informação é retornada.</span><span class="sxs-lookup"><span data-stu-id="52c8e-152">Describes how paged conversation information is returned.</span></span>  <br/> |
|[<span data-ttu-id="52c8e-153">SeekToConditionPageItemView</span><span class="sxs-lookup"><span data-stu-id="52c8e-153">SeekToConditionPageItemView</span></span>](seektoconditionpageitemview.md) <br/> |<span data-ttu-id="52c8e-154">Especifica a condição que é usada para identificar o final de uma pesquisa, o índice inicial de uma pesquisa, as entradas máxima para retornar e as instruções de pesquisa para uma pesquisa **FindItem** ou **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="52c8e-154">Specifies the condition that is used to identify the end of a search, the starting index of a search, the maximum entries to return, and the search directions for a **FindItem** or **FindConversation** search.</span></span>  <br/> |
|[<span data-ttu-id="52c8e-155">SortOrder</span><span class="sxs-lookup"><span data-stu-id="52c8e-155">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="52c8e-156">Define como os itens são classificados em uma solicitação de [operação FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="52c8e-156">Defines how items are sorted in a [FindConversation operation](findconversation-operation.md) request.</span></span> <span data-ttu-id="52c8e-157">A propriedade de **Conversa: LastDeliveryTime** é a única propriedade que tem suporte para a classificação quando a operação **FindConversation** é usada.</span><span class="sxs-lookup"><span data-stu-id="52c8e-157">The **conversation:LastDeliveryTime** property is the only property that is supported for sorting when the **FindConversation** operation is used.</span></span>  <br/> |
|[<span data-ttu-id="52c8e-158">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="52c8e-158">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="52c8e-159">Identifica a pasta para procurar conversas.</span><span class="sxs-lookup"><span data-stu-id="52c8e-159">Identifies the folder to search for conversations.</span></span>  <br/> |
|[<span data-ttu-id="52c8e-160">MailboxScope</span><span class="sxs-lookup"><span data-stu-id="52c8e-160">MailboxScope</span></span>](mailboxscope.md) <br/> |<span data-ttu-id="52c8e-161">Especifica se uma pesquisa ou fetch para uma conversa deve abranger a caixa de correio primária, caixa de correio de arquivo morto ou ambos os primário e arquivar caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="52c8e-161">Specifies whether a search or fetch for a conversation should span either the primary mailbox, archive mailbox, or both the primary and archive mailbox.</span></span>  <br/> |
|[<span data-ttu-id="52c8e-162">QueryString (QueryStringType)</span><span class="sxs-lookup"><span data-stu-id="52c8e-162">QueryString (QueryStringType)</span></span>](querystring-querystringtype.md) <br/> |<span data-ttu-id="52c8e-163">Especifica uma cadeia de caracteres de consulta de caixa de correio com base na sintaxe de consulta avançada (AQS).</span><span class="sxs-lookup"><span data-stu-id="52c8e-163">Specifies a mailbox query string based on Advanced Query Syntax (AQS).</span></span>  <br/> |
|[<span data-ttu-id="52c8e-164">ConversationShape</span><span class="sxs-lookup"><span data-stu-id="52c8e-164">ConversationShape</span></span>](conversationshape.md) <br/> |<span data-ttu-id="52c8e-165">Identifica a propriedade definida para retornar em uma resposta de [operação FindConversation](findconversation-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="52c8e-165">Identifies the property set to return in a [FindConversation operation](findconversation-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="52c8e-166">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="52c8e-166">Parent elements</span></span>

<span data-ttu-id="52c8e-167">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="52c8e-167">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="52c8e-168">Comentários</span><span class="sxs-lookup"><span data-stu-id="52c8e-168">Remarks</span></span>

<span data-ttu-id="52c8e-169">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="52c8e-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="52c8e-170">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="52c8e-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="52c8e-171">Namespace</span><span class="sxs-lookup"><span data-stu-id="52c8e-171">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="52c8e-172">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="52c8e-172">Schema Name</span></span>  <br/> |<span data-ttu-id="52c8e-173">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="52c8e-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="52c8e-174">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="52c8e-174">Validation File</span></span>  <br/> |<span data-ttu-id="52c8e-175">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="52c8e-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="52c8e-176">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="52c8e-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="52c8e-177">False</span><span class="sxs-lookup"><span data-stu-id="52c8e-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="52c8e-178">Ver também</span><span class="sxs-lookup"><span data-stu-id="52c8e-178">See also</span></span>



[<span data-ttu-id="52c8e-179">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="52c8e-179">FindConversation operation</span></span>](findconversation-operation.md)


- [<span data-ttu-id="52c8e-180">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="52c8e-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="52c8e-181">Conversas no EWS</span><span class="sxs-lookup"><span data-stu-id="52c8e-181">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

