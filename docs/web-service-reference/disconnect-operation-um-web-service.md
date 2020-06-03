---
title: Operação de desconexão (serviço Web da UM)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Disconnect
api_type:
- schema
ms.assetid: a987000b-d6e6-49d7-944c-e9c278d0236f
description: A operação de desconexão encerra a chamada identificada pelo callid especificado (serviço da Web da UM).
ms.openlocfilehash: a1268f9ea3d879f472e019bf1847fc13d65d1819
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529067"
---
# <a name="disconnect-operation-um-web-service"></a><span data-ttu-id="658cc-103">Operação de desconexão (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="658cc-103">Disconnect operation (UM web service)</span></span>

<span data-ttu-id="658cc-104">A operação de desconexão encerra a chamada identificada pelo [callid especificado (serviço da Web da um)](callid-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="658cc-104">The Disconnect operation terminates the call that is identified by the specified [CallId (UM web service)](callid-um-web-service.md).</span></span>
  
## <a name="disconnect-request-example"></a><span data-ttu-id="658cc-105">Exemplo de solicitação de desconexão</span><span class="sxs-lookup"><span data-stu-id="658cc-105">Disconnect request example</span></span>

### <a name="description"></a><span data-ttu-id="658cc-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="658cc-106">Description</span></span>

<span data-ttu-id="658cc-107">O exemplo a seguir de uma solicitação de desconexão mostra como formar uma solicitação para desconectar uma chamada.</span><span class="sxs-lookup"><span data-stu-id="658cc-107">The following example of a Disconnect request shows how to form a request to disconnect a call.</span></span>
  
### <a name="code"></a><span data-ttu-id="658cc-108">Código</span><span class="sxs-lookup"><span data-stu-id="658cc-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <Disconnect xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </Disconnect>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-disconnect-response-example"></a><span data-ttu-id="658cc-109">Exemplo de resposta de desconexão bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="658cc-109">Successful Disconnect response example</span></span>

### <a name="description"></a><span data-ttu-id="658cc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="658cc-110">Description</span></span>

<span data-ttu-id="658cc-111">O exemplo a seguir de uma resposta de desconexão mostra uma resposta à solicitação de desconexão.</span><span class="sxs-lookup"><span data-stu-id="658cc-111">The following example of a Disconnect response shows a response to the Disconnect request.</span></span>
  
### <a name="code"></a><span data-ttu-id="658cc-112">Código</span><span class="sxs-lookup"><span data-stu-id="658cc-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <DisconnectResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="658cc-113">Confira também</span><span class="sxs-lookup"><span data-stu-id="658cc-113">See also</span></span>

- [<span data-ttu-id="658cc-114">Desconectar (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="658cc-114">Disconnect (UM web service)</span></span>](disconnect-um-web-service.md) 
- [<span data-ttu-id="658cc-115">DisconnectResponse (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="658cc-115">DisconnectResponse (UM web service)</span></span>](disconnectresponse-um-web-service.md) 
- [<span data-ttu-id="658cc-116">Callid (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="658cc-116">CallId (UM web service)</span></span>](callid-um-web-service.md)

