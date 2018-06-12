---
title: Trabalhar com conversas usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7750528c-acb2-43e5-a1e1-ee201c0e1730
description: Saiba mais sobre como localizar conversas, aplicar ações a conversas e obter itens em conversas usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: 71ef7674086607e1544111071928f3dd74073a77
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750853"
---
# <a name="work-with-conversations-by-using-ews-in-exchange"></a><span data-ttu-id="8365f-103">Trabalhar com conversas usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8365f-103">Work with conversations by using EWS in Exchange</span></span>

<span data-ttu-id="8365f-104">Saiba mais sobre como localizar conversas, aplicar ações a conversas e obter itens em conversas usando a API gerenciada de EWS ou EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="8365f-104">Learn about how to find conversations, apply actions to conversations, and get items in conversations by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="8365f-105">No contexto do Exchange, conversas são uma forma de grupo e gerenciar um conjunto relacionado de mensagens de email.</span><span class="sxs-lookup"><span data-stu-id="8365f-105">In the context of Exchange, conversations are a way to group and manage a related set of email messages.</span></span> <span data-ttu-id="8365f-106">Eles também podem fornecer uma maneira de exibir mensagens relacionadas.</span><span class="sxs-lookup"><span data-stu-id="8365f-106">They can also provide a way to view related messages.</span></span> <span data-ttu-id="8365f-107">Exchange define as conversas de acordo com o valor de **ID de mensagem** da primeira mensagem de email em um segmento.</span><span class="sxs-lookup"><span data-stu-id="8365f-107">Exchange defines conversations based on the **Message-ID** value of the first email message in a thread.</span></span> <span data-ttu-id="8365f-108">Cabeçalho de **Message-ID** da mensagem original em suas **referências** de referência de todas as respostas e mensagens relacionadas e **In-responder para** cabeçalhos.</span><span class="sxs-lookup"><span data-stu-id="8365f-108">All replies and related messages reference the original message's **Message-ID** header in their **References** and **In-Reply-To** headers.</span></span> 
  
<span data-ttu-id="8365f-109">Além disso, dentro do envelope SOAP, para cada mensagem recebida em uma caixa de correio Exchange define elementos e propriedades específicas.</span><span class="sxs-lookup"><span data-stu-id="8365f-109">Additionally, inside the SOAP envelope, for each message received in a mailbox, Exchange sets specific properties and elements.</span></span>
  
<span data-ttu-id="8365f-110">**Tabela 1. Propriedades de conversa e elementos definir em todas as mensagens de email**</span><span class="sxs-lookup"><span data-stu-id="8365f-110">**Table 1. Conversation properties and elements set on all email messages**</span></span>

|<span data-ttu-id="8365f-111">**Propriedade API gerenciada de EWS**</span><span class="sxs-lookup"><span data-stu-id="8365f-111">**EWS Managed API property**</span></span>|<span data-ttu-id="8365f-112">**Elemento EWS**</span><span class="sxs-lookup"><span data-stu-id="8365f-112">**EWS element**</span></span>|<span data-ttu-id="8365f-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8365f-113">**Description**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="8365f-114">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="8365f-114">ConversationTopic</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.conversationtopic%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8365f-115">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="8365f-115">ConversationTopic</span></span>](http://msdn.microsoft.com/library/46cacf42-4039-4c8a-9b20-c42cdd9f2760%28Office.15%29.aspx) <br/> |<span data-ttu-id="8365f-116">Contém um formulário normalizado do valor entidade que foi definido para a mensagem original.</span><span class="sxs-lookup"><span data-stu-id="8365f-116">Contains a normalized form of the subject value that was set on the original message.</span></span> <span data-ttu-id="8365f-117">Isso é o mesmo que o cabeçalho da mensagem de **Thread-tópico** .</span><span class="sxs-lookup"><span data-stu-id="8365f-117">This is the same as the **Thread-Topic** message header.</span></span> <span data-ttu-id="8365f-118">Esse valor é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8365f-118">This value is read-only.</span></span>  <br/> |
|[<span data-ttu-id="8365f-119">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="8365f-119">ConversationIndex</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.conversationindex%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8365f-120">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="8365f-120">ConversationIndex</span></span>](http://msdn.microsoft.com/library/fdf47e22-8d93-4ae4-883b-0c9f07f48724%28Office.15%29.aspx) <br/> |<span data-ttu-id="8365f-121">Representa a posição do item da conversa.</span><span class="sxs-lookup"><span data-stu-id="8365f-121">Represents the position of the item in the conversation.</span></span> <span data-ttu-id="8365f-122">Isso é o mesmo que o cabeçalho da mensagem de **Índice de segmento** .</span><span class="sxs-lookup"><span data-stu-id="8365f-122">This is the same as the **Thread-Index** message header.</span></span> <span data-ttu-id="8365f-123">Esse valor é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8365f-123">This value is read-only.</span></span>  <br/> |
   
<span data-ttu-id="8365f-124">Exchange aplica o mesmo valor **ConversationTopic** às respostas à primeira mensagem e, em seguida, atualiza o valor de **ConversationIndex** para representar a posição da mensagem em relação à mensagem original.</span><span class="sxs-lookup"><span data-stu-id="8365f-124">Exchange applies the same **ConversationTopic** value to replies to the first message and then updates the **ConversationIndex** value to represent the message's position relative to the original message.</span></span> <span data-ttu-id="8365f-125">Se o assunto do thread email for alterado, o Exchange aplica um novo valor **ConversationTopic** e novos valores **ConversationIndex** para a nova conversa.</span><span class="sxs-lookup"><span data-stu-id="8365f-125">If the subject of the email thread changes, Exchange applies a new **ConversationTopic** value and new **ConversationIndex** values to the new conversation.</span></span> 
  
<span data-ttu-id="8365f-126">**Tabela 2. Operações de EWS para trabalhar com conversas e métodos de API gerenciada de EWS**</span><span class="sxs-lookup"><span data-stu-id="8365f-126">**Table 2. EWS Managed API methods and EWS operations for working with conversations**</span></span>

|<span data-ttu-id="8365f-127">**Para...**</span><span class="sxs-lookup"><span data-stu-id="8365f-127">**In order to…**</span></span>|<span data-ttu-id="8365f-128">**Use este método de API gerenciada de EWS ou os métodos**</span><span class="sxs-lookup"><span data-stu-id="8365f-128">**Use this EWS Managed API method or methods**</span></span>|<span data-ttu-id="8365f-129">**Use esta operação EWS**</span><span class="sxs-lookup"><span data-stu-id="8365f-129">**Use this EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="8365f-130">Localizar conversas</span><span class="sxs-lookup"><span data-stu-id="8365f-130">Find conversations</span></span>  <br/> |[<span data-ttu-id="8365f-131">ExchangeService.FindConversation</span><span class="sxs-lookup"><span data-stu-id="8365f-131">ExchangeService.FindConversation</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findconversation%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8365f-132">FindConversation</span><span class="sxs-lookup"><span data-stu-id="8365f-132">FindConversation</span></span>](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="8365f-133">Aplicar ações de conversa</span><span class="sxs-lookup"><span data-stu-id="8365f-133">Apply conversation actions</span></span>  <br/> |[<span data-ttu-id="8365f-134">Conversation.EnableAlwaysCategorizeItems</span><span class="sxs-lookup"><span data-stu-id="8365f-134">Conversation.EnableAlwaysCategorizeItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.conversation.enablealwayscategorizeitems%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="8365f-135">Conversation.EnableAlwaysDeleteItems</span><span class="sxs-lookup"><span data-stu-id="8365f-135">Conversation.EnableAlwaysDeleteItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.conversation.enablealwaysdeleteitems%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="8365f-136">Conversation.EnableAlwaysMoveItems</span><span class="sxs-lookup"><span data-stu-id="8365f-136">Conversation.EnableAlwaysMoveItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.conversation.enablealwaysmoveitems%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="8365f-137">ExchangeService.CopyItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="8365f-137">ExchangeService.CopyItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.copyitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="8365f-138">ExchangeService.DeleteItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="8365f-138">ExchangeService.DeleteItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.deleteitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="8365f-139">ExchangeService.DisableAlwaysCategorizeItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="8365f-139">ExchangeService.DisableAlwaysCategorizeItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.disablealwayscategorizeitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="8365f-140">ExchangeService.DisableAlwaysDeleteItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="8365f-140">ExchangeService.DisableAlwaysDeleteItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.disablealwaysdeleteitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="8365f-141">ExchangeService.DisableAlwaysMoveItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="8365f-141">ExchangeService.DisableAlwaysMoveItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.disablealwaysmoveitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="8365f-142">ExchangeService.EnableAlwaysCategorizeItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="8365f-142">ExchangeService.EnableAlwaysCategorizeItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.enablealwayscategorizeitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="8365f-143">ExchangeService.EnableAlwaysDeleteItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="8365f-143">ExchangeService.EnableAlwaysDeleteItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.enablealwaysdeleteitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="8365f-144">ExchangeService.EnableAlwaysMoveItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="8365f-144">ExchangeService.EnableAlwaysMoveItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.enablealwaysmoveitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="8365f-145">ExchangeService.MoveItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="8365f-145">ExchangeService.MoveItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.moveitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="8365f-146">ExchangeService.SetFlagStatusForItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="8365f-146">ExchangeService.SetFlagStatusForItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.setflagstatusforitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="8365f-147">ExchangeService.SetReadStateForItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="8365f-147">ExchangeService.SetReadStateForItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.setreadstateforitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="8365f-148">ExchangeService.SetRetentionPolicyForItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="8365f-148">ExchangeService.SetRetentionPolicyForItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.setretentionpolicyforitemsinconversations%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8365f-149">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="8365f-149">ApplyConversationAction</span></span>](http://msdn.microsoft.com/library/73d7943d-d361-4f8b-9948-d85f886efa1a%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="8365f-150">Obter itens em conversas de uma ou mais</span><span class="sxs-lookup"><span data-stu-id="8365f-150">Get items in one or more conversations</span></span>  <br/> |[<span data-ttu-id="8365f-151">ExchangeService.GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="8365f-151">ExchangeService.GetConversationItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8365f-152">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="8365f-152">GetConversationItems</span></span>](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) <br/> |

<span data-ttu-id="8365f-153"><a name="bk_findewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="8365f-153"></span></span>

## <a name="find-a-conversation-by-using-the-ews-managed-api"></a><span data-ttu-id="8365f-154">Localizar uma conversa usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="8365f-154">Find a conversation by using the EWS Managed API</span></span>

<span data-ttu-id="8365f-155">Você pode encontrar conversas usando o método [ExchangeService.FindConversation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findconversation%28v=exchg.80%29.aspx) EWS Managed API, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="8365f-155">You can find conversations by using the [ExchangeService.FindConversation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findconversation%28v=exchg.80%29.aspx) EWS Managed API method, as shown in the following example.</span></span> <span data-ttu-id="8365f-156">Este exemplo obtém as 10 primeiros conversas na pasta caixa de entrada que têm um assunto que contém a palavra "notícias".</span><span class="sxs-lookup"><span data-stu-id="8365f-156">This example gets the first 10 conversations in the Inbox folder that have a subject that contains the word "news".</span></span> <span data-ttu-id="8365f-157">O exemplo grava o tópico de conversação, último horário de entrega e lista de destinatários exclusiva global para a janela do console.</span><span class="sxs-lookup"><span data-stu-id="8365f-157">The example then writes the conversation topic, last delivery time, and global unique recipient list to the console window.</span></span> 
  
<span data-ttu-id="8365f-158">Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="8365f-158">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

<span data-ttu-id="8365f-159"><a name="bk_findews"> </a></span><span class="sxs-lookup"><span data-stu-id="8365f-159"></span></span>

## <a name="find-a-conversation-by-using-ews"></a><span data-ttu-id="8365f-160">Localizar uma conversa usando o EWS</span><span class="sxs-lookup"><span data-stu-id="8365f-160">Find a conversation by using EWS</span></span>

<span data-ttu-id="8365f-161">Você pode encontrar conversas usando a operação [FindConversation](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) EWS, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="8365f-161">You can find conversations by using the [FindConversation](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) EWS operation, as shown in the following example.</span></span> <span data-ttu-id="8365f-162">Este exemplo obtém as dez primeiros conversas na pasta caixa de entrada que têm um assunto que contém a palavra "notícias".</span><span class="sxs-lookup"><span data-stu-id="8365f-162">This example gets the first ten conversations in the Inbox folder that have a subject that contains the word "news".</span></span> <span data-ttu-id="8365f-163">Isso também é a solicitação XML que o EWS Managed API envia quando você usar a API gerenciada de EWS para [Localizar uma conversa](#bk_findewsma).</span><span class="sxs-lookup"><span data-stu-id="8365f-163">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [find a conversation](#bk_findewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="8365f-164">O servidor responde à solicitação **FindConversation** com uma mensagem de [FindConversationResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError** para indicar que a operação foi concluída com êxito.</span><span class="sxs-lookup"><span data-stu-id="8365f-164">The server responds to the **FindConversation** request with a [FindConversationResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** to indicate that the operation completed successfully.</span></span> <span data-ttu-id="8365f-165">A resposta também inclui a conversa somente na caixa de correio que tenha um assunto que contém a palavra "notícias".</span><span class="sxs-lookup"><span data-stu-id="8365f-165">The response also includes the only conversation in the mailbox that has a subject that contains the word "news".</span></span> 
  
<span data-ttu-id="8365f-166">Os elementos **ItemId** **ChangeKey**e **ConversationId** foram diminuídos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8365f-166">The **ItemId**, **ChangeKey**, and **ConversationId** elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="883"
                         MinorBuildNumber="10"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <FindConversationResponse ResponseClass="Success"
                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Conversations>
        <Conversation xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="8365f-167"><a name="bk_applyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="8365f-167"></span></span>

## <a name="apply-conversation-actions-by-using-the-ews-managed-api"></a><span data-ttu-id="8365f-168">Aplicar ações de conversa usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="8365f-168">Apply conversation actions by using the EWS Managed API</span></span>

<span data-ttu-id="8365f-169">Você pode aplicar ações de conversação para uma conversa usando vários métodos de API gerenciada de EWS, conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="8365f-169">You can apply conversation actions to a conversation by using a number of EWS Managed API methods, as shown in the following example.</span></span> <span data-ttu-id="8365f-170">Este exemplo adiciona categorias a itens existentes em uma conversa e aplica as mesmas categorias a itens futuros da conversa.</span><span class="sxs-lookup"><span data-stu-id="8365f-170">This example adds categories to existing items in a conversation and applies the same categories to future items in the conversation.</span></span> <span data-ttu-id="8365f-171">Ele também mostra como habilitar a movimentação automática de itens na conversa para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="8365f-171">It also shows how to enable the automatic moving of items in the conversation to a folder.</span></span> <span data-ttu-id="8365f-172">Neste exemplo, os itens são movidas para a pasta Rascunhos.</span><span class="sxs-lookup"><span data-stu-id="8365f-172">In this example, items are moved to the Drafts folder.</span></span>
  
<span data-ttu-id="8365f-173">Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="8365f-173">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
<span data-ttu-id="8365f-174">Para obter uma lista completa dos métodos que se aplicam as ações de conversa, consulte a tabela 2.</span><span class="sxs-lookup"><span data-stu-id="8365f-174">For a complete list of methods that apply conversation actions, see Table 2.</span></span>
  
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

<span data-ttu-id="8365f-175"><a name="bk_applyews"> </a></span><span class="sxs-lookup"><span data-stu-id="8365f-175"></span></span>

## <a name="apply-conversation-actions-by-using-ews"></a><span data-ttu-id="8365f-176">Aplicar ações de conversa usando o EWS</span><span class="sxs-lookup"><span data-stu-id="8365f-176">Apply conversation actions by using EWS</span></span>

<span data-ttu-id="8365f-177">Você pode aplicar ações de conversa, tais como categorizar, excluir e mover, usando a operação [ApplyConversationAction](http://msdn.microsoft.com/library/73d7943d-d361-4f8b-9948-d85f886efa1a%28Office.15%29.aspx) , conforme mostrado no exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="8365f-177">You can apply conversation actions, such as categorize, delete, and move, by using the [ApplyConversationAction](http://msdn.microsoft.com/library/73d7943d-d361-4f8b-9948-d85f886efa1a%28Office.15%29.aspx) operation, as shown in the following example.</span></span> <span data-ttu-id="8365f-178">Este exemplo adiciona categorias a itens existentes em uma conversa e aplica as mesmas categorias a itens futuros da conversa.</span><span class="sxs-lookup"><span data-stu-id="8365f-178">This example adds categories to existing items in a conversation and applies the same categories to future items in the conversation.</span></span> <span data-ttu-id="8365f-179">Ele também mostra como habilitar a movimentação automática de itens na conversa para uma pasta; Neste exemplo, os itens são movidas para a pasta Rascunhos.</span><span class="sxs-lookup"><span data-stu-id="8365f-179">It also shows how to enable the automatic moving of items in the conversation to a folder; in this example, items are moved to the Drafts folder.</span></span> <span data-ttu-id="8365f-180">Isso também é a solicitação XML que o EWS Managed API envia quando você usar a API gerenciada de EWS para [Aplicar ações de conversa](#bk_applyewsma).</span><span class="sxs-lookup"><span data-stu-id="8365f-180">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [apply conversation actions](#bk_applyewsma).</span></span>
  
<span data-ttu-id="8365f-181">O elemento **ConversationId** foi reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8365f-181">The **ConversationId** element has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="8365f-182">O servidor responde à solicitação **ApplyConversationAction** com uma mensagem de [ApplyConversationActionResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError** para indicar que a operação foi concluída com êxito.</span><span class="sxs-lookup"><span data-stu-id="8365f-182">The server responds to the **ApplyConversationAction** request with a [ApplyConversationActionResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** to indicate that the operation completed successfully.</span></span> 

<span data-ttu-id="8365f-183"><a name="bk_getitemssingleewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="8365f-183"></span></span>

## <a name="get-items-in-a-single-conversation-by-using-the-conversation-identifier-in-the-ews-managed-api"></a><span data-ttu-id="8365f-184">Obter itens em uma única conversa usando o identificador de conversa na API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="8365f-184">Get items in a single conversation by using the conversation identifier in the EWS Managed API</span></span>

<span data-ttu-id="8365f-185">Você pode obter itens em uma conversa usando o método de API gerenciada de EWS [ExchangeService.GetConversationItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8365f-185">You can get items in a conversation by using the [ExchangeService.GetConversationItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) EWS Managed API method.</span></span> <span data-ttu-id="8365f-186">Este exemplo fornece o conjunto de nós de conversa para a conversa primeira na caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="8365f-186">This example provides the set of conversation nodes for the first conversation in the Inbox.</span></span> <span data-ttu-id="8365f-187">O identificador do item, o assunto e a hora de recebimento para cada item são retornados na resposta, junto com as propriedades conversa índice e parent conversa índice.</span><span class="sxs-lookup"><span data-stu-id="8365f-187">The item identifier, subject, and received time for each item are returned in the response, along with the conversation index and parent conversation index properties.</span></span> <span data-ttu-id="8365f-188">Você pode usar as propriedades do índice de conversação para reconstruir a hierarquia do nó.</span><span class="sxs-lookup"><span data-stu-id="8365f-188">You can use the conversation index properties to reconstruct the node hierarchy.</span></span> 
  
<span data-ttu-id="8365f-189">Neste exemplo, todos os itens de conversa nas pastas padrão itens excluídos e rascunhos são ignorados.</span><span class="sxs-lookup"><span data-stu-id="8365f-189">In this example, all conversation items in the default Deleted Items and Drafts folders are ignored.</span></span>
  
<span data-ttu-id="8365f-190">Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="8365f-190">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

<span data-ttu-id="8365f-191">Recomendamos que você armazena em cache a propriedade de **estado de sincronização** para solicitações subsequentes obter itens na conversa.</span><span class="sxs-lookup"><span data-stu-id="8365f-191">We recommend that you cache the **SyncState** property for subsequent requests to get items in the conversation.</span></span> 

<span data-ttu-id="8365f-192"><a name="bk_getitemsmanyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="8365f-192"></span></span>

## <a name="get-items-in-many-conversations-by-using-the-conversationrequest-object-in-the-ews-managed-api"></a><span data-ttu-id="8365f-193">Obter itens em várias conversas usando o objeto ConversationRequest na API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="8365f-193">Get items in many conversations by using the ConversationRequest object in the EWS Managed API</span></span>

<span data-ttu-id="8365f-194">Você pode usar o objeto [ConversationRequest](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.conversationrequest%28v=exchg.80%29.aspx) e o método de API gerenciada de EWS [ExchangeService.GetConversationItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) para obter itens em conversas por dois ou mais.</span><span class="sxs-lookup"><span data-stu-id="8365f-194">You can use the [ConversationRequest](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.conversationrequest%28v=exchg.80%29.aspx) object and the [ExchangeService.GetConversationItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) EWS Managed API method to get items from two or more conversations.</span></span> <span data-ttu-id="8365f-195">Este exemplo fornece um conjunto de nós de conversa para as duas primeiras conversas na caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="8365f-195">This example provides a set of conversation nodes for the first two conversations in the Inbox.</span></span> <span data-ttu-id="8365f-196">O identificador do item, assunto e a hora de recebimento de cada item serão retornados na resposta, junto com as propriedades conversa índice e parent conversa índice.</span><span class="sxs-lookup"><span data-stu-id="8365f-196">The item identifier, subject, and the received time for each item will be returned in the response, along with the conversation index and parent conversation index properties.</span></span> <span data-ttu-id="8365f-197">Você pode usar as propriedades do índice de conversação para reconstruir a hierarquia do nó.</span><span class="sxs-lookup"><span data-stu-id="8365f-197">You can use the conversation index properties to reconstruct the node hierarchy.</span></span> <span data-ttu-id="8365f-198">Este exemplo presume que os primeiros dois itens na caixa de entrada estão em conversas diferentes.</span><span class="sxs-lookup"><span data-stu-id="8365f-198">This example assumes that the first two items in the Inbox are from different conversations.</span></span> 
  
<span data-ttu-id="8365f-199">Neste exemplo, todos os itens de conversa nas pastas padrão itens excluídos e rascunhos são ignorados.</span><span class="sxs-lookup"><span data-stu-id="8365f-199">In this example, all conversation items in the default Deleted Items and Drafts folders are ignored.</span></span>
  
<span data-ttu-id="8365f-200">Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="8365f-200">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

<span data-ttu-id="8365f-201">Como prática recomendada, recomendamos que você retorne apenas as propriedades que requer que o aplicativo cliente, em vez de usar a opção **FirstClassProperties** para a classe **BasePropertySet** .</span><span class="sxs-lookup"><span data-stu-id="8365f-201">As a best practice, we recommend that you return only the properties that the client application requires, rather than using the **FirstClassProperties** option for the **BasePropertySet** class.</span></span> <span data-ttu-id="8365f-202">Recomendamos que você armazena em cache a propriedade de **estado de sincronização** para solicitações subsequentes obter itens na conversa.</span><span class="sxs-lookup"><span data-stu-id="8365f-202">We recommend that you cache the **SyncState** property for subsequent requests to get items in the conversation.</span></span> 

<span data-ttu-id="8365f-203"><a name="bk_getitemsews"> </a></span><span class="sxs-lookup"><span data-stu-id="8365f-203"></span></span>

## <a name="get-items-in-conversations-by-using-the-conversation-identifier-in-ews"></a><span data-ttu-id="8365f-204">Obter itens em conversas usando o identificador de conversação no EWS</span><span class="sxs-lookup"><span data-stu-id="8365f-204">Get items in conversations by using the conversation identifier in EWS</span></span>

<span data-ttu-id="8365f-205">Você pode obter itens em uma conversa usando a operação de EWS [GetConversationItems](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8365f-205">You can get items in a conversation by using the [GetConversationItems](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="8365f-206">Este exemplo fornece um conjunto de nós de conversa para a conversa primeira na caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="8365f-206">This example provides a set of conversation nodes for the first conversation in the Inbox.</span></span> <span data-ttu-id="8365f-207">O identificador do item, o assunto e a hora de recebimento para cada item são retornados na resposta, junto com as propriedades conversa índice e parent conversa índice.</span><span class="sxs-lookup"><span data-stu-id="8365f-207">The item identifier, subject, and received time for each item are returned in the response, along with the conversation index and parent conversation index properties.</span></span> <span data-ttu-id="8365f-208">Você pode usar as propriedades do índice de conversação para reconstruir a hierarquia do nó.</span><span class="sxs-lookup"><span data-stu-id="8365f-208">You can use the conversation index properties to reconstruct the node hierarchy.</span></span> 
  
<span data-ttu-id="8365f-209">Neste exemplo, todos os itens de conversa nas pastas padrão itens excluídos e rascunhos são ignorados.</span><span class="sxs-lookup"><span data-stu-id="8365f-209">In this example, all conversation items in the default Deleted Items and Drafts folders are ignored.</span></span>
  
<span data-ttu-id="8365f-210">O elemento **ConversationId** foi reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8365f-210">The **ConversationId** element has been shortened for readability.</span></span> 
  
<span data-ttu-id="8365f-211">Para obter itens da conversa mais de um, inclua elementos adicionais de **conversa** .</span><span class="sxs-lookup"><span data-stu-id="8365f-211">To get items from more than one conversation, include additional **Conversation** elements.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m=http://schemas.microsoft.com/exchange/services/2006/messages
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
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
          <t:ConversationId Id="LUQFH6Q=" />
        </t:Conversation>
      </m:Conversations>
    </m:GetConversationItems>
  </soap:Body>
</soap:Envelope>
```

O servidor responde à solicitação **GetConversationItems** com uma mensagem de [GetConversationItemsResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NoError** para indicar que a operação foi concluída com êxito. <span data-ttu-id="8365f-213">A resposta também inclui o [ConversationNodes](http://msdn.microsoft.com/library/5c8a35b8-a940-4b3e-8768-9ba95766fd79%28Office.15%29.aspx) na conversa.</span><span class="sxs-lookup"><span data-stu-id="8365f-213">The response also includes the [ConversationNodes](http://msdn.microsoft.com/library/5c8a35b8-a940-4b3e-8768-9ba95766fd79%28Office.15%29.aspx) in the conversation.</span></span> 
  
<span data-ttu-id="8365f-214">Os elementos **ItemId**, **estado de sincronização**e **ConversationId** foram diminuídos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8365f-214">The **ItemId**, **SyncState**, and **ConversationId** elements have been shortened for readability.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="873"
                         MinorBuildNumber="9"
                         Version="V2_9"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetConversationItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="8365f-215"><a name="bk_versiondiffs"> </a></span><span class="sxs-lookup"><span data-stu-id="8365f-215"></span></span>

## <a name="version-differences"></a><span data-ttu-id="8365f-216">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="8365f-216">Version differences</span></span>

<span data-ttu-id="8365f-217">Quando você estiver usando o Exchange Server 2010 Service Pack 1 (SP1), o método [FindConversation](http://msdn.microsoft.com/en-us/library/office/jj220668%28v=exchg.80%29.aspx) tem menos opções disponíveis e a operação [FindConversation](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) tem menos de elementos na solicitação.</span><span class="sxs-lookup"><span data-stu-id="8365f-217">When you are using Exchange Server 2010 Service Pack 1 (SP1), the [FindConversation](http://msdn.microsoft.com/en-us/library/office/jj220668%28v=exchg.80%29.aspx) method has fewer options available, and the [FindConversation](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) operation has fewer elements in the request.</span></span> 
  
<span data-ttu-id="8365f-218">**Tabela 3. Suporte de versão do Exchange 2010 SP1 para FindConversation**</span><span class="sxs-lookup"><span data-stu-id="8365f-218">**Table 3. Exchange 2010 SP1 version support for FindConversation**</span></span>

|<span data-ttu-id="8365f-219">**Método API gerenciada de EWS**</span><span class="sxs-lookup"><span data-stu-id="8365f-219">**EWS Managed API method**</span></span>|<span data-ttu-id="8365f-220">**Elementos EWS**</span><span class="sxs-lookup"><span data-stu-id="8365f-220">**EWS elements**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8365f-221">FindConversation (ViewBase, FolderId)</span><span class="sxs-lookup"><span data-stu-id="8365f-221">FindConversation (ViewBase, FolderId)</span></span>](http://msdn.microsoft.com/en-us/library/office/jj220668%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="8365f-222">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="8365f-222">IndexedPageItemView</span></span>](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) <br/> [<span data-ttu-id="8365f-223">SortOrder</span><span class="sxs-lookup"><span data-stu-id="8365f-223">SortOrder</span></span>](http://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) <br/> [<span data-ttu-id="8365f-224">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="8365f-224">ParentFolderId</span></span>](http://msdn.microsoft.com/library/0e3e6e5f-06d0-499b-8ca4-d36036521658%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="8365f-225">O método de API gerenciada de EWS [GetConversationItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) e a operação de EWS [GetConversationItems](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) foram introduzidos no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8365f-225">The [GetConversationItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) EWS Managed API method and the [GetConversationItems](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) EWS operation were introduced in Exchange Server 2013.</span></span> <span data-ttu-id="8365f-226">Aplicativos que têm como alvo de versões anteriores do Exchange só podem aplicar ações de conversa para conversas, conforme listado na tabela 2.</span><span class="sxs-lookup"><span data-stu-id="8365f-226">Applications that target earlier versions of Exchange can only apply conversation actions to conversations, as listed in Table 2.</span></span> 
  
<span data-ttu-id="8365f-227">O método **FindConversation** EWS Managed API e o método EWS **FindConversation** não estão disponíveis na versão inicial do Exchange 2010 ou no Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="8365f-227">The **FindConversation** EWS Managed API method and the **FindConversation** EWS method are not available in the initial release version of Exchange 2010 or in Exchange 2007.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="8365f-228">Confira também</span><span class="sxs-lookup"><span data-stu-id="8365f-228">See also</span></span>

- [<span data-ttu-id="8365f-229">Email e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8365f-229">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
- [<span data-ttu-id="8365f-230">Use os filtros de pesquisa com o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8365f-230">Use search filters with EWS in Exchange</span></span>](how-to-use-search-filters-with-ews-in-exchange.md)   
- [<span data-ttu-id="8365f-231">Exchange 2013: Localizar conversas em caixas de correio programaticamente</span><span class="sxs-lookup"><span data-stu-id="8365f-231">Exchange 2013: Find conversations in mailboxes programmatically</span></span>](http://code.msdn.microsoft.com/exchange/Exchange-2013-Find-d4b6b3af)    
- [<span data-ttu-id="8365f-232">Exchange 2013: Aplicar ações para gerenciar conversas em uma caixa de correio</span><span class="sxs-lookup"><span data-stu-id="8365f-232">Exchange 2013: Apply actions to manage conversations in a mailbox</span></span>](http://code.msdn.microsoft.com/exchange/Exchange-2013-Apply-accde0b5)
    

