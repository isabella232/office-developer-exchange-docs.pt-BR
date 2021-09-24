---
title: Operação SetMissedCallNotificationEnabled (serviço Web de Unificação de Mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- SetMissedCallNotificationEnabled
api_type:
- schema
ms.assetid: 6693b5db-ac6b-43bc-af83-a9c94fc425bf
description: A operação SetMissedCallNotificationEnabled habilita ou desabilita notificações de chamada perdidas.
ms.openlocfilehash: 31f59887041aac02e5876b596931902373870203
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521414"
---
# <a name="setmissedcallnotificationenabled-operation-um-web-service"></a>Operação SetMissedCallNotificationEnabled (serviço Web de Unificação de Mensagens)

A operação SetMissedCallNotificationEnabled habilita ou desabilita notificações de chamada perdidas.
  
## <a name="setmissedcallnotificationenabled-request-example"></a>Exemplo de solicitação SetMissedCallNotificationEnabled

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação SetMissedCallNotificationEnabled mostra como formar uma solicitação para habilitar notificações de chamada perdidas.
  
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

## <a name="see-also"></a>Confira também



[SetMissedCallNotificationEnabled (serviço Web de Unificação de Mensagens)](setmissedcallnotificationenabled-um-web-service.md)
  
[SetMissedCallNotificationEnabledResponse (serviço Web de Unificação de Mensagens)](setmissedcallnotificationenabledresponse-um-web-service.md)
  
[Status (serviço Web de Unificação de Mensagens – SetMissedCallNotificationEnabled)](status-um-web-servicesetmissedcallnotificationenabled.md)

