---
title: Desconectar a operação (serviço web de Unificação de mensagens)
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
description: A operação de desconexão encerra a chamada que é identificada pelo CallId especificado (serviço web de Unificação de mensagens).
ms.openlocfilehash: 1e04e65fa1951a6aa46e2c8b6dd5fe524c84a8fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751844"
---
# <a name="disconnect-operation-um-web-service"></a>Desconectar a operação (serviço web de Unificação de mensagens)

A operação de desconexão encerra a chamada que é identificada pelo especificado [CallId (serviço web de Unificação de mensagens)](callid-um-web-service.md).
  
## <a name="disconnect-request-example"></a>Desconectar um exemplo de solicitação

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de desconexão mostra como uma solicitação para desconectar uma chamada de formulário.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <Disconnect xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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
    <DisconnectResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Confira também

- [Desconectar (serviço web de Unificação de mensagens)](disconnect-um-web-service.md) 
- [DisconnectResponse (serviço web de Unificação de mensagens)](disconnectresponse-um-web-service.md) 
- [CallId (serviço web de Unificação de mensagens)](callid-um-web-service.md)

