---
title: MoreEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoreEvents
api_type:
- schema
ms.assetid: 76a7ea58-a44f-49b8-baba-d21302d742ad
description: O elemento MoreEvents indica se há mais eventos na fila sejam entregues ao cliente.
ms.openlocfilehash: cc3f7ed3b4b5f5ce27a9d45d508506bfa62e5086
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824489"
---
# <a name="moreevents"></a>MoreEvents

O elemento **MoreEvents** indica se há mais eventos na fila sejam entregues ao cliente. 
  
```xml
<MoreEvents/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Notificação](notification-ex15websvcsotherref.md) <br/> |Contém informações sobre a inscrição e os eventos que ocorreram desde a última notificação.  <br/> |
   
## <a name="text-value"></a>Text value

O valor de texto representa um valor booleano. Um valor **true** indica que mais eventos na fila. Um valor **false** indica que não há mais eventos estão na fila. Esta propriedade é somente leitura. 
  
## <a name="remarks"></a>Comentários

No caso de notificações de recepção, um valor **verdadeiro** nesse elemento indica ao cliente que a outra solicitação GetEvents deve ser emitida para obter os eventos restantes. Supondo que as especificações do cliente exigem latência mínima para notificações de evento, Solicitações GetEvents devem continuar em uma sucessão contínua até que um **Falso** **MoreEvents** valor será retornado. 
  
No caso de notificações de Push, um valor **true** para **MoreEvents** indica ao cliente que outra solicitação de notificação será enviada para o cliente para fornecer os eventos restantes. Semelhante ao notificações de recepção, essas solicitações de acompanhamento continuarão sucessivamente contínuo até que a fila de eventos no servidor de acesso para cliente está vazia. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Inscrever-se a operação](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)

