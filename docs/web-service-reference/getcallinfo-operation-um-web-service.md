---
title: Operação de GetCallInfo (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetCallInfo
api_type:
- schema
ms.assetid: 6bccd418-caf7-4eb9-8a6f-410e56a635c3
description: A operação GetCallInfo retorna o status da chamada de saída que é especificada pelo CallId (serviço web de Unificação de mensagens).
ms.openlocfilehash: 36f9cba3690520ebb457a4cb2bfbcde3fea4b8dc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752417"
---
# <a name="getcallinfo-operation-um-web-service"></a>Operação de GetCallInfo (serviço web de Unificação de mensagens)

A operação GetCallInfo retorna o status da chamada de saída que é especificada pelo [CallId (serviço web de Unificação de mensagens)](callid-um-web-service.md).
  
## <a name="getcallinfo-request-example"></a>Exemplo de solicitação de GetCallInfo

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de GetCallInfo mostra como formar uma solicitação para obter mais informações sobre uma chamada de saída especificada.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetCallInfo xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </GetCallInfo>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getcallinfo-response-example"></a>Exemplo de resposta bem-sucedida GetCallInfo

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta GetCallInfo mostra uma resposta a uma solicitação GetCallInfo.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetCallInfoResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <GetCallInfoResponse>
        <CallState>Connected</CallState> 
        <EventCause>None</EventCause> 
      </GetCallInfoResponse>
    </GetCallInfoResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Confira também



[GetCallInfo (serviço web de Unificação de mensagens)](getcallinfo-um-web-service.md)
  
[GetCallInfoResponse (serviço web de Unificação de mensagens)](getcallinforesponse-um-web-service.md)
  
[CallId (serviço web de Unificação de mensagens)](callid-um-web-service.md)
  
[CallState (serviço web de Unificação de mensagens)](callstate-um-web-service.md)
  
[EventCause (serviço web de Unificação de mensagens)](eventcause-um-web-service.md)

