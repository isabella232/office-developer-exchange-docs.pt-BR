---
title: Operação PlayOnPhoneGreeting (serviço Web de Unificação de Mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- PlayOnPhoneGreeting
api_type:
- schema
ms.assetid: 6deafc40-290b-4bce-9914-b6bcc529f38a
description: A operação PlayOnPhoneGreeting faz uma chamada de saída e reproduz uma das duas mensagens de saudação no telefone.
ms.openlocfilehash: 540cd44d35e70e2588446996aec19aeab17f83e9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543132"
---
# <a name="playonphonegreeting-operation-um-web-service"></a>Operação PlayOnPhoneGreeting (serviço Web de Unificação de Mensagens)

A operação PlayOnPhoneGreeting faz uma chamada de saída e reproduz uma das duas mensagens de saudação no telefone.
  
## <a name="playonphonegreeting-request-example"></a>Exemplo da solicitação PlayOnPhoneGreeting

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação PlayOnPhoneGreeting mostra como formar uma solicitação para fazer uma chamada de saída e reproduzir a mensagem de saudação normal em um telefone.
  
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

## <a name="successful-playonphonegreeting-response-example"></a>Exemplo de resposta bem-sucedida do PlayOnPhoneGreeting

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



[PlayOnPhoneGreeting (serviço Web de Unificação de Mensagens)](playonphonegreeting-um-web-service.md)
  
[PlayOnPhoneGreetingResponse (serviço Web de Unificação de Mensagens)](playonphonegreetingresponse-um-web-service.md)
  
[GreetingType (serviço Web de Unificação de Mensagens)](greetingtype-um-web-service.md)
  
[dialString (serviço Web de Unificação de Mensagens)](dialstring-um-web-service.md)

