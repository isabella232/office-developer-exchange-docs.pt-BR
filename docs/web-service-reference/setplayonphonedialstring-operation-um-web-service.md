---
title: Operação SetPlayOnPhoneDialString (serviço Web da UM)
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
description: A operação SetPlayOnPhoneDialString define a cadeia de caracteres de discagem a ser usada como padrão para a operação PlayOnPhone (serviço Web da UM) e a operação PlayOnPhoneGreeting (serviço Web da UM).
ms.openlocfilehash: 7df806eedc2d6d037394f31ec4ccbfe28aaf3372
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458639"
---
# <a name="setplayonphonedialstring-operation-um-web-service"></a>Operação SetPlayOnPhoneDialString (serviço Web da UM)

A operação SetPlayOnPhoneDialString define a cadeia de caracteres de discagem a ser usada como padrão para a [operação PlayOnPhone (serviço Web da um)](playonphone-operation-um-web-service.md) e a [operação PlayOnPhoneGreeting (serviço Web da um)](playonphonegreeting-operation-um-web-service.md).
  
## <a name="setplayonphonedialstring-request-example"></a>Exemplo de solicitação SetPlayOnPhoneDialString

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

## <a name="successful-setplayonphonedialstring-response-example"></a>Exemplo de resposta SetPlayOnPhoneDialString bem-sucedida

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

## <a name="see-also"></a>Também consulte



[SetPlayOnPhoneDialString (serviço Web da UM)](setplayonphonedialstring-um-web-service.md)
  
[SetPlayOnPhoneDialStringResponse (serviço Web da UM)](setplayonphonedialstringresponse-um-web-service.md)
  
[dialstring (serviço Web da UM)](dialstring-um-web-service.md)

