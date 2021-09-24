---
title: CallState (serviço Web de Unificação de Mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- CallState
api_type:
- schema
ms.assetid: 88670707-12f7-41c5-ac81-dda0c354a2cb
description: O elemento CallState contém um valor que indica o status de uma chamada.
ms.openlocfilehash: 9435124e98cfb75beab5917c1e832096ca193e0c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519965"
---
# <a name="callstate-um-web-service"></a>CallState (serviço Web de Unificação de Mensagens)

O **elemento CallState** contém um valor que indica o status de uma chamada. 
  
[GetCallInfoResponse (serviço Web de Unificação de Mensagens)](getcallinforesponse-um-web-service.md)
  
[CallState (serviço Web de Unificação de Mensagens)](callstate-um-web-service.md)
  
```xml
<CallState/>
```

 **UMCallState**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetCallInfoResponse (serviço Web de Unificação de Mensagens)](getcallinforesponse-um-web-service.md) <br/> |Define uma resposta a uma [operação GetCallInfo (serviço Web de UM)](getcallinfo-operation-um-web-service.md).  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário. Veja a seguir os valores possíveis:
  
- Idle
    
- Connecting
    
- Alertado
    
- Conectado
    
- Disconnected
    
- Incoming
    
- Transferência
    
- Encaminhamento
    
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/message  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetCallInfo (serviço Web de Unificação de Mensagens)](getcallinfo-operation-um-web-service.md)
  
[GetCallInfoResponse (serviço Web de Unificação de Mensagens)](getcallinforesponse-um-web-service.md)

