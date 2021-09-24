---
title: Efetuar pull de notificações sobre eventos de caixa de correio usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: eb25cbd1-2244-4c3f-a71a-5ee20f81c41f
description: Saiba como usar a API Gerenciada do EWS ou o EWS para assinar notificações de pull e obter eventos.
ms.openlocfilehash: eb694eddd16567e42ccc43b2854f0432c54dc6b1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513098"
---
# <a name="pull-notifications-about-mailbox-events-by-using-ews-in-exchange"></a>Efetuar pull de notificações sobre eventos de caixa de correio usando o EWS no Exchange

Saiba como usar a API Gerenciada do EWS ou o EWS para assinar notificações de pull e obter eventos.
  
O EWS no Exchange usa notificações pull para permitir que os clientes solicitem (ou puxem) notificações sobre alterações na caixa de correio do servidor para o cliente.
  
Se você estiver se inscrevendo para receber notificações usando a API [](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullewsma) Gerenciada do EWS, inscreva-se e receba notificações pull usando o método [SubscribeToPullNotifications.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) Em seguida, você recebe eventos do servidor usando o [método GetEvents.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) 
  
Para assinar notificações de pull usando o EWS, crie uma assinatura usando a [](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_getpull) operação [Assinar,](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx)analisar [a](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullews) resposta e receber as notificações usando a operação [GetEvents](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx).
  
Depois que o cliente recebe notificações de itens que são alterados ou criados no servidor, ele pode [sincronizar as alterações](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).
  
## <a name="subscribe-to-and-get-pull-notifications-by-using-the-ews-managed-api"></a>Inscreva-se e receba notificações de pull usando a API Gerenciada do EWS
<a name="bk_cepullewsma"> </a>

O exemplo de código a seguir mostra como usar o método [SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) para assinar notificações de pull para todos os eventos na pasta Caixa de Entrada. O exemplo usa o método [GetEvents](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) para recuperar eventos do servidor. Neste exemplo, presumimos que o **serviço é** uma associação válida [do ExchangeService.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) 
  
```cs
// Subscribe to pull notifications in the Inbox.
PullSubscription subscription = service.SubscribeToPullNotifications( 
    new FolderId[] { WellKnownFolderName.Inbox }, 30, null, 
    EventType.NewMail, EventType.Created, EventType.Deleted,
    EventType.Modified, EventType.Moved, EventType.Copied, EventType.FreeBusyChanged); 
 
// Call GetEvents to retrieve events from the server. 
GetEventsResults events = subscription.GetEvents(); 
```

Depois de receber um evento do servidor, você pode [sincronizar essas alterações com o servidor](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps). Use um dos métodos unsubscribe especificados em [How do I unsubscribe to notifications?](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe) to end the subscription with the server when the subscription is not longer needed. 
  
## <a name="subscribe-to-pull-notifications-by-using-ews"></a>Inscrever-se para receber notificações usando o EWS
<a name="bk_cepullews"> </a>

O exemplo a seguir mostra a solicitação XML para enviar ao servidor para assinar todos [os EventTypes](https://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) na pasta Caixa de Entrada usando a operação [Assinar](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx). Essa também é a solicitação XML que a API Gerenciada do EWS envia ao inscrever-se para receber notificações usando o [método SubscribeToPullNotifications.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) 
  
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

O exemplo XML a seguir mostra a mensagem [SubscribeResponse](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) que é enviada do servidor para o cliente em resposta à solicitação de operação **Assinar.** A inclusão do valor NoError para o [elemento ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) significa que a assinatura foi criada com êxito. O [elemento SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) identifica exclusivamente a assinatura de notificação pull no servidor. O [elemento Watermark](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) representa um indicador na fila de eventos da caixa de correio. 
  
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

Depois de criar a assinatura, agora você pode obter eventos usando **a SubscriptionId** retornada na **mensagem SubscribeResponse.** 
  
## <a name="get-pull-notifications-by-using-ews"></a>Obter notificações de pull usando o EWS
<a name="bk_getpull"> </a>

O exemplo XML a seguir mostra a mensagem de solicitação de operação [GetEvents](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) que é enviada do cliente para o servidor para receber notificações para [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) retornadas na mensagem [SubscribeResponse.](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) Para a primeira **solicitação GetEvents,** use a [marca d'água](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) retornada na resposta **Assinar.** Para **solicitações GetEvents subsequentes,** use o último **Watermark** retornado na solicitação **GetEvents** anterior. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEvents xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <SubscriptionId xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
  <Watermark xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">AAAAAGUhAAAAAAAAAQ==</Watermark>
</GetEvents>
```

O exemplo XML a seguir mostra a mensagem de resposta **GetEvents** que é enviada do servidor para o cliente. Cada **resposta GetEvents** inclui informações sobre um ou mais eventos. Uma **marca d'água** é retornada para cada evento. A última **Marca d'água** deve ser salva e usada na próxima **solicitação GetEvents.** Se nenhum evento de armazenamento tiver ocorrido desde a última solicitação **GetEvents,** um evento de status será retornado. 
  
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

Depois de receber um evento do servidor, [sincronizar as alterações no cliente](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps). Use a [operação Cancelar assinatura](https://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) para encerrar a assinatura com o servidor quando a assinatura não for mais necessária. 
  
## <a name="next-steps"></a>Próximas etapas
<a name="bk_nextsteps"> </a>

Depois de receber notificações, você [](how-to-synchronize-folders-by-using-ews-in-exchange.md) pode sincronizar a hierarquia de pastas ou sincronizar o [conteúdo da pasta que foi alterada](how-to-synchronize-items-by-using-ews-in-exchange.md).
  
## <a name="see-also"></a>Confira também


- [Assinaturas de notificação, eventos de caixa de correio e EWS no Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [Transmitir notificações sobre eventos de caixa de correio usando o EWS no Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [Manter afinidade entre um grupo de assinaturas e o servidor de caixa de correio no Exchange](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [Manipulação de erros relacionados a notificações no EWS no Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Sincronização de caixa de correio e EWS no Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    

