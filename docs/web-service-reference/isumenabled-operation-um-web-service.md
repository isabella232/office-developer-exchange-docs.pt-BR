---
title: Operação IsUMEnabled (serviço Web da UM)
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
ms.openlocfilehash: b1478f5a113059251fe1b036ac7d77e5a4ab4f50
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458233"
---
# <a name="isumenabled-operation-um-web-service"></a>Operação IsUMEnabled (serviço Web da UM)

A operação IsUMEnabled determina se uma caixa de correio está habilitada para Unificação de mensagens.
  
## <a name="isumenabled-request-example"></a>Exemplo de solicitação IsUMEnabled

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação IsUMEnabled mostra como formar uma solicitação para determinar se uma caixa de correio está habilitada para Unificação de mensagens.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <IsUMEnabled xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-isumenabled-response-example"></a>Exemplo de resposta IsUMEnabled bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação IsUMEnabled.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <IsUMEnabledResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <IsUMEnabledResponse>true</IsUMEnabledResponse> 
    </IsUMEnabledResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Também consulte



[IsUMEnabled (serviço Web da UM)](isumenabled-um-web-service.md)
  
[IsUMEnabledResponse (serviço Web da UM)](isumenabledresponse-um-web-service.md)


[Elementos XML do serviço Web de Unificação de mensagens para o Exchange](unified-messaging-web-service-xml-elements-for-exchange.md)

