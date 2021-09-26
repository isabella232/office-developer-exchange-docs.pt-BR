---
title: Operação SetOofStatus (serviço Web de Unificação de Mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- SetOofStatus
api_type:
- schema
ms.assetid: 97c271e9-506e-43eb-89cd-46803fc47ee5
description: A operação SetOofStatus define um valor que indica se a saudação Out of Office (OOF) deve ser tocada para o usuário que faz a solicitação.
ms.openlocfilehash: ce736e7d7bea39f65843923187af3ae616ae1c86
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544749"
---
# <a name="setoofstatus-operation-um-web-service"></a>Operação SetOofStatus (serviço Web de Unificação de Mensagens)

A operação SetOofStatus define um valor que indica se a saudação Out of Office (OOF) deve ser tocada para o usuário que faz a solicitação.
  
## <a name="setoofstatus-request-example"></a>Exemplo de solicitação SetOofStatus

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação SetOofStatus mostra como formar uma solicitação para habilitar a saudação Fora de Office para uma caixa de correio.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetOofStatus xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetOofStatus>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setoofstatus-response-example"></a>Exemplo de resposta SetOofStatus bem-sucedido

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta SetOofStatus mostra uma resposta à solicitação SetOofStatus.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetOofStatusResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Confira também



[SetOofStatus (serviço Web de Unificação de Mensagens)](setoofstatus-um-web-service.md)
  
[SetOofStatusResponse (serviço Web de Unificação de Mensagens)](setoofstatusresponse-um-web-service.md)
  
[Status (serviço Web de Unificação de Mensagens – SetOofStatus)](status-um-web-servicesetoofstatus.md)

