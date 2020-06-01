---
title: Callstate (serviço Web da UM)
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
description: O elemento Callstate contém um valor que indica o status de uma chamada.
ms.openlocfilehash: 44614c460286ff49ebc2373263c1827c6be5cc08
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44454607"
---
# <a name="callstate-um-web-service"></a>Callstate (serviço Web da UM)

O elemento **callstate** contém um valor que indica o status de uma chamada. 
  
[GetCallInfoResponse (serviço Web da UM)](getcallinforesponse-um-web-service.md)
  
[Callstate (serviço Web da UM)](callstate-um-web-service.md)
  
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
|[GetCallInfoResponse (serviço Web da UM)](getcallinforesponse-um-web-service.md) <br/> |Define uma resposta a uma [operação GetCallInfo (serviço da um)](getcallinfo-operation-um-web-service.md).  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é obrigatório. Veja a seguir os valores possíveis:
  
- Estado
    
- Connecting
    
- Alertado
    
- Conectado
    
- Disconnected
    
- Electrónico
    
- Transfer
    
- Encaminhamento
    
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/message  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetCallInfo (serviço Web da UM)](getcallinfo-operation-um-web-service.md)
  
[GetCallInfoResponse (serviço Web da UM)](getcallinforesponse-um-web-service.md)

