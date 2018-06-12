---
title: Operação de GetCallInfo (serviço web de Unificação de mensagens)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetCallInfo
api_type:
- schema
ms.assetid: 6bccd418-caf7-4eb9-8a6f-410e56a635c3
description: A operação GetCallInfo retorna o status da chamada de saída que é especificada pelo CallId (serviço web de Unificação de mensagens).
ms.openlocfilehash: 36f9cba3690520ebb457a4cb2bfbcde3fea4b8dc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752417"
---
# <a name="getcallinfo-operation-um-web-service"></a><span data-ttu-id="5746f-103">Operação de GetCallInfo (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="5746f-103">GetCallInfo operation (UM web service)</span></span>

<span data-ttu-id="5746f-104">A operação GetCallInfo retorna o status da chamada de saída que é especificada pelo [CallId (serviço web de Unificação de mensagens)](callid-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="5746f-104">The GetCallInfo operation returns the status of the outbound call that is specified by [CallId (UM web service)](callid-um-web-service.md).</span></span>
  
## <a name="getcallinfo-request-example"></a><span data-ttu-id="5746f-105">Exemplo de solicitação de GetCallInfo</span><span class="sxs-lookup"><span data-stu-id="5746f-105">GetCallInfo request example</span></span>

### <a name="description"></a><span data-ttu-id="5746f-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="5746f-106">Description</span></span>

<span data-ttu-id="5746f-107">O exemplo a seguir de uma solicitação de GetCallInfo mostra como formar uma solicitação para obter mais informações sobre uma chamada de saída especificada.</span><span class="sxs-lookup"><span data-stu-id="5746f-107">The following example of a GetCallInfo request shows how to form a request to get information about a specified outbound call.</span></span>
  
### <a name="code"></a><span data-ttu-id="5746f-108">Código</span><span class="sxs-lookup"><span data-stu-id="5746f-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetCallInfo xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </GetCallInfo>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getcallinfo-response-example"></a><span data-ttu-id="5746f-109">Exemplo de resposta bem-sucedida GetCallInfo</span><span class="sxs-lookup"><span data-stu-id="5746f-109">Successful GetCallInfo response example</span></span>

### <a name="description"></a><span data-ttu-id="5746f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5746f-110">Description</span></span>

<span data-ttu-id="5746f-111">O exemplo a seguir de uma resposta GetCallInfo mostra uma resposta a uma solicitação GetCallInfo.</span><span class="sxs-lookup"><span data-stu-id="5746f-111">The following example of a GetCallInfo response shows a response to a GetCallInfo request.</span></span>
  
### <a name="code"></a><span data-ttu-id="5746f-112">Código</span><span class="sxs-lookup"><span data-stu-id="5746f-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetCallInfoResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <GetCallInfoResponse>
        <CallState>Connected</CallState> 
        <EventCause>None</EventCause> 
      </GetCallInfoResponse>
    </GetCallInfoResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="5746f-113">Confira também</span><span class="sxs-lookup"><span data-stu-id="5746f-113">See also</span></span>



[<span data-ttu-id="5746f-114">GetCallInfo (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="5746f-114">GetCallInfo (UM web service)</span></span>](getcallinfo-um-web-service.md)
  
[<span data-ttu-id="5746f-115">GetCallInfoResponse (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="5746f-115">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
[<span data-ttu-id="5746f-116">CallId (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="5746f-116">CallId (UM web service)</span></span>](callid-um-web-service.md)
  
[<span data-ttu-id="5746f-117">CallState (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="5746f-117">CallState (UM web service)</span></span>](callstate-um-web-service.md)
  
[<span data-ttu-id="5746f-118">EventCause (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="5746f-118">EventCause (UM web service)</span></span>](eventcause-um-web-service.md)

