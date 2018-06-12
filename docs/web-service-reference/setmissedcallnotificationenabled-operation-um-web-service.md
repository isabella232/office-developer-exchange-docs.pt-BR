---
title: Operação de SetMissedCallNotificationEnabled (serviço web de Unificação de mensagens)
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
description: A operação SetMissedCallNotificationEnabled habilita ou desabilita as notificações de chamada não atendida.
ms.openlocfilehash: be9479d6ed2c5238ed19c3d22e028fca62b8deed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825434"
---
# <a name="setmissedcallnotificationenabled-operation-um-web-service"></a><span data-ttu-id="5111f-103">Operação de SetMissedCallNotificationEnabled (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="5111f-103">SetMissedCallNotificationEnabled operation (UM web service)</span></span>

<span data-ttu-id="5111f-104">A operação SetMissedCallNotificationEnabled habilita ou desabilita as notificações de chamada não atendida.</span><span class="sxs-lookup"><span data-stu-id="5111f-104">The SetMissedCallNotificationEnabled operation enables or disables missed call notifications.</span></span>
  
## <a name="setmissedcallnotificationenabled-request-example"></a><span data-ttu-id="5111f-105">Exemplo de solicitação de SetMissedCallNotificationEnabled</span><span class="sxs-lookup"><span data-stu-id="5111f-105">SetMissedCallNotificationEnabled request example</span></span>

### <a name="description"></a><span data-ttu-id="5111f-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="5111f-106">Description</span></span>

<span data-ttu-id="5111f-107">O exemplo a seguir de uma solicitação de SetMissedCallNotificationEnabled mostra como formar uma solicitação para habilitar as notificações de chamada não atendida.</span><span class="sxs-lookup"><span data-stu-id="5111f-107">The following example of a SetMissedCallNotificationEnabled request shows how to form a request to enable missed call notifications.</span></span>
  
### <a name="code"></a><span data-ttu-id="5111f-108">Código</span><span class="sxs-lookup"><span data-stu-id="5111f-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetMissedCallNotificationEnabled xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetMissedCallNotificationEnabled>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setmissedcallnotificationenabled-response-example"></a><span data-ttu-id="5111f-109">Exemplo de resposta bem-sucedida SetMissedCallNotificationEnabled</span><span class="sxs-lookup"><span data-stu-id="5111f-109">Successful SetMissedCallNotificationEnabled response example</span></span>

### <a name="description"></a><span data-ttu-id="5111f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5111f-110">Description</span></span>

<span data-ttu-id="5111f-111">O exemplo a seguir de uma resposta PlayOnPhoneGreeting mostra uma resposta à solicitação de SetMissedCallNotificationEnabled.</span><span class="sxs-lookup"><span data-stu-id="5111f-111">The following example of a PlayOnPhoneGreeting response shows a response to the SetMissedCallNotificationEnabled request.</span></span>
  
### <a name="code"></a><span data-ttu-id="5111f-112">Código</span><span class="sxs-lookup"><span data-stu-id="5111f-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetMissedCallNotificationEnabledResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="5111f-113">Confira também</span><span class="sxs-lookup"><span data-stu-id="5111f-113">See also</span></span>



[<span data-ttu-id="5111f-114">SetMissedCallNotificationEnabled (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="5111f-114">SetMissedCallNotificationEnabled (UM web service)</span></span>](setmissedcallnotificationenabled-um-web-service.md)
  
[<span data-ttu-id="5111f-115">SetMissedCallNotificationEnabledResponse (serviço web de Unificação de mensagens)</span><span class="sxs-lookup"><span data-stu-id="5111f-115">SetMissedCallNotificationEnabledResponse (UM web service)</span></span>](setmissedcallnotificationenabledresponse-um-web-service.md)
  
[<span data-ttu-id="5111f-116">Status (UM serviço web - SetMissedCallNotificationEnabled)</span><span class="sxs-lookup"><span data-stu-id="5111f-116">Status (UM web service - SetMissedCallNotificationEnabled)</span></span>](status-um-web-servicesetmissedcallnotificationenabled.md)

