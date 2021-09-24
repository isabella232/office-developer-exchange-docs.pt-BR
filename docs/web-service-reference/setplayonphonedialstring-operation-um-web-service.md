---
title: Operação SetPlayOnPhoneDialString (serviço Web de Unificação de Mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- SetPlayOnPhoneDialString
api_type:
- schema
ms.assetid: a68479f2-d900-4dd8-a5ce-dbea8247e841
description: A operação SetPlayOnPhoneDialString define a cadeia de caracteres de discagem a ser usada como padrão para a operação PlayOnPhone (serviço Web de UM) e a operação PlayOnPhoneGreeting (serviço Web de UM).
ms.openlocfilehash: 89f83d7b0a1d56cb0adeccbf4fa0bb67f1197253
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531906"
---
# <a name="setplayonphonedialstring-operation-um-web-service"></a>Operação SetPlayOnPhoneDialString (serviço Web de Unificação de Mensagens)

A operação SetPlayOnPhoneDialString define a cadeia de caracteres de discagem a ser usada como o padrão para a operação [PlayOnPhone (serviço Web de UM)](playonphone-operation-um-web-service.md) e a operação [PlayOnPhoneGreeting (serviço Web](playonphonegreeting-operation-um-web-service.md)de UM) .
  
## <a name="setplayonphonedialstring-request-example"></a>Exemplo da solicitação SetPlayOnPhoneDialString

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação SetPlayOnPhoneDialString mostra como formar uma solicitação para definir a cadeia de caracteres de discagem padrão para uma caixa de correio.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetPlayOnPhoneDialString xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <dialString>12345</dialString>
    </SetPlayOnPhoneDialString>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setplayonphonedialstring-response-example"></a>Exemplo da resposta SetPlayOnPhoneDialString bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta SetPlayOnePhoneDialString mostra uma resposta à solicitação SetPlayOnPhoneDialString.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetPlayOnPhoneDialStringResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Confira também



[SetPlayOnPhoneDialString (serviço Web de Unificação de Mensagens)](setplayonphonedialstring-um-web-service.md)
  
[SetPlayOnPhoneDialStringResponse (serviço Web de Unificação de Mensagens)](setplayonphonedialstringresponse-um-web-service.md)
  
[dialString (serviço Web de Unificação de Mensagens)](dialstring-um-web-service.md)

