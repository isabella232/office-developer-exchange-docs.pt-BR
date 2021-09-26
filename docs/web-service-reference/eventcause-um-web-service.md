---
title: EventCause (serviço Web de Unificação de Mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- EventCause
api_type:
- schema
ms.assetid: 7b3c1db8-cad4-4050-a50d-b06f065db530
description: O elemento EventCause contém um valor que indica a causa de um evento de chamada em uma resposta a uma solicitação de operação GetCallInfo (serviço Web de UM).
ms.openlocfilehash: 203cefa1a70294bec4d6f4b41aa157da6e639fce
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546571"
---
# <a name="eventcause-um-web-service"></a>EventCause (serviço Web de Unificação de Mensagens)

O **elemento EventCause** contém um valor que indica a causa de um evento de chamada em uma resposta a uma solicitação de operação [GetCallInfo (serviço Web](getcallinfo-operation-um-web-service.md) de UM). 
  
[GetCallInfoResponse (serviço Web de Unificação de Mensagens)](getcallinforesponse-um-web-service.md)
  
[EventCause (serviço Web de Unificação de Mensagens)](eventcause-um-web-service.md)
  
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
|[GetCallInfoResponse (serviço Web de Unificação de Mensagens)](getcallinforesponse-um-web-service.md) <br/> |Define uma resposta a uma [solicitação de operação GetCallInfo (serviço Web de UM).](getcallinfo-operation-um-web-service.md)  <br/> |
   
## <a name="text-value"></a>Valor de texto

Um valor de texto é necessário. Veja a seguir os valores possíveis:
  
- Nenhum
    
- UserBusy
    
- NoAnswer
    
- Outros
    
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetCallInfo (serviço Web de Unificação de Mensagens)](getcallinfo-operation-um-web-service.md)
  
[GetCallInfoResponse (serviço Web de Unificação de Mensagens)](getcallinforesponse-um-web-service.md)

