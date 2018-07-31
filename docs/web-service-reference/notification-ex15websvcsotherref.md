---
title: Notification
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Notification
api_type:
- schema
ms.assetid: c9070936-0930-438e-839c-91127256a6c8
description: O elemento de notificação contém informações sobre a inscrição e os eventos que ocorreram desde a última notificação.
ms.openlocfilehash: 942ec18521fc484a7a3aa1385fb54f480ce9d11f
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354348"
---
# <a name="notification"></a>Notification

O elemento de **notificação** contém informações sobre a inscrição e os eventos que ocorreram desde a última notificação. 
  
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

## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[SubscriptionId (GetEvents)](subscriptionid-getevents.md) <br/> |Representa o identificador de uma assinatura.  <br/> |
|[PreviousWatermark](previouswatermark.md) <br/> |Representa a marca d'água do evento mais recente que foi comunicada com êxito para o cliente para a assinatura.  <br/> |
|[MoreEvents](moreevents.md) <br/> |Indica se há mais eventos na fila sejam entregues ao cliente.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Representa um evento no qual uma pasta ou um item é copiada.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Representa um evento no qual uma pasta ou um item é criada.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Representa um evento no qual uma pasta ou um item é excluída.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Representa um evento no qual um item ou pasta é modificada.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Representa um evento na qual um item ou pasta é movida de uma pasta pai para outra pasta pai.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Representa um evento que é disparado por um novo item de email em uma caixa de correio.  <br/> |
|[StatusEvent](statusevent.md) <br/> |Representa uma notificação que nenhuma nova atividade ocorreu na caixa de correio.  <br/> |
|[FreeBusyChangedEvent](freebusychangedevent.md) <br/> |Representa um evento no qual o tempo de disponibilidade de um item foi alterada.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetEventsResponseMessage](geteventsresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação GetEvents.  <br/> |
|[SendNotificationResponseMessage](sendnotificationresponsemessage.md) <br/> |Contém o status e o resultado de uma única solicitação SendNotification.  <br/> |
   
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também

- [Inscrever-se a operação](subscribe-operation.md) 
- [Operação GetEvents](getevents-operation.md) 
- [Operação GetStreamingEvents](getstreamingevents-operation.md) 
- [Cancelar a operação](unsubscribe-operation.md)

