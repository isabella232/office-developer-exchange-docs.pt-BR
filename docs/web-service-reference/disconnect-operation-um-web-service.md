---
title: Operação de desconexão (serviço Web da UM)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Disconnect
api_type:
- schema
ms.assetid: a987000b-d6e6-49d7-944c-e9c278d0236f
description: A operação de desconexão encerra a chamada identificada pelo callid especificado (serviço da Web da UM).
ms.openlocfilehash: a1268f9ea3d879f472e019bf1847fc13d65d1819
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529067"
---
# <a name="disconnect-operation-um-web-service"></a>Operação de desconexão (serviço Web da UM)

A operação de desconexão encerra a chamada identificada pelo [callid especificado (serviço da Web da um)](callid-um-web-service.md).
  
## <a name="disconnect-request-example"></a>Exemplo de solicitação de desconexão

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de desconexão mostra como formar uma solicitação para desconectar uma chamada.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <Disconnect xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </Disconnect>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-disconnect-response-example"></a>Exemplo de resposta de desconexão bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta de desconexão mostra uma resposta à solicitação de desconexão.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <DisconnectResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Confira também

- [Desconectar (serviço Web da UM)](disconnect-um-web-service.md) 
- [DisconnectResponse (serviço Web da UM)](disconnectresponse-um-web-service.md) 
- [Callid (serviço Web da UM)](callid-um-web-service.md)

