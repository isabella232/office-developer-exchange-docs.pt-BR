---
title: Operação de SetPlayOnPhoneDialString (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetPlayOnPhoneDialString
api_type:
- schema
ms.assetid: a68479f2-d900-4dd8-a5ce-dbea8247e841
description: A operação SetPlayOnPhoneDialString define a sequência de discagem para usar como o padrão para a operação PlayOnPhone (serviço web de Unificação de mensagens) e a operação de PlayOnPhoneGreeting (serviço web de Unificação de mensagens).
ms.openlocfilehash: 0d1a879784740777e5eab0cbd5f85e59a6479461
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825446"
---
# <a name="setplayonphonedialstring-operation-um-web-service"></a>Operação de SetPlayOnPhoneDialString (serviço web de Unificação de mensagens)

A operação SetPlayOnPhoneDialString define a sequência de discagem para usar como o padrão para a [operação PlayOnPhone (serviço web de Unificação de mensagens)](playonphone-operation-um-web-service.md) e a [operação PlayOnPhoneGreeting (serviço web de Unificação de mensagens)](playonphonegreeting-operation-um-web-service.md).
  
## <a name="setplayonphonedialstring-request-example"></a>Exemplo de solicitação de SetPlayOnPhoneDialString

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de SetPlayOnPhoneDialString mostra como uma solicitação para definir a sequência de discagem padrão para uma caixa de correio de formulário.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetPlayOnPhoneDialString xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <dialString>12345</dialString>
    </SetPlayOnPhoneDialString>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setplayonphonedialstring-response-example"></a>Exemplo de resposta bem-sucedida SetPlayOnPhoneDialString

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta SetPlayOnePhoneDialString mostra uma resposta à solicitação de SetPlayOnPhoneDialString.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetPlayOnPhoneDialStringResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Confira também



[SetPlayOnPhoneDialString (serviço web de Unificação de mensagens)](setplayonphonedialstring-um-web-service.md)
  
[SetPlayOnPhoneDialStringResponse (serviço web de Unificação de mensagens)](setplayonphonedialstringresponse-um-web-service.md)
  
[dialString (serviço web de Unificação de mensagens)](dialstring-um-web-service.md)

