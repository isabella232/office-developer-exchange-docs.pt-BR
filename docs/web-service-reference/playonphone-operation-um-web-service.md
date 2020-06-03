---
title: Operação PlayOnPhone (serviço Web da UM)
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
description: A operação PlayOnPhone faz uma chamada de saída e reproduz uma mensagem especificada pelo telefone que é especificado pelo elemento de discagem.
ms.openlocfilehash: c5ff82bcd822aa2c659d1782ea4a1349d198bc80
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466231"
---
# <a name="playonphone-operation-um-web-service"></a>Operação PlayOnPhone (serviço Web da UM)

A operação PlayOnPhone faz uma chamada de saída e reproduz uma mensagem especificada pelo telefone que é especificado pelo elemento de **discagem** . 
  
## <a name="playonphone-request-example"></a>Exemplo de solicitação PlayOnPhone

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação PlayOnPhone mostra como formar uma solicitação para fazer uma chamada de saída e reproduzir uma mensagem.
  
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

## <a name="successful-playonphone-response-example"></a>Exemplo de resposta PlayOnPhone bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta PlayOnPhone mostra uma resposta à solicitação PlayOnPhone.
  
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



[PlayOnPhone (serviço Web da UM)](playonphone-um-web-service.md)
  
[PlayOnPhoneResponse (serviço Web da UM)](playonphoneresponse-um-web-service.md)
  
[Operação PlayOnPhoneGreeting (serviço Web da UM)](playonphonegreeting-operation-um-web-service.md)

