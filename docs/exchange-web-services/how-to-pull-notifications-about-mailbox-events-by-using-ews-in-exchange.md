---
title: Receber notificações sobre eventos de caixa de correio usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: eb25cbd1-2244-4c3f-a71a-5ee20f81c41f
description: Descubra como usar a API gerenciada de EWS ou o EWS para assinar notificações de recepção e obtenha eventos.
ms.openlocfilehash: 6a04aaf0102c149691a30c2bd2f499e03265bce8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750811"
---
# <a name="pull-notifications-about-mailbox-events-by-using-ews-in-exchange"></a>Receber notificações sobre eventos de caixa de correio usando o EWS no Exchange

Descubra como usar a API gerenciada de EWS ou o EWS para assinar notificações de recepção e obtenha eventos.
  
EWS no Exchange usa notificações de recepção para permitir que os clientes a solicitação (ou recepção) notificações sobre alterações à caixa de correio do servidor para o cliente.
  
Se você está inscrevendo às notificações de recepção usando a API gerenciada do EWS, você [inscrever-se e obter notificações de recepção](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullewsma) usando o método [SubscribeToPullNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) . Em seguida, obtenha eventos do servidor usando o método [GetEvents](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) . 
  
Para assinar notificações de recepção usando o EWS, [Crie uma inscrição](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullews) usando a [operação Subscribe](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx), analisar a resposta e [obter as notificações](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_getpull) usando a [operação GetEvents](http://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx).
  
Depois que o cliente recebe notificações de itens que foram alterados ou criados no servidor, ele pode então [sincronizar as alterações](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).
  
## <a name="subscribe-to-and-get-pull-notifications-by-using-the-ews-managed-api"></a>Inscrever-se e obter notificações de recepção usando a API gerenciada de EWS
<a name="bk_cepullewsma"> </a>

O exemplo de código a seguir mostra como usar o método [SubscribeToPullNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) para assinar notificações de recepção para todos os eventos na pasta caixa de entrada. O exemplo, em seguida, usa o método de [GetEvents](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) para recuperar os eventos do servidor. Neste exemplo, vamos pressupor que esse **serviço** é uma vinculação [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válida. 
  
```cs
// Subscribe to pull notifications in the Inbox.
PullSubscription subscription = service.SubscribeToPullNotifications( 
    new FolderId[] { WellKnownFolderName.Inbox }, 30, null, 
    EventType.NewMail, EventType.Created, EventType.Deleted,
    EventType.Modified, EventType.Moved, EventType.Copied, EventType.FreeBusyChanged); 
 
// Call GetEvents to retrieve events from the server. 
GetEventsResults events = subscription.GetEvents(); 
```

Após receber um evento do servidor, você pode [sincronizar as alterações com o servidor](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps). Use um dos métodos de cancelamento da assinatura especificados em [como cancelar o às notificações?](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe) para encerrar a assinatura com o servidor quando a assinatura não é mais necessária. 
  
## <a name="subscribe-to-pull-notifications-by-using-ews"></a>Assine as notificações de recepção usando o EWS
<a name="bk_cepullews"> </a>

O exemplo a seguir mostra a solicitação XML para enviar para o servidor para assinar todas as [EventTypes](http://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) na pasta caixa de entrada usando a [operação de assinatura](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx). Isso também é a solicitação XML que o EWS Managed API envia ao inscrever-se às notificações de recepção usando o método [SubscribeToPullNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Subscribe xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <PullSubscriptionRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <FolderIds xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
      <DistinguishedFolderId Id="inbox" />
    </FolderIds>
    <EventTypes xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
            <EventType>NewMailEvent</EventType>
            <EventType>CreatedEvent</EventType>
            <EventType>DeletedEvent</EventType>
            <EventType>ModifiedEvent</EventType>
            <EventType>MovedEvent</EventType>
            <EventType>CopiedEvent</EventType>
            <EventType>FreeBusyChangedEvent</EventType>
    </EventTypes>
    <Timeout xmlns="http://schemas.microsoft.com/exchange/services/2006/types">30</Timeout>
  </PullSubscriptionRequest>
</Subscribe>
```

O exemplo XML a seguir mostra a mensagem [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) que é enviada ao cliente em resposta à solicitação **Subscribe** operação do servidor. A inclusão do valor para o elemento [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) NoError significa que a assinatura foi criada com êxito. O elemento [SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) identifica exclusivamente a inscrição de notificação de recepção no servidor. O elemento de [marca d'água](http://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) representa um indicador na fila de eventos de caixa de correio. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<SubscribeResponse xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                   xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <SubscribeResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <SubscriptionId>d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
      <Watermark>AAAAAGUhAAAAAAAAAQ==</Watermark>
    </SubscribeResponseMessage>
  </ResponseMessages>
</SubscribeResponse>
```

Depois de criar a assinatura, agora você pode obter eventos usando a **SubscriptionId** retornado na mensagem **SubscribeResponse** . 
  
## <a name="get-pull-notifications-by-using-ews"></a>Obter notificações de recepção usando o EWS
<a name="bk_getpull"> </a>

O exemplo XML a seguir mostra a mensagem de solicitação de [operação GetEvents](http://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) é enviada pelo cliente para o servidor para receber as notificações para a [SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) retornado na mensagem [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) . Para a primeira solicitação **GetEvents** , use a [marca d'água](http://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) retornados na resposta da **inscrição** . Para solicitações **GetEvents** subsequentes, use a última **marca d'água** que foi retornado na solicitação **GetEvents** anterior. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEvents xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <SubscriptionId xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
  <Watermark xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">AAAAAGUhAAAAAAAAAQ==</Watermark>
</GetEvents>
```

O exemplo XML a seguir mostra a mensagem de resposta **GetEvents** que é enviada do servidor para o cliente. Cada resposta **GetEvents** inclui informações sobre um ou mais eventos. Uma **marca d'água** é retornada para cada evento. A última **marca d'água** deve ser salvo e usado na próxima solicitação **GetEvents** . Se nenhum repositório de eventos ocorreram desde o último pedido **GetEvents** , um evento de status será retornado. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEventsResponseType xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <GetEventsResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <Notification>
        <SubscriptionId xmlns="http://schemas.microsoft.com/exchange/services/2006/types">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
        <PreviousWatermark xmlns="http://schemas.microsoft.com/exchange/services/2006/types">AAAAAGUhAAAAAAAAAQ==</PreviousWatermark>
        <MoreEvents xmlns="http://schemas.microsoft.com/exchange/services/2006/types">false</MoreEvents>
        <NewMailEvent xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

Depois que você receber um evento no servidor, [sincronizar as alterações para o cliente](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps). Use a [operação de cancelamento da assinatura](http://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) para encerrar a assinatura com o servidor quando a assinatura não é mais necessária. 
  
## <a name="next-steps"></a>Próximas etapas
<a name="bk_nextsteps"> </a>

Depois que você estiver recebido notificações, você pode [sincronizar a hierarquia de pastas](how-to-synchronize-folders-by-using-ews-in-exchange.md) ou [sincronizar o conteúdo da pasta que é alterado](how-to-synchronize-items-by-using-ews-in-exchange.md).
  
## <a name="see-also"></a>Confira também


- [Inscrições de notificação, eventos de caixa de correio e EWS no Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [Notificações de fluxo sobre eventos de caixa de correio usando o EWS no Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [Manter a afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [Tratando erros relacionados a notificação no EWS no Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Sincronização de caixa de correio e EWS no Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    

