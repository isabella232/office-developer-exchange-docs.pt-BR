---
title: GetCallInfoResponse (serviço Web da UM)
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
description: O elemento GetCallInfoResponse define uma resposta a uma solicitação de operação GetCallInfo (serviço Web da UM).
ms.openlocfilehash: 6e54ec61a9a5ebecd96bbd39dad68f8cc011b8a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461202"
---
# <a name="getcallinforesponse-um-web-service"></a>GetCallInfoResponse (serviço Web da UM)

O elemento **GetCallInfoResponse** define uma resposta a uma solicitação de [operação GetCallInfo (serviço Web da um)](getcallinfo-operation-um-web-service.md) . 
  
[GetCallInfoResponse (serviço Web da UM)](getcallinforesponse-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <CallState/>
  <EventCause/>
</GetCallInfoResponse>
```

 **UMCallInfo**
## <a name="attributes-and-elements"></a>Atributos e elementos

As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.
  
### <a name="attributes"></a>Atributos

Nenhum
  
### <a name="child-elements"></a>Elementos filho

|**Elemento**|**Descrição**|
|:-----|:-----|
|Callstate  <br/> |Contém um valor que indica o status de uma chamada para a qual a [operação do GetCallInfo (serviço Web da um)](getcallinfo-operation-um-web-service.md) solicitou informações.  <br/> |
|EventCause  <br/> |Contém um valor que indica a causa de um evento para uma chamada para a qual a [operação do GetCallInfo (serviço Web da um)](getcallinfo-operation-um-web-service.md) solicitou informações.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="text-value"></a>Valor de texto

Nenhum
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetCallInfo (serviço Web da UM)](getcallinfo-operation-um-web-service.md)
  
[Callstate (serviço Web da UM)](callstate-um-web-service.md)
  
[EventCause (serviço Web da UM)](eventcause-um-web-service.md)

