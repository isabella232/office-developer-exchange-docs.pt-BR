---
title: Operação de PlayOnPhone (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhone
api_type:
- schema
ms.assetid: 7d55be55-f8b6-4e96-a61e-26fa190217fd
description: A operação PlayOnPhone faz uma chamada de saída e reproduz uma mensagem especificada pelo telefone especificado pelo elemento DialString.
ms.openlocfilehash: b55bb45d6654f57503879f33e1cd5013ddb69a2e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824818"
---
# <a name="playonphone-operation-um-web-service"></a>Operação de PlayOnPhone (serviço web de Unificação de mensagens)

A operação PlayOnPhone faz uma chamada de saída e reproduz uma mensagem especificada pelo telefone especificado pelo elemento **DialString** . 
  
## <a name="playonphone-request-example"></a>Exemplo de solicitação de PlayOnPhone

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de PlayOnPhone mostra como uma solicitação para fazer uma chamada realizada e reproduzir uma mensagem de formulário.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <PlayOnPhone xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <entryId>AAAAAGsd2rbQLVtLobUGbrq/9IUHAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAACxVpEl+KVVLl957wp//x6UAGAetcDUAAA==</entryId>
      <DialString>12345</DialString>
    </PlayOnPhone>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-playonphone-response-example"></a>Exemplo de resposta bem-sucedida PlayOnPhone

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta PlayOnPhone mostra uma resposta à solicitação de PlayOnPhone.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <PlayOnPhoneResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <PlayOnPhoneResponse>NDEzYjEzNmMtZTE2Zi00NTJlLWI3YzctNDhkMTE3MDE3YjlmQGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</PlayOnPhoneResponse> 
    </PlayOnPhoneResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Confira também



[PlayOnPhone (serviço web de Unificação de mensagens)](playonphone-um-web-service.md)
  
[PlayOnPhoneResponse (serviço web de Unificação de mensagens)](playonphoneresponse-um-web-service.md)
  
[Operação de PlayOnPhoneGreeting (serviço web de Unificação de mensagens)](playonphonegreeting-operation-um-web-service.md)

