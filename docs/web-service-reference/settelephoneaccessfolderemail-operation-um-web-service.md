---
title: Operação SetTelephoneAccessFolderEmail (serviço Web da UM)
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
description: A operação SetTelephoneAccessFolderEmail define a pasta da qual a Unificação de mensagens lerá as mensagens para o usuário por telefone.
ms.openlocfilehash: a2bb630f812ca811b4cbe68db1308dc18e5d3ba0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467330"
---
# <a name="settelephoneaccessfolderemail-operation-um-web-service"></a><span data-ttu-id="95bae-103">Operação SetTelephoneAccessFolderEmail (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="95bae-103">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>

<span data-ttu-id="95bae-104">A operação SetTelephoneAccessFolderEmail define a pasta da qual a Unificação de mensagens lerá as mensagens para o usuário por telefone.</span><span class="sxs-lookup"><span data-stu-id="95bae-104">The SetTelephoneAccessFolderEmail operation sets the folder from which Unified Messaging will read back messages to the user over the telephone.</span></span>
  
## <a name="settelephoneaccessfolderemail-request-example"></a><span data-ttu-id="95bae-105">Exemplo de solicitação SetTelephoneAccessFolderEmail</span><span class="sxs-lookup"><span data-stu-id="95bae-105">SetTelephoneAccessFolderEmail request example</span></span>

### <a name="description"></a><span data-ttu-id="95bae-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="95bae-106">Description</span></span>

<span data-ttu-id="95bae-107">O exemplo a seguir de uma solicitação SetTelephoneAccessFolderEmail mostra como formar uma solicitação para definir a pasta da qual a Unificação de mensagens lerá para o usuário por telefone.</span><span class="sxs-lookup"><span data-stu-id="95bae-107">The following example of a SetTelephoneAccessFolderEmail request shows how to form a request to set the folder from which Unified Messaging will read back to the user over the telephone.</span></span>
  
### <a name="code"></a><span data-ttu-id="95bae-108">Código</span><span class="sxs-lookup"><span data-stu-id="95bae-108">Code</span></span>

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

## <a name="successful-settelephoneaccessfolderemail-response-example"></a><span data-ttu-id="95bae-109">Exemplo de resposta SetTelephoneAccessFolderEmail bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="95bae-109">Successful SetTelephoneAccessFolderEmail response example</span></span>

### <a name="description"></a><span data-ttu-id="95bae-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="95bae-110">Description</span></span>

<span data-ttu-id="95bae-111">O exemplo a seguir de uma resposta SetTelephoneAccessFolderEmail mostra uma resposta à solicitação SetTelephoneAccessFolderEmail.</span><span class="sxs-lookup"><span data-stu-id="95bae-111">The following example of a SetTelephoneAccessFolderEmail response shows a response to the SetTelephoneAccessFolderEmail request.</span></span>
  
### <a name="code"></a><span data-ttu-id="95bae-112">Código</span><span class="sxs-lookup"><span data-stu-id="95bae-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetTelephoneAccessFolderEmailResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="95bae-113">Confira também</span><span class="sxs-lookup"><span data-stu-id="95bae-113">See also</span></span>



[<span data-ttu-id="95bae-114">SetTelephoneAccessFolderEmail (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="95bae-114">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
[<span data-ttu-id="95bae-115">SetTelephoneAccessFolderEmailResponse (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="95bae-115">SetTelephoneAccessFolderEmailResponse (UM web service)</span></span>](settelephoneaccessfolderemailresponse-um-web-service.md)
  
[<span data-ttu-id="95bae-116">base64FolderId (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="95bae-116">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md)

