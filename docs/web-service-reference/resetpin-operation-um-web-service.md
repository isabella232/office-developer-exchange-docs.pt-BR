---
title: Operação ResetPIN (serviço Web de Unificação de Mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- ResetPIN
api_type:
- schema
ms.assetid: c0f14a15-3389-4311-8bac-f87930c5f5d4
description: A operação ResetPIN altera o PIN (senha TUI) para um novo valor aleatório.
ms.openlocfilehash: 12f1e5719184df84f6c29ab3d02cc362f87abc76
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539105"
---
# <a name="resetpin-operation-um-web-service"></a>Operação ResetPIN (serviço Web de Unificação de Mensagens)

A operação ResetPIN altera o PIN (senha TUI) para um novo valor aleatório.
  
## <a name="remarks"></a>Comentários

A operação ResetPIN cria um novo PIN com base nas políticas de PIN. Se a operação for bem-sucedida, uma mensagem de email que contém o novo PIN será enviada para a caixa de correio do usuário. Se a operação falhar, ela lançará uma exceção que contém informações sobre a falha.
  
## <a name="resetpin-request-example"></a>Exemplo de solicitação ResetPIN

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação ResetPIN mostra como formar uma solicitação para redefinir o PIN de uma caixa de correio.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <ResetPIN xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-resetpin-response-example"></a>Exemplo de resposta ResetPIN bem-sucedida

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta ResetPIN mostra uma resposta à solicitação ResetPIN.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResetPINResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Confira também



[ResetPIN (serviço Web de Unificação de Mensagens)](resetpin-um-web-service.md)
  
[ResetPINResponse (serviço Web de Unificação de Mensagens)](resetpinresponse-um-web-service.md)

