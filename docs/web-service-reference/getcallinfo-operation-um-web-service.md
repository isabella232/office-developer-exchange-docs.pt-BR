---
title: Operação GetCallInfo (serviço Web da UM)
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
description: A operação GetCallInfo retorna o status da chamada de saída especificada por callid (serviço da Web da UM).
ms.openlocfilehash: 6b5664dfe16f9c74cc7175098145141b815a6355
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461237"
---
# <a name="getcallinfo-operation-um-web-service"></a>Operação GetCallInfo (serviço Web da UM)

A operação GetCallInfo retorna o status da chamada de saída especificada por [callid (serviço da Web da um)](callid-um-web-service.md).
  
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

## <a name="successful-getcallinfo-response-example"></a>Exemplo de resposta GetCallInfo bem-sucedida

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



[GetCallInfo (serviço Web da UM)](getcallinfo-um-web-service.md)
  
[GetCallInfoResponse (serviço Web da UM)](getcallinforesponse-um-web-service.md)
  
[Callid (serviço Web da UM)](callid-um-web-service.md)
  
[Callstate (serviço Web da UM)](callstate-um-web-service.md)
  
[EventCause (serviço Web da UM)](eventcause-um-web-service.md)

