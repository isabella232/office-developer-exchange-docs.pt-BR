---
title: Desconectar a operação (serviço web de Unificação de mensagens)
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
description: A operação de desconexão encerra a chamada que é identificada pelo CallId especificado (serviço web de Unificação de mensagens).
ms.openlocfilehash: 1e04e65fa1951a6aa46e2c8b6dd5fe524c84a8fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751844"
---
# <a name="disconnect-operation-um-web-service"></a><span data-ttu-id="f2dab-103">Desconectar a operação (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="f2dab-103">Disconnect operation (UM web service)</span></span>

<span data-ttu-id="f2dab-104">A operação de desconexão encerra a chamada que é identificada pelo especificado [CallId (serviço web de Unificação de mensagens)](callid-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="f2dab-104">The Disconnect operation terminates the call that is identified by the specified [CallId (UM web service)](callid-um-web-service.md).</span></span>
  
## <a name="disconnect-request-example"></a><span data-ttu-id="f2dab-105">Desconectar um exemplo de solicitação</span><span class="sxs-lookup"><span data-stu-id="f2dab-105">Disconnect request example</span></span>

### <a name="description"></a><span data-ttu-id="f2dab-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2dab-106">Description</span></span>

<span data-ttu-id="f2dab-107">O exemplo a seguir de uma solicitação de desconexão mostra como uma solicitação para desconectar uma chamada de formulário.</span><span class="sxs-lookup"><span data-stu-id="f2dab-107">The following example of a Disconnect request shows how to form a request to disconnect a call.</span></span>
  
### <a name="code"></a><span data-ttu-id="f2dab-108">Código</span><span class="sxs-lookup"><span data-stu-id="f2dab-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <Disconnect xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </Disconnect>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-disconnect-response-example"></a><span data-ttu-id="f2dab-109">Exemplo de resposta de desconexão bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="f2dab-109">Successful Disconnect response example</span></span>

### <a name="description"></a><span data-ttu-id="f2dab-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2dab-110">Description</span></span>

<span data-ttu-id="f2dab-111">O exemplo a seguir de uma resposta de desconexão mostra uma resposta à solicitação de desconexão.</span><span class="sxs-lookup"><span data-stu-id="f2dab-111">The following example of a Disconnect response shows a response to the Disconnect request.</span></span>
  
### <a name="code"></a><span data-ttu-id="f2dab-112">Código</span><span class="sxs-lookup"><span data-stu-id="f2dab-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <DisconnectResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="f2dab-113">Confira também</span><span class="sxs-lookup"><span data-stu-id="f2dab-113">See also</span></span>

- [<span data-ttu-id="f2dab-114">Desconectar (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="f2dab-114">Disconnect (UM web service)</span></span>](disconnect-um-web-service.md) 
- [<span data-ttu-id="f2dab-115">DisconnectResponse (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="f2dab-115">DisconnectResponse (UM web service)</span></span>](disconnectresponse-um-web-service.md) 
- [<span data-ttu-id="f2dab-116">CallId (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="f2dab-116">CallId (UM web service)</span></span>](callid-um-web-service.md)

