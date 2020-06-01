---
title: Receber notificações sobre eventos de caixa de correio usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: eb25cbd1-2244-4c3f-a71a-5ee20f81c41f
description: Descubra como usar a API gerenciada do EWS ou o EWS para se inscrever em notificações de recebimento e obter eventos.
ms.openlocfilehash: 3d77c0d4efb8fc853eea64ff2429af5c3dbead27
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456718"
---
# <a name="pull-notifications-about-mailbox-events-by-using-ews-in-exchange"></a><span data-ttu-id="9a798-103">Receber notificações sobre eventos de caixa de correio usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9a798-103">Pull notifications about mailbox events by using EWS in Exchange</span></span>

<span data-ttu-id="9a798-104">Descubra como usar a API gerenciada do EWS ou o EWS para se inscrever em notificações de recebimento e obter eventos.</span><span class="sxs-lookup"><span data-stu-id="9a798-104">Find out how to use the EWS Managed API or EWS to subscribe to pull notifications and get events.</span></span>
  
<span data-ttu-id="9a798-105">O EWS no Exchange usa notificações de recebimento para permitir que clientes solicitem (ou recebam) notificações sobre alterações na caixa de correio do servidor para o cliente.</span><span class="sxs-lookup"><span data-stu-id="9a798-105">EWS in Exchange uses pull notifications to enable clients to request (or pull) notifications about changes to the mailbox from the server to the client.</span></span>
  
<span data-ttu-id="9a798-106">Se você estiver assinando notificações de recepção usando a API gerenciada do EWS, [assine e receba notificações de recebimento](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullewsma) usando o método [SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="9a798-106">If you're subscribing to pull notifications by using the EWS Managed API, you [subscribe to and get pull notifications](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullewsma) by using the [SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="9a798-107">Em seguida, você obtém eventos do servidor usando o método [GetEvents](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="9a798-107">You then get events from the server by using the [GetEvents](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="9a798-108">Para se inscrever em notificações de recebimento usando o EWS, você [cria uma assinatura](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullews) usando a [operação Subscribe](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx), analisa a resposta e, em seguida, [Obtém as notificações](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_getpull) usando a [operação GetEvents](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="9a798-108">To subscribe to pull notifications by using EWS, you [create a subscription](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullews) by using the [Subscribe operation](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx), parse the response, and then [get the notifications](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_getpull) by using the [GetEvents operation](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx).</span></span>
  
<span data-ttu-id="9a798-109">Depois que o cliente recebe notificações de itens que são alterados ou criados no servidor, ele pode [sincronizar as alterações](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="9a798-109">After the client receives notifications of items that are changed or created on the server, it can then [synchronize the changes](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).</span></span>
  
## <a name="subscribe-to-and-get-pull-notifications-by-using-the-ews-managed-api"></a><span data-ttu-id="9a798-110">Inscrever-se e obter notificações de recebimento usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="9a798-110">Subscribe to and get pull notifications by using the EWS Managed API</span></span>
<span data-ttu-id="9a798-111"><a name="bk_cepullewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="9a798-111"><a name="bk_cepullewsma"> </a></span></span>

<span data-ttu-id="9a798-112">O exemplo de código a seguir mostra como usar o método [SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) para inscrever-se para receber notificações de todos os eventos na pasta caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="9a798-112">The following code example shows how to use the [SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) method to subscribe to pull notifications for all events in the Inbox folder.</span></span> <span data-ttu-id="9a798-113">O exemplo, em seguida, usa o método [GetEvents](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) para recuperar eventos do servidor.</span><span class="sxs-lookup"><span data-stu-id="9a798-113">The example then uses the [GetEvents](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) method to retrieve events from the server.</span></span> <span data-ttu-id="9a798-114">Neste exemplo, assumimos que **Service** é uma associação [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válida.</span><span class="sxs-lookup"><span data-stu-id="9a798-114">In this example, we assume that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) binding.</span></span> 
  
```cs
// Subscribe to pull notifications in the Inbox.
PullSubscription subscription = service.SubscribeToPullNotifications( 
    new FolderId[] { WellKnownFolderName.Inbox }, 30, null, 
    EventType.NewMail, EventType.Created, EventType.Deleted,
    EventType.Modified, EventType.Moved, EventType.Copied, EventType.FreeBusyChanged); 
 
// Call GetEvents to retrieve events from the server. 
GetEventsResults events = subscription.GetEvents(); 
```

<span data-ttu-id="9a798-115">Após receber um evento do servidor, você pode [sincronizar essas alterações com o servidor](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="9a798-115">After you receive an event from the server, you can [synchronize those changes with the server](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).</span></span> <span data-ttu-id="9a798-116">Use um dos métodos de cancelamento de assinatura especificados em [como eu cancelo a inscrição para notificações?](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe) para encerrar a assinatura com o servidor quando a assinatura não for mais necessária.</span><span class="sxs-lookup"><span data-stu-id="9a798-116">Use one of the unsubscribe methods specified in [How do I unsubscribe to notifications?](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe) to end the subscription with the server when the subscription is no longer needed.</span></span> 
  
## <a name="subscribe-to-pull-notifications-by-using-ews"></a><span data-ttu-id="9a798-117">Assinar notificações de recebimento usando EWS</span><span class="sxs-lookup"><span data-stu-id="9a798-117">Subscribe to pull notifications by using EWS</span></span>
<span data-ttu-id="9a798-118"><a name="bk_cepullews"> </a></span><span class="sxs-lookup"><span data-stu-id="9a798-118"><a name="bk_cepullews"> </a></span></span>

<span data-ttu-id="9a798-119">O exemplo a seguir mostra a solicitação XML a ser enviada ao servidor para inscrever-se em todos os [EventTypes](https://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) da pasta caixa de entrada usando a [operação inscrever](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="9a798-119">The following example shows the XML request to send to the server to subscribe to all [EventTypes](https://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) in the Inbox folder by using the [Subscribe operation](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx).</span></span> <span data-ttu-id="9a798-120">Essa é também a solicitação XML que a API gerenciada do EWS envia ao assinar notificações de recebimento usando o método [SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="9a798-120">This is also the XML request that the EWS Managed API sends when subscribing to pull notifications by using the [SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Subscribe xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <PullSubscriptionRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <FolderIds xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
      <DistinguishedFolderId Id="inbox" />
    </FolderIds>
    <EventTypes xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
            <EventType>NewMailEvent</EventType>
            <EventType>CreatedEvent</EventType>
            <EventType>DeletedEvent</EventType>
            <EventType>ModifiedEvent</EventType>
            <EventType>MovedEvent</EventType>
            <EventType>CopiedEvent</EventType>
            <EventType>FreeBusyChangedEvent</EventType>
    </EventTypes>
    <Timeout xmlns="https://schemas.microsoft.com/exchange/services/2006/types">30</Timeout>
  </PullSubscriptionRequest>
</Subscribe>
```

<span data-ttu-id="9a798-121">O exemplo de XML a seguir mostra a mensagem [SubscribeResponse](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) que é enviada do servidor para o cliente em resposta à solicitação de operação de **assinatura** .</span><span class="sxs-lookup"><span data-stu-id="9a798-121">The following XML example shows the [SubscribeResponse](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) message that is sent from the server to the client in response to the **Subscribe** operation request.</span></span> <span data-ttu-id="9a798-122">A inclusão do valor NoError para o elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) significa que a assinatura foi criada com êxito.</span><span class="sxs-lookup"><span data-stu-id="9a798-122">The inclusion of the NoError value for the [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element means that the subscription was created successfully.</span></span> <span data-ttu-id="9a798-123">O elemento [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) identifica exclusivamente a assinatura de notificação pull no servidor.</span><span class="sxs-lookup"><span data-stu-id="9a798-123">The [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) element uniquely identifies the pull notification subscription on the server.</span></span> <span data-ttu-id="9a798-124">O elemento [Watermark](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) representa um indicador na fila de eventos da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="9a798-124">The [Watermark](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) element represents a bookmark in the mailbox event queue.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<SubscribeResponse xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                   xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <SubscribeResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <SubscriptionId>d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
      <Watermark>AAAAAGUhAAAAAAAAAQ==</Watermark>
    </SubscribeResponseMessage>
  </ResponseMessages>
</SubscribeResponse>
```

<span data-ttu-id="9a798-125">Depois de criar a assinatura, agora você pode obter eventos usando o **SubscriptionId** que é retornado na mensagem **SubscribeResponse** .</span><span class="sxs-lookup"><span data-stu-id="9a798-125">After creating the subscription, you can now get events by using the **SubscriptionId** that is returned in the **SubscribeResponse** message.</span></span> 
  
## <a name="get-pull-notifications-by-using-ews"></a><span data-ttu-id="9a798-126">Obter notificações de recepção usando o EWS</span><span class="sxs-lookup"><span data-stu-id="9a798-126">Get pull notifications by using EWS</span></span>
<span data-ttu-id="9a798-127"><a name="bk_getpull"> </a></span><span class="sxs-lookup"><span data-stu-id="9a798-127"><a name="bk_getpull"> </a></span></span>

<span data-ttu-id="9a798-128">O exemplo de XML a seguir mostra a mensagem de solicitação de [operação GetEvents](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) que é enviada do cliente para o servidor para obter notificações para a [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) retornada na mensagem [SubscribeResponse](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="9a798-128">The following XML example shows the [GetEvents operation](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) request message that is sent from the client to the server to get notifications for the [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) that is returned in the [SubscribeResponse](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) message.</span></span> <span data-ttu-id="9a798-129">Para a primeira solicitação **GetEvents** , use a [marca d' água](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) retornada na resposta de **assinatura** .</span><span class="sxs-lookup"><span data-stu-id="9a798-129">For the first **GetEvents** request, use the [Watermark](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) returned in the **Subscribe** response.</span></span> <span data-ttu-id="9a798-130">Para solicitações **GetEvents** subsequentes, use a última **marca d' água** que foi retornada na solicitação **GetEvents** anterior.</span><span class="sxs-lookup"><span data-stu-id="9a798-130">For subsequent **GetEvents** requests, use the last **Watermark** that was returned in the previous **GetEvents** request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEvents xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <SubscriptionId xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
  <Watermark xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">AAAAAGUhAAAAAAAAAQ==</Watermark>
</GetEvents>
```

<span data-ttu-id="9a798-131">O exemplo de XML a seguir mostra a mensagem de resposta **GetEvents** que é enviada do servidor para o cliente.</span><span class="sxs-lookup"><span data-stu-id="9a798-131">The following XML example shows the **GetEvents** response message that is sent from the server to the client.</span></span> <span data-ttu-id="9a798-132">Cada resposta **GetEvents** inclui informações sobre um ou mais eventos.</span><span class="sxs-lookup"><span data-stu-id="9a798-132">Each **GetEvents** response includes information about one or more events.</span></span> <span data-ttu-id="9a798-133">Uma **marca d' água** é retornada para cada evento.</span><span class="sxs-lookup"><span data-stu-id="9a798-133">A **Watermark** is returned for each event.</span></span> <span data-ttu-id="9a798-134">A última **marca d' água** deve ser salva e usada na próxima solicitação **GetEvents** .</span><span class="sxs-lookup"><span data-stu-id="9a798-134">The last **Watermark** must be saved and used in the next **GetEvents** request.</span></span> <span data-ttu-id="9a798-135">Se nenhum evento de armazenamento tiver ocorrido desde a última solicitação **GetEvents** , um evento status será retornado.</span><span class="sxs-lookup"><span data-stu-id="9a798-135">If no store events have occurred since the last **GetEvents** request, a status event is returned.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEventsResponseType xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <GetEventsResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <Notification>
        <SubscriptionId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
        <PreviousWatermark xmlns="https://schemas.microsoft.com/exchange/services/2006/types">AAAAAGUhAAAAAAAAAQ==</PreviousWatermark>
        <MoreEvents xmlns="https://schemas.microsoft.com/exchange/services/2006/types">false</MoreEvents>
        <NewMailEvent xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Watermark>AAAAAHMhAAAAAAAAAQ==</Watermark>
          <TimeStamp>2013-09-15T21:37:01Z</TimeStamp>
          <ItemId Id="AAAtA=" ChangeKey="CQAAAA==" />
          <ParentFolderId Id="AQAtAEFkbWA==" ChangeKey="AQAAAA==" />
        </NewMailEvent>
      </Notification>
    </GetEventsResponseMessage>
  </ResponseMessages>
</GetEventsResponse>
```

Após receber um evento do servidor, [sincronize as alterações no cliente](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps). <span data-ttu-id="9a798-137">Use a [operação de cancelamento](https://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) de assinatura para finalizar a assinatura com o servidor quando a assinatura não for mais necessária.</span><span class="sxs-lookup"><span data-stu-id="9a798-137">Use the [Unsubscribe operation](https://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) to end the subscription with the server when the subscription is no longer needed.</span></span> 
  
## <a name="next-steps"></a><span data-ttu-id="9a798-138">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="9a798-138">Next steps</span></span>
<span data-ttu-id="9a798-139"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="9a798-139"><a name="bk_nextsteps"> </a></span></span>

<span data-ttu-id="9a798-140">Após receber notificações, você pode [sincronizar a hierarquia de pastas](how-to-synchronize-folders-by-using-ews-in-exchange.md) ou [sincronizar o conteúdo da pasta que foi alterada](how-to-synchronize-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="9a798-140">After you're received notifications, you can [sync the folder hierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md) or [sync the contents of the folder that changed](how-to-synchronize-items-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="9a798-141">Também consulte</span><span class="sxs-lookup"><span data-stu-id="9a798-141">See also</span></span>


- [<span data-ttu-id="9a798-142">Assinaturas de notificação, eventos de caixa de correio e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9a798-142">Notification subscriptions, mailbox events, and EWS in Exchange</span></span>](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [<span data-ttu-id="9a798-143">Transmitir notificações sobre eventos de caixa de correio usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9a798-143">Stream notifications about mailbox events by using EWS in Exchange</span></span>](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="9a798-144">Manter a afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange</span><span class="sxs-lookup"><span data-stu-id="9a798-144">Maintain affinity between a group of subscriptions and the Mailbox server in Exchange</span></span>](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [<span data-ttu-id="9a798-145">Tratamento de erros relacionados à notificação no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9a798-145">Handling notification-related errors in EWS in Exchange</span></span>](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="9a798-146">Sincronização de caixa de correio e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9a798-146">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    

