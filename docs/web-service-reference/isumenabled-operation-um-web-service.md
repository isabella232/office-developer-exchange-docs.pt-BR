---
title: Operação de IsUMEnabled (serviço web de Unificação de mensagens)
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
ms.openlocfilehash: 9d94a359d6b11e41762d21aa2fe5501bd9f7b577
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824107"
---
# <a name="isumenabled-operation-um-web-service"></a><span data-ttu-id="74cb2-103">Operação de IsUMEnabled (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="74cb2-103">IsUMEnabled operation (UM web service)</span></span>

<span data-ttu-id="74cb2-104">A operação IsUMEnabled determina se uma caixa de correio está habilitada para Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="74cb2-104">The IsUMEnabled operation determines whether a mailbox is enabled for Unified Messaging.</span></span>
  
## <a name="isumenabled-request-example"></a><span data-ttu-id="74cb2-105">Exemplo de solicitação de IsUMEnabled</span><span class="sxs-lookup"><span data-stu-id="74cb2-105">IsUMEnabled request example</span></span>

### <a name="description"></a><span data-ttu-id="74cb2-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="74cb2-106">Description</span></span>

<span data-ttu-id="74cb2-107">O exemplo a seguir de uma solicitação de IsUMEnabled mostra como formar uma solicitação para determinar se uma caixa de correio está habilitada para Unificação de mensagens.</span><span class="sxs-lookup"><span data-stu-id="74cb2-107">The following example of an IsUMEnabled request shows how to form a request to determine whether a mailbox is enabled for Unified Messaging.</span></span>
  
### <a name="code"></a><span data-ttu-id="74cb2-108">Código</span><span class="sxs-lookup"><span data-stu-id="74cb2-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <IsUMEnabled xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-isumenabled-response-example"></a><span data-ttu-id="74cb2-109">Exemplo de resposta bem-sucedida IsUMEnabled</span><span class="sxs-lookup"><span data-stu-id="74cb2-109">Successful IsUMEnabled response example</span></span>

### <a name="description"></a><span data-ttu-id="74cb2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="74cb2-110">Description</span></span>

<span data-ttu-id="74cb2-111">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação IsUMEnabled.</span><span class="sxs-lookup"><span data-stu-id="74cb2-111">The following example shows a successful response to an IsUMEnabled request.</span></span>
  
### <a name="code"></a><span data-ttu-id="74cb2-112">Código</span><span class="sxs-lookup"><span data-stu-id="74cb2-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <IsUMEnabledResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <IsUMEnabledResponse>true</IsUMEnabledResponse> 
    </IsUMEnabledResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="74cb2-113">Confira também</span><span class="sxs-lookup"><span data-stu-id="74cb2-113">See also</span></span>



[<span data-ttu-id="74cb2-114">IsUMEnabled (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="74cb2-114">IsUMEnabled (UM web service)</span></span>](isumenabled-um-web-service.md)
  
[<span data-ttu-id="74cb2-115">IsUMEnabledResponse (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="74cb2-115">IsUMEnabledResponse (UM web service)</span></span>](isumenabledresponse-um-web-service.md)


[<span data-ttu-id="74cb2-116">Unified Messaging web service os elementos XML para o Exchange</span><span class="sxs-lookup"><span data-stu-id="74cb2-116">Unified Messaging web service XML elements for Exchange</span></span>](unified-messaging-web-service-xml-elements-for-exchange.md)

