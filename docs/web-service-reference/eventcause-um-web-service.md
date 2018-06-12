---
title: EventCause (serviço web de Unificação de mensagens)
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
description: O elemento EventCause contém um valor que indica a causa para um evento de chamada em resposta a uma solicitação do GetCallInfo operação (serviço web de Unificação de mensagens).
ms.openlocfilehash: dd73d93527bebb3b522ad0a6cdae5b9faee1a6a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752103"
---
# <a name="eventcause-um-web-service"></a>EventCause (serviço web de Unificação de mensagens)

O elemento **EventCause** contém um valor que indica a causa para um evento de chamada em resposta a uma solicitação de [operação GetCallInfo (serviço web de Unificação de mensagens)](getcallinfo-operation-um-web-service.md) . 
  
[GetCallInfoResponse (serviço web de Unificação de mensagens)](getcallinforesponse-um-web-service.md)
  
[EventCause (serviço web de Unificação de mensagens)](eventcause-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <EventCause/>
</GetCallInfoResponse>
```

 **UMEventCause**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

Nenhum.
  
### <a name="parent-elements"></a>Elementos pai

|**Elemento**|**Descrição**|
|:-----|:-----|
|[GetCallInfoResponse (serviço web de Unificação de mensagens)](getcallinforesponse-um-web-service.md) <br/> |Define uma resposta a uma solicitação de [operação GetCallInfo (serviço web de Unificação de mensagens)](getcallinfo-operation-um-web-service.md) .  <br/> |
   
## <a name="text-value"></a>Text value

É necessário um valor de texto. Veja a seguir os valores possíveis:
  
- None
    
- UserBusy
    
- NoAnswer
    
- Outro
    
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação de GetCallInfo (serviço web de Unificação de mensagens)](getcallinfo-operation-um-web-service.md)
  
[GetCallInfoResponse (serviço web de Unificação de mensagens)](getcallinforesponse-um-web-service.md)

