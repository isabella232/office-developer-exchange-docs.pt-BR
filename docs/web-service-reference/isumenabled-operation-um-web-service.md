---
title: Operação IsUMEnabled (serviço Web da UM)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- IsUMEnabled
api_type:
- schema
ms.assetid: fbe6cd95-f7a5-42b9-8a9d-b6159a269d55
description: A operação IsUMEnabled determina se uma caixa de correio está habilitada para Unificação de mensagens.
ms.openlocfilehash: b1478f5a113059251fe1b036ac7d77e5a4ab4f50
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458233"
---
# <a name="isumenabled-operation-um-web-service"></a><span data-ttu-id="f951d-103">Operação IsUMEnabled (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="f951d-103">IsUMEnabled operation (UM web service)</span></span>

<span data-ttu-id="f951d-104">A operação IsUMEnabled determina se uma caixa de correio está habilitada para Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="f951d-104">The IsUMEnabled operation determines whether a mailbox is enabled for Unified Messaging.</span></span>
  
## <a name="isumenabled-request-example"></a><span data-ttu-id="f951d-105">Exemplo de solicitação IsUMEnabled</span><span class="sxs-lookup"><span data-stu-id="f951d-105">IsUMEnabled request example</span></span>

### <a name="description"></a><span data-ttu-id="f951d-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="f951d-106">Description</span></span>

<span data-ttu-id="f951d-107">O exemplo a seguir de uma solicitação IsUMEnabled mostra como formar uma solicitação para determinar se uma caixa de correio está habilitada para Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="f951d-107">The following example of an IsUMEnabled request shows how to form a request to determine whether a mailbox is enabled for Unified Messaging.</span></span>
  
### <a name="code"></a><span data-ttu-id="f951d-108">Código</span><span class="sxs-lookup"><span data-stu-id="f951d-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <IsUMEnabled xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-isumenabled-response-example"></a><span data-ttu-id="f951d-109">Exemplo de resposta IsUMEnabled bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="f951d-109">Successful IsUMEnabled response example</span></span>

### <a name="description"></a><span data-ttu-id="f951d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f951d-110">Description</span></span>

<span data-ttu-id="f951d-111">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação IsUMEnabled.</span><span class="sxs-lookup"><span data-stu-id="f951d-111">The following example shows a successful response to an IsUMEnabled request.</span></span>
  
### <a name="code"></a><span data-ttu-id="f951d-112">Código</span><span class="sxs-lookup"><span data-stu-id="f951d-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <IsUMEnabledResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <IsUMEnabledResponse>true</IsUMEnabledResponse> 
    </IsUMEnabledResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="f951d-113">Também consulte</span><span class="sxs-lookup"><span data-stu-id="f951d-113">See also</span></span>



[<span data-ttu-id="f951d-114">IsUMEnabled (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="f951d-114">IsUMEnabled (UM web service)</span></span>](isumenabled-um-web-service.md)
  
[<span data-ttu-id="f951d-115">IsUMEnabledResponse (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="f951d-115">IsUMEnabledResponse (UM web service)</span></span>](isumenabledresponse-um-web-service.md)


[<span data-ttu-id="f951d-116">Elementos XML do serviço Web de Unificação de mensagens para o Exchange</span><span class="sxs-lookup"><span data-stu-id="f951d-116">Unified Messaging web service XML elements for Exchange</span></span>](unified-messaging-web-service-xml-elements-for-exchange.md)

