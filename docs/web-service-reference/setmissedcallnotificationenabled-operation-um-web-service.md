---
title: Operação SetMissedCallNotificationEnabled (serviço Web da UM)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetMissedCallNotificationEnabled
api_type:
- schema
ms.assetid: 6693b5db-ac6b-43bc-af83-a9c94fc425bf
description: A operação SetMissedCallNotificationEnabled habilita ou desabilita notificações de chamada não atendida.
ms.openlocfilehash: ca4942942a81bc187e8e18a5e6f003f8587f79d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467393"
---
# <a name="setmissedcallnotificationenabled-operation-um-web-service"></a><span data-ttu-id="1d0ac-103">Operação SetMissedCallNotificationEnabled (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="1d0ac-103">SetMissedCallNotificationEnabled operation (UM web service)</span></span>

<span data-ttu-id="1d0ac-104">A operação SetMissedCallNotificationEnabled habilita ou desabilita notificações de chamada não atendida.</span><span class="sxs-lookup"><span data-stu-id="1d0ac-104">The SetMissedCallNotificationEnabled operation enables or disables missed call notifications.</span></span>
  
## <a name="setmissedcallnotificationenabled-request-example"></a><span data-ttu-id="1d0ac-105">Exemplo de solicitação SetMissedCallNotificationEnabled</span><span class="sxs-lookup"><span data-stu-id="1d0ac-105">SetMissedCallNotificationEnabled request example</span></span>

### <a name="description"></a><span data-ttu-id="1d0ac-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d0ac-106">Description</span></span>

<span data-ttu-id="1d0ac-107">O exemplo a seguir de uma solicitação SetMissedCallNotificationEnabled mostra como formar uma solicitação para habilitar notificações de chamadas perdidas.</span><span class="sxs-lookup"><span data-stu-id="1d0ac-107">The following example of a SetMissedCallNotificationEnabled request shows how to form a request to enable missed call notifications.</span></span>
  
### <a name="code"></a><span data-ttu-id="1d0ac-108">Código</span><span class="sxs-lookup"><span data-stu-id="1d0ac-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetMissedCallNotificationEnabled xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetMissedCallNotificationEnabled>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setmissedcallnotificationenabled-response-example"></a><span data-ttu-id="1d0ac-109">Exemplo de resposta SetMissedCallNotificationEnabled bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="1d0ac-109">Successful SetMissedCallNotificationEnabled response example</span></span>

### <a name="description"></a><span data-ttu-id="1d0ac-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d0ac-110">Description</span></span>

<span data-ttu-id="1d0ac-111">O exemplo a seguir de uma resposta PlayOnPhoneGreeting mostra uma resposta à solicitação SetMissedCallNotificationEnabled.</span><span class="sxs-lookup"><span data-stu-id="1d0ac-111">The following example of a PlayOnPhoneGreeting response shows a response to the SetMissedCallNotificationEnabled request.</span></span>
  
### <a name="code"></a><span data-ttu-id="1d0ac-112">Código</span><span class="sxs-lookup"><span data-stu-id="1d0ac-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetMissedCallNotificationEnabledResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="1d0ac-113">Também consulte</span><span class="sxs-lookup"><span data-stu-id="1d0ac-113">See also</span></span>



[<span data-ttu-id="1d0ac-114">SetMissedCallNotificationEnabled (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="1d0ac-114">SetMissedCallNotificationEnabled (UM web service)</span></span>](setmissedcallnotificationenabled-um-web-service.md)
  
[<span data-ttu-id="1d0ac-115">SetMissedCallNotificationEnabledResponse (serviço Web da UM)</span><span class="sxs-lookup"><span data-stu-id="1d0ac-115">SetMissedCallNotificationEnabledResponse (UM web service)</span></span>](setmissedcallnotificationenabledresponse-um-web-service.md)
  
[<span data-ttu-id="1d0ac-116">Status (serviço Web da UM-SetMissedCallNotificationEnabled)</span><span class="sxs-lookup"><span data-stu-id="1d0ac-116">Status (UM web service - SetMissedCallNotificationEnabled)</span></span>](status-um-web-servicesetmissedcallnotificationenabled.md)

