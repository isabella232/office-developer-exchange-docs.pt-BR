---
title: Cancelar a operação
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Unsubscribe
api_type:
- schema
ms.assetid: 994a9d2b-1501-4804-90f0-12bd914496ec
description: A operação unsubscribe é usada para encerrar uma assinatura de notificação de recepção. Use essa operação, em vez de deixar um tempo limite de assinatura. Essa operação só é válida para notificações de recepção.
ms.openlocfilehash: 054f89af1ba5c780c7de5016a6dfe34086c97f02
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468023"
---
# <a name="unsubscribe-operation"></a><span data-ttu-id="aa7d5-105">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="aa7d5-105">Unsubscribe operation</span></span>

<span data-ttu-id="aa7d5-106">A operação unsubscribe é usada para encerrar uma assinatura de notificação de recepção.</span><span class="sxs-lookup"><span data-stu-id="aa7d5-106">The Unsubscribe operation is used to end a pull notification subscription.</span></span> <span data-ttu-id="aa7d5-107">Use essa operação, em vez de deixar um tempo limite de assinatura.</span><span class="sxs-lookup"><span data-stu-id="aa7d5-107">Use this operation rather than letting a subscription timeout.</span></span> <span data-ttu-id="aa7d5-108">Essa operação só é válida para notificações de recepção.</span><span class="sxs-lookup"><span data-stu-id="aa7d5-108">This operation is only valid for pull notifications.</span></span>
  
## <a name="unsubscribe-request-example"></a><span data-ttu-id="aa7d5-109">Exemplo de solicitação de cancelamento de assinatura</span><span class="sxs-lookup"><span data-stu-id="aa7d5-109">Unsubscribe request example</span></span>

### <a name="description"></a><span data-ttu-id="aa7d5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa7d5-110">Description</span></span>

<span data-ttu-id="aa7d5-111">O exemplo a seguir mostra a mensagem XML do SOAP que é enviada para cancelar a assinatura de um cliente do serviço de notificação.</span><span class="sxs-lookup"><span data-stu-id="aa7d5-111">The following example shows the SOAP XML message that is sent to unsubscribe a client from the Notification service.</span></span>
  
### <a name="code"></a><span data-ttu-id="aa7d5-112">Código</span><span class="sxs-lookup"><span data-stu-id="aa7d5-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Unsubscribe xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>e6fbf5c1-7e26-4bc6-a5f2-882063d5e34e</SubscriptionId>  
    </Unsubscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-request-elements"></a><span data-ttu-id="aa7d5-113">Cancelar assinatura de elementos Request</span><span class="sxs-lookup"><span data-stu-id="aa7d5-113">Unsubscribe request elements</span></span>

<span data-ttu-id="aa7d5-114">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="aa7d5-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="aa7d5-115">Cancelar assinatura</span><span class="sxs-lookup"><span data-stu-id="aa7d5-115">Unsubscribe</span></span>](unsubscribe.md)
    
- [<span data-ttu-id="aa7d5-116">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="aa7d5-116">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
## <a name="successful-unsubscribe-response-example"></a><span data-ttu-id="aa7d5-117">Exemplo de resposta de cancelamento de assinatura bem-sucedido</span><span class="sxs-lookup"><span data-stu-id="aa7d5-117">Successful Unsubscribe response example</span></span>

### <a name="description"></a><span data-ttu-id="aa7d5-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa7d5-118">Description</span></span>

<span data-ttu-id="aa7d5-119">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de cancelamento de assinatura.</span><span class="sxs-lookup"><span data-stu-id="aa7d5-119">The following example shows a successful response to an Unsubscribe request.</span></span>
  
### <a name="code"></a><span data-ttu-id="aa7d5-120">Código</span><span class="sxs-lookup"><span data-stu-id="aa7d5-120">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UnsubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UnsubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:UnsubscribeResponseMessage>
      </m:ResponseMessages>
    </UnsubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-response-elements"></a><span data-ttu-id="aa7d5-121">Cancelar assinatura dos elementos de resposta</span><span class="sxs-lookup"><span data-stu-id="aa7d5-121">Unsubscribe response elements</span></span>

<span data-ttu-id="aa7d5-122">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="aa7d5-122">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="aa7d5-123">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="aa7d5-123">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="aa7d5-124">Cancelar assinatura</span><span class="sxs-lookup"><span data-stu-id="aa7d5-124">Unsubscribe</span></span>](unsubscribe.md)
    
- [<span data-ttu-id="aa7d5-125">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="aa7d5-125">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="aa7d5-126">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="aa7d5-126">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md)
    
- [<span data-ttu-id="aa7d5-127">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="aa7d5-127">ResponseCode</span></span>](responsecode.md)
    
## <a name="unsubscribe-error-response-example"></a><span data-ttu-id="aa7d5-128">Exemplo de resposta de erro de cancelamento de assinatura</span><span class="sxs-lookup"><span data-stu-id="aa7d5-128">Unsubscribe Error response example</span></span>

### <a name="description"></a><span data-ttu-id="aa7d5-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa7d5-129">Description</span></span>

<span data-ttu-id="aa7d5-130">O exemplo a seguir de uma resposta de erro de cancelamento de assinatura ocorre em resposta a uma tentativa de cancelar a assinatura usando um identificador de assinatura que não pode ser localizado no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="aa7d5-130">The following example of an Unsubscribe error response occurs in response to an attempt to unsubscribe by using a subscription identifier that cannot be located in the Exchange store.</span></span>
  
### <a name="code"></a><span data-ttu-id="aa7d5-131">Código</span><span class="sxs-lookup"><span data-stu-id="aa7d5-131">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UnsubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UnsubscribeResponseMessage ResponseClass="Error">
          <m:MessageText>The specified subscription was not found.</m:MessageText>
          <m:ResponseCode>ErrorSubscriptionNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:UnsubscribeResponseMessage>
      </m:ResponseMessages>
    </UnsubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-error-response-elements"></a><span data-ttu-id="aa7d5-132">Cancelar assinatura de elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="aa7d5-132">Unsubscribe Error response elements</span></span>

<span data-ttu-id="aa7d5-133">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="aa7d5-133">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="aa7d5-134">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="aa7d5-134">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="aa7d5-135">UnsubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="aa7d5-135">UnsubscribeResponse</span></span>](unsubscriberesponse.md)
    
- [<span data-ttu-id="aa7d5-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="aa7d5-136">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="aa7d5-137">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="aa7d5-137">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md)
    
- [<span data-ttu-id="aa7d5-138">MessageText</span><span class="sxs-lookup"><span data-stu-id="aa7d5-138">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="aa7d5-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="aa7d5-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="aa7d5-140">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="aa7d5-140">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="aa7d5-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="aa7d5-141">See also</span></span>

- [<span data-ttu-id="aa7d5-142">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="aa7d5-142">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="aa7d5-143">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="aa7d5-143">GetEvents operation</span></span>](getevents-operation.md)
- [<span data-ttu-id="aa7d5-144">Usando assinaturas pull</span><span class="sxs-lookup"><span data-stu-id="aa7d5-144">Using Pull Subscriptions</span></span>](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)

