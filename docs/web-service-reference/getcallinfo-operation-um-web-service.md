---
title: Operação GetCallInfo (serviço Web de Unificação de Mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- GetCallInfo
api_type:
- schema
ms.assetid: 6bccd418-caf7-4eb9-8a6f-410e56a635c3
description: A operação GetCallInfo retorna o status da chamada de saída especificada por CallId (serviço Web de UM).
ms.openlocfilehash: 0563190ab267b3a48d7ccacbdb1e136c6e3da0b4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509940"
---
# <a name="getcallinfo-operation-um-web-service"></a>Operação GetCallInfo (serviço Web de Unificação de Mensagens)

A operação GetCallInfo retorna o status da chamada de saída especificada por [CallId (serviço Web da UM)](callid-um-web-service.md).
  
## <a name="getcallinfo-request-example"></a>Exemplo de solicitação GetCallInfo

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação GetCallInfo mostra como formar uma solicitação para obter informações sobre uma chamada de saída especificada.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetCallInfo xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </GetCallInfo>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getcallinfo-response-example"></a>Exemplo de resposta GetCallInfo bem-sucedido

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta GetCallInfo mostra uma resposta a uma solicitação GetCallInfo.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetCallInfoResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <GetCallInfoResponse>
        <CallState>Connected</CallState> 
        <EventCause>None</EventCause> 
      </GetCallInfoResponse>
    </GetCallInfoResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Confira também



[GetCallInfo (serviço Web de Unificação de Mensagens)](getcallinfo-um-web-service.md)
  
[GetCallInfoResponse (serviço Web de Unificação de Mensagens)](getcallinforesponse-um-web-service.md)
  
[CallId (serviço Web de Unificação de Mensagens)](callid-um-web-service.md)
  
[CallState (serviço Web de Unificação de Mensagens)](callstate-um-web-service.md)
  
[EventCause (serviço Web de Unificação de Mensagens)](eventcause-um-web-service.md)

