---
title: Operação Disconnect (serviço Web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- Disconnect
api_type:
- schema
ms.assetid: a987000b-d6e6-49d7-944c-e9c278d0236f
description: A operação Disconnect encerra a chamada identificada pelo CallId (serviço Web de UM) especificado.
ms.openlocfilehash: 42e069233fbfc255d43983571c0bb28475a1fe90
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522009"
---
# <a name="disconnect-operation-um-web-service"></a>Operação Disconnect (serviço Web de Unificação de mensagens)

A operação Disconnect encerra a chamada identificada pelo [CallId (serviço Web de UM)](callid-um-web-service.md)especificado.
  
## <a name="disconnect-request-example"></a>Exemplo de solicitação de desconexão

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação Disconnect mostra como formar uma solicitação para desconectar uma chamada.
  
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

O exemplo a seguir de uma resposta Disconnect mostra uma resposta à solicitação Disconnect.
  
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

- [Disconnect (serviço Web de Unificação de Mensagens)](disconnect-um-web-service.md) 
- [DisconnectResponse (serviço Web de Unificação de Mensagens)](disconnectresponse-um-web-service.md) 
- [CallId (serviço Web de Unificação de Mensagens)](callid-um-web-service.md)

