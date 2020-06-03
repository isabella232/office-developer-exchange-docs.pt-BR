---
title: EventType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EventTypes
api_type:
- schema
ms.assetid: 29ded9e5-f191-4aa3-bc3e-500de2fc8818
description: O elemento EventTypes contém uma coleção de tipos de notificação de eventos que são usados para criar uma assinatura.
ms.openlocfilehash: 45ce1ed0699c8140029ae3fb7f667a5132f4731e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530625"
---
# <a name="eventtypes"></a>EventType

O elemento **EventTypes** contém uma coleção de tipos de notificação de eventos que são usados para criar uma assinatura. 
  
```xml
<EventTypes>
   <EventType/>
</EventTypes>
```

 **NonEmptyArrayOfNotificationEventTypesType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[EventType](eventtype.md) <br/> |Representa um tipo de notificação de evento solicitado que é usado para criar uma assinatura.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |Representa uma assinatura para uma assinatura de notificação de eventos baseada em pull.  <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Representa uma assinatura para uma assinatura de notificação de eventos baseada em push.  <br/> |
|[StreamingSubscriptionRequest](streamingsubscriptionrequest.md) <br/> |Representa uma assinatura para uma assinatura de notificação de eventos de streaming.  <br/> |
   
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="remarks"></a>Comentários

O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação Subscribe](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Operação GetStreamingEvents](getstreamingevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)

