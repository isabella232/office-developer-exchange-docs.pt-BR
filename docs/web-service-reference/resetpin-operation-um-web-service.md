---
title: Operação ResetPIN (serviço Web da UM)
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
description: A operação ResetPIN altera o PIN (TUI senha) para um novo valor aleatório.
ms.openlocfilehash: 8de64ce7a47e9c426f8eb9298e1ca00508fb616c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465489"
---
# <a name="resetpin-operation-um-web-service"></a>Operação ResetPIN (serviço Web da UM)

A operação ResetPIN altera o PIN (TUI senha) para um novo valor aleatório.
  
## <a name="remarks"></a>Comentários

A operação ResetPIN cria um novo PIN com base nas políticas de PIN. Se a operação for bem-sucedida, uma mensagem de email que contenha o novo PIN será enviada para a caixa de correio do usuário. Se a operação falhar, ela gerará uma exceção que contém informações sobre a falha.
  
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



[ResetPIN (serviço Web da UM)](resetpin-um-web-service.md)
  
[ResetPINResponse (serviço Web da UM)](resetpinresponse-um-web-service.md)

