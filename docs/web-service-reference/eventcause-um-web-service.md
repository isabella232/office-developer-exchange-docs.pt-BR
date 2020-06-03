---
title: EventCause (serviço Web da UM)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- EventCause
api_type:
- schema
ms.assetid: 7b3c1db8-cad4-4050-a50d-b06f065db530
description: O elemento EventCause contém um valor que indica a causa de um evento de chamada em uma resposta a uma solicitação de operação do GetCallInfo (serviço Web da UM).
ms.openlocfilehash: 9d49fd4b16236d0dd87889fbbd039f2e271a5968
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458674"
---
# <a name="eventcause-um-web-service"></a>EventCause (serviço Web da UM)

O elemento **EventCause** contém um valor que indica a causa de um evento de chamada em uma resposta a uma solicitação de [operação do GetCallInfo (serviço Web da um)](getcallinfo-operation-um-web-service.md) . 
  
[GetCallInfoResponse (serviço Web da UM)](getcallinforesponse-um-web-service.md)
  
[EventCause (serviço Web da UM)](eventcause-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <EventCause/>
</GetCallInfoResponse>
```

 **UMEventCause**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetCallInfoResponse (serviço Web da UM)](getcallinforesponse-um-web-service.md) <br/> |Define uma resposta a uma solicitação de [operação do GetCallInfo (serviço Web da um)](getcallinfo-operation-um-web-service.md) .  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é obrigatório. Veja a seguir os valores possíveis:
  
- Nenhum
    
- Userbusy
    
- NOANSWER
    
- Outros
    
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetCallInfo (serviço Web da UM)](getcallinfo-operation-um-web-service.md)
  
[GetCallInfoResponse (serviço Web da UM)](getcallinforesponse-um-web-service.md)

