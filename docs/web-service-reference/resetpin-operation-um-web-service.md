---
title: Operação de ResetPIN (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- ResetPIN
api_type:
- schema
ms.assetid: c0f14a15-3389-4311-8bac-f87930c5f5d4
description: A operação ResetPIN altera o PIN (senha TUI) para um novo valor aleatório.
ms.openlocfilehash: e6417b86ce17c0d34fe857cf1209a18972cbef63
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825146"
---
# <a name="resetpin-operation-um-web-service"></a>Operação de ResetPIN (serviço web de Unificação de mensagens)

A operação ResetPIN altera o PIN (senha TUI) para um novo valor aleatório.
  
## <a name="remarks"></a>Comentários

A operação ResetPIN cria um novo PIN baseado nas diretivas de PIN. Se a operação for bem-sucedida, uma mensagem de email que contém o novo PIN é enviada à caixa de correio do usuário. Se a operação falhar, ele lançará uma exceção que contém informações sobre a falha.
  
## <a name="resetpin-request-example"></a>Exemplo de solicitação de ResetPIN

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de ResetPIN mostra como uma solicitação para redefinir o PIN para uma caixa de correio de formulário.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <ResetPIN xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-resetpin-response-example"></a>Exemplo de resposta bem-sucedida ResetPIN

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta ResetPIN mostra uma resposta à solicitação de ResetPIN.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResetPINResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Confira também



[ResetPIN (serviço web de Unificação de mensagens)](resetpin-um-web-service.md)
  
[ResetPINResponse (serviço web de Unificação de mensagens)](resetpinresponse-um-web-service.md)

