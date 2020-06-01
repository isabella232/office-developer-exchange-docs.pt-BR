---
title: Operação GetConversationItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8ae00a99-b37b-4194-829c-fe300db6ab99
description: Encontre informações sobre a operação GetConversationItems.
ms.openlocfilehash: ddeb5386e56653a32ca2e6d212518704cd0f0c58
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457778"
---
# <a name="getconversationitems-operation"></a><span data-ttu-id="667f4-103">Operação GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="667f4-103">GetConversationItems operation</span></span>

<span data-ttu-id="667f4-104">Encontre informações sobre a operação **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="667f4-104">Find information about the **GetConversationItems** operation.</span></span> 
  
<span data-ttu-id="667f4-105">A operação **GetConversationItems** Obtém um ou mais conjuntos de itens que são organizados em para nós em uma conversa.</span><span class="sxs-lookup"><span data-stu-id="667f4-105">The **GetConversationItems** operation gets one or more sets of items that are organized in to nodes in a conversation.</span></span> 
  
<span data-ttu-id="667f4-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="667f4-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getconversationitems-operation"></a><span data-ttu-id="667f4-107">Usando a operação GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="667f4-107">Using the GetConversationItems operation</span></span>

<span data-ttu-id="667f4-108">Você pode usar a operação **GetConversationItems** para obter itens em conversas para caixas de correio primárias e de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="667f4-108">You can use the **GetConversationItems** operation to get items in conversations for both primary and archive mailboxes.</span></span> 
  
### <a name="getconversationitems-operation-soap-headers"></a><span data-ttu-id="667f4-109">Cabeçalhos SOAP de operação GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="667f4-109">GetConversationItems operation SOAP headers</span></span>

<span data-ttu-id="667f4-110">A operação **GetConversationItems** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="667f4-110">The **GetConversationItems** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="667f4-111">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="667f4-111">**Header name**</span></span>|<span data-ttu-id="667f4-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="667f4-112">**Element**</span></span>|<span data-ttu-id="667f4-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="667f4-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="667f4-114">**Representação**</span><span class="sxs-lookup"><span data-stu-id="667f4-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="667f4-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="667f4-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="667f4-116">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="667f4-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="667f4-117">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="667f4-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="667f4-118">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="667f4-118">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="667f4-119">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="667f4-119">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="667f4-120">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="667f4-120">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="667f4-121">O valor mínimo para esse elemento é **Exchange2013**.</span><span class="sxs-lookup"><span data-stu-id="667f4-121">The minimum value for this element is **Exchange2013**.</span></span> <span data-ttu-id="667f4-122">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="667f4-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="667f4-123">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="667f4-123">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="667f4-124">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="667f4-124">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="667f4-125">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="667f4-125">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="667f4-126">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="667f4-126">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getconversationitems-operation-request-example-get-items-in-a-single-conversation"></a><span data-ttu-id="667f4-127">Exemplo de solicitação de operação GetConversationItems: obter itens em uma única conversa</span><span class="sxs-lookup"><span data-stu-id="667f4-127">GetConversationItems operation request example: Get items in a single conversation</span></span>

<span data-ttu-id="667f4-128">O exemplo a seguir de uma solicitação de operação **GetConversationItems** mostra como obter todos os itens de conversa em uma única conversa, com exceção dos itens localizados nas pastas itens excluídos e rascunhos.</span><span class="sxs-lookup"><span data-stu-id="667f4-128">The following example of a **GetConversationItems** operation request shows how to get all conversation items in a single conversation, with the exception of items located in the Deleted Items and Drafts folders.</span></span> <span data-ttu-id="667f4-129">Cada item retornado na resposta conterá um identificador de item, um assunto e a hora em que o item foi recebido na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="667f4-129">Each item returned in the response will contain an item identifier, a subject, and the time that the item was received in the mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="667f4-130">Todos os identificadores de item e as chaves de alteração deste artigo foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="667f4-130">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:GetConversationItems>
         <m:ItemShape>
            <t:BaseShape>IdOnly</t:BaseShape>
            <t:AdditionalProperties>
               <t:FieldURI FieldURI="item:Subject" />
               <t:FieldURI FieldURI="item:DateTimeReceived" />
            </t:AdditionalProperties>
         </m:ItemShape>
         <m:FoldersToIgnore>
            <t:DistinguishedFolderId Id="deleteditems" />
            <t:DistinguishedFolderId Id="drafts" />
         </m:FoldersToIgnore>
         <m:SortOrder>TreeOrderDescending</m:SortOrder>
         <m:Conversations>
            <t:Conversation>
               <t:ConversationId Id="AAQkADEzOTExYjJkakJCs=" />
            </t:Conversation>
         </m:Conversations>
      </m:GetConversationItems>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="667f4-131">Este exemplo de uma solicitação **GetConversationItems** não inclui as seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="667f4-131">This example of a **GetConversationItems** request does not include the following options:</span></span> 
  
- <span data-ttu-id="667f4-132">O elemento [MaxItemsToReturn](maxitemstoreturn.md) , que define o número máximo de itens a serem retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="667f4-132">The [MaxItemsToReturn](maxitemstoreturn.md) element, which sets the maximum number of items to return in the response.</span></span> 
    
- <span data-ttu-id="667f4-133">O elemento [MailboxScope](mailboxscope.md) , que define o escopo da caixa de correio, indicando se a operação **GetConversationItems** deve ser executada na caixa de correio principal, na caixa de correio de arquivo morto ou nas duas caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="667f4-133">The [MailboxScope](mailboxscope.md) element, which sets the mailbox scope by indicating whether the **GetConversationItems** operation is to be performed on the primary mailbox, the archive mailbox, or both mailboxes.</span></span> 
    
- <span data-ttu-id="667f4-134">O elemento [SyncState (base64Binary)](syncstate-base64binary.md) , que define o estado de sincronização para obter apenas itens de conversa novos ou atualizados na conversa.</span><span class="sxs-lookup"><span data-stu-id="667f4-134">The [SyncState (base64Binary)](syncstate-base64binary.md) element, which sets the synchronization state to only get conversation items that are new or updated in the conversation.</span></span> <span data-ttu-id="667f4-135">Este elemento é definido para cada conversa.</span><span class="sxs-lookup"><span data-stu-id="667f4-135">This element is set for each conversation.</span></span> 
    
<span data-ttu-id="667f4-136">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="667f4-136">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="667f4-137">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="667f4-137">GetConversationItems</span></span>](getconversationitems.md)
    
- [<span data-ttu-id="667f4-138">Shape</span><span class="sxs-lookup"><span data-stu-id="667f4-138">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="667f4-139">BaseShape</span><span class="sxs-lookup"><span data-stu-id="667f4-139">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="667f4-140">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="667f4-140">AdditionalProperties</span></span>](additionalproperties.md)
    
- [<span data-ttu-id="667f4-141">FieldURI</span><span class="sxs-lookup"><span data-stu-id="667f4-141">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="667f4-142">FoldersToIgnore</span><span class="sxs-lookup"><span data-stu-id="667f4-142">FoldersToIgnore</span></span>](folderstoignore.md)
    
- [<span data-ttu-id="667f4-143">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="667f4-143">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="667f4-144">SortOrder (ConversationNodeSortOrder)</span><span class="sxs-lookup"><span data-stu-id="667f4-144">SortOrder (ConversationNodeSortOrder)</span></span>](sortorder-conversationnodesortorder.md)
    
- [<span data-ttu-id="667f4-145">Conversas</span><span class="sxs-lookup"><span data-stu-id="667f4-145">Conversations</span></span>](conversations-ex15websvcsotherref.md)
    
- [<span data-ttu-id="667f4-146">Conversa (ConversationRequestType)</span><span class="sxs-lookup"><span data-stu-id="667f4-146">Conversation (ConversationRequestType)</span></span>](conversation-conversationrequesttype.md)
    
- [<span data-ttu-id="667f4-147">ConversationId</span><span class="sxs-lookup"><span data-stu-id="667f4-147">ConversationId</span></span>](conversationid.md)
    
## <a name="successful-getconversationitems-operation-response"></a><span data-ttu-id="667f4-148">Resposta de operação GetConversationItems bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="667f4-148">Successful GetConversationItems operation response</span></span>

<span data-ttu-id="667f4-149">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetConversationItems** para obter itens em uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="667f4-149">The following example shows a successful response to a **GetConversationItems** operation request to get items in a single conversation.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15"
                           MinorVersion="0"
                           MajorBuildNumber="545"
                           MinorBuildNumber="11"
                           Version="Exchange2013"
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetConversationItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:GetConversationItemsResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Conversation>
                  <t:ConversationId Id="AAQkADEzOTExYjJkakJCs=" />
                  <t:SyncState>AQIAAABNVkUwAgIAAABhHqHUAwIAAABNVkUxBAIAAABhHqHfBAIAAABhHqHV</t:SyncState>
                  <t:ConversationNodes>
                     <t:ConversationNode>
                        <t:InternetMessageId>6a4838fa804045e09d40c1a39b9ea916@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>15a56698d503438fbdaa18186d5b81b7@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkADEzOTQrAABhHqHfAAA=" ChangeKey="CQAAABYAAACYAABhPpaq" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T18:42:27Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>2695d2b837954d68846b0c30491f5af1@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>15a56698d503438fbdaa18186d5b81b7@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkADEzOTExYjJkLTYxZDAt" ChangeKey="CQAAABQrAABhPpaP" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:38:26Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>15a56698d503438fbdaa18186d5b81b7@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>d3113e59c89c4288ae13100d033f8dbc@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkADEzOTFNVkUxAAA=" ChangeKey="CQAAABY4QrAABhPvYK" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:37:00Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>d3113e59c89c4288ae13100d033f8dbc@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>189b712056c2430dbce334b40496ad00@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkm4QrAABhHqHUAAA=" ChangeKey="CQAAABQrAABhPpaN" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:37:05Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>189b712056c2430dbce334b40496ad00@contoso.com</t:InternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkArAABNVkUwAAA=" ChangeKey="CQAAABm4QrAABhPvYJ" />
                              <t:Subject>Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:36:00Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                  </t:ConversationNodes>
               </m:Conversation>
            </m:GetConversationItemsResponseMessage>
         </m:ResponseMessages>
      </m:GetConversationItemsResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="667f4-150">Recomendamos que você salve o SyncState para solicitações de operação **GetConversationItems** subsequentes.</span><span class="sxs-lookup"><span data-stu-id="667f4-150">We recommend that you save the SyncState for subsequent **GetConversationItems** operation requests.</span></span> 
  
<span data-ttu-id="667f4-151">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="667f4-151">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="667f4-152">GetConversationItemsResponse</span><span class="sxs-lookup"><span data-stu-id="667f4-152">GetConversationItemsResponse</span></span>](getconversationitemsresponse.md)
    
- [<span data-ttu-id="667f4-153">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="667f4-153">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="667f4-154">GetConversationItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="667f4-154">GetConversationItemsResponseMessage</span></span>](getconversationitemsresponsemessage.md)
    
- [<span data-ttu-id="667f4-155">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="667f4-155">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="667f4-156">Conversa (ConversationResponseType)</span><span class="sxs-lookup"><span data-stu-id="667f4-156">Conversation (ConversationResponseType)</span></span>](conversation-conversationresponsetype.md)
    
- [<span data-ttu-id="667f4-157">ConversationId</span><span class="sxs-lookup"><span data-stu-id="667f4-157">ConversationId</span></span>](conversationid.md)
    
- [<span data-ttu-id="667f4-158">SyncState (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="667f4-158">SyncState (base64Binary)</span></span>](syncstate-base64binary.md)
    
- [<span data-ttu-id="667f4-159">ConversationNodes</span><span class="sxs-lookup"><span data-stu-id="667f4-159">ConversationNodes</span></span>](conversationnodes.md)
    
- [<span data-ttu-id="667f4-160">ConversationNode</span><span class="sxs-lookup"><span data-stu-id="667f4-160">ConversationNode</span></span>](conversationnode.md)
    
- [<span data-ttu-id="667f4-161">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="667f4-161">InternetMessageId</span></span>](internetmessageid.md)
    
- [<span data-ttu-id="667f4-162">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="667f4-162">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="667f4-163">Message</span><span class="sxs-lookup"><span data-stu-id="667f4-163">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="667f4-164">ItemId</span><span class="sxs-lookup"><span data-stu-id="667f4-164">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="667f4-165">Assunto</span><span class="sxs-lookup"><span data-stu-id="667f4-165">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="667f4-166">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="667f4-166">DateTimeReceived</span></span>](datetimereceived.md)
    
## <a name="getconversationitems-operation-error-response"></a><span data-ttu-id="667f4-167">Resposta de erro de operação GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="667f4-167">GetConversationItems operation error response</span></span>

<span data-ttu-id="667f4-168">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **GetConversationItems** para obter itens em uma conversa que não existe mais na caixa de correio ou para os quais todos os itens de conversa estão localizados em pastas ignoradas.</span><span class="sxs-lookup"><span data-stu-id="667f4-168">The following example shows an error response to a **GetConversationItems** operation request to get items in a conversation that either no longer exists in the mailbox, or for which all the conversation items are located in folders that are ignored.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="556" MinorBuildNumber="8" Version="Exchange2013" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetConversationItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetConversationItemsResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:GetConversationItemsResponseMessage>
      </m:ResponseMessages>
    </m:GetConversationItemsResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="667f4-169">Também consulte</span><span class="sxs-lookup"><span data-stu-id="667f4-169">See also</span></span>

- [<span data-ttu-id="667f4-170">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="667f4-170">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="667f4-171">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="667f4-171">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
    
- [<span data-ttu-id="667f4-172">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="667f4-172">FindConversation operation</span></span>](findconversation-operation.md)
    

