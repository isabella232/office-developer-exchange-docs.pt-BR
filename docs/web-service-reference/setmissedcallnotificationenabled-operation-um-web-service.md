---
title: Operação de SetMissedCallNotificationEnabled (serviço web de Unificação de mensagens)
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
description: A operação SetMissedCallNotificationEnabled habilita ou desabilita as notificações de chamada não atendida.
ms.openlocfilehash: be9479d6ed2c5238ed19c3d22e028fca62b8deed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825434"
---
# <a name="setmissedcallnotificationenabled-operation-um-web-service"></a>Operação de SetMissedCallNotificationEnabled (serviço web de Unificação de mensagens)

A operação SetMissedCallNotificationEnabled habilita ou desabilita as notificações de chamada não atendida.
  
## <a name="setmissedcallnotificationenabled-request-example"></a>Exemplo de solicitação de SetMissedCallNotificationEnabled

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de SetMissedCallNotificationEnabled mostra como formar uma solicitação para habilitar as notificações de chamada não atendida.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetMissedCallNotificationEnabled xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetMissedCallNotificationEnabled>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setmissedcallnotificationenabled-response-example"></a>Exemplo de resposta bem-sucedida SetMissedCallNotificationEnabled

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta PlayOnPhoneGreeting mostra uma resposta à solicitação de SetMissedCallNotificationEnabled.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetMissedCallNotificationEnabledResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Confira também



[SetMissedCallNotificationEnabled (serviço web de Unificação de mensagens)](setmissedcallnotificationenabled-um-web-service.md)
  
[SetMissedCallNotificationEnabledResponse (serviço web de Unificação de mensagens)](setmissedcallnotificationenabledresponse-um-web-service.md)
  
[Status (UM serviço web - SetMissedCallNotificationEnabled)](status-um-web-servicesetmissedcallnotificationenabled.md)

