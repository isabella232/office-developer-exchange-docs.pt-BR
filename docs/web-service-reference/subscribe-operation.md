---
title: Operação Subscribe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Subscribe
api_type:
- schema
ms.assetid: f17c3d08-c79e-41f1-ba31-6e41e7aafd87
description: A operação de assinatura é usada para assinar aplicativos cliente para notificações por Push ou pull. É importante estar ciente de que a estrutura das mensagens e respostas de solicitação é diferente dependendo do tipo de notificação de evento.
ms.openlocfilehash: c40e0e434f698c6535ff5d03fd4d45a453959dd6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467043"
---
# <a name="subscribe-operation"></a>Operação Subscribe

A operação de assinatura é usada para assinar aplicativos cliente para notificações por Push ou pull. É importante estar ciente de que a estrutura das mensagens e respostas de solicitação é diferente dependendo do tipo de notificação de evento. 
  
## <a name="pull-subscription-subscribe-request-example"></a>Exemplo de solicitação de assinatura pull Subscription

### <a name="description"></a>Descrição

O exemplo de código a seguir mostra como se inscrever em uma assinatura de notificação de evento de recepção. A assinatura informa ao aplicativo cliente se novos emails são adicionados à caixa de entrada e se um item é excluído da caixa de entrada. A assinatura expirará se o cliente não solicitar informações sobre os eventos em dez minutos. Se a assinatura expirar, uma nova assinatura deve ser estabelecida para continuar a solicitar notificações.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Subscribe xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <PullSubscriptionRequest>
        <t:FolderIds>
          <t:DistinguishedFolderId Id="inbox"/>
        </t:FolderIds>
        <t:EventTypes>
          <t:EventType>NewMailEvent</t:EventType>
          <t:EventType>DeletedEvent</t:EventType>
        </t:EventTypes>
        <t:Timeout>10</t:Timeout>
      </PullSubscriptionRequest>
    </Subscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="pull-subscription-subscribe-request-elements"></a>Elementos de solicitação de inscrição de assinatura pull

Os seguintes elementos são usados na solicitação:
  
- [Assinar](subscribe.md)
    
- [PullSubscriptionRequest](pullsubscriptionrequest.md)
    
- [FolderIds](folderids.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [EventType](eventtypes.md)
    
- [EventType](eventtype.md)
    
- [Timeout](timeout.md)
    
Para encontrar outras opções para a mensagem de solicitação da operação de assinatura, explore a hierarquia do esquema. Inicie no elemento [PullSubscriptionRequest](pullsubscriptionrequest.md) . 
  
## <a name="successful-pull-subscription-subscribe-response-example"></a>Exemplo de resposta de inscrição de assinatura pull bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta de assinatura pull bem-sucedida. A resposta contém o identificador de assinatura e a marca d' água que é usada para obter a matriz de eventos que estão associados a uma assinatura. O identificador de assinatura também é usado para cancelar a assinatura de um cliente de uma assinatura.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SubscriptionId>39ea5d0f-f062-455e-a1e9-89c0304390f4</m:SubscriptionId>
          <m:Watermark>AAAAAHgGAAAAAAAAAQ==</m:Watermark>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </SubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="pull-subscription-subscribe-response-elements"></a>Elementos de resposta de assinatura pull Subscription

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SubscribeResponse](subscriberesponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SubscribeResponseMessage](subscriberesponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [SubscriptionId (GetEvents)](subscriptionid-getevents.md)
    
- [Marca d'água](watermark.md)
    
## <a name="pull-subscription-subscribe-error-response-example"></a>Exemplo de resposta de erro de assinatura pull Subscription

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta de erro a uma solicitação de assinatura. O erro é causado por uma tentativa de inscrever-se em notificações usando o acesso de representante.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Error">
          <m:MessageText>Subscriptions are not supported for delegate user access.</m:MessageText>
          <m:ResponseCode>ErrorSubscriptionDelegateAccessNotSupported</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </SubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="pull-subscription-error-response-elements"></a>Elementos de resposta de erro de assinatura pull

Os seguintes elementos são usados na resposta de erro:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SubscribeResponse](subscriberesponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SubscribeResponseMessage](subscriberesponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="push-subscription-request-example"></a>Exemplo de solicitação de assinatura push

### <a name="description"></a>Descrição

O exemplo de código a seguir mostra como se inscrever em uma assinatura de notificação por push de eventos. A solicitação identifica as pastas a serem monitoradas, os tipos de eventos a serem monitorados, a frequência das notificações de status e a URL do serviço Web cliente que escuta as notificações por push.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Subscribe xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <PushSubscriptionRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <FolderIds xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <DistinguishedFolderId Id="inbox" />
        </FolderIds>
        <EventTypes xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <EventType>NewMailEvent</EventType>
          <EventType>CopiedEvent</EventType>
          <EventType>CreatedEvent</EventType>
          <EventType>DeletedEvent</EventType>
          <EventType>ModifiedEvent</EventType>
          <EventType>MovedEvent</EventType>
        </EventTypes>
        <StatusFrequency xmlns="https://schemas.microsoft.com/exchange/services/2006/types">1</StatusFrequency>
        <URL xmlns="https://schemas.microsoft.com/exchange/services/2006/types">http://clientWebService/Service.asmx</URL>
      </PushSubscriptionRequest>
    </Subscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comentários

O serviço Web do cliente deve ser configurado antes que a solicitação de assinatura de notificação por push seja enviada; caso contrário, a primeira notificação não será enviada para um ponto de extremidade válido e a notificação por push falhará. Para mais informações, consulte [aplicativo de exemplo de notificação por push](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx).
  
Uma nova [SubscriptionId (GetEvents)](subscriptionid-getevents.md) é criada ao se reinscrever. Use a marca d' água de uma assinatura anterior para se reinscrever no ponto em que a assinatura anterior terminou. 
  
### <a name="push-subscription-request-elements"></a>Elementos de solicitação de assinatura push

Os seguintes elementos são usados na solicitação:
  
- [Assinar](subscribe.md)
    
- [PushSubscriptionRequest](pushsubscriptionrequest.md)
    
- [FolderIds](folderids.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [EventType](eventtypes.md)
    
- [EventType](eventtype.md)
    
- [StatusFrequency](statusfrequency.md)
    
- [Endereço](url-ex15websvcsotherref.md)
    
## <a name="successful-push-subscription-response-example"></a>Exemplo de resposta de assinatura push bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta de assinatura push bem-sucedida. 
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages>
        <SubscribeResponseMessage ResponseClass="Success">
          <ResponseCode>NoError</ResponseCode>
          <SubscriptionId>83826921-afdf-48be-b469-628cc02b5f49</SubscriptionId>
          <Watermark>AQAAAOpvG0LURVdOhQkPOWZLPcI8EgAAAAAAAAE=</Watermark>
        </SubscribeResponseMessage>
      </ResponseMessages>
    </SubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="push-subscription-response-elements"></a>Elementos de resposta de assinatura push

Os seguintes elementos são usados na resposta:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SubscribeResponse](subscriberesponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SubscribeResponseMessage](subscriberesponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [SubscriptionId (GetEvents)](subscriptionid-getevents.md)
    
- [Marca d'água](watermark.md)
    
## <a name="see-also"></a>Também consulte



[Cancelar a operação](unsubscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)


[Usando assinaturas pull](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[Aplicativo de amostra de notificação por push](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

