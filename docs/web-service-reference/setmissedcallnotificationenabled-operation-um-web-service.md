---
title: Operação SetMissedCallNotificationEnabled (serviço Web da UM)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetMissedCallNotificationEnabled
api_type:
- schema
ms.assetid: 6693b5db-ac6b-43bc-af83-a9c94fc425bf
description: A operação SetMissedCallNotificationEnabled habilita ou desabilita notificações de chamada não atendida.
ms.openlocfilehash: ca4942942a81bc187e8e18a5e6f003f8587f79d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467393"
---
# <a name="setmissedcallnotificationenabled-operation-um-web-service"></a>Operação SetMissedCallNotificationEnabled (serviço Web da UM)

A operação SetMissedCallNotificationEnabled habilita ou desabilita notificações de chamada não atendida.
  
## <a name="setmissedcallnotificationenabled-request-example"></a>Exemplo de solicitação SetMissedCallNotificationEnabled

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação SetMissedCallNotificationEnabled mostra como formar uma solicitação para habilitar notificações de chamadas perdidas.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetMissedCallNotificationEnabled xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetMissedCallNotificationEnabled>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setmissedcallnotificationenabled-response-example"></a>Exemplo de resposta SetMissedCallNotificationEnabled bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta PlayOnPhoneGreeting mostra uma resposta à solicitação SetMissedCallNotificationEnabled.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetMissedCallNotificationEnabledResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Também consulte



[SetMissedCallNotificationEnabled (serviço Web da UM)](setmissedcallnotificationenabled-um-web-service.md)
  
[SetMissedCallNotificationEnabledResponse (serviço Web da UM)](setmissedcallnotificationenabledresponse-um-web-service.md)
  
[Status (serviço Web da UM-SetMissedCallNotificationEnabled)](status-um-web-servicesetmissedcallnotificationenabled.md)

