---
title: ConnectionStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConnectionStatus
api_type:
- schema
ms.assetid: 4300f9d6-8bf9-48c2-9f07-d80197864e17
description: O elemento ConnectionStatus fornece uma descrição de texto do status de uma assinatura de streaming.
ms.openlocfilehash: 05ff80ac3e6c3c8bf1341a179a14c9d052c9947f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59536848"
---
# <a name="connectionstatus"></a>ConnectionStatus

O **elemento ConnectionStatus** fornece uma descrição de texto do status de uma assinatura de streaming. 
  
```xml
<ConnectionStatus>OK or Closed</ConnectionStatus>
```

 **ConnectionStatusType**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetStreamingEventsResponseMessage](getstreamingeventsresponsemessage.md) <br/> |Contém o status e o resultado de uma única [solicitação de operação GetStreamingEvents.](getstreamingevents-operation.md)  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário. Veja a seguir os valores de texto possíveis para este elemento:
  
- OK
    
- Fechado
    
## <a name="remarks"></a>Comentários

O esquema que descreve esse elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services. Esse elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Esquema de mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetStreamingEvents](getstreamingevents-operation.md)


- [Elementos XML do EWS no Exchange](ews-xml-elements-in-exchange.md)

