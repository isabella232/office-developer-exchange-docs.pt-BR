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
# <a name="pull-notifications-about-mailbox-events-by-using-ews-in-exchange"></a>Receber notificações sobre eventos de caixa de correio usando o EWS no Exchange

Descubra como usar a API gerenciada do EWS ou o EWS para se inscrever em notificações de recebimento e obter eventos.
  
O EWS no Exchange usa notificações de recebimento para permitir que clientes solicitem (ou recebam) notificações sobre alterações na caixa de correio do servidor para o cliente.
  
Se você estiver assinando notificações de recepção usando a API gerenciada do EWS, [assine e receba notificações de recebimento](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullewsma) usando o método [SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) . Em seguida, você obtém eventos do servidor usando o método [GetEvents](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) . 
  
Para se inscrever em notificações de recebimento usando o EWS, você [cria uma assinatura](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullews) usando a [operação Subscribe](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx), analisa a resposta e, em seguida, [Obtém as notificações](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_getpull) usando a [operação GetEvents](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx).
  
Depois que o cliente recebe notificações de itens que são alterados ou criados no servidor, ele pode [sincronizar as alterações](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).
  
## <a name="subscribe-to-and-get-pull-notifications-by-using-the-ews-managed-api"></a>Inscrever-se e obter notificações de recebimento usando a API gerenciada do EWS
<a name="bk_cepullewsma"> </a>

O exemplo de código a seguir mostra como usar o método [SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) para inscrever-se para receber notificações de todos os eventos na pasta caixa de entrada. O exemplo, em seguida, usa o método [GetEvents](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) para recuperar eventos do servidor. Neste exemplo, assumimos que **Service** é uma associação [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válida. 
  
```cs
// Subscribe to pull notifications in the Inbox.
PullSubscription subscription = service.SubscribeToPullNotifications( 
    new FolderId[] { WellKnownFolderName.Inbox }, 30, null, 
    EventType.NewMail, EventType.Created, EventType.Deleted,
    EventType.Modified, EventType.Moved, EventType.Copied, EventType.FreeBusyChanged); 
 
// Call GetEvents to retrieve events from the server. 
GetEventsResults events = subscription.GetEvents(); 
```

Após receber um evento do servidor, você pode [sincronizar essas alterações com o servidor](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps). Use um dos métodos de cancelamento de assinatura especificados em [como eu cancelo a inscrição para notificações?](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe) para encerrar a assinatura com o servidor quando a assinatura não for mais necessária. 
  
## <a name="subscribe-to-pull-notifications-by-using-ews"></a>Assinar notificações de recebimento usando EWS
<a name="bk_cepullews"> </a>

O exemplo a seguir mostra a solicitação XML a ser enviada ao servidor para inscrever-se em todos os [EventTypes](https://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) da pasta caixa de entrada usando a [operação inscrever](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx). Essa é também a solicitação XML que a API gerenciada do EWS envia ao assinar notificações de recebimento usando o método [SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) . 
  
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

O exemplo de XML a seguir mostra a mensagem [SubscribeResponse](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) que é enviada do servidor para o cliente em resposta à solicitação de operação de **assinatura** . A inclusão do valor NoError para o elemento [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) significa que a assinatura foi criada com êxito. O elemento [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) identifica exclusivamente a assinatura de notificação pull no servidor. O elemento [Watermark](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) representa um indicador na fila de eventos da caixa de correio. 
  
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

Depois de criar a assinatura, agora você pode obter eventos usando o **SubscriptionId** que é retornado na mensagem **SubscribeResponse** . 
  
## <a name="get-pull-notifications-by-using-ews"></a>Obter notificações de recepção usando o EWS
<a name="bk_getpull"> </a>

O exemplo de XML a seguir mostra a mensagem de solicitação de [operação GetEvents](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) que é enviada do cliente para o servidor para obter notificações para a [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) retornada na mensagem [SubscribeResponse](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) . Para a primeira solicitação **GetEvents** , use a [marca d' água](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) retornada na resposta de **assinatura** . Para solicitações **GetEvents** subsequentes, use a última **marca d' água** que foi retornada na solicitação **GetEvents** anterior. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEvents xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <SubscriptionId xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
  <Watermark xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">AAAAAGUhAAAAAAAAAQ==</Watermark>
</GetEvents>
```

O exemplo de XML a seguir mostra a mensagem de resposta **GetEvents** que é enviada do servidor para o cliente. Cada resposta **GetEvents** inclui informações sobre um ou mais eventos. Uma **marca d' água** é retornada para cada evento. A última **marca d' água** deve ser salva e usada na próxima solicitação **GetEvents** . Se nenhum evento de armazenamento tiver ocorrido desde a última solicitação **GetEvents** , um evento status será retornado. 
  
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

Após receber um evento do servidor, [sincronize as alterações no cliente](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps). Use a [operação de cancelamento](https://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) de assinatura para finalizar a assinatura com o servidor quando a assinatura não for mais necessária. 
  
## <a name="next-steps"></a>Próximas etapas
<a name="bk_nextsteps"> </a>

Após receber notificações, você pode [sincronizar a hierarquia de pastas](how-to-synchronize-folders-by-using-ews-in-exchange.md) ou [sincronizar o conteúdo da pasta que foi alterada](how-to-synchronize-items-by-using-ews-in-exchange.md).
  
## <a name="see-also"></a>Também consulte


- [Assinaturas de notificação, eventos de caixa de correio e EWS no Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [Transmitir notificações sobre eventos de caixa de correio usando o EWS no Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [Manter a afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [Tratamento de erros relacionados à notificação no EWS no Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Sincronização de caixa de correio e EWS no Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    

