---
title: Operação GetUMProperties (serviço Web de Unificação de Mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- GetUMProperties
api_type:
- schema
ms.assetid: 301fb9a3-67df-44c4-8ffe-0600237fc344
description: A operação GetUMProperties obtém todas as propriedades de Unificação de Mensagens para a caixa de correio do usuário que está fazendo a solicitação.
ms.openlocfilehash: 8d051196e83e1f927692b517e1ab3e95bb0060db
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515814"
---
# <a name="getumproperties-operation-um-web-service"></a>Operação GetUMProperties (serviço Web de Unificação de Mensagens)

A operação GetUMProperties obtém todas as propriedades de Unificação de Mensagens para a caixa de correio do usuário que está fazendo a solicitação.
  
## <a name="getumproperties-request-example"></a>Exemplo de solicitação GetUMProperties

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação GetUMProperties mostra como formar uma solicitação para obter as propriedades de Unificação de Mensagens de uma caixa de correio.
  
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

## <a name="see-also"></a>Confira também



[GetUMProperties (serviço Web de Unificação de Mensagens)](getumproperties-um-web-service.md)
  
[GetUMPropertiesResponse (serviço Web de Unificação de Mensagens)](getumpropertiesresponse-um-web-service.md)

