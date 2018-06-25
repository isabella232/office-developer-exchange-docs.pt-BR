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
description: A operação de cancelamento da assinatura é usada para encerrar uma inscrição de notificação de recepção. Use essa operação em vez de deixar um tempo limite de inscrição. Essa operação só será válida para notificações de recepção.
ms.openlocfilehash: 64514a718d473f0fd7d0320bd1ccecddb1940ac8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837869"
---
# <a name="unsubscribe-operation"></a><span data-ttu-id="8e285-105">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="8e285-105">Unsubscribe operation</span></span>

<span data-ttu-id="8e285-106">A operação de cancelamento da assinatura é usada para encerrar uma inscrição de notificação de recepção.</span><span class="sxs-lookup"><span data-stu-id="8e285-106">The Unsubscribe operation is used to end a pull notification subscription.</span></span> <span data-ttu-id="8e285-107">Use essa operação em vez de deixar um tempo limite de inscrição.</span><span class="sxs-lookup"><span data-stu-id="8e285-107">Use this operation rather than letting a subscription timeout.</span></span> <span data-ttu-id="8e285-108">Essa operação só será válida para notificações de recepção.</span><span class="sxs-lookup"><span data-stu-id="8e285-108">This operation is only valid for pull notifications.</span></span>
  
## <a name="unsubscribe-request-example"></a><span data-ttu-id="8e285-109">Exemplo de solicitação de cancelamento de inscrição</span><span class="sxs-lookup"><span data-stu-id="8e285-109">Unsubscribe request example</span></span>

### <a name="description"></a><span data-ttu-id="8e285-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e285-110">Description</span></span>

<span data-ttu-id="8e285-111">O exemplo a seguir mostra a mensagem SOAP XML que será enviada para cancelar a assinatura de um cliente do serviço de notificação.</span><span class="sxs-lookup"><span data-stu-id="8e285-111">The following example shows the SOAP XML message that is sent to unsubscribe a client from the Notification service.</span></span>
  
### <a name="code"></a><span data-ttu-id="8e285-112">Código</span><span class="sxs-lookup"><span data-stu-id="8e285-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Unsubscribe xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>e6fbf5c1-7e26-4bc6-a5f2-882063d5e34e</SubscriptionId>  
    </Unsubscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-request-elements"></a><span data-ttu-id="8e285-113">Cancelar a assinatura de elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8e285-113">Unsubscribe request elements</span></span>

<span data-ttu-id="8e285-114">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="8e285-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="8e285-115">Cancelar assinatura</span><span class="sxs-lookup"><span data-stu-id="8e285-115">Unsubscribe</span></span>](unsubscribe.md)
    
- [<span data-ttu-id="8e285-116">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="8e285-116">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
## <a name="successful-unsubscribe-response-example"></a><span data-ttu-id="8e285-117">Exemplo de resposta bem-sucedida cancelamento da assinatura</span><span class="sxs-lookup"><span data-stu-id="8e285-117">Successful Unsubscribe response example</span></span>

### <a name="description"></a><span data-ttu-id="8e285-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e285-118">Description</span></span>

<span data-ttu-id="8e285-119">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de cancelamento da assinatura.</span><span class="sxs-lookup"><span data-stu-id="8e285-119">The following example shows a successful response to an Unsubscribe request.</span></span>
  
### <a name="code"></a><span data-ttu-id="8e285-120">Código</span><span class="sxs-lookup"><span data-stu-id="8e285-120">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UnsubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UnsubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:UnsubscribeResponseMessage>
      </m:ResponseMessages>
    </UnsubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-response-elements"></a><span data-ttu-id="8e285-121">Cancelar a assinatura de elementos de resposta</span><span class="sxs-lookup"><span data-stu-id="8e285-121">Unsubscribe response elements</span></span>

<span data-ttu-id="8e285-122">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="8e285-122">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="8e285-123">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="8e285-123">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="8e285-124">Cancelar assinatura</span><span class="sxs-lookup"><span data-stu-id="8e285-124">Unsubscribe</span></span>](unsubscribe.md)
    
- [<span data-ttu-id="8e285-125">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8e285-125">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="8e285-126">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8e285-126">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md)
    
- [<span data-ttu-id="8e285-127">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8e285-127">ResponseCode</span></span>](responsecode.md)
    
## <a name="unsubscribe-error-response-example"></a><span data-ttu-id="8e285-128">Exemplo de resposta de erro de cancelamento de inscrição</span><span class="sxs-lookup"><span data-stu-id="8e285-128">Unsubscribe Error response example</span></span>

### <a name="description"></a><span data-ttu-id="8e285-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="8e285-129">Description</span></span>

<span data-ttu-id="8e285-130">O exemplo a seguir de uma resposta de erro de cancelamento da assinatura ocorre em resposta a uma tentativa de cancelar a assinatura usando um identificador de assinatura que não pode ser localizado no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8e285-130">The following example of an Unsubscribe error response occurs in response to an attempt to unsubscribe by using a subscription identifier that cannot be located in the Exchange store.</span></span>
  
### <a name="code"></a><span data-ttu-id="8e285-131">Código</span><span class="sxs-lookup"><span data-stu-id="8e285-131">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UnsubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="unsubscribe-error-response-elements"></a><span data-ttu-id="8e285-132">Cancelar a assinatura de elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="8e285-132">Unsubscribe Error response elements</span></span>

<span data-ttu-id="8e285-133">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="8e285-133">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="8e285-134">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="8e285-134">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="8e285-135">UnsubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="8e285-135">UnsubscribeResponse</span></span>](unsubscriberesponse.md)
    
- [<span data-ttu-id="8e285-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8e285-136">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="8e285-137">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8e285-137">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md)
    
- [<span data-ttu-id="8e285-138">MessageText</span><span class="sxs-lookup"><span data-stu-id="8e285-138">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="8e285-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8e285-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="8e285-140">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="8e285-140">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="8e285-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="8e285-141">See also</span></span>

- [<span data-ttu-id="8e285-142">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="8e285-142">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="8e285-143">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="8e285-143">GetEvents operation</span></span>](getevents-operation.md)
- [<span data-ttu-id="8e285-144">Usando inscrições de recepção</span><span class="sxs-lookup"><span data-stu-id="8e285-144">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)

