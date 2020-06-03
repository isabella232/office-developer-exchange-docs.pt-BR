---
title: Operação GetCallInfo (serviço Web da UM)
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
description: A operação GetCallInfo retorna o status da chamada de saída especificada por callid (serviço da Web da UM).
ms.openlocfilehash: 6b5664dfe16f9c74cc7175098145141b815a6355
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461237"
---
# <a name="getcallinfo-operation-um-web-service"></a><span data-ttu-id="95194-103">Operação GetCallInfo (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="95194-103">GetCallInfo operation (UM web service)</span></span>

<span data-ttu-id="95194-104">A operação GetCallInfo retorna o status da chamada de saída especificada por [callid (serviço da Web da um)](callid-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="95194-104">The GetCallInfo operation returns the status of the outbound call that is specified by [CallId (UM web service)](callid-um-web-service.md).</span></span>
  
## <a name="getcallinfo-request-example"></a><span data-ttu-id="95194-105">Exemplo de solicitação GetCallInfo</span><span class="sxs-lookup"><span data-stu-id="95194-105">GetCallInfo request example</span></span>

### <a name="description"></a><span data-ttu-id="95194-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="95194-106">Description</span></span>

<span data-ttu-id="95194-107">O exemplo a seguir de uma solicitação GetCallInfo mostra como formar uma solicitação para obter informações sobre uma chamada de saída especificada.</span><span class="sxs-lookup"><span data-stu-id="95194-107">The following example of a GetCallInfo request shows how to form a request to get information about a specified outbound call.</span></span>
  
### <a name="code"></a><span data-ttu-id="95194-108">Código</span><span class="sxs-lookup"><span data-stu-id="95194-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetCallInfo xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </GetCallInfo>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getcallinfo-response-example"></a><span data-ttu-id="95194-109">Exemplo de resposta GetCallInfo bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="95194-109">Successful GetCallInfo response example</span></span>

### <a name="description"></a><span data-ttu-id="95194-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="95194-110">Description</span></span>

<span data-ttu-id="95194-111">O exemplo a seguir de uma resposta GetCallInfo mostra uma resposta a uma solicitação GetCallInfo.</span><span class="sxs-lookup"><span data-stu-id="95194-111">The following example of a GetCallInfo response shows a response to a GetCallInfo request.</span></span>
  
### <a name="code"></a><span data-ttu-id="95194-112">Código</span><span class="sxs-lookup"><span data-stu-id="95194-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetCallInfoResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <GetCallInfoResponse>
        <CallState>Connected</CallState> 
        <EventCause>None</EventCause> 
      </GetCallInfoResponse>
    </GetCallInfoResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="95194-113">Confira também</span><span class="sxs-lookup"><span data-stu-id="95194-113">See also</span></span>



[<span data-ttu-id="95194-114">GetCallInfo (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="95194-114">GetCallInfo (UM web service)</span></span>](getcallinfo-um-web-service.md)
  
[<span data-ttu-id="95194-115">GetCallInfoResponse (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="95194-115">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
[<span data-ttu-id="95194-116">Callid (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="95194-116">CallId (UM web service)</span></span>](callid-um-web-service.md)
  
[<span data-ttu-id="95194-117">Callstate (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="95194-117">CallState (UM web service)</span></span>](callstate-um-web-service.md)
  
[<span data-ttu-id="95194-118">EventCause (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="95194-118">EventCause (UM web service)</span></span>](eventcause-um-web-service.md)

