---
title: Operação SetTelephoneAccessFolderEmail (serviço Web de Unificação de Mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- SetTelephoneAccessFolderEmail
api_type:
- schema
ms.assetid: 2c92d914-bdee-4337-b3ea-0655fdb658e9
description: A operação SetTelephoneAccessFolderEmail define a pasta da qual a Unificação de Mensagens lerá mensagens para o usuário por telefone.
ms.openlocfilehash: cf8e80e021d6467ba3a724cc0d04e165e00e8397
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544714"
---
# <a name="settelephoneaccessfolderemail-operation-um-web-service"></a>Operação SetTelephoneAccessFolderEmail (serviço Web de Unificação de Mensagens)

A operação SetTelephoneAccessFolderEmail define a pasta da qual a Unificação de Mensagens lerá mensagens para o usuário por telefone.
  
## <a name="settelephoneaccessfolderemail-request-example"></a>Exemplo de solicitação SetTelephoneAccessFolderEmail

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação SetTelephoneAccessFolderEmail mostra como formar uma solicitação para definir a pasta da qual a Unificação de Mensagens será lida para o usuário por telefone.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetTelephoneAccessFolderEmail xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <base64FolderID>AAAAAGsd2rbQLVtLobUGbrq/9IUBAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAAA==</base64FolderID>
    </SetTelephoneAccessFolderEmail>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-settelephoneaccessfolderemail-response-example"></a>Exemplo de resposta SetTelephoneAccessFolderEmail bem-sucedido

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta SetTelephoneAccessFolderEmail mostra uma resposta à solicitação SetTelephoneAccessFolderEmail.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetTelephoneAccessFolderEmailResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Confira também



[SetTelephoneAccessFolderEmail (serviço Web de Unificação de Mensagens)](settelephoneaccessfolderemail-um-web-service.md)
  
[SetTelephoneAccessFolderEmailResponse (serviço Web de Unificação de Mensagens)](settelephoneaccessfolderemailresponse-um-web-service.md)
  
[base64FolderId (serviço Web de Unificação de mensagens)](base64folderid-um-web-service.md)

