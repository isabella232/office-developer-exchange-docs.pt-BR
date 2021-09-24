---
title: GetCallInfoResponse (serviço Web de Unificação de Mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- GetCallInfoResponse
api_type:
- schema
ms.assetid: aa5196bf-f5f3-455c-94ea-304fb7920c79
description: O elemento GetCallInfoResponse define uma resposta a uma solicitação de operação GetCallInfo (serviço Web de UM).
ms.openlocfilehash: 4b631bdee87e57c1612e906c725adabb9f9ce63e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526186"
---
# <a name="getcallinforesponse-um-web-service"></a>GetCallInfoResponse (serviço Web de Unificação de Mensagens)

O **elemento GetCallInfoResponse** define uma resposta a uma solicitação de operação [GetCallInfo (serviço Web de UM).](getcallinfo-operation-um-web-service.md) 
  
[GetCallInfoResponse (serviço Web de Unificação de Mensagens)](getcallinforesponse-um-web-service.md)
  
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
|CallState  <br/> |Contém um valor que indica o status de uma chamada para a qual a operação [GetCallInfo (serviço Web da UM)](getcallinfo-operation-um-web-service.md) solicitou informações.  <br/> |
|EventCause  <br/> |Contém um valor que indica a causa de um evento para uma chamada para a qual a operação [GetCallInfo (serviço Web da UM)](getcallinfo-operation-um-web-service.md) solicitou informações.  <br/> |
   
### <a name="parent-elements"></a>Elementos pai

Nenhum
  
## <a name="text-value"></a>Valor de texto

Nenhum.
  
## <a name="element-information"></a>Elemento de informações

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nome do esquema  <br/> |Mensagens  <br/> |
|Arquivo de validação  <br/> |Messages.xsd  <br/> |
|Pode ser vazio  <br/> |False  <br/> |
   
## <a name="see-also"></a>Confira também



[Operação GetCallInfo (serviço Web de Unificação de Mensagens)](getcallinfo-operation-um-web-service.md)
  
[CallState (serviço Web de Unificação de Mensagens)](callstate-um-web-service.md)
  
[EventCause (serviço Web de Unificação de Mensagens)](eventcause-um-web-service.md)

