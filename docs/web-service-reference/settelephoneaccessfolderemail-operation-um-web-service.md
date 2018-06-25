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
# <a name="settelephoneaccessfolderemail-operation-um-web-service"></a><span data-ttu-id="c2b45-103">Operação de SetTelephoneAccessFolderEmail (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="c2b45-103">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>

<span data-ttu-id="c2b45-104">A operação SetTelephoneAccessFolderEmail define a pasta em que Unificação de mensagens lerá regressivos mensagens ao usuário pelo telefone.</span><span class="sxs-lookup"><span data-stu-id="c2b45-104">The SetTelephoneAccessFolderEmail operation sets the folder from which Unified Messaging will read back messages to the user over the telephone.</span></span>
  
## <a name="settelephoneaccessfolderemail-request-example"></a><span data-ttu-id="c2b45-105">Exemplo de solicitação de SetTelephoneAccessFolderEmail</span><span class="sxs-lookup"><span data-stu-id="c2b45-105">SetTelephoneAccessFolderEmail request example</span></span>

### <a name="description"></a><span data-ttu-id="c2b45-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2b45-106">Description</span></span>

<span data-ttu-id="c2b45-107">O exemplo a seguir de uma solicitação de SetTelephoneAccessFolderEmail mostra como formar uma solicitação para definir a pasta em que Unificação de mensagens lerá volta ao usuário pelo telefone.</span><span class="sxs-lookup"><span data-stu-id="c2b45-107">The following example of a SetTelephoneAccessFolderEmail request shows how to form a request to set the folder from which Unified Messaging will read back to the user over the telephone.</span></span>
  
### <a name="code"></a><span data-ttu-id="c2b45-108">Código</span><span class="sxs-lookup"><span data-stu-id="c2b45-108">Code</span></span>

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

## <a name="successful-settelephoneaccessfolderemail-response-example"></a><span data-ttu-id="c2b45-109">Exemplo de resposta bem-sucedida SetTelephoneAccessFolderEmail</span><span class="sxs-lookup"><span data-stu-id="c2b45-109">Successful SetTelephoneAccessFolderEmail response example</span></span>

### <a name="description"></a><span data-ttu-id="c2b45-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2b45-110">Description</span></span>

<span data-ttu-id="c2b45-111">O exemplo a seguir de uma resposta SetTelephoneAccessFolderEmail mostra uma resposta à solicitação de SetTelephoneAccessFolderEmail.</span><span class="sxs-lookup"><span data-stu-id="c2b45-111">The following example of a SetTelephoneAccessFolderEmail response shows a response to the SetTelephoneAccessFolderEmail request.</span></span>
  
### <a name="code"></a><span data-ttu-id="c2b45-112">Código</span><span class="sxs-lookup"><span data-stu-id="c2b45-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetTelephoneAccessFolderEmailResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="c2b45-113">Confira também</span><span class="sxs-lookup"><span data-stu-id="c2b45-113">See also</span></span>



[<span data-ttu-id="c2b45-114">SetTelephoneAccessFolderEmail (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="c2b45-114">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
[<span data-ttu-id="c2b45-115">SetTelephoneAccessFolderEmailResponse (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="c2b45-115">SetTelephoneAccessFolderEmailResponse (UM web service)</span></span>](settelephoneaccessfolderemailresponse-um-web-service.md)
  
[<span data-ttu-id="c2b45-116">base64FolderId (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="c2b45-116">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md)

