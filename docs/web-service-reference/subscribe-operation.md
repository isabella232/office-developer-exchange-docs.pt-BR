---
title: Operação Subscribe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Subscribe
api_type:
- schema
ms.assetid: f17c3d08-c79e-41f1-ba31-6e41e7aafd87
description: A operação de assinatura é usada para assinar aplicativos cliente para notificações por Push ou pull. É importante estar ciente de que a estrutura das mensagens e respostas de solicitação é diferente dependendo do tipo de notificação de evento.
ms.openlocfilehash: c40e0e434f698c6535ff5d03fd4d45a453959dd6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467043"
---
# <a name="subscribe-operation"></a><span data-ttu-id="ce009-104">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="ce009-104">Subscribe operation</span></span>

<span data-ttu-id="ce009-105">A operação de assinatura é usada para assinar aplicativos cliente para notificações por Push ou pull.</span><span class="sxs-lookup"><span data-stu-id="ce009-105">The Subscribe operation is used to subscribe client applications to either push or pull notifications.</span></span> <span data-ttu-id="ce009-106">É importante estar ciente de que a estrutura das mensagens e respostas de solicitação é diferente dependendo do tipo de notificação de evento.</span><span class="sxs-lookup"><span data-stu-id="ce009-106">It is important to be aware that the structure of the request messages and responses is different depending on the type of event notification.</span></span> 
  
## <a name="pull-subscription-subscribe-request-example"></a><span data-ttu-id="ce009-107">Exemplo de solicitação de assinatura pull Subscription</span><span class="sxs-lookup"><span data-stu-id="ce009-107">Pull Subscription Subscribe request example</span></span>

### <a name="description"></a><span data-ttu-id="ce009-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce009-108">Description</span></span>

<span data-ttu-id="ce009-109">O exemplo de código a seguir mostra como se inscrever em uma assinatura de notificação de evento de recepção.</span><span class="sxs-lookup"><span data-stu-id="ce009-109">The following code example shows how to subscribe to a pull event notification subscription.</span></span> <span data-ttu-id="ce009-110">A assinatura informa ao aplicativo cliente se novos emails são adicionados à caixa de entrada e se um item é excluído da caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="ce009-110">The subscription informs the client application if new mail is added to the Inbox and if an item is deleted from the Inbox.</span></span> <span data-ttu-id="ce009-111">A assinatura expirará se o cliente não solicitar informações sobre os eventos em dez minutos.</span><span class="sxs-lookup"><span data-stu-id="ce009-111">The subscription will time out if the client does not request information about events within ten minutes.</span></span> <span data-ttu-id="ce009-112">Se a assinatura expirar, uma nova assinatura deve ser estabelecida para continuar a solicitar notificações.</span><span class="sxs-lookup"><span data-stu-id="ce009-112">If the subscription expires, a new subscription must be established to continue to request notifications.</span></span>
  
### <a name="code"></a><span data-ttu-id="ce009-113">Código</span><span class="sxs-lookup"><span data-stu-id="ce009-113">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Subscribe xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <PullSubscriptionRequest>
        <t:FolderIds>
          <t:DistinguishedFolderId Id="inbox"/>
        </t:FolderIds>
        <t:EventTypes>
          <t:EventType>NewMailEvent</t:EventType>
          <t:EventType>DeletedEvent</t:EventType>
        </t:EventTypes>
        <t:Timeout>10</t:Timeout>
      </PullSubscriptionRequest>
    </Subscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="pull-subscription-subscribe-request-elements"></a><span data-ttu-id="ce009-114">Elementos de solicitação de inscrição de assinatura pull</span><span class="sxs-lookup"><span data-stu-id="ce009-114">Pull Subscription Subscribe Request Elements</span></span>

<span data-ttu-id="ce009-115">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="ce009-115">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="ce009-116">Assinar</span><span class="sxs-lookup"><span data-stu-id="ce009-116">Subscribe</span></span>](subscribe.md)
    
- [<span data-ttu-id="ce009-117">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="ce009-117">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md)
    
- [<span data-ttu-id="ce009-118">FolderIds</span><span class="sxs-lookup"><span data-stu-id="ce009-118">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="ce009-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="ce009-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="ce009-120">EventType</span><span class="sxs-lookup"><span data-stu-id="ce009-120">EventTypes</span></span>](eventtypes.md)
    
- [<span data-ttu-id="ce009-121">EventType</span><span class="sxs-lookup"><span data-stu-id="ce009-121">EventType</span></span>](eventtype.md)
    
- [<span data-ttu-id="ce009-122">Timeout</span><span class="sxs-lookup"><span data-stu-id="ce009-122">Timeout</span></span>](timeout.md)
    
<span data-ttu-id="ce009-123">Para encontrar outras opções para a mensagem de solicitação da operação de assinatura, explore a hierarquia do esquema.</span><span class="sxs-lookup"><span data-stu-id="ce009-123">To find other options for the request message of the Subscribe operation, explore the schema hierarchy.</span></span> <span data-ttu-id="ce009-124">Inicie no elemento [PullSubscriptionRequest](pullsubscriptionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="ce009-124">Start at the [PullSubscriptionRequest](pullsubscriptionrequest.md) element.</span></span> 
  
## <a name="successful-pull-subscription-subscribe-response-example"></a><span data-ttu-id="ce009-125">Exemplo de resposta de inscrição de assinatura pull bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="ce009-125">Successful Pull Subscription Subscribe response example</span></span>

### <a name="description"></a><span data-ttu-id="ce009-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce009-126">Description</span></span>

<span data-ttu-id="ce009-127">O exemplo a seguir mostra uma resposta de assinatura pull bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="ce009-127">The following example shows a successful pull subscription response.</span></span> <span data-ttu-id="ce009-128">A resposta contém o identificador de assinatura e a marca d' água que é usada para obter a matriz de eventos que estão associados a uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="ce009-128">The response contains the subscription identifier and watermark that is used to get the array of events that are associated with a subscription.</span></span> <span data-ttu-id="ce009-129">O identificador de assinatura também é usado para cancelar a assinatura de um cliente de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="ce009-129">The subscription identifier is also used to unsubscribe a client from a subscription.</span></span>
  
### <a name="code"></a><span data-ttu-id="ce009-130">Código</span><span class="sxs-lookup"><span data-stu-id="ce009-130">Code</span></span>

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
    <SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SubscriptionId>39ea5d0f-f062-455e-a1e9-89c0304390f4</m:SubscriptionId>
          <m:Watermark>AAAAAHgGAAAAAAAAAQ==</m:Watermark>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </SubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="pull-subscription-subscribe-response-elements"></a><span data-ttu-id="ce009-131">Elementos de resposta de assinatura pull Subscription</span><span class="sxs-lookup"><span data-stu-id="ce009-131">Pull Subscription Subscribe response elements</span></span>

<span data-ttu-id="ce009-132">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="ce009-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="ce009-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ce009-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ce009-134">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="ce009-134">SubscribeResponse</span></span>](subscriberesponse.md)
    
- [<span data-ttu-id="ce009-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ce009-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ce009-136">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ce009-136">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
    
- [<span data-ttu-id="ce009-137">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ce009-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ce009-138">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="ce009-138">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="ce009-139">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="ce009-139">Watermark</span></span>](watermark.md)
    
## <a name="pull-subscription-subscribe-error-response-example"></a><span data-ttu-id="ce009-140">Exemplo de resposta de erro de assinatura pull Subscription</span><span class="sxs-lookup"><span data-stu-id="ce009-140">Pull Subscription Subscribe Error response example</span></span>

### <a name="description"></a><span data-ttu-id="ce009-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce009-141">Description</span></span>

<span data-ttu-id="ce009-142">O exemplo a seguir mostra uma resposta de erro a uma solicitação de assinatura.</span><span class="sxs-lookup"><span data-stu-id="ce009-142">The following example shows an error response to a Subscribe request.</span></span> <span data-ttu-id="ce009-143">O erro é causado por uma tentativa de inscrever-se em notificações usando o acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="ce009-143">The error is caused by an attempt to subscribe to notifications by using delegate access.</span></span>
  
### <a name="code"></a><span data-ttu-id="ce009-144">Código</span><span class="sxs-lookup"><span data-stu-id="ce009-144">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Error">
          <m:MessageText>Subscriptions are not supported for delegate user access.</m:MessageText>
          <m:ResponseCode>ErrorSubscriptionDelegateAccessNotSupported</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </SubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="pull-subscription-error-response-elements"></a><span data-ttu-id="ce009-145">Elementos de resposta de erro de assinatura pull</span><span class="sxs-lookup"><span data-stu-id="ce009-145">Pull Subscription Error response elements</span></span>

<span data-ttu-id="ce009-146">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="ce009-146">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="ce009-147">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ce009-147">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ce009-148">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="ce009-148">SubscribeResponse</span></span>](subscriberesponse.md)
    
- [<span data-ttu-id="ce009-149">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ce009-149">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ce009-150">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ce009-150">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
    
- [<span data-ttu-id="ce009-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="ce009-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="ce009-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ce009-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ce009-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ce009-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="push-subscription-request-example"></a><span data-ttu-id="ce009-154">Exemplo de solicitação de assinatura push</span><span class="sxs-lookup"><span data-stu-id="ce009-154">Push Subscription request example</span></span>

### <a name="description"></a><span data-ttu-id="ce009-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce009-155">Description</span></span>

<span data-ttu-id="ce009-156">O exemplo de código a seguir mostra como se inscrever em uma assinatura de notificação por push de eventos.</span><span class="sxs-lookup"><span data-stu-id="ce009-156">The following code example shows how to subscribe to a push event notification subscription.</span></span> <span data-ttu-id="ce009-157">A solicitação identifica as pastas a serem monitoradas, os tipos de eventos a serem monitorados, a frequência das notificações de status e a URL do serviço Web cliente que escuta as notificações por push.</span><span class="sxs-lookup"><span data-stu-id="ce009-157">The request identifies the folders to monitor, the types of events to monitor, the frequency of status notifications, and the URL of the client Web service that listens for the push notifications.</span></span>
  
### <a name="code"></a><span data-ttu-id="ce009-158">Código</span><span class="sxs-lookup"><span data-stu-id="ce009-158">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Subscribe xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <PushSubscriptionRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <FolderIds xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <DistinguishedFolderId Id="inbox" />
        </FolderIds>
        <EventTypes xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <EventType>NewMailEvent</EventType>
          <EventType>CopiedEvent</EventType>
          <EventType>CreatedEvent</EventType>
          <EventType>DeletedEvent</EventType>
          <EventType>ModifiedEvent</EventType>
          <EventType>MovedEvent</EventType>
        </EventTypes>
        <StatusFrequency xmlns="https://schemas.microsoft.com/exchange/services/2006/types">1</StatusFrequency>
        <URL xmlns="https://schemas.microsoft.com/exchange/services/2006/types">http://clientWebService/Service.asmx</URL>
      </PushSubscriptionRequest>
    </Subscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="ce009-159">Comentários</span><span class="sxs-lookup"><span data-stu-id="ce009-159">Comments</span></span>

<span data-ttu-id="ce009-160">O serviço Web do cliente deve ser configurado antes que a solicitação de assinatura de notificação por push seja enviada; caso contrário, a primeira notificação não será enviada para um ponto de extremidade válido e a notificação por push falhará.</span><span class="sxs-lookup"><span data-stu-id="ce009-160">The client Web service must be set up before the push notification subscribe request is sent; otherwise, the first notification will not be sent to a valid endpoint and the push notification will fail.</span></span> <span data-ttu-id="ce009-161">Para mais informações, consulte [aplicativo de exemplo de notificação por push](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="ce009-161">For more information, see [Push Notification Sample Application](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx).</span></span>
  
<span data-ttu-id="ce009-162">Uma nova [SubscriptionId (GetEvents)](subscriptionid-getevents.md) é criada ao se reinscrever.</span><span class="sxs-lookup"><span data-stu-id="ce009-162">A new [SubscriptionId (GetEvents)](subscriptionid-getevents.md) is created when you resubscribe.</span></span> <span data-ttu-id="ce009-163">Use a marca d' água de uma assinatura anterior para se reinscrever no ponto em que a assinatura anterior terminou.</span><span class="sxs-lookup"><span data-stu-id="ce009-163">Use the watermark of a previous subscription to resubscribe at the point where the previous subscription ended.</span></span> 
  
### <a name="push-subscription-request-elements"></a><span data-ttu-id="ce009-164">Elementos de solicitação de assinatura push</span><span class="sxs-lookup"><span data-stu-id="ce009-164">Push Subscription Request Elements</span></span>

<span data-ttu-id="ce009-165">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="ce009-165">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="ce009-166">Assinar</span><span class="sxs-lookup"><span data-stu-id="ce009-166">Subscribe</span></span>](subscribe.md)
    
- [<span data-ttu-id="ce009-167">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="ce009-167">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
    
- [<span data-ttu-id="ce009-168">FolderIds</span><span class="sxs-lookup"><span data-stu-id="ce009-168">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="ce009-169">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="ce009-169">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="ce009-170">EventType</span><span class="sxs-lookup"><span data-stu-id="ce009-170">EventTypes</span></span>](eventtypes.md)
    
- [<span data-ttu-id="ce009-171">EventType</span><span class="sxs-lookup"><span data-stu-id="ce009-171">EventType</span></span>](eventtype.md)
    
- [<span data-ttu-id="ce009-172">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="ce009-172">StatusFrequency</span></span>](statusfrequency.md)
    
- [<span data-ttu-id="ce009-173">Endereço</span><span class="sxs-lookup"><span data-stu-id="ce009-173">Url </span></span>](url-ex15websvcsotherref.md)
    
## <a name="successful-push-subscription-response-example"></a><span data-ttu-id="ce009-174">Exemplo de resposta de assinatura push bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="ce009-174">Successful Push Subscription response example</span></span>

### <a name="description"></a><span data-ttu-id="ce009-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce009-175">Description</span></span>

<span data-ttu-id="ce009-176">O exemplo a seguir mostra uma resposta de assinatura push bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="ce009-176">The following example shows a successful push subscription response.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ce009-177">Código</span><span class="sxs-lookup"><span data-stu-id="ce009-177">Code</span></span>

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
    <SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages>
        <SubscribeResponseMessage ResponseClass="Success">
          <ResponseCode>NoError</ResponseCode>
          <SubscriptionId>83826921-afdf-48be-b469-628cc02b5f49</SubscriptionId>
          <Watermark>AQAAAOpvG0LURVdOhQkPOWZLPcI8EgAAAAAAAAE=</Watermark>
        </SubscribeResponseMessage>
      </ResponseMessages>
    </SubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="push-subscription-response-elements"></a><span data-ttu-id="ce009-178">Elementos de resposta de assinatura push</span><span class="sxs-lookup"><span data-stu-id="ce009-178">Push Subscription response elements</span></span>

<span data-ttu-id="ce009-179">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="ce009-179">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="ce009-180">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ce009-180">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ce009-181">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="ce009-181">SubscribeResponse</span></span>](subscriberesponse.md)
    
- [<span data-ttu-id="ce009-182">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ce009-182">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ce009-183">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ce009-183">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
    
- [<span data-ttu-id="ce009-184">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ce009-184">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ce009-185">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="ce009-185">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="ce009-186">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="ce009-186">Watermark</span></span>](watermark.md)
    
## <a name="see-also"></a><span data-ttu-id="ce009-187">Confira também</span><span class="sxs-lookup"><span data-stu-id="ce009-187">See also</span></span>



[<span data-ttu-id="ce009-188">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="ce009-188">Unsubscribe operation</span></span>](unsubscribe-operation.md)
  
[<span data-ttu-id="ce009-189">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="ce009-189">GetEvents operation</span></span>](getevents-operation.md)


[<span data-ttu-id="ce009-190">Usando assinaturas pull</span><span class="sxs-lookup"><span data-stu-id="ce009-190">Using Pull Subscriptions</span></span>](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[<span data-ttu-id="ce009-191">Aplicativo de amostra de notificação por push</span><span class="sxs-lookup"><span data-stu-id="ce009-191">Push Notification Sample Application</span></span>](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

