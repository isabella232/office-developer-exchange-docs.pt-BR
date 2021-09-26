---
title: StatusEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- StatusEvent
api_type:
- schema
ms.assetid: d3901818-2640-4bed-aad8-21a61aee62a1
description: O elemento StatusEvent representa uma notificação de que nenhuma nova atividade ocorreu na caixa de correio.
ms.openlocfilehash: 777d5cd22e47fea6e7bf7432e58e5d58d1ef67a4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543972"
---
# <a name="statusevent"></a>StatusEvent

O **elemento StatusEvent** representa uma notificação de que nenhuma nova atividade ocorreu na caixa de correio. 
  
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
|[Watermark](watermark.md) <br/> |Representa a última marca d'água válida para uma assinatura.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Notificação](notification-ex15websvcsotherref.md) <br/> |Contém informações sobre a assinatura e os eventos que ocorreram desde a última notificação.  <br/> |
   
## <a name="remarks"></a>Comentários

O **elemento StatusEvent** é retornado em uma notificação por um dos seguintes motivos: 
  
- Um cliente pull emite uma solicitação GetEvents em uma assinatura que não tem atividade.
    
- Um cliente push não tem eventos na fila quando [o StatusFrequency](statusfrequency.md) foi atingido. 
    
A **marca d'água StatusEvent**[é](watermark.md) usada por um aplicativo cliente da mesma maneira que as outras marcas d'água do tipo de evento. No entanto, a marca d'água **do StatusEvent** não é igual às marcas d'água usadas para outros eventos. Por exemplo, uma assinatura tem eventos com marcas d'água 1, 2 e 3 e esses eventos foram comunicados com êxito em uma notificação. Ocorre um período de inatividade e uma **solicitação GetEvents** é enviada. O servidor de Acesso para Cliente (CAS) retorna um evento de status e inclui a última marca d'água, 3, como [PreviousWatermark](previouswatermark.md) e [a marca d'água atual](watermark.md).
  
A marca d'água não permanecerá a mesma em todos os casos. Entradas de eventos são mantidas por 30 dias. Para manter uma assinatura ativa, o CAS atualiza periodicamente as marcas d'água para filas de assinatura. As marcas d'água atualizadas são enviadas aos clientes para manter uma assinatura ativa.
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode estar vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação Subscribe](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)

