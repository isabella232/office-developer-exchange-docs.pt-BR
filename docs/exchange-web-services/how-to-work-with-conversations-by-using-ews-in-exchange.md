---
title: Trabalhar com conversas usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7750528c-acb2-43e5-a1e1-ee201c0e1730
description: Saiba mais sobre como encontrar conversas, aplicar ações a conversas e obter itens em conversas usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 2dc66195f8d37836c32fc33737728c61fc5444ae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456784"
---
# <a name="work-with-conversations-by-using-ews-in-exchange"></a><span data-ttu-id="a1a37-103">Trabalhar com conversas usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a1a37-103">Work with conversations by using EWS in Exchange</span></span>

<span data-ttu-id="a1a37-104">Saiba mais sobre como encontrar conversas, aplicar ações a conversas e obter itens em conversas usando a API gerenciada do EWS ou o EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="a1a37-104">Learn about how to find conversations, apply actions to conversations, and get items in conversations by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="a1a37-105">No contexto do Exchange, as conversas são uma maneira de agrupar e gerenciar um conjunto relacionado de mensagens de email.</span><span class="sxs-lookup"><span data-stu-id="a1a37-105">In the context of Exchange, conversations are a way to group and manage a related set of email messages.</span></span> <span data-ttu-id="a1a37-106">Eles também podem fornecer uma maneira de exibir mensagens relacionadas.</span><span class="sxs-lookup"><span data-stu-id="a1a37-106">They can also provide a way to view related messages.</span></span> <span data-ttu-id="a1a37-107">O Exchange define conversas com base no valor **Message-ID** da primeira mensagem de email em um thread.</span><span class="sxs-lookup"><span data-stu-id="a1a37-107">Exchange defines conversations based on the **Message-ID** value of the first email message in a thread.</span></span> <span data-ttu-id="a1a37-108">Todas as respostas e mensagens relacionadas fazem referência ao cabeçalho **Message-ID** da mensagem original em suas **referências** e cabeçalhos **in-reply-to** .</span><span class="sxs-lookup"><span data-stu-id="a1a37-108">All replies and related messages reference the original message's **Message-ID** header in their **References** and **In-Reply-To** headers.</span></span> 
  
<span data-ttu-id="a1a37-109">Além disso, dentro do envelope SOAP, para cada mensagem recebida em uma caixa de correio, o Exchange define propriedades e elementos específicos.</span><span class="sxs-lookup"><span data-stu-id="a1a37-109">Additionally, inside the SOAP envelope, for each message received in a mailbox, Exchange sets specific properties and elements.</span></span>
  
<span data-ttu-id="a1a37-110">**Tabela 1. Propriedades e elementos de conversa definidos em todas as mensagens de email**</span><span class="sxs-lookup"><span data-stu-id="a1a37-110">**Table 1. Conversation properties and elements set on all email messages**</span></span>

|<span data-ttu-id="a1a37-111">**Propriedade da API gerenciada do EWS**</span><span class="sxs-lookup"><span data-stu-id="a1a37-111">**EWS Managed API property**</span></span>|<span data-ttu-id="a1a37-112">**Elemento do EWS**</span><span class="sxs-lookup"><span data-stu-id="a1a37-112">**EWS element**</span></span>|<span data-ttu-id="a1a37-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a1a37-113">**Description**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="a1a37-114">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="a1a37-114">ConversationTopic</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.conversationtopic%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="a1a37-115">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="a1a37-115">ConversationTopic</span></span>](https://msdn.microsoft.com/library/46cacf42-4039-4c8a-9b20-c42cdd9f2760%28Office.15%29.aspx) <br/> |<span data-ttu-id="a1a37-116">Contém uma forma normalizada do valor de entidade que foi definido na mensagem original.</span><span class="sxs-lookup"><span data-stu-id="a1a37-116">Contains a normalized form of the subject value that was set on the original message.</span></span> <span data-ttu-id="a1a37-117">É o mesmo que o cabeçalho da mensagem do **tópico de thread** .</span><span class="sxs-lookup"><span data-stu-id="a1a37-117">This is the same as the **Thread-Topic** message header.</span></span> <span data-ttu-id="a1a37-118">Esse valor é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a1a37-118">This value is read-only.</span></span>  <br/> |
|[<span data-ttu-id="a1a37-119">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="a1a37-119">ConversationIndex</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.conversationindex%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="a1a37-120">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="a1a37-120">ConversationIndex</span></span>](https://msdn.microsoft.com/library/fdf47e22-8d93-4ae4-883b-0c9f07f48724%28Office.15%29.aspx) <br/> |<span data-ttu-id="a1a37-121">Representa a posição do item na conversa.</span><span class="sxs-lookup"><span data-stu-id="a1a37-121">Represents the position of the item in the conversation.</span></span> <span data-ttu-id="a1a37-122">É o mesmo que o cabeçalho da mensagem de **índice de thread** .</span><span class="sxs-lookup"><span data-stu-id="a1a37-122">This is the same as the **Thread-Index** message header.</span></span> <span data-ttu-id="a1a37-123">Esse valor é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a1a37-123">This value is read-only.</span></span>  <br/> |
   
<span data-ttu-id="a1a37-124">O Exchange aplica o mesmo valor de **ConversationTopic** a respostas à primeira mensagem e atualiza o valor **ConversationIndex** para representar a posição da mensagem em relação à mensagem original.</span><span class="sxs-lookup"><span data-stu-id="a1a37-124">Exchange applies the same **ConversationTopic** value to replies to the first message and then updates the **ConversationIndex** value to represent the message's position relative to the original message.</span></span> <span data-ttu-id="a1a37-125">Se o assunto do thread de email for alterado, o Exchange aplicará um novo valor de **ConversationTopic** e novos valores de **ConversationIndex** à nova conversa.</span><span class="sxs-lookup"><span data-stu-id="a1a37-125">If the subject of the email thread changes, Exchange applies a new **ConversationTopic** value and new **ConversationIndex** values to the new conversation.</span></span> 
  
<span data-ttu-id="a1a37-126">**Tabela 2. Métodos da API gerenciada do EWS e operações do EWS para trabalhar com conversas**</span><span class="sxs-lookup"><span data-stu-id="a1a37-126">**Table 2. EWS Managed API methods and EWS operations for working with conversations**</span></span>

|<span data-ttu-id="a1a37-127">**Para...**</span><span class="sxs-lookup"><span data-stu-id="a1a37-127">**In order to…**</span></span>|<span data-ttu-id="a1a37-128">**Usar este método ou métodos da API gerenciada do EWS**</span><span class="sxs-lookup"><span data-stu-id="a1a37-128">**Use this EWS Managed API method or methods**</span></span>|<span data-ttu-id="a1a37-129">**Use esta operação do EWS**</span><span class="sxs-lookup"><span data-stu-id="a1a37-129">**Use this EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a1a37-130">Localizar conversas</span><span class="sxs-lookup"><span data-stu-id="a1a37-130">Find conversations</span></span>  <br/> |[<span data-ttu-id="a1a37-131">ExchangeService. FindConversation</span><span class="sxs-lookup"><span data-stu-id="a1a37-131">ExchangeService.FindConversation</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findconversation%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="a1a37-132">FindConversation</span><span class="sxs-lookup"><span data-stu-id="a1a37-132">FindConversation</span></span>](https://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="a1a37-133">Aplicar ações de conversa</span><span class="sxs-lookup"><span data-stu-id="a1a37-133">Apply conversation actions</span></span>  <br/> |[<span data-ttu-id="a1a37-134">CONVERSATION. EnableAlwaysCategorizeItems</span><span class="sxs-lookup"><span data-stu-id="a1a37-134">Conversation.EnableAlwaysCategorizeItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.conversation.enablealwayscategorizeitems%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="a1a37-135">CONVERSATION. EnableAlwaysDeleteItems</span><span class="sxs-lookup"><span data-stu-id="a1a37-135">Conversation.EnableAlwaysDeleteItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.conversation.enablealwaysdeleteitems%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="a1a37-136">CONVERSATION. EnableAlwaysMoveItems</span><span class="sxs-lookup"><span data-stu-id="a1a37-136">Conversation.EnableAlwaysMoveItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.conversation.enablealwaysmoveitems%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="a1a37-137">ExchangeService. CopyItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="a1a37-137">ExchangeService.CopyItemsInConversations</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.copyitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="a1a37-138">ExchangeService. DeleteItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="a1a37-138">ExchangeService.DeleteItemsInConversations</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.deleteitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="a1a37-139">ExchangeService. DisableAlwaysCategorizeItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="a1a37-139">ExchangeService.DisableAlwaysCategorizeItemsInConversations</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.disablealwayscategorizeitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="a1a37-140">ExchangeService. DisableAlwaysDeleteItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="a1a37-140">ExchangeService.DisableAlwaysDeleteItemsInConversations</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.disablealwaysdeleteitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="a1a37-141">ExchangeService. DisableAlwaysMoveItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="a1a37-141">ExchangeService.DisableAlwaysMoveItemsInConversations</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.disablealwaysmoveitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="a1a37-142">ExchangeService. EnableAlwaysCategorizeItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="a1a37-142">ExchangeService.EnableAlwaysCategorizeItemsInConversations</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.enablealwayscategorizeitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="a1a37-143">ExchangeService. EnableAlwaysDeleteItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="a1a37-143">ExchangeService.EnableAlwaysDeleteItemsInConversations</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.enablealwaysdeleteitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="a1a37-144">ExchangeService. EnableAlwaysMoveItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="a1a37-144">ExchangeService.EnableAlwaysMoveItemsInConversations</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.enablealwaysmoveitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="a1a37-145">ExchangeService. MoveItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="a1a37-145">ExchangeService.MoveItemsInConversations</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.moveitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="a1a37-146">ExchangeService. SetFlagStatusForItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="a1a37-146">ExchangeService.SetFlagStatusForItemsInConversations</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.setflagstatusforitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="a1a37-147">ExchangeService. SetReadStateForItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="a1a37-147">ExchangeService.SetReadStateForItemsInConversations</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.setreadstateforitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="a1a37-148">ExchangeService. SetRetentionPolicyForItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="a1a37-148">ExchangeService.SetRetentionPolicyForItemsInConversations</span></span>](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.setretentionpolicyforitemsinconversations%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="a1a37-149">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="a1a37-149">ApplyConversationAction</span></span>](https://msdn.microsoft.com/library/73d7943d-d361-4f8b-9948-d85f886efa1a%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="a1a37-150">Obter itens em uma ou mais conversas</span><span class="sxs-lookup"><span data-stu-id="a1a37-150">Get items in one or more conversations</span></span>  <br/> |[<span data-ttu-id="a1a37-151">ExchangeService. GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="a1a37-151">ExchangeService.GetConversationItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="a1a37-152">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="a1a37-152">GetConversationItems</span></span>](https://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) <br/> |

<span data-ttu-id="a1a37-153"><a name="bk_findewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="a1a37-153"><a name="bk_findewsma"> </a></span></span>

## <a name="find-a-conversation-by-using-the-ews-managed-api"></a><span data-ttu-id="a1a37-154">Localizar uma conversa usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="a1a37-154">Find a conversation by using the EWS Managed API</span></span>

<span data-ttu-id="a1a37-155">Você pode encontrar conversas usando o método de API gerenciada do EWS [ExchangeService. FindConversation](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findconversation%28v=exchg.80%29.aspx) , conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="a1a37-155">You can find conversations by using the [ExchangeService.FindConversation](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findconversation%28v=exchg.80%29.aspx) EWS Managed API method, as shown in the following example.</span></span> <span data-ttu-id="a1a37-156">Este exemplo obtém as 10 primeiras conversas na pasta caixa de entrada que têm um assunto que contém a palavra "notícias".</span><span class="sxs-lookup"><span data-stu-id="a1a37-156">This example gets the first 10 conversations in the Inbox folder that have a subject that contains the word "news".</span></span> <span data-ttu-id="a1a37-157">Em seguida, o exemplo grava o tópico de conversa, a última hora de entrega e a lista global de destinatários exclusivos na janela do console.</span><span class="sxs-lookup"><span data-stu-id="a1a37-157">The example then writes the conversation topic, last delivery time, and global unique recipient list to the console window.</span></span> 
  
<span data-ttu-id="a1a37-158">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="a1a37-158">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
static void FindConversation(ExchangeService service)
{
    // Create the view of conversations returned in the response. This view will return at most 10 results.
    ConversationIndexedItemView view = new ConversationIndexedItemView(10);
    // Create the query string to search for.
    String queryString = "subject:news";
    // Search the Inbox for conversations and return a results set with the specified view.
    // This method call results in a FindConversation call to EWS. 
    ICollection<Conversation> conversations = service.FindConversation(view, WellKnownFolderName.Inbox, queryString);
    // Examine properties on each conversation returned in the response.
    foreach (Conversation conversation in conversations)
    {
        Console.WriteLine("Conversation Topic: " + conversation.Topic);
        Console.WriteLine("Last Delivered: " + conversation.LastDeliveryTime.ToString());
        ApplyConversationActions(service, conversation);
        foreach (string GlUniqRec in conversation.GlobalUniqueRecipients)
        {
            Console.WriteLine("Global Unique Recipient: " + GlUniqRec);
        }
        Console.WriteLine("");
    }
}
```

<span data-ttu-id="a1a37-159"><a name="bk_findews"> </a></span><span class="sxs-lookup"><span data-stu-id="a1a37-159"><a name="bk_findews"> </a></span></span>

## <a name="find-a-conversation-by-using-ews"></a><span data-ttu-id="a1a37-160">Localizar uma conversa usando o EWS</span><span class="sxs-lookup"><span data-stu-id="a1a37-160">Find a conversation by using EWS</span></span>

<span data-ttu-id="a1a37-161">Você pode encontrar conversas usando a operação [FindConversation](https://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) EWS, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="a1a37-161">You can find conversations by using the [FindConversation](https://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) EWS operation, as shown in the following example.</span></span> <span data-ttu-id="a1a37-162">Este exemplo obtém as dez primeiras conversas na pasta caixa de entrada que têm um assunto que contém a palavra "notícias".</span><span class="sxs-lookup"><span data-stu-id="a1a37-162">This example gets the first ten conversations in the Inbox folder that have a subject that contains the word "news".</span></span> <span data-ttu-id="a1a37-163">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa a API gerenciada do EWS para [Localizar uma conversa](#bk_findewsma).</span><span class="sxs-lookup"><span data-stu-id="a1a37-163">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [find a conversation](#bk_findewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:FindConversation>
      <m:IndexedPageItemView MaxEntriesReturned="10"
                             Offset="0"
                             BasePoint="Beginning" />
      <m:ParentFolderId>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderId>
      <m:QueryString>subject:news</m:QueryString>
    </m:FindConversation>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="a1a37-164">O servidor responde à solicitação **FindConversation** com uma mensagem [FindConversationResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor de [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR** para indicar que a operação foi concluída com êxito.</span><span class="sxs-lookup"><span data-stu-id="a1a37-164">The server responds to the **FindConversation** request with a [FindConversationResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** to indicate that the operation completed successfully.</span></span> <span data-ttu-id="a1a37-165">A resposta também inclui a única conversa na caixa de correio que tem um assunto que contém a palavra "notícias".</span><span class="sxs-lookup"><span data-stu-id="a1a37-165">The response also includes the only conversation in the mailbox that has a subject that contains the word "news".</span></span> 
  
<span data-ttu-id="a1a37-166">Os elementos **ItemId**, **ChangeKey**e **conversaid** foram reduzidos para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a1a37-166">The **ItemId**, **ChangeKey**, and **ConversationId** elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="883"
                         MinorBuildNumber="10"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <FindConversationResponse ResponseClass="Success"
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Conversations>
        <Conversation xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <ConversationId Id="aO2NM+Q=" />
          <ConversationTopic>Today's top news headlines</ConversationTopic>
          <UniqueRecipients>
            <String>Sadie Daniels</String>
          </UniqueRecipients>
          <GlobalUniqueRecipients>
            <String>Sadie Daniels</String>
          </GlobalUniqueRecipients>
          <UniqueUnreadSenders>
            <String>Ronnie Sturgis</String>
          </UniqueUnreadSenders>
          <GlobalUniqueUnreadSenders>
            <String>Ronnie Sturgis</String>
          </GlobalUniqueUnreadSenders>
          <UniqueSenders>
            <String>Ronnie Sturgis</String>
          </UniqueSenders>
          <GlobalUniqueSenders>
            <String>Ronnie Sturgis</String>
          </GlobalUniqueSenders>
          <LastDeliveryTime>2014-02-18T20:42:26Z</LastDeliveryTime>
          <GlobalLastDeliveryTime>2014-02-18T20:42:26Z</GlobalLastDeliveryTime>
          <HasAttachments>false</HasAttachments>
          <GlobalHasAttachments>false</GlobalHasAttachments>
          <MessageCount>1</MessageCount>
          <GlobalMessageCount>1</GlobalMessageCount>
          <UnreadCount>1</UnreadCount>
          <GlobalUnreadCount>1</GlobalUnreadCount>
          <Size>9330</Size>
          <GlobalSize>9330</GlobalSize>
          <ItemClasses>
            <ItemClass>IPM.Note</ItemClass>
          </ItemClasses>
          <GlobalItemClasses>
            <ItemClass>IPM.Note</ItemClass>
          </GlobalItemClasses>
          <Importance>Normal</Importance>
          <GlobalImportance>Normal</GlobalImportance>
          <ItemIds>
            <ItemId Id="sVCyAAA="
                    ChangeKey="CQAAAA==" />
          </ItemIds>
          <GlobalItemIds>
            <ItemId Id="sVCyAAA="
                    ChangeKey="CQAAAA==" />
          </GlobalItemIds>
          <LastModifiedTime>2014-02-18T20:42:26Z</LastModifiedTime>
          <InstanceKey>AQAAAAAAAQABAAAACbFYggAAAAA=</InstanceKey>
          <HasIrm>false</HasIrm>
          <GlobalHasIrm>false</GlobalHasIrm>
        </Conversation>
      </Conversations>
      <TotalConversationsInView>1</TotalConversationsInView>
      <IndexedOffset>1</IndexedOffset>
    </FindConversationResponse>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="a1a37-167"><a name="bk_applyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="a1a37-167"><a name="bk_applyewsma"> </a></span></span>

## <a name="apply-conversation-actions-by-using-the-ews-managed-api"></a><span data-ttu-id="a1a37-168">Aplicar ações de conversa usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="a1a37-168">Apply conversation actions by using the EWS Managed API</span></span>

<span data-ttu-id="a1a37-169">Você pode aplicar ações de conversa a uma conversa usando vários métodos de API gerenciada do EWS, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="a1a37-169">You can apply conversation actions to a conversation by using a number of EWS Managed API methods, as shown in the following example.</span></span> <span data-ttu-id="a1a37-170">Este exemplo adiciona categorias a itens existentes em uma conversa e aplica as mesmas categorias a itens futuros na conversa.</span><span class="sxs-lookup"><span data-stu-id="a1a37-170">This example adds categories to existing items in a conversation and applies the same categories to future items in the conversation.</span></span> <span data-ttu-id="a1a37-171">Também mostra como habilitar a movimentação automática de itens na conversa para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="a1a37-171">It also shows how to enable the automatic moving of items in the conversation to a folder.</span></span> <span data-ttu-id="a1a37-172">Neste exemplo, os itens são movidos para a pasta Rascunhos.</span><span class="sxs-lookup"><span data-stu-id="a1a37-172">In this example, items are moved to the Drafts folder.</span></span>
  
<span data-ttu-id="a1a37-173">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="a1a37-173">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
<span data-ttu-id="a1a37-174">Para obter uma lista completa dos métodos que aplicam ações de conversa, consulte a tabela 2.</span><span class="sxs-lookup"><span data-stu-id="a1a37-174">For a complete list of methods that apply conversation actions, see Table 2.</span></span>
  
```cs
static void ApplyConversationActions(ExchangeService service, Conversation conversation)
{
   // Create a list of categories to apply to a conversation.
   List<string> categories = new List<string>();
   categories.Add("Customer");
   categories.Add("System Integrator");
   // Apply categorization to all items in the conversation and process the request
   // synchronously after enabling this rule and after all item categorization has been applied. 
   // This method call results in an ApplyConversationAction call to EWS.
   conversation.EnableAlwaysCategorizeItems(categories, true);
   // Apply an always move rule to all items in the conversation and move the items
   // to the Drafts folder. Process the request asynchronously and return the response. 
   // immediately. This method call results in an ApplyConversationAction call to EWS.
   conversation.EnableAlwaysMoveItems(WellKnownFolderName.Drafts, false);
}

```

<span data-ttu-id="a1a37-175"><a name="bk_applyews"> </a></span><span class="sxs-lookup"><span data-stu-id="a1a37-175"><a name="bk_applyews"> </a></span></span>

## <a name="apply-conversation-actions-by-using-ews"></a><span data-ttu-id="a1a37-176">Aplicar ações de conversa usando o EWS</span><span class="sxs-lookup"><span data-stu-id="a1a37-176">Apply conversation actions by using EWS</span></span>

<span data-ttu-id="a1a37-177">Você pode aplicar ações de conversa, como categorizar, excluir e mover, usando a operação [ApplyConversationAction](https://msdn.microsoft.com/library/73d7943d-d361-4f8b-9948-d85f886efa1a%28Office.15%29.aspx) , conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="a1a37-177">You can apply conversation actions, such as categorize, delete, and move, by using the [ApplyConversationAction](https://msdn.microsoft.com/library/73d7943d-d361-4f8b-9948-d85f886efa1a%28Office.15%29.aspx) operation, as shown in the following example.</span></span> <span data-ttu-id="a1a37-178">Este exemplo adiciona categorias a itens existentes em uma conversa e aplica as mesmas categorias a itens futuros na conversa.</span><span class="sxs-lookup"><span data-stu-id="a1a37-178">This example adds categories to existing items in a conversation and applies the same categories to future items in the conversation.</span></span> <span data-ttu-id="a1a37-179">Também mostra como habilitar a movimentação automática de itens na conversa para uma pasta; Neste exemplo, os itens são movidos para a pasta Rascunhos.</span><span class="sxs-lookup"><span data-stu-id="a1a37-179">It also shows how to enable the automatic moving of items in the conversation to a folder; in this example, items are moved to the Drafts folder.</span></span> <span data-ttu-id="a1a37-180">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você usa a API gerenciada do EWS para [aplicar ações de conversa](#bk_applyewsma).</span><span class="sxs-lookup"><span data-stu-id="a1a37-180">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [apply conversation actions](#bk_applyewsma).</span></span>
  
<span data-ttu-id="a1a37-181">O elemento **Conversation** foi reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a1a37-181">The **ConversationId** element has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:ApplyConversationAction>
      <m:ConversationActions>
        <t:ConversationAction>
          <t:Action>AlwaysMove</t:Action>
          <t:ConversationId Id="jG6WVpg=" />
          <t:ProcessRightAway>false</t:ProcessRightAway>
          <t:DestinationFolderId>
            <t:DistinguishedFolderId Id="drafts" />
          </t:DestinationFolderId>
        </t:ConversationAction>
      </m:ConversationActions>
    </m:ApplyConversationAction>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="a1a37-182">O servidor responde à solicitação **ApplyConversationAction** com uma mensagem [ApplyConversationActionResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor de [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR** para indicar que a operação foi concluída com êxito.</span><span class="sxs-lookup"><span data-stu-id="a1a37-182">The server responds to the **ApplyConversationAction** request with a [ApplyConversationActionResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** to indicate that the operation completed successfully.</span></span> 

<span data-ttu-id="a1a37-183"><a name="bk_getitemssingleewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="a1a37-183"><a name="bk_getitemssingleewsma"> </a></span></span>

## <a name="get-items-in-a-single-conversation-by-using-the-conversation-identifier-in-the-ews-managed-api"></a><span data-ttu-id="a1a37-184">Obter itens em uma única conversa usando o identificador de conversa na API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="a1a37-184">Get items in a single conversation by using the conversation identifier in the EWS Managed API</span></span>

<span data-ttu-id="a1a37-185">Você pode obter itens em uma conversa usando o método de API gerenciada do EWS [ExchangeService. GetConversationItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="a1a37-185">You can get items in a conversation by using the [ExchangeService.GetConversationItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) EWS Managed API method.</span></span> <span data-ttu-id="a1a37-186">Este exemplo fornece o conjunto de nós de conversa para a primeira conversa na caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="a1a37-186">This example provides the set of conversation nodes for the first conversation in the Inbox.</span></span> <span data-ttu-id="a1a37-187">O identificador de item, o assunto e o horário de recebimento de cada item são retornados na resposta, juntamente com as propriedades de índice de conversa pai e índice de conversa.</span><span class="sxs-lookup"><span data-stu-id="a1a37-187">The item identifier, subject, and received time for each item are returned in the response, along with the conversation index and parent conversation index properties.</span></span> <span data-ttu-id="a1a37-188">Você pode usar as propriedades do índice de conversa para reconstruir a hierarquia do nó.</span><span class="sxs-lookup"><span data-stu-id="a1a37-188">You can use the conversation index properties to reconstruct the node hierarchy.</span></span> 
  
<span data-ttu-id="a1a37-189">Neste exemplo, todos os itens de conversa nas pastas itens excluídos padrão e rascunhos são ignorados.</span><span class="sxs-lookup"><span data-stu-id="a1a37-189">In this example, all conversation items in the default Deleted Items and Drafts folders are ignored.</span></span>
  
<span data-ttu-id="a1a37-190">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="a1a37-190">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
static void GetConversationItemsSingleConversation(ExchangeService service)
{
   try
   {
      // Find the first item in the mailbox.
      // This method call results in an FindItem call to EWS.
      FindItemsResults<Item> results = service.FindItems(WellKnownFolderName.Inbox,
                                                         new ItemView(1));
      // Get the conversation identifier of the item. 
      ConversationId convId = results.Items[0].ConversationId;
      // Specify the properties that will be 
      // returned for the items in the conversation.
      PropertySet properties = new PropertySet(BasePropertySet.IdOnly,
                                                ItemSchema.Subject,
                                                ItemSchema.DateTimeReceived);
      // Identify the folders to ignore.
      Collection<FolderId> foldersToIgnore = new Collection<FolderId>() 
          { WellKnownFolderName.DeletedItems, WellKnownFolderName.Drafts };
      // Request the conversation items.
      // This method call results in an GetConversationItems call to EWS.
      ConversationResponse response = service.GetConversationItems(convId,
                                                   properties,
                                                  null,
                                                  foldersToIgnore,
                                                  ConversationSortOrder.TreeOrderDescending);
      // Get the synchronization state of the conversation.
      Console.WriteLine("SyncState: " + response.SyncState);
      Collection<Item> items = new Collection<Item>();
      // Process each node of conversation items.
      foreach (ConversationNode node in response.ConversationNodes)
      {
         Console.WriteLine("Parent conversation index: " + node.ParentConversationIndex);
         Console.WriteLine("Conversation index: " + node.ConversationIndex);
         Console.WriteLine("Conversation node items:");
         // Process each item in the conversation node.
         foreach (Item item in node.Items)
         {
            Console.WriteLine("   Item ID: " + item.Id.UniqueId);
            Console.WriteLine("   Subject: " + item.Subject);
            Console.WriteLine("   Received: " + item.DateTimeReceived);
            items.Add(item);
         }
      }
   }
   // This exception occurs if there is an error with the service.
   catch (ServiceResponseException srException)
   {
      Console.WriteLine(srException);
   }
}

```

<span data-ttu-id="a1a37-191">Recomendamos que você armazene em cache a propriedade **SyncState** para solicitações subsequentes para obter itens na conversa.</span><span class="sxs-lookup"><span data-stu-id="a1a37-191">We recommend that you cache the **SyncState** property for subsequent requests to get items in the conversation.</span></span> 

<span data-ttu-id="a1a37-192"><a name="bk_getitemsmanyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="a1a37-192"><a name="bk_getitemsmanyewsma"> </a></span></span>

## <a name="get-items-in-many-conversations-by-using-the-conversationrequest-object-in-the-ews-managed-api"></a><span data-ttu-id="a1a37-193">Obter itens em várias conversas usando o objeto ConversationRequest na API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="a1a37-193">Get items in many conversations by using the ConversationRequest object in the EWS Managed API</span></span>

<span data-ttu-id="a1a37-194">Você pode usar o objeto [ConversationRequest](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.conversationrequest%28v=exchg.80%29.aspx) e o método de API gerenciada do EWS do [ExchangeService. GetConversationItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) para obter itens de duas ou mais conversas.</span><span class="sxs-lookup"><span data-stu-id="a1a37-194">You can use the [ConversationRequest](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.conversationrequest%28v=exchg.80%29.aspx) object and the [ExchangeService.GetConversationItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) EWS Managed API method to get items from two or more conversations.</span></span> <span data-ttu-id="a1a37-195">Este exemplo fornece um conjunto de nós de conversa para as duas primeiras conversas na caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="a1a37-195">This example provides a set of conversation nodes for the first two conversations in the Inbox.</span></span> <span data-ttu-id="a1a37-196">O identificador de item, o assunto e o horário de recebimento de cada item serão retornados na resposta, juntamente com as propriedades de índice de conversa pai e índice de conversa.</span><span class="sxs-lookup"><span data-stu-id="a1a37-196">The item identifier, subject, and the received time for each item will be returned in the response, along with the conversation index and parent conversation index properties.</span></span> <span data-ttu-id="a1a37-197">Você pode usar as propriedades do índice de conversa para reconstruir a hierarquia do nó.</span><span class="sxs-lookup"><span data-stu-id="a1a37-197">You can use the conversation index properties to reconstruct the node hierarchy.</span></span> <span data-ttu-id="a1a37-198">Este exemplo pressupõe que os primeiros dois itens na caixa de entrada são de conversas diferentes.</span><span class="sxs-lookup"><span data-stu-id="a1a37-198">This example assumes that the first two items in the Inbox are from different conversations.</span></span> 
  
<span data-ttu-id="a1a37-199">Neste exemplo, todos os itens de conversa nas pastas itens excluídos padrão e rascunhos são ignorados.</span><span class="sxs-lookup"><span data-stu-id="a1a37-199">In this example, all conversation items in the default Deleted Items and Drafts folders are ignored.</span></span>
  
<span data-ttu-id="a1a37-200">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="a1a37-200">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
static void GetConversationItemsManyConversations(ExchangeService service)
{
   try
   {
      // Find the first two items in the Inbox. This item will be used to call the GetConversationItems operation.
      // This method call results in an FindItem call to EWS.
      FindItemsResults<Item> results = service.FindItems(WellKnownFolderName.Inbox, new ItemView(2));
      // Get the conversation identifier of the first two items in the Inbox. 
      ConversationId convId1 = results.Items[0].ConversationId;
      ConversationId convId2 = results.Items[1].ConversationId;
      
      // Identify two conversation requests. 
      ConversationRequest convR1 = new ConversationRequest();
      convR1.ConversationId = convId1;
      ConversationRequest convR2 = new ConversationRequest();
      convR2.ConversationId = convId2;
      // Create a collection of conversations to fetch. 
      Collection<ConversationRequest> conversations = new Collection<ConversationRequest>();
      conversations.Add(convR1);
      conversations.Add(convR2);
      // Specify the properties that will be returned for the items in the conversation.
      PropertySet properties = new PropertySet(BasePropertySet.IdOnly,
                                                ItemSchema.Subject,
                                                ItemSchema.DateTimeReceived);
      // Identify the folders to ignore.
      Collection<FolderId> foldersToIgnore = new Collection<FolderId>() 
          { WellKnownFolderName.DeletedItems, WellKnownFolderName.Drafts };
      // Request the conversation items.
      // This method call results in an GetConversationItems call to EWS.
      ServiceResponseCollection<GetConversationItemsResponse> responses = 
          service.GetConversationItems(conversations, properties, foldersToIgnore, 
          ConversationSortOrder.TreeOrderDescending);
      // Process each conversation.
      foreach (GetConversationItemsResponse resp in responses)
      {
         // Identify the synchronization state of the conversation.
         Console.WriteLine("Sync State: " + resp.Conversation.SyncState);
         // Process each node in the conversation.
         foreach (ConversationNode node in resp.Conversation.ConversationNodes)
         {
            Console.WriteLine("Parent conversation index: " + node.ParentConversationIndex);
            Console.WriteLine("Conversation index: " + node.ConversationIndex);
            Console.WriteLine("Conversation node items:");
            // Process each item in the conversation node.
            foreach (Item item in node.Items)
            {
               Console.WriteLine("   Item ID: " + item.Id.UniqueId);
               Console.WriteLine("   Subject: " + item.Subject);
               Console.WriteLine("   Received: " + item.DateTimeReceived);
            }
         }
      }
   }
   // This exception occurs if there is an error with the service.
   catch (ServiceResponseException srException)
   { 
      Console.WriteLine(srException);
   }
}

```

<span data-ttu-id="a1a37-201">Como prática recomendada, recomendamos que você retorne apenas as propriedades exigidas pelo aplicativo cliente, em vez de usar a opção **FirstClassProperties** para a classe **BasePropertySet** .</span><span class="sxs-lookup"><span data-stu-id="a1a37-201">As a best practice, we recommend that you return only the properties that the client application requires, rather than using the **FirstClassProperties** option for the **BasePropertySet** class.</span></span> <span data-ttu-id="a1a37-202">Recomendamos que você armazene em cache a propriedade **SyncState** para solicitações subsequentes para obter itens na conversa.</span><span class="sxs-lookup"><span data-stu-id="a1a37-202">We recommend that you cache the **SyncState** property for subsequent requests to get items in the conversation.</span></span> 

<span data-ttu-id="a1a37-203"><a name="bk_getitemsews"> </a></span><span class="sxs-lookup"><span data-stu-id="a1a37-203"><a name="bk_getitemsews"> </a></span></span>

## <a name="get-items-in-conversations-by-using-the-conversation-identifier-in-ews"></a><span data-ttu-id="a1a37-204">Obter itens em conversas usando o identificador de conversa no EWS</span><span class="sxs-lookup"><span data-stu-id="a1a37-204">Get items in conversations by using the conversation identifier in EWS</span></span>

<span data-ttu-id="a1a37-205">Você pode obter itens em uma conversa usando a operação [GetConversationItems](https://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) do EWS.</span><span class="sxs-lookup"><span data-stu-id="a1a37-205">You can get items in a conversation by using the [GetConversationItems](https://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="a1a37-206">Este exemplo fornece um conjunto de nós de conversa para a primeira conversa na caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="a1a37-206">This example provides a set of conversation nodes for the first conversation in the Inbox.</span></span> <span data-ttu-id="a1a37-207">O identificador de item, o assunto e o horário de recebimento de cada item são retornados na resposta, juntamente com as propriedades de índice de conversa pai e índice de conversa.</span><span class="sxs-lookup"><span data-stu-id="a1a37-207">The item identifier, subject, and received time for each item are returned in the response, along with the conversation index and parent conversation index properties.</span></span> <span data-ttu-id="a1a37-208">Você pode usar as propriedades do índice de conversa para reconstruir a hierarquia do nó.</span><span class="sxs-lookup"><span data-stu-id="a1a37-208">You can use the conversation index properties to reconstruct the node hierarchy.</span></span> 
  
<span data-ttu-id="a1a37-209">Neste exemplo, todos os itens de conversa nas pastas itens excluídos padrão e rascunhos são ignorados.</span><span class="sxs-lookup"><span data-stu-id="a1a37-209">In this example, all conversation items in the default Deleted Items and Drafts folders are ignored.</span></span>
  
<span data-ttu-id="a1a37-210">O elemento **Conversation** foi reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a1a37-210">The **ConversationId** element has been shortened for readability.</span></span> 
  
<span data-ttu-id="a1a37-211">Para obter itens de mais de uma conversa, inclua elementos de **conversa** adicionais.</span><span class="sxs-lookup"><span data-stu-id="a1a37-211">To get items from more than one conversation, include additional **Conversation** elements.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m=https://schemas.microsoft.com/exchange/services/2006/messages
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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
          <t:ConversationId Id="LUQFH6Q=" />
        </t:Conversation>
      </m:Conversations>
    </m:GetConversationItems>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **GetConversationItems** com uma mensagem [GetConversationItemsResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor de [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR** para indicar que a operação foi concluída com êxito. <span data-ttu-id="a1a37-213">A resposta também inclui o [ConversationNodes](https://msdn.microsoft.com/library/5c8a35b8-a940-4b3e-8768-9ba95766fd79%28Office.15%29.aspx) na conversa.</span><span class="sxs-lookup"><span data-stu-id="a1a37-213">The response also includes the [ConversationNodes](https://msdn.microsoft.com/library/5c8a35b8-a940-4b3e-8768-9ba95766fd79%28Office.15%29.aspx) in the conversation.</span></span> 
  
<span data-ttu-id="a1a37-214">Os elementos **ItemId**, **SyncState**e **conversable** foram reduzidos para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="a1a37-214">The **ItemId**, **SyncState**, and **ConversationId** elements have been shortened for readability.</span></span> 
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="873"
                         MinorBuildNumber="9"
                         Version="V2_9"
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
            <t:ConversationId Id="LUQFH6Q=" />
            <t:SyncState>AAAAYAm1</t:SyncState>
            <t:ConversationNodes>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;994051d7c1a346efbfce8dec2cbad509
                    @SN2SR01MB006.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;faa2b1df30074380abe3527b0cd18ca5
                    @SN2SR01MB001.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AYB1NAAA="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYCHq" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T13:15:00Z</t:DateTimeReceived>
                  </t:Message>
                </t:Items>
              </t:ConversationNode>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;faa2b1df30074380abe3527b0cd18ca5
                    @SN2SR01MB001.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;6a8e7658524b41cda7cdc3f23c1074a5
                    @SN2SR01MB001.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="lQAAAA=="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYAu8" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T10:02:08Z</t:DateTimeReceived>
                  </t:Message>
                </t:Items>
              </t:ConversationNode>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;bcdb185495834370a874a1e7ebedbb96
                    @SN2SR01MB005.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;e52a4de6b98d484887e141da094a2ce6
                    @SN2SR01MB006.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="igAAAA=="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYAuj" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T16:20:10Z</t:DateTimeReceived>
                  </t:Message>
                </t:Items>
              </t:ConversationNode>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;e52a4de6b98d484887e141da094a2ce6
                    @SN2SR01MB006.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;f0db3ead01db4fe087d98022149aa16f
                    @SN2SR01MB001.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="iwAAAA=="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYAul" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T15:30:10Z</t:DateTimeReceived>
                  </t:Message>
                </t:Items>
              </t:ConversationNode>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;f0db3ead01db4fe087d98022149aa16f
                    @SN2SR01MB001.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;88b1884ecaaa4f68b081c009d827e8c6
                    @SN2SR01MB003.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="jQAAAA=="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYAuq" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T14:20:10Z</t:DateTimeReceived>
                  </t:Message>
                </t:Items>
              </t:ConversationNode>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;88b1884ecaaa4f68b081c009d827e8c6
                    @SN2SR01MB003.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;faa2b1df30074380abe3527b0cd18ca5
                    @SN2SR01MB001.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="kAAAAA=="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYAux" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T12:52:09Z</t:DateTimeReceived>
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

<span data-ttu-id="a1a37-215"><a name="bk_versiondiffs"> </a></span><span class="sxs-lookup"><span data-stu-id="a1a37-215"><a name="bk_versiondiffs"> </a></span></span>

## <a name="version-differences"></a><span data-ttu-id="a1a37-216">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="a1a37-216">Version differences</span></span>

<span data-ttu-id="a1a37-217">Quando você estiver usando o Exchange Server 2010 Service Pack 1 (SP1), o método [FindConversation](https://msdn.microsoft.com/library/office/jj220668%28v=exchg.80%29.aspx) terá menos opções disponíveis e a operação [FindConversation](https://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) terá menos elementos na solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1a37-217">When you are using Exchange Server 2010 Service Pack 1 (SP1), the [FindConversation](https://msdn.microsoft.com/library/office/jj220668%28v=exchg.80%29.aspx) method has fewer options available, and the [FindConversation](https://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) operation has fewer elements in the request.</span></span> 
  
<span data-ttu-id="a1a37-218">**Tabela 3. Suporte para o Exchange 2010 SP1 versão para FindConversation**</span><span class="sxs-lookup"><span data-stu-id="a1a37-218">**Table 3. Exchange 2010 SP1 version support for FindConversation**</span></span>

|<span data-ttu-id="a1a37-219">**Método de API gerenciada do EWS**</span><span class="sxs-lookup"><span data-stu-id="a1a37-219">**EWS Managed API method**</span></span>|<span data-ttu-id="a1a37-220">**Elementos do EWS**</span><span class="sxs-lookup"><span data-stu-id="a1a37-220">**EWS elements**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1a37-221">FindConversation (ViewBase, FolderId)</span><span class="sxs-lookup"><span data-stu-id="a1a37-221">FindConversation (ViewBase, FolderId)</span></span>](https://msdn.microsoft.com/library/office/jj220668%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="a1a37-222">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="a1a37-222">IndexedPageItemView</span></span>](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) <br/> [<span data-ttu-id="a1a37-223">SortOrder</span><span class="sxs-lookup"><span data-stu-id="a1a37-223">SortOrder</span></span>](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) <br/> [<span data-ttu-id="a1a37-224">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="a1a37-224">ParentFolderId</span></span>](https://msdn.microsoft.com/library/0e3e6e5f-06d0-499b-8ca4-d36036521658%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="a1a37-225">O método da API gerenciada do EWS do [GetConversationItems](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) e a operação do EWS do [GetConversationItems](https://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) foram introduzidos no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a1a37-225">The [GetConversationItems](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) EWS Managed API method and the [GetConversationItems](https://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) EWS operation were introduced in Exchange Server 2013.</span></span> <span data-ttu-id="a1a37-226">Os aplicativos que direcionam versões anteriores do Exchange só podem aplicar ações de conversa a conversas, conforme listado na tabela 2.</span><span class="sxs-lookup"><span data-stu-id="a1a37-226">Applications that target earlier versions of Exchange can only apply conversation actions to conversations, as listed in Table 2.</span></span> 
  
<span data-ttu-id="a1a37-227">O método de API gerenciada do EWS do **FindConversation** e o método EWS **FindConversation** não estão disponíveis na versão inicial do Exchange 2010 ou no Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="a1a37-227">The **FindConversation** EWS Managed API method and the **FindConversation** EWS method are not available in the initial release version of Exchange 2010 or in Exchange 2007.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="a1a37-228">Também consulte</span><span class="sxs-lookup"><span data-stu-id="a1a37-228">See also</span></span>

- [<span data-ttu-id="a1a37-229">Email e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a1a37-229">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
- [<span data-ttu-id="a1a37-230">Usar filtros de pesquisa com o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a1a37-230">Use search filters with EWS in Exchange</span></span>](how-to-use-search-filters-with-ews-in-exchange.md)   
- [<span data-ttu-id="a1a37-231">Exchange 2013: localizar conversas em caixas de correio de forma programática</span><span class="sxs-lookup"><span data-stu-id="a1a37-231">Exchange 2013: Find conversations in mailboxes programmatically</span></span>](https://code.msdn.microsoft.com/exchange/Exchange-2013-Find-d4b6b3af)    
- [<span data-ttu-id="a1a37-232">Exchange 2013: aplicar ações para gerenciar conversas em uma caixa de correio</span><span class="sxs-lookup"><span data-stu-id="a1a37-232">Exchange 2013: Apply actions to manage conversations in a mailbox</span></span>](https://code.msdn.microsoft.com/exchange/Exchange-2013-Apply-accde0b5)
    

