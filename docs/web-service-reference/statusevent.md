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
description: O elemento StatusEvent representa uma notificação que nenhuma nova atividade ocorreu na caixa de correio.
ms.openlocfilehash: e214918f9795e9e29061d4aac72ab144d2b24267
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825592"
---
# <a name="statusevent"></a>StatusEvent

O elemento **StatusEvent** representa uma notificação que nenhuma nova atividade ocorreu na caixa de correio. 
  
```xml
<StatusEvent>
   <Watermark/>
</StatusEvent>
```

 **BaseNotificationEventType**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Marca d'água](watermark.md) <br/> |Representa a última marca d'água válida de uma assinatura.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Notificação](notification-ex15websvcsotherref.md) <br/> |Contém informações sobre a inscrição e os eventos que ocorreram desde a última notificação.  <br/> |
   
## <a name="remarks"></a>Comentários

O elemento **StatusEvent** é retornado em uma notificação de um dos seguintes motivos: 
  
- Um cliente de recepção emite uma solicitação de GetEvents em uma assinatura que não tenha nenhuma atividade.
    
- Um cliente de push não tem nenhum evento na fila quando o [StatusFrequency](statusfrequency.md) foi atingido. 
    
O **StatusEvent**[marca d'água](watermark.md) é usada por um aplicativo cliente da mesma maneira como as outras eventos tipo marcas d'água. No entanto, a marca d'água para o **StatusEvent** não é o mesmo que as marcas d'água usadas para outros eventos. Por exemplo, uma assinatura tiver eventos com marcas d'água 1, 2 e 3 e esses eventos foram com êxito comunicados em uma notificação. Ocorre um período de inatividade e uma solicitação **GetEvents** é enviada. O servidor de acesso para cliente (CAS) retorna um evento de status e inclui a última marca d'água, 3, como o [PreviousWatermark](previouswatermark.md) e o atual [marca d'água](watermark.md).
  
A marca d'água não permanecerá a mesma em todos os casos. Entradas de evento são mantidas por 30 dias. Para manter uma assinatura ativa, o CAS atualiza periodicamente as marcas d'água para filas de assinatura. As marcas d'água atualizadas serão enviadas aos clientes para manter uma assinatura ativa.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Inscrever-se a operação](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)

