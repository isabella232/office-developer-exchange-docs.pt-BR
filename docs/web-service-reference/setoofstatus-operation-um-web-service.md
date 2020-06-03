---
title: Operação SetOofStatus (serviço Web da UM)
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
description: A operação SetOofStatus define um valor que indica se a saudação de ausência temporária (OOF) deve ser reproduzida para o usuário que faz a solicitação.
ms.openlocfilehash: 2311b6137ac25d15ad3d06668450c1d0f7ec1fad
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467351"
---
# <a name="setoofstatus-operation-um-web-service"></a>Operação SetOofStatus (serviço Web da UM)

A operação SetOofStatus define um valor que indica se a saudação de ausência temporária (OOF) deve ser reproduzida para o usuário que faz a solicitação.
  
## <a name="setoofstatus-request-example"></a>Exemplo de solicitação SetOofStatus

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação SetOofStatus mostra como formar uma solicitação para habilitar a saudação de ausência temporária para uma caixa de correio.
  
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

## <a name="successful-setoofstatus-response-example"></a>Exemplo de resposta SetOofStatus bem-sucedida

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



[SetOofStatus (serviço Web da UM)](setoofstatus-um-web-service.md)
  
[SetOofStatusResponse (serviço Web da UM)](setoofstatusresponse-um-web-service.md)
  
[Status (serviço Web da UM-SetOofStatus)](status-um-web-servicesetoofstatus.md)

