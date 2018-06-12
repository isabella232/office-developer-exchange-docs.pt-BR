---
title: Operação de PlayOnPhoneGreeting (serviço web de Unificação de mensagens)
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
description: A operação PlayOnPhoneGreeting faz uma chamada de saída e reproduz uma das mensagens de dois saudação pelo telefone.
ms.openlocfilehash: 85ba76c7638911678c1ef1aef88f47fdab2c6a4e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824828"
---
# <a name="playonphonegreeting-operation-um-web-service"></a>Operação de PlayOnPhoneGreeting (serviço web de Unificação de mensagens)

A operação PlayOnPhoneGreeting faz uma chamada de saída e reproduz uma das mensagens de dois saudação pelo telefone.
  
## <a name="playonphonegreeting-request-example"></a>Exemplo de solicitação de PlayOnPhoneGreeting

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de PlayOnPhoneGreeting mostra como uma solicitação para fazer uma chamada realizada e reproduzir a mensagem de saudação normal em um telefone de formulário.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <PlayOnPhoneGreeting xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <GreetingType>NormalCustom</GreetingType>
      <DialString>12345</DialString>
    </PlayOnPhoneGreeting>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-playonphonegreeting-response-example"></a>Exemplo de resposta bem-sucedida PlayOnPhoneGreeting

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta PlayOnPhoneGreeting mostra uma resposta à solicitação de PlayOnPhoneGreeting.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <PlayOnPhoneGreetingResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <PlayOnPhoneGreetingResponse>MjA4MTQ5MmItMTBmZC00ZGFmLThiMzEtNDllNDJjM2Y3MjIxQGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</PlayOnPhoneGreetingResponse> 
    </PlayOnPhoneGreetingResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Confira também



[PlayOnPhoneGreeting (serviço web de Unificação de mensagens)](playonphonegreeting-um-web-service.md)
  
[PlayOnPhoneGreetingResponse (serviço web de Unificação de mensagens)](playonphonegreetingresponse-um-web-service.md)
  
[GreetingType (serviço web de Unificação de mensagens)](greetingtype-um-web-service.md)
  
[dialString (serviço web de Unificação de mensagens)](dialstring-um-web-service.md)

