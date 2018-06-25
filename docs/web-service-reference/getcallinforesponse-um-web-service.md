---
title: GetCallInfoResponse (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetCallInfoResponse
api_type:
- schema
ms.assetid: aa5196bf-f5f3-455c-94ea-304fb7920c79
description: O elemento de GetCallInfoResponse define uma resposta a uma solicitação do GetCallInfo operação (serviço web de Unificação de mensagens).
ms.openlocfilehash: d9658dd9cb47f925e05dc21a8651c98dce1f0a2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752421"
---
# <a name="getcallinforesponse-um-web-service"></a>GetCallInfoResponse (serviço web de Unificação de mensagens)

O elemento de **GetCallInfoResponse** define uma resposta a uma solicitação de [operação GetCallInfo (serviço web de Unificação de mensagens)](getcallinfo-operation-um-web-service.md) . 
  
[GetCallInfoResponse (serviço web de Unificação de mensagens)](getcallinforesponse-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <CallState/>
  <EventCause/>
</GetCallInfoResponse>
```

 **UMCallInfo**
## <a name="attributes-and-elements"></a>Attributes and elements

As seções a seguir descrevem os atributos e elementos filho elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum.
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|CallState  <br/> |Contém um valor que indica o status de uma chamada para o qual a [operação GetCallInfo (serviço web de Unificação de mensagens)](getcallinfo-operation-um-web-service.md) informações solicitadas.  <br/> |
|EventCause  <br/> |Contém um valor que indica a causa de um evento para uma chamada para o qual a [operação GetCallInfo (serviço web de Unificação de mensagens)](getcallinfo-operation-um-web-service.md) informações solicitadas.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum.
  
## <a name="text-value"></a>Text value

Nenhum.
  
## <a name="element-information"></a>Informações de elemento

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Ver também



[Operação de GetCallInfo (serviço web de Unificação de mensagens)](getcallinfo-operation-um-web-service.md)
  
[CallState (serviço web de Unificação de mensagens)](callstate-um-web-service.md)
  
[EventCause (serviço web de Unificação de mensagens)](eventcause-um-web-service.md)

