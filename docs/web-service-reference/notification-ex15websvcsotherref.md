---
title: Notificação
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Notification
api_type:
- schema
ms.assetid: c9070936-0930-438e-839c-91127256a6c8
description: O elemento Notification contém informações sobre a assinatura e os eventos que ocorreram desde a última notificação.
ms.openlocfilehash: affd44bb4c1f16029d6da92419908aeac3c26a44
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515408"
---
# <a name="notification"></a>Notificação

O **elemento Notification** contém informações sobre a assinatura e os eventos que ocorreram desde a última notificação. 
  
```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <CopiedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <CreatedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <DeletedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <ModifiedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <MovedEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <NewMailEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <StatusEvent/>
</Notification>
```

```xml
<Notification>
   <SubscriptionId/>
   <PreviousWatermark/>
   <MoreEvents/>
   <FreeBusyChangedEvent/>
</Notification>
```

**NotificationType**

## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SubscriptionId (GetEvents)](subscriptionid-getevents.md) <br/> |Representa o identificador de uma assinatura.  <br/> |
|[PreviousWatermark](previouswatermark.md) <br/> |Representa a marca d'água do evento mais recente que foi comunicado com êxito ao cliente para a assinatura.  <br/> |
|[MoreEvents](moreevents.md) <br/> |Indica se há mais eventos na fila a serem entregues ao cliente.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Representa um evento no qual um item ou pasta é copiado.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Representa um evento no qual um item ou pasta é criado.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Representa um evento no qual um item ou pasta é excluído.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Representa um evento no qual um item ou pasta é modificado.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Representa um evento no qual um item ou pasta é movido de uma pasta pai para outra pasta pai.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Representa um evento disparado por um novo item de email em uma caixa de correio.  <br/> |
|[StatusEvent](statusevent.md) <br/> |Representa uma notificação de que nenhuma nova atividade ocorreu na caixa de correio.  <br/> |
|[FreeBusyChangedEvent](freebusychangedevent.md) <br/> |Representa um evento no qual o tempo livre/ocupado de um item foi alterado.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação GetEvents.  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação SendNotification.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também

- [Operação Subscribe](subscribe-operation.md) 
- [Operação GetEvents](getevents-operation.md) 
- [Operação GetStreamingEvents](getstreamingevents-operation.md) 
- [Cancelar a operação](unsubscribe-operation.md)

