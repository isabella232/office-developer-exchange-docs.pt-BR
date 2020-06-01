---
title: StatusEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StatusEvent
api_type:
- schema
ms.assetid: d3901818-2640-4bed-aad8-21a61aee62a1
description: O elemento StatusEvent representa uma notificação de que nenhuma atividade nova ocorreu na caixa de correio.
ms.openlocfilehash: 8158a47937a810be2ea22346384b4e61da56ac48
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468254"
---
# <a name="statusevent"></a>StatusEvent

O elemento **StatusEvent** representa uma notificação de que nenhuma atividade nova ocorreu na caixa de correio. 
  
```xml
<StatusEvent>
   <Watermark/>
</StatusEvent>
```

 **BaseNotificationEventType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Marca d'água](watermark.md) <br/> |Representa a última marca d' água válida para uma assinatura.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Notificação](notification-ex15websvcsotherref.md) <br/> |Contém informações sobre a assinatura e os eventos que ocorreram desde a última notificação.  <br/> |
   
## <a name="remarks"></a>Comentários

O elemento **StatusEvent** é retornado em uma notificação por uma das seguintes razões: 
  
- Um cliente de recepção emite uma solicitação GetEvents em uma assinatura sem atividade.
    
- Um cliente de envio não tem eventos na fila quando o [StatusFrequency](statusfrequency.md) foi alcançado. 
    
A **StatusEvent**[marca d' água](watermark.md) StatusEvent é usada por um aplicativo cliente da mesma maneira que as marcas d' água de outro tipo de evento. No entanto, a marca d' água de **StatusEvent** não é a mesma que as marcas d' água usadas para outros eventos. Por exemplo, uma assinatura tem eventos com marcas d' água 1, 2 e 3, e esses eventos foram comunicados com êxito em uma notificação. Um período de inatividade ocorre e uma solicitação **GetEvents** é enviada. O servidor de acesso para cliente (CAS) retorna um evento de status e inclui a última marca d' água, 3, como [PreviousWatermark](previouswatermark.md) e a [marca d' água](watermark.md)atual.
  
A marca d' água não permanecerá a mesma em todos os casos. As entradas de evento são mantidas por 30 dias. Para manter uma assinatura ativa, o CAS atualiza periodicamente as marcas d' água das filas de assinatura. As marcas d' água atualizadas são enviadas aos clientes para manter uma assinatura ativa.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types. xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação Subscribe](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)

