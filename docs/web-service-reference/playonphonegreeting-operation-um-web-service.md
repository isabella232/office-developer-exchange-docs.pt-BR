---
title: Operação PlayOnPhoneGreeting (serviço Web da UM)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhoneGreeting
api_type:
- schema
ms.assetid: 6deafc40-290b-4bce-9914-b6bcc529f38a
description: A operação PlayOnPhoneGreeting faz uma chamada de saída e reproduz uma das duas mensagens de saudação no telefone.
ms.openlocfilehash: 3af120b9ac8d7a368742fad2850c924228488662
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528890"
---
# <a name="playonphonegreeting-operation-um-web-service"></a>Operação PlayOnPhoneGreeting (serviço Web da UM)

A operação PlayOnPhoneGreeting faz uma chamada de saída e reproduz uma das duas mensagens de saudação no telefone.
  
## <a name="playonphonegreeting-request-example"></a>Exemplo de solicitação PlayOnPhoneGreeting

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação PlayOnPhoneGreeting mostra como formar uma solicitação para fazer uma chamada de saída e tocar a mensagem de saudação normal em um telefone.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <PlayOnPhoneGreeting xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <GreetingType>NormalCustom</GreetingType>
      <DialString>12345</DialString>
    </PlayOnPhoneGreeting>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-playonphonegreeting-response-example"></a>Exemplo de resposta PlayOnPhoneGreeting bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta PlayOnPhoneGreeting mostra uma resposta à solicitação PlayOnPhoneGreeting.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <PlayOnPhoneGreetingResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <PlayOnPhoneGreetingResponse>MjA4MTQ5MmItMTBmZC00ZGFmLThiMzEtNDllNDJjM2Y3MjIxQGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</PlayOnPhoneGreetingResponse> 
    </PlayOnPhoneGreetingResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Confira também



[PlayOnPhoneGreeting (serviço Web da UM)](playonphonegreeting-um-web-service.md)
  
[PlayOnPhoneGreetingResponse (serviço Web da UM)](playonphonegreetingresponse-um-web-service.md)
  
[Greetingtype (serviço Web da UM)](greetingtype-um-web-service.md)
  
[dialstring (serviço Web da UM)](dialstring-um-web-service.md)

