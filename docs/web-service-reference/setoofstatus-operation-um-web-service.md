---
title: Operação de SetOofStatus (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetOofStatus
api_type:
- schema
ms.assetid: 97c271e9-506e-43eb-89cd-46803fc47ee5
description: A operação SetOofStatus define um valor que indica se a saudação de ausência temporária deve ser reproduzida para o usuário que faz com que a solicitação.
ms.openlocfilehash: 2bb1deeec8ddb5be56979bfb2fae3396672298a3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825445"
---
# <a name="setoofstatus-operation-um-web-service"></a><span data-ttu-id="6a405-103">Operação de SetOofStatus (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="6a405-103">SetOofStatus operation (UM web service)</span></span>

<span data-ttu-id="6a405-104">A operação SetOofStatus define um valor que indica se a saudação de ausência temporária deve ser reproduzida para o usuário que faz com que a solicitação.</span><span class="sxs-lookup"><span data-stu-id="6a405-104">The SetOofStatus operation sets a value that indicates whether the Out of Office (OOF) greeting should be played for the user who makes the request.</span></span>
  
## <a name="setoofstatus-request-example"></a><span data-ttu-id="6a405-105">Exemplo de solicitação de SetOofStatus</span><span class="sxs-lookup"><span data-stu-id="6a405-105">SetOofStatus request example</span></span>

### <a name="description"></a><span data-ttu-id="6a405-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a405-106">Description</span></span>

<span data-ttu-id="6a405-107">O exemplo a seguir de uma solicitação de SetOofStatus mostra como uma solicitação para ativar a saudação de ausência temporária para uma caixa de correio de formulário.</span><span class="sxs-lookup"><span data-stu-id="6a405-107">The following example of a SetOofStatus request shows how to form a request to enable the Out of Office greeting for a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="6a405-108">Código</span><span class="sxs-lookup"><span data-stu-id="6a405-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetOofStatus xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetOofStatus>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setoofstatus-response-example"></a><span data-ttu-id="6a405-109">Exemplo de resposta bem-sucedida SetOofStatus</span><span class="sxs-lookup"><span data-stu-id="6a405-109">Successful SetOofStatus response example</span></span>

### <a name="description"></a><span data-ttu-id="6a405-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a405-110">Description</span></span>

<span data-ttu-id="6a405-111">O exemplo a seguir de uma resposta SetOofStatus mostra uma resposta à solicitação de SetOofStatus.</span><span class="sxs-lookup"><span data-stu-id="6a405-111">The following example of a SetOofStatus response shows a response to the SetOofStatus request.</span></span>
  
### <a name="code"></a><span data-ttu-id="6a405-112">Código</span><span class="sxs-lookup"><span data-stu-id="6a405-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetOofStatusResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="6a405-113">Confira também</span><span class="sxs-lookup"><span data-stu-id="6a405-113">See also</span></span>



[<span data-ttu-id="6a405-114">SetOofStatus (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="6a405-114">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md)
  
[<span data-ttu-id="6a405-115">SetOofStatusResponse (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="6a405-115">SetOofStatusResponse (UM web service)</span></span>](setoofstatusresponse-um-web-service.md)
  
[<span data-ttu-id="6a405-116">Status (UM serviço web - SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="6a405-116">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md)

