---
title: MoreEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MoreEvents
api_type:
- schema
ms.assetid: 76a7ea58-a44f-49b8-baba-d21302d742ad
description: O elemento MoreEvents indica se há mais eventos na fila a serem entregues ao cliente.
ms.openlocfilehash: 7a19349e406a7e55e52c8a8cf0c3febba0a7301b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521806"
---
# <a name="moreevents"></a>MoreEvents

O **elemento MoreEvents** indica se há mais eventos na fila a serem entregues ao cliente. 
  
```xml
<MoreEvents/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[Notificação](notification-ex15websvcsotherref.md) <br/> |Contém informações sobre a assinatura e os eventos que ocorreram desde a última notificação.  <br/> |
   
## <a name="text-value"></a>Valor de texto

O valor de texto representa um valor Boolean. Um valor **true** indica que mais eventos estão na fila. Um valor **false** indica que não há mais eventos na fila. Essa propriedade é somente leitura. 
  
## <a name="remarks"></a>Comentários

No caso de notificações pull, um valor verdadeiro neste elemento indica ao cliente que outra solicitação GetEvents deve ser emitida para obter os eventos restantes.  Supondo que as especificações do cliente exigem latência mínima para notificações de  eventos, as solicitações getEvents devem continuar em uma sucessão contínua até que um valor **Falso MoreEvents** seja retornado. 
  
No caso de notificações por  Push, um valor verdadeiro para **MoreEvents** indica ao cliente que outra solicitação de notificação será enviada ao cliente para entregar os eventos restantes. Semelhante às notificações pull, essas solicitações de acompanhamento continuarão em sucessão contínua até que a fila de eventos no servidor de Acesso para Cliente seja vazia. 
  
O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nome do esquema  <br/> |Esquema de tipos  <br/> |
|Arquivo de validação  <br/> |Types.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação Subscribe](subscribe-operation.md)
  
[Operação GetEvents](getevents-operation.md)
  
[Cancelar a operação](unsubscribe-operation.md)

