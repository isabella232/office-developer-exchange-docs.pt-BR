---
title: Operação PlayOnPhone (serviço Web de Unificação de Mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- PlayOnPhone
api_type:
- schema
ms.assetid: 7d55be55-f8b6-4e96-a61e-26fa190217fd
description: A operação PlayOnPhone faz uma chamada de saída e reproduz uma mensagem especificada no telefone especificada pelo elemento DialString.
ms.openlocfilehash: 4d18727da18c36e6410c3cc6ab3bbf873993be72
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516561"
---
# <a name="playonphone-operation-um-web-service"></a>Operação PlayOnPhone (serviço Web de Unificação de Mensagens)

A operação PlayOnPhone faz uma chamada de saída e reproduz uma mensagem especificada no telefone especificada pelo **elemento DialString.** 
  
## <a name="playonphone-request-example"></a>Exemplo de solicitação do PlayOnPhone

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação do PlayOnPhone mostra como formar uma solicitação para fazer uma chamada de saída e reproduzir uma mensagem.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <PlayOnPhone xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <entryId>AAAAAGsd2rbQLVtLobUGbrq/9IUHAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAACxVpEl+KVVLl957wp//x6UAGAetcDUAAA==</entryId>
      <DialString>12345</DialString>
    </PlayOnPhone>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-playonphone-response-example"></a>Exemplo de resposta bem-sucedida do PlayOnPhone

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta Do PlayOnPhone mostra uma resposta à solicitação do PlayOnPhone.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <PlayOnPhoneResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <PlayOnPhoneResponse>NDEzYjEzNmMtZTE2Zi00NTJlLWI3YzctNDhkMTE3MDE3YjlmQGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</PlayOnPhoneResponse> 
    </PlayOnPhoneResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Confira também



[PlayOnPhone (serviço Web de Unificação de Mensagens)](playonphone-um-web-service.md)
  
[PlayOnPhoneResponse (serviço Web de Unificação de Mensagens)](playonphoneresponse-um-web-service.md)
  
[Operação PlayOnPhoneGreeting (serviço Web de Unificação de Mensagens)](playonphonegreeting-operation-um-web-service.md)

