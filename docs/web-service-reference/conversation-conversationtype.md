---
title: Conversa (Conversatype)
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
ms.openlocfilehash: 9969a6cfe1f977b1c24e03771f231f4eb03d1ac6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458933"
---
# <a name="conversation-conversationtype"></a><span data-ttu-id="83372-103">Conversa (Conversatype)</span><span class="sxs-lookup"><span data-stu-id="83372-103">Conversation (ConversationType)</span></span>

<span data-ttu-id="83372-104">O elemento **Conversation** representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="83372-104">The **Conversation** element represents a single conversation.</span></span> 
  
[<span data-ttu-id="83372-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="83372-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="83372-106">Conversas</span><span class="sxs-lookup"><span data-stu-id="83372-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="83372-107">Conversa (Conversatype)</span><span class="sxs-lookup"><span data-stu-id="83372-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
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

 <span data-ttu-id="83372-108">**Conversation**</span><span class="sxs-lookup"><span data-stu-id="83372-108">**ConversationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="83372-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="83372-109">Attributes and elements</span></span>

<span data-ttu-id="83372-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="83372-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="83372-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="83372-111">Attributes</span></span>

<span data-ttu-id="83372-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="83372-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="83372-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="83372-113">Child elements</span></span>

|<span data-ttu-id="83372-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="83372-114">**Element**</span></span>|<span data-ttu-id="83372-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="83372-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="83372-116">ConversationId</span><span class="sxs-lookup"><span data-stu-id="83372-116">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="83372-117">Representa o identificador de uma conversa.</span><span class="sxs-lookup"><span data-stu-id="83372-117">Represents the identifier of a conversation.</span></span>  <br/> |
|[<span data-ttu-id="83372-118">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="83372-118">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="83372-119">Representa o tópico da conversa.</span><span class="sxs-lookup"><span data-stu-id="83372-119">Represents the conversation topic.</span></span> <span data-ttu-id="83372-120">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="83372-120">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="83372-121">UniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="83372-121">UniqueRecipients</span></span>](uniquerecipients.md) <br/> |<span data-ttu-id="83372-122">Contém a lista de destinatários de uma conversa agregada a partir de uma pasta específica.</span><span class="sxs-lookup"><span data-stu-id="83372-122">Contains the recipient list of a conversation aggregated from a particular folder.</span></span> <span data-ttu-id="83372-123">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="83372-123">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="83372-124">GlobalUniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="83372-124">GlobalUniqueRecipients</span></span>](globaluniquerecipients.md) <br/> |<span data-ttu-id="83372-125">Contém a lista de destinatários de uma conversa agregada em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="83372-125">Contains the recipient list of a conversation aggregated across a mailbox.</span></span> <span data-ttu-id="83372-126">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="83372-126">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="83372-127">UniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="83372-127">UniqueUnreadSenders</span></span>](uniqueunreadsenders.md) <br/> |<span data-ttu-id="83372-128">Contém uma lista de todas as pessoas que enviaram mensagens não lidas atualmente nesta conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="83372-128">Contains a list of all the people who have sent messages that are currently unread in this conversation in the current folder.</span></span> <span data-ttu-id="83372-129">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="83372-129">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="83372-130">GlobalUniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="83372-130">GlobalUniqueUnreadSenders</span></span>](globaluniqueunreadsenders.md) <br/> |<span data-ttu-id="83372-131">Contém uma lista de todas as pessoas que enviaram mensagens não lidas atualmente nesta conversa em todas as pastas da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="83372-131">Contains a list of all the people who have sent messages that are currently unread in this conversation across all folders in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="83372-132">UniqueSenders</span><span class="sxs-lookup"><span data-stu-id="83372-132">UniqueSenders</span></span>](uniquesenders.md) <br/> |<span data-ttu-id="83372-133">Contém uma lista de todos os remetentes dos itens de conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="83372-133">Contains a list of all the senders of conversation items in the current folder.</span></span> <span data-ttu-id="83372-134">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="83372-134">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="83372-135">GlobalUniqueSenders</span><span class="sxs-lookup"><span data-stu-id="83372-135">GlobalUniqueSenders</span></span>](globaluniquesenders.md) <br/> |<span data-ttu-id="83372-136">Contém uma lista de todos os remetentes de itens de conversa na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="83372-136">Contains a list of all the senders of conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="83372-137">LastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="83372-137">LastDeliveryTime</span></span>](lastdeliverytime.md) <br/> |<span data-ttu-id="83372-138">Contém o tempo de entrega da mensagem que foi recebida pela última vez nesta conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="83372-138">Contains the delivery time of the message that was last received in this conversation in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="83372-139">GlobalLastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="83372-139">GlobalLastDeliveryTime</span></span>](globallastdeliverytime.md) <br/> |<span data-ttu-id="83372-140">Contém o tempo de entrega da mensagem que foi recebida pela última vez nesta conversa em todas as pastas da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="83372-140">Contains the delivery time of the message that was last received in this conversation across all folders in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="83372-141">Categorias</span><span class="sxs-lookup"><span data-stu-id="83372-141">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="83372-142">Contém uma coleção de cadeias de caracteres que identificam as categorias que são aplicadas a todos os itens de conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="83372-142">Contains a collection of strings that identify the categories that are applied to all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="83372-143">GlobalCategories</span><span class="sxs-lookup"><span data-stu-id="83372-143">GlobalCategories</span></span>](globalcategories.md) <br/> |<span data-ttu-id="83372-144">Contém a lista de categorias de todos os itens de conversa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="83372-144">Contains the category list for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="83372-145">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="83372-145">FlagStatus</span></span>](flagstatus.md) <br/> |<span data-ttu-id="83372-146">Contém o status de sinalizador agregado para itens de conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="83372-146">Contains the aggregated flag status for conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="83372-147">GlobalFlagStatus</span><span class="sxs-lookup"><span data-stu-id="83372-147">GlobalFlagStatus</span></span>](globalflagstatus.md) <br/> |<span data-ttu-id="83372-148">Contém o status de sinalizador agregado para todos os itens de conversa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="83372-148">Contains the aggregated flag status for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="83372-149">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="83372-149">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="83372-150">Contém um valor que indica se pelo menos um item de conversa na pasta atual tem um anexo.</span><span class="sxs-lookup"><span data-stu-id="83372-150">Contains a value that indicates whether at least one conversation item in the current folder has an attachment.</span></span>  <br/> |
|[<span data-ttu-id="83372-151">GlobalHasAttachments</span><span class="sxs-lookup"><span data-stu-id="83372-151">GlobalHasAttachments</span></span>](globalhasattachments.md) <br/> |<span data-ttu-id="83372-152">Contém um valor que indica se pelo menos um item de conversa em uma caixa de correio tem um anexo.</span><span class="sxs-lookup"><span data-stu-id="83372-152">Contains a value that indicates whether at least one conversation item in a mailbox has an attachment.</span></span>  <br/> |
|[<span data-ttu-id="83372-153">MessageCount</span><span class="sxs-lookup"><span data-stu-id="83372-153">MessageCount</span></span>](messagecount.md) <br/> |<span data-ttu-id="83372-154">Contém o número total de itens de conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="83372-154">Contains the total number of conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="83372-155">GlobalMessageCount</span><span class="sxs-lookup"><span data-stu-id="83372-155">GlobalMessageCount</span></span>](globalmessagecount.md) <br/> |<span data-ttu-id="83372-156">Contém o número total de itens de conversa na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="83372-156">Contains the total number of conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="83372-157">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="83372-157">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="83372-158">Contém a contagem de itens de conversa não lidos em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="83372-158">Contains the count of unread conversation items within a folder.</span></span>  <br/> |
|[<span data-ttu-id="83372-159">GlobalUnreadCount</span><span class="sxs-lookup"><span data-stu-id="83372-159">GlobalUnreadCount</span></span>](globalunreadcount.md) <br/> |<span data-ttu-id="83372-160">Contém uma contagem de todos os itens de conversa não lidos na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="83372-160">Contains a count of all the unread conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="83372-161">Tamanho</span><span class="sxs-lookup"><span data-stu-id="83372-161">Size</span></span>](size.md) <br/> |<span data-ttu-id="83372-162">Contém o tamanho da conversa calculado a partir do tamanho de todos os itens de conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="83372-162">Contains the conversation size calculated from the size of all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="83372-163">GlobalSize</span><span class="sxs-lookup"><span data-stu-id="83372-163">GlobalSize</span></span>](globalsize.md) <br/> |<span data-ttu-id="83372-164">Contém o tamanho da conversa calculada a partir do tamanho de todos os itens de conversa da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="83372-164">Contains the size of the conversation calculated from the size of all conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="83372-165">Doclasss (ArrayOfItemClassType)</span><span class="sxs-lookup"><span data-stu-id="83372-165">ItemClasses (ArrayOfItemClassType)</span></span>](itemclasses-arrayofitemclasstype.md) <br/> |<span data-ttu-id="83372-166">Contém uma lista de classes de item que representa todas as classes de item dos itens de conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="83372-166">Contains a list of item classes that represents all the item classes of the conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="83372-167">GlobalItemClasses</span><span class="sxs-lookup"><span data-stu-id="83372-167">GlobalItemClasses</span></span>](globalitemclasses.md) <br/> |<span data-ttu-id="83372-168">Contém uma lista de classes de item que representa todas as classes de item dos itens de conversa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="83372-168">Contains a list of item classes that represents all the item classes of the conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="83372-169">Importance</span><span class="sxs-lookup"><span data-stu-id="83372-169">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="83372-170">Contém a importância agregada para todos os itens de conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="83372-170">Contains the aggregated importance for all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="83372-171">GlobalImportance</span><span class="sxs-lookup"><span data-stu-id="83372-171">GlobalImportance</span></span>](globalimportance.md) <br/> |<span data-ttu-id="83372-172">Contém a importância agregada para todos os itens de conversa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="83372-172">Contains the aggregated importance for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="83372-173">ItemIds</span><span class="sxs-lookup"><span data-stu-id="83372-173">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="83372-174">Contém a coleção de identificadores de item para todos os itens de conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="83372-174">Contains the collection of item identifiers for all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="83372-175">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="83372-175">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="83372-176">Contém a coleção de identificadores de item para todos os itens de conversa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="83372-176">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="83372-177">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="83372-177">Parent elements</span></span>

|<span data-ttu-id="83372-178">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="83372-178">**Element**</span></span>|<span data-ttu-id="83372-179">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="83372-179">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="83372-180">Conversas</span><span class="sxs-lookup"><span data-stu-id="83372-180">Conversations</span></span>](conversations-ex15websvcsotherref.md) <br/> |<span data-ttu-id="83372-181">Contém uma matriz de conversas que são retornadas na resposta **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="83372-181">Contains an array of conversations that are returned in the **FindConversation** response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="83372-182">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="83372-182">Text value</span></span>

<span data-ttu-id="83372-183">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="83372-183">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="83372-184">Comentários</span><span class="sxs-lookup"><span data-stu-id="83372-184">Remarks</span></span>

<span data-ttu-id="83372-185">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="83372-185">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="83372-186">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="83372-186">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="83372-187">Namespace</span><span class="sxs-lookup"><span data-stu-id="83372-187">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="83372-188">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="83372-188">Schema name</span></span>  <br/> |<span data-ttu-id="83372-189">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="83372-189">Types schema</span></span>  <br/> |
|<span data-ttu-id="83372-190">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="83372-190">Validation file</span></span>  <br/> |<span data-ttu-id="83372-191">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="83372-191">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="83372-192">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="83372-192">Can be empty</span></span>  <br/> |<span data-ttu-id="83372-193">False</span><span class="sxs-lookup"><span data-stu-id="83372-193">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="83372-194">Confira também</span><span class="sxs-lookup"><span data-stu-id="83372-194">See also</span></span>



[<span data-ttu-id="83372-195">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="83372-195">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="83372-196">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="83372-196">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="83372-197">Conversas no EWS</span><span class="sxs-lookup"><span data-stu-id="83372-197">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

