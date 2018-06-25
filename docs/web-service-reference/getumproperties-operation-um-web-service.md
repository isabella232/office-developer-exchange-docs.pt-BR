---
title: Operação de GetUMProperties (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetUMProperties
api_type:
- schema
ms.assetid: 301fb9a3-67df-44c4-8ffe-0600237fc344
description: A operação GetUMProperties obtém todas as propriedades de Unificação de mensagens para a caixa de correio do usuário que está fazendo a solicitação.
ms.openlocfilehash: 8878099bbd907fe0648f7d64dde3cd9600c2c45f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823678"
---
# <a name="getumproperties-operation-um-web-service"></a><span data-ttu-id="2dc4d-103">Operação de GetUMProperties (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="2dc4d-103">GetUMProperties operation (UM web service)</span></span>

<span data-ttu-id="2dc4d-104">A operação GetUMProperties obtém todas as propriedades de Unificação de mensagens para a caixa de correio do usuário que está fazendo a solicitação.</span><span class="sxs-lookup"><span data-stu-id="2dc4d-104">The GetUMProperties operation gets all the Unified Messaging properties for the mailbox of the user who is making the request.</span></span>
  
## <a name="getumproperties-request-example"></a><span data-ttu-id="2dc4d-105">Exemplo de solicitação de GetUMProperties</span><span class="sxs-lookup"><span data-stu-id="2dc4d-105">GetUMProperties request example</span></span>

### <a name="description"></a><span data-ttu-id="2dc4d-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="2dc4d-106">Description</span></span>

<span data-ttu-id="2dc4d-107">O exemplo a seguir de uma solicitação de GetUMProperties mostra como uma solicitação para obter as propriedades de Unificação de mensagens de uma caixa de correio de formulário.</span><span class="sxs-lookup"><span data-stu-id="2dc4d-107">The following example of a GetUMProperties request shows how to form a request to get the Unified Messaging properties of a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="2dc4d-108">Código</span><span class="sxs-lookup"><span data-stu-id="2dc4d-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUMProperties xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getumproperties-response-example"></a><span data-ttu-id="2dc4d-109">Exemplo de resposta bem-sucedida GetUMProperties</span><span class="sxs-lookup"><span data-stu-id="2dc4d-109">Successful GetUMProperties response example</span></span>

### <a name="description"></a><span data-ttu-id="2dc4d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2dc4d-110">Description</span></span>

<span data-ttu-id="2dc4d-111">O exemplo a seguir de uma resposta GetUMProperties mostra uma resposta à solicitação de GetUMProperties.</span><span class="sxs-lookup"><span data-stu-id="2dc4d-111">The following example of a GetUMProperties response shows a response to the GetUMProperties request.</span></span>
  
### <a name="code"></a><span data-ttu-id="2dc4d-112">Código</span><span class="sxs-lookup"><span data-stu-id="2dc4d-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetUMPropertiesResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <GetUMPropertiesResponse>
        <OofStatus>false</OofStatus> 
        <MissedCallNotificationEnabled>true</MissedCallNotificationEnabled> 
        <PlayOnPhoneDialString>12345</PlayOnPhoneDialString> 
        <TelephoneAccessNumbers>54321</TelephoneAccessNumbers> 
        <TelephoneAccessFolderEmail>AAAAAGsd2rbQLVtLobUGbrq/9IUBAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAAA==</TelephoneAccessFolderEmail> 
      </GetUMPropertiesResponse>
    </GetUMPropertiesResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="2dc4d-113">Confira também</span><span class="sxs-lookup"><span data-stu-id="2dc4d-113">See also</span></span>



[<span data-ttu-id="2dc4d-114">GetUMProperties (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="2dc4d-114">GetUMProperties (UM web service)</span></span>](getumproperties-um-web-service.md)
  
[<span data-ttu-id="2dc4d-115">GetUMPropertiesResponse (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="2dc4d-115">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)

