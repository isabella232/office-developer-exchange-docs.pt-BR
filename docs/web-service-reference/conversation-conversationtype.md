---
title: Conversa (ConversationType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Conversation
api_type:
- schema
ms.assetid: 59d014cd-5886-49ea-8d36-ba5de7e675de
description: O elemento Conversation representa uma única conversa.
ms.openlocfilehash: e1ae055d6a77fc5a9b483341830b978e0c1a5b5a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751522"
---
# <a name="conversation-conversationtype"></a><span data-ttu-id="05113-103">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="05113-103">Conversation (ConversationType)</span></span>

<span data-ttu-id="05113-104">O elemento **Conversation** representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="05113-104">The **Conversation** element represents a single conversation.</span></span> 
  
[<span data-ttu-id="05113-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="05113-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="05113-106">Conversas</span><span class="sxs-lookup"><span data-stu-id="05113-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="05113-107">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="05113-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
```XML
<Conversation>
   <ConversationId/>
   <ConversationTopic/>
   <UniqueRecipients/>
   <GlobalUniqueRecipients/>
   <UniqueUnreadSenders/>
   <GlobalUniqueUnreadSenders/>
   <UniqueSenders/>
   <GlobalUniqueSenders/>
   <LastDeliveryTime/>
   <GlobalLastDeliveryTime/>
   <Categories/>
   <GlobalCategories/>
   <FlagStatus/>
   <GlobalFlagStatus/>
   <HasAttachments/>
   <GlobalHasAttachments/>
   <MessageCount/>
   <GlobalMessageCount/>
   <UnreadCount/>
   <GlobalUnreadCount/>
   <Size/>   <GlobalSize/>
   <ItemClasses/>
   <GlobalItemClasses/>
   <Importance/>
   <GlobalImportance/>
   <ItemIds/>
   <GlobalItemIds/>
</Conversation>
```

 <span data-ttu-id="05113-108">**ConversationType**</span><span class="sxs-lookup"><span data-stu-id="05113-108">**ConversationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="05113-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="05113-109">Attributes and elements</span></span>

<span data-ttu-id="05113-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="05113-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05113-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="05113-111">Attributes</span></span>

<span data-ttu-id="05113-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="05113-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05113-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="05113-113">Child elements</span></span>

|<span data-ttu-id="05113-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="05113-114">**Element**</span></span>|<span data-ttu-id="05113-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="05113-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05113-116">ConversationId</span><span class="sxs-lookup"><span data-stu-id="05113-116">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="05113-117">Representa o identificador de uma conversa.</span><span class="sxs-lookup"><span data-stu-id="05113-117">Represents the identifier of a conversation.</span></span>  <br/> |
|[<span data-ttu-id="05113-118">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="05113-118">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="05113-119">Representa o tópico de conversação.</span><span class="sxs-lookup"><span data-stu-id="05113-119">Represents the conversation topic.</span></span> <span data-ttu-id="05113-120">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05113-120">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="05113-121">UniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="05113-121">UniqueRecipients</span></span>](uniquerecipients.md) <br/> |<span data-ttu-id="05113-122">Contém a lista de destinatários de uma conversa agregada de uma determinada pasta.</span><span class="sxs-lookup"><span data-stu-id="05113-122">Contains the recipient list of a conversation aggregated from a particular folder.</span></span> <span data-ttu-id="05113-123">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05113-123">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="05113-124">GlobalUniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="05113-124">GlobalUniqueRecipients</span></span>](globaluniquerecipients.md) <br/> |<span data-ttu-id="05113-125">Contém a lista de destinatários de uma conversa agregada em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="05113-125">Contains the recipient list of a conversation aggregated across a mailbox.</span></span> <span data-ttu-id="05113-126">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05113-126">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="05113-127">UniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="05113-127">UniqueUnreadSenders</span></span>](uniqueunreadsenders.md) <br/> |<span data-ttu-id="05113-128">Contém uma lista de todas as pessoas que tenham enviado mensagens que estão atualmente não lidas nesta conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="05113-128">Contains a list of all the people who have sent messages that are currently unread in this conversation in the current folder.</span></span> <span data-ttu-id="05113-129">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05113-129">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="05113-130">GlobalUniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="05113-130">GlobalUniqueUnreadSenders</span></span>](globaluniqueunreadsenders.md) <br/> |<span data-ttu-id="05113-131">Contém uma lista de todas as pessoas que tenham enviado mensagens que estão atualmente não lidas nesta conversa entre todas as pastas na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="05113-131">Contains a list of all the people who have sent messages that are currently unread in this conversation across all folders in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="05113-132">UniqueSenders</span><span class="sxs-lookup"><span data-stu-id="05113-132">UniqueSenders</span></span>](uniquesenders.md) <br/> |<span data-ttu-id="05113-133">Contém uma lista de todos os remetentes dos itens de conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="05113-133">Contains a list of all the senders of conversation items in the current folder.</span></span> <span data-ttu-id="05113-134">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="05113-134">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="05113-135">GlobalUniqueSenders</span><span class="sxs-lookup"><span data-stu-id="05113-135">GlobalUniqueSenders</span></span>](globaluniquesenders.md) <br/> |<span data-ttu-id="05113-136">Contém uma lista de todos os remetentes dos itens de conversa na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="05113-136">Contains a list of all the senders of conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="05113-137">LastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="05113-137">LastDeliveryTime</span></span>](lastdeliverytime.md) <br/> |<span data-ttu-id="05113-138">Contém o tempo de entrega da mensagem foi recebida pela última nesta conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="05113-138">Contains the delivery time of the message that was last received in this conversation in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="05113-139">GlobalLastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="05113-139">GlobalLastDeliveryTime</span></span>](globallastdeliverytime.md) <br/> |<span data-ttu-id="05113-140">Contém o tempo de entrega da mensagem foi recebida pela última nesta conversa entre todas as pastas na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="05113-140">Contains the delivery time of the message that was last received in this conversation across all folders in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="05113-141">Categorias</span><span class="sxs-lookup"><span data-stu-id="05113-141">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="05113-142">Contém uma coleção de cadeias de caracteres que identificam as categorias que são aplicadas a todos os itens de conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="05113-142">Contains a collection of strings that identify the categories that are applied to all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="05113-143">GlobalCategories</span><span class="sxs-lookup"><span data-stu-id="05113-143">GlobalCategories</span></span>](globalcategories.md) <br/> |<span data-ttu-id="05113-144">Contém a lista de categorias para todos os itens de conversa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="05113-144">Contains the category list for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="05113-145">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="05113-145">FlagStatus</span></span>](flagstatus.md) <br/> |<span data-ttu-id="05113-146">Contém o status do sinalizador agregados para itens de conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="05113-146">Contains the aggregated flag status for conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="05113-147">GlobalFlagStatus</span><span class="sxs-lookup"><span data-stu-id="05113-147">GlobalFlagStatus</span></span>](globalflagstatus.md) <br/> |<span data-ttu-id="05113-148">Contém o status do sinalizador agregados de todos os itens de conversa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="05113-148">Contains the aggregated flag status for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="05113-149">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="05113-149">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="05113-150">Contém um valor que indica se o item de pelo menos uma conversa na pasta atual tiver um anexo.</span><span class="sxs-lookup"><span data-stu-id="05113-150">Contains a value that indicates whether at least one conversation item in the current folder has an attachment.</span></span>  <br/> |
|[<span data-ttu-id="05113-151">GlobalHasAttachments</span><span class="sxs-lookup"><span data-stu-id="05113-151">GlobalHasAttachments</span></span>](globalhasattachments.md) <br/> |<span data-ttu-id="05113-152">Contém um valor que indica se o item de pelo menos uma conversa em uma caixa de correio tem um anexo.</span><span class="sxs-lookup"><span data-stu-id="05113-152">Contains a value that indicates whether at least one conversation item in a mailbox has an attachment.</span></span>  <br/> |
|[<span data-ttu-id="05113-153">MessageCount</span><span class="sxs-lookup"><span data-stu-id="05113-153">MessageCount</span></span>](messagecount.md) <br/> |<span data-ttu-id="05113-154">Contém o número total de itens de conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="05113-154">Contains the total number of conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="05113-155">GlobalMessageCount</span><span class="sxs-lookup"><span data-stu-id="05113-155">GlobalMessageCount</span></span>](globalmessagecount.md) <br/> |<span data-ttu-id="05113-156">Contém o número total de itens de conversa, na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="05113-156">Contains the total number of conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="05113-157">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="05113-157">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="05113-158">Contém a contagem de itens não lidos conversa dentro de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="05113-158">Contains the count of unread conversation items within a folder.</span></span>  <br/> |
|[<span data-ttu-id="05113-159">GlobalUnreadCount</span><span class="sxs-lookup"><span data-stu-id="05113-159">GlobalUnreadCount</span></span>](globalunreadcount.md) <br/> |<span data-ttu-id="05113-160">Contém uma contagem de todos os itens de conversa não lidas na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="05113-160">Contains a count of all the unread conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="05113-161">Size</span><span class="sxs-lookup"><span data-stu-id="05113-161">Size</span></span>](size.md) <br/> |<span data-ttu-id="05113-162">Contém o tamanho de conversa calculado a partir do tamanho de todos os itens de conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="05113-162">Contains the conversation size calculated from the size of all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="05113-163">GlobalSize</span><span class="sxs-lookup"><span data-stu-id="05113-163">GlobalSize</span></span>](globalsize.md) <br/> |<span data-ttu-id="05113-164">Contém o tamanho da conversa calculado a partir do tamanho de todos os itens de conversa, na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="05113-164">Contains the size of the conversation calculated from the size of all conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="05113-165">ItemClasses (ArrayOfItemClassType)</span><span class="sxs-lookup"><span data-stu-id="05113-165">ItemClasses (ArrayOfItemClassType)</span></span>](itemclasses-arrayofitemclasstype.md) <br/> |<span data-ttu-id="05113-166">Contém uma lista das classes de item que representa todas as classes de item, os itens de conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="05113-166">Contains a list of item classes that represents all the item classes of the conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="05113-167">GlobalItemClasses</span><span class="sxs-lookup"><span data-stu-id="05113-167">GlobalItemClasses</span></span>](globalitemclasses.md) <br/> |<span data-ttu-id="05113-168">Contém uma lista das classes de item que representa todas as classes de item, os itens de conversa de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="05113-168">Contains a list of item classes that represents all the item classes of the conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="05113-169">Importância</span><span class="sxs-lookup"><span data-stu-id="05113-169">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="05113-170">Contém a importância agregada de todos os itens de conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="05113-170">Contains the aggregated importance for all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="05113-171">GlobalImportance</span><span class="sxs-lookup"><span data-stu-id="05113-171">GlobalImportance</span></span>](globalimportance.md) <br/> |<span data-ttu-id="05113-172">Contém a importância agregada de todos os itens de conversa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="05113-172">Contains the aggregated importance for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="05113-173">ItemIds</span><span class="sxs-lookup"><span data-stu-id="05113-173">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="05113-174">Contém o conjunto de identificadores de item para todos os itens de conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="05113-174">Contains the collection of item identifiers for all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="05113-175">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="05113-175">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="05113-176">Contém o conjunto de identificadores de item para todos os itens de conversa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="05113-176">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="05113-177">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="05113-177">Parent elements</span></span>

|<span data-ttu-id="05113-178">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="05113-178">**Element**</span></span>|<span data-ttu-id="05113-179">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="05113-179">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05113-180">Conversas</span><span class="sxs-lookup"><span data-stu-id="05113-180">Conversations</span></span>](conversations-ex15websvcsotherref.md) <br/> |<span data-ttu-id="05113-181">Contém uma matriz de conversas que são retornados na resposta **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="05113-181">Contains an array of conversations that are returned in the **FindConversation** response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="05113-182">Text value</span><span class="sxs-lookup"><span data-stu-id="05113-182">Text value</span></span>

<span data-ttu-id="05113-183">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="05113-183">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="05113-184">Comentários</span><span class="sxs-lookup"><span data-stu-id="05113-184">Remarks</span></span>

<span data-ttu-id="05113-185">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="05113-185">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05113-186">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="05113-186">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05113-187">Namespace</span><span class="sxs-lookup"><span data-stu-id="05113-187">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="05113-188">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="05113-188">Schema name</span></span>  <br/> |<span data-ttu-id="05113-189">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="05113-189">Types schema</span></span>  <br/> |
|<span data-ttu-id="05113-190">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="05113-190">Validation file</span></span>  <br/> |<span data-ttu-id="05113-191">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="05113-191">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="05113-192">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="05113-192">Can be empty</span></span>  <br/> |<span data-ttu-id="05113-193">False</span><span class="sxs-lookup"><span data-stu-id="05113-193">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="05113-194">Ver também</span><span class="sxs-lookup"><span data-stu-id="05113-194">See also</span></span>



[<span data-ttu-id="05113-195">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="05113-195">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="05113-196">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="05113-196">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="05113-197">Conversas no EWS</span><span class="sxs-lookup"><span data-stu-id="05113-197">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

