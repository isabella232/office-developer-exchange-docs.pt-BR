---
title: Operação de IsUMEnabled (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- IsUMEnabled
api_type:
- schema
ms.assetid: fbe6cd95-f7a5-42b9-8a9d-b6159a269d55
description: A operação IsUMEnabled determina se uma caixa de correio está habilitada para Unificação de mensagens.
ms.openlocfilehash: 9d94a359d6b11e41762d21aa2fe5501bd9f7b577
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824107"
---
# <a name="isumenabled-operation-um-web-service"></a>Operação de IsUMEnabled (serviço web de Unificação de mensagens)

A operação IsUMEnabled determina se uma caixa de correio está habilitada para Unificação de mensagens.
  
## <a name="isumenabled-request-example"></a>Exemplo de solicitação de IsUMEnabled

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de IsUMEnabled mostra como formar uma solicitação para determinar se uma caixa de correio está habilitada para Unificação de mensagens.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <IsUMEnabled xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-isumenabled-response-example"></a>Exemplo de resposta bem-sucedida IsUMEnabled

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação IsUMEnabled.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <IsUMEnabledResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <IsUMEnabledResponse>true</IsUMEnabledResponse> 
    </IsUMEnabledResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Confira também



[IsUMEnabled (serviço web de Unificação de mensagens)](isumenabled-um-web-service.md)
  
[IsUMEnabledResponse (serviço web de Unificação de mensagens)](isumenabledresponse-um-web-service.md)


[Unified Messaging web service os elementos XML para o Exchange](unified-messaging-web-service-xml-elements-for-exchange.md)

