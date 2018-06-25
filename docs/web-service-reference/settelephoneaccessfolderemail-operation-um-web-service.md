---
title: Operação de SetTelephoneAccessFolderEmail (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetTelephoneAccessFolderEmail
api_type:
- schema
ms.assetid: 2c92d914-bdee-4337-b3ea-0655fdb658e9
description: A operação SetTelephoneAccessFolderEmail define a pasta em que Unificação de mensagens lerá regressivos mensagens ao usuário pelo telefone.
ms.openlocfilehash: 9497e58f66b8efcf7e358aa529223942298a3bed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825459"
---
# <a name="settelephoneaccessfolderemail-operation-um-web-service"></a>Operação de SetTelephoneAccessFolderEmail (serviço web de Unificação de mensagens)

A operação SetTelephoneAccessFolderEmail define a pasta em que Unificação de mensagens lerá regressivos mensagens ao usuário pelo telefone.
  
## <a name="settelephoneaccessfolderemail-request-example"></a>Exemplo de solicitação de SetTelephoneAccessFolderEmail

### <a name="description"></a>Descrição

O exemplo a seguir de uma solicitação de SetTelephoneAccessFolderEmail mostra como formar uma solicitação para definir a pasta em que Unificação de mensagens lerá volta ao usuário pelo telefone.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetTelephoneAccessFolderEmail xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <base64FolderID>AAAAAGsd2rbQLVtLobUGbrq/9IUBAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAAA==</base64FolderID>
    </SetTelephoneAccessFolderEmail>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-settelephoneaccessfolderemail-response-example"></a>Exemplo de resposta bem-sucedida SetTelephoneAccessFolderEmail

### <a name="description"></a>Descrição

O exemplo a seguir de uma resposta SetTelephoneAccessFolderEmail mostra uma resposta à solicitação de SetTelephoneAccessFolderEmail.
  
### <a name="code"></a>Código

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetTelephoneAccessFolderEmailResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Confira também



[SetTelephoneAccessFolderEmail (serviço web de Unificação de mensagens)](settelephoneaccessfolderemail-um-web-service.md)
  
[SetTelephoneAccessFolderEmailResponse (serviço web de Unificação de mensagens)](settelephoneaccessfolderemailresponse-um-web-service.md)
  
[base64FolderId (serviço web de Unificação de mensagens)](base64folderid-um-web-service.md)

