---
title: Operação IsUMEnabled (serviço Web de Unificação de Mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- IsUMEnabled
api_type:
- schema
ms.assetid: fbe6cd95-f7a5-42b9-8a9d-b6159a269d55
description: A operação IsUMEnabled determina se uma caixa de correio está habilitada para a Unificação de Mensagens.
ms.openlocfilehash: 2c637711fc34a1d1ccc484b14be3199632aaaaa3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514456"
---
# <a name="isumenabled-operation-um-web-service"></a>Operação IsUMEnabled (serviço Web de Unificação de Mensagens)

A operação IsUMEnabled determina se uma caixa de correio está habilitada para a Unificação de Mensagens.
  
## <a name="isumenabled-request-example"></a>Exemplo de solicitação IsUMEnabled

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação IsUMEnabled mostra como formar uma solicitação para determinar se uma caixa de correio está habilitada para a Unificação de Mensagens.
  
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

## <a name="see-also"></a>Confira também



[IsUMEnabled (serviço Web de Unificação de Mensagens)](isumenabled-um-web-service.md)
  
[IsUMEnabledResponse (serviço Web de Unificação de Mensagens)](isumenabledresponse-um-web-service.md)


[Elementos XML do serviço Web de Unificação de Mensagens para Exchange](unified-messaging-web-service-xml-elements-for-exchange.md)

