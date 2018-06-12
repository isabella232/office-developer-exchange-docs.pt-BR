---
title: CallState (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- CallState
api_type:
- schema
ms.assetid: 88670707-12f7-41c5-ac81-dda0c354a2cb
description: O elemento CallState contém um valor que indica o status de uma chamada.
ms.openlocfilehash: e751c2e38783c6634a44d8e1b830a9224cdf300a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751373"
---
# <a name="callstate-um-web-service"></a>CallState (serviço web de Unificação de mensagens)

O elemento **CallState** contém um valor que indica o status de uma chamada. 
  
[GetCallInfoResponse (serviço web de Unificação de mensagens)](getcallinforesponse-um-web-service.md)
  
[CallState (serviço web de Unificação de mensagens)](callstate-um-web-service.md)
  
```xml
<CallState/>
```

 **UMCallState**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetCallInfoResponse (serviço web de Unificação de mensagens)](getcallinforesponse-um-web-service.md) <br/> |Define uma resposta a uma [operação de GetCallInfo (serviço web de Unificação de mensagens)](getcallinfo-operation-um-web-service.md).  <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto. Veja a seguir os valores possíveis:
  
- Ocioso
    
- Connecting
    
- Alertado
    
- Connected
    
- Disconnected
    
- Entrada
    
- Transferindo
    
- Encaminhamento
    
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/message  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação de GetCallInfo (serviço web de Unificação de mensagens)](getcallinfo-operation-um-web-service.md)
  
[GetCallInfoResponse (serviço web de Unificação de mensagens)](getcallinforesponse-um-web-service.md)

