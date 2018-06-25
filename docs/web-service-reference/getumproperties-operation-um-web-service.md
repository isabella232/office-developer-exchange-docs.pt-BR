---
title: Operação de GetUMProperties (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetUMProperties
api_type:
- schema
ms.assetid: 301fb9a3-67df-44c4-8ffe-0600237fc344
description: A operação GetUMProperties obtém todas as propriedades de Unificação de mensagens para a caixa de correio do usuário que está fazendo a solicitação.
ms.openlocfilehash: 8878099bbd907fe0648f7d64dde3cd9600c2c45f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823678"
---
# <a name="getumproperties-operation-um-web-service"></a>Operação de GetUMProperties (serviço web de Unificação de mensagens)

A operação GetUMProperties obtém todas as propriedades de Unificação de mensagens para a caixa de correio do usuário que está fazendo a solicitação.
  
## <a name="getumproperties-request-example"></a>Exemplo de solicitação de GetUMProperties

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de GetUMProperties mostra como uma solicitação para obter as propriedades de Unificação de mensagens de uma caixa de correio de formulário.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUMProperties xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getumproperties-response-example"></a>Exemplo de resposta bem-sucedida GetUMProperties

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta GetUMProperties mostra uma resposta à solicitação de GetUMProperties.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetUMPropertiesResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <GetUMPropertiesResponse>
        <OofStatus>false</OofStatus> 
        <MissedCallNotificationEnabled>true</MissedCallNotificationEnabled> 
        <PlayOnPhoneDialString>12345</PlayOnPhoneDialString> 
        <TelephoneAccessNumbers>54321</TelephoneAccessNumbers> 
        <TelephoneAccessFolderEmail>AAAAAGsd2rbQLVtLobUGbrq/9IUBAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAAA==</TelephoneAccessFolderEmail> 
      </GetUMPropertiesResponse>
    </GetUMPropertiesResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Confira também



[GetUMProperties (serviço web de Unificação de mensagens)](getumproperties-um-web-service.md)
  
[GetUMPropertiesResponse (serviço web de Unificação de mensagens)](getumpropertiesresponse-um-web-service.md)

