---
title: Operação GetUMProperties (serviço Web da UM)
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
ms.openlocfilehash: 42176d9cd0288af6515aeea616a4f216a419410c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462469"
---
# <a name="getumproperties-operation-um-web-service"></a>Operação GetUMProperties (serviço Web da UM)

A operação GetUMProperties obtém todas as propriedades de Unificação de mensagens para a caixa de correio do usuário que está fazendo a solicitação.
  
## <a name="getumproperties-request-example"></a>Exemplo de solicitação GetUMProperties

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação GetUMProperties mostra como formar uma solicitação para obter as propriedades de Unificação de mensagens de uma caixa de correio.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUMProperties xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getumproperties-response-example"></a>Exemplo de resposta GetUMProperties bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta GetUMProperties mostra uma resposta à solicitação GetUMProperties.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetUMPropertiesResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="see-also"></a>Também consulte



[GetUMProperties (serviço Web da UM)](getumproperties-um-web-service.md)
  
[GetUMPropertiesResponse (serviço Web da UM)](getumpropertiesresponse-um-web-service.md)

