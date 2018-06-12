---
title: Operação de SetOofStatus (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetOofStatus
api_type:
- schema
ms.assetid: 97c271e9-506e-43eb-89cd-46803fc47ee5
description: A operação SetOofStatus define um valor que indica se a saudação de ausência temporária deve ser reproduzida para o usuário que faz com que a solicitação.
ms.openlocfilehash: 2bb1deeec8ddb5be56979bfb2fae3396672298a3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825445"
---
# <a name="setoofstatus-operation-um-web-service"></a>Operação de SetOofStatus (serviço web de Unificação de mensagens)

A operação SetOofStatus define um valor que indica se a saudação de ausência temporária deve ser reproduzida para o usuário que faz com que a solicitação.
  
## <a name="setoofstatus-request-example"></a>Exemplo de solicitação de SetOofStatus

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de SetOofStatus mostra como uma solicitação para ativar a saudação de ausência temporária para uma caixa de correio de formulário.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetOofStatus xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetOofStatus>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setoofstatus-response-example"></a>Exemplo de resposta bem-sucedida SetOofStatus

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta SetOofStatus mostra uma resposta à solicitação de SetOofStatus.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetOofStatusResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Confira também



[SetOofStatus (serviço web de Unificação de mensagens)](setoofstatus-um-web-service.md)
  
[SetOofStatusResponse (serviço web de Unificação de mensagens)](setoofstatusresponse-um-web-service.md)
  
[Status (UM serviço web - SetOofStatus)](status-um-web-servicesetoofstatus.md)

