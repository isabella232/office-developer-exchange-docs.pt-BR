---
title: Operação SetOofStatus (serviço Web da UM)
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
description: A operação SetOofStatus define um valor que indica se a saudação de ausência temporária (OOF) deve ser reproduzida para o usuário que faz a solicitação.
ms.openlocfilehash: 2311b6137ac25d15ad3d06668450c1d0f7ec1fad
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467351"
---
# <a name="setoofstatus-operation-um-web-service"></a><span data-ttu-id="d7aa5-103">Operação SetOofStatus (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="d7aa5-103">SetOofStatus operation (UM web service)</span></span>

<span data-ttu-id="d7aa5-104">A operação SetOofStatus define um valor que indica se a saudação de ausência temporária (OOF) deve ser reproduzida para o usuário que faz a solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7aa5-104">The SetOofStatus operation sets a value that indicates whether the Out of Office (OOF) greeting should be played for the user who makes the request.</span></span>
  
## <a name="setoofstatus-request-example"></a><span data-ttu-id="d7aa5-105">Exemplo de solicitação SetOofStatus</span><span class="sxs-lookup"><span data-stu-id="d7aa5-105">SetOofStatus request example</span></span>

### <a name="description"></a><span data-ttu-id="d7aa5-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7aa5-106">Description</span></span>

<span data-ttu-id="d7aa5-107">O exemplo a seguir de uma solicitação SetOofStatus mostra como formar uma solicitação para habilitar a saudação de ausência temporária para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d7aa5-107">The following example of a SetOofStatus request shows how to form a request to enable the Out of Office greeting for a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="d7aa5-108">Código</span><span class="sxs-lookup"><span data-stu-id="d7aa5-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetOofStatus xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetOofStatus>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setoofstatus-response-example"></a><span data-ttu-id="d7aa5-109">Exemplo de resposta SetOofStatus bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="d7aa5-109">Successful SetOofStatus response example</span></span>

### <a name="description"></a><span data-ttu-id="d7aa5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7aa5-110">Description</span></span>

<span data-ttu-id="d7aa5-111">O exemplo a seguir de uma resposta SetOofStatus mostra uma resposta à solicitação SetOofStatus.</span><span class="sxs-lookup"><span data-stu-id="d7aa5-111">The following example of a SetOofStatus response shows a response to the SetOofStatus request.</span></span>
  
### <a name="code"></a><span data-ttu-id="d7aa5-112">Código</span><span class="sxs-lookup"><span data-stu-id="d7aa5-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetOofStatusResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="d7aa5-113">Também consulte</span><span class="sxs-lookup"><span data-stu-id="d7aa5-113">See also</span></span>



[<span data-ttu-id="d7aa5-114">SetOofStatus (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="d7aa5-114">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md)
  
[<span data-ttu-id="d7aa5-115">SetOofStatusResponse (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="d7aa5-115">SetOofStatusResponse (UM web service)</span></span>](setoofstatusresponse-um-web-service.md)
  
[<span data-ttu-id="d7aa5-116">Status (serviço Web da UM-SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="d7aa5-116">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md)

