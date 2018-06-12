---
title: Inscrever-se a operação
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
description: A operação Subscribe é usada para assinar notificações de envio ou recepção aplicativos de cliente. É importante estar ciente de que a estrutura das respostas e mensagens de solicitação é diferente, dependendo do tipo de notificação de evento.
ms.openlocfilehash: f6cacab80c8ca2e505ab63a162a161fcf5de8585
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825619"
---
# <a name="subscribe-operation"></a><span data-ttu-id="7f40e-104">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="7f40e-104">Subscribe operation</span></span>

<span data-ttu-id="7f40e-105">A operação Subscribe é usada para assinar notificações de envio ou recepção aplicativos de cliente.</span><span class="sxs-lookup"><span data-stu-id="7f40e-105">The Subscribe operation is used to subscribe client applications to either push or pull notifications.</span></span> <span data-ttu-id="7f40e-106">É importante estar ciente de que a estrutura das respostas e mensagens de solicitação é diferente, dependendo do tipo de notificação de evento.</span><span class="sxs-lookup"><span data-stu-id="7f40e-106">It is important to be aware that the structure of the request messages and responses is different depending on the type of event notification.</span></span> 
  
## <a name="pull-subscription-subscribe-request-example"></a><span data-ttu-id="7f40e-107">Exemplo de solicitação de assinatura assinar recepção</span><span class="sxs-lookup"><span data-stu-id="7f40e-107">Pull Subscription Subscribe request example</span></span>

### <a name="description"></a><span data-ttu-id="7f40e-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f40e-108">Description</span></span>

<span data-ttu-id="7f40e-109">O exemplo de código a seguir mostra como se inscrever para uma inscrição de notificação de evento de recepção.</span><span class="sxs-lookup"><span data-stu-id="7f40e-109">The following code example shows how to subscribe to a pull event notification subscription.</span></span> <span data-ttu-id="7f40e-110">A assinatura informa o aplicativo cliente se novos emails é adicionado à caixa de entrada e se um item é excluído da caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="7f40e-110">The subscription informs the client application if new mail is added to the Inbox and if an item is deleted from the Inbox.</span></span> <span data-ttu-id="7f40e-111">A assinatura será o tempo limite se o cliente não requisitar informações sobre eventos dentro de dez minutos.</span><span class="sxs-lookup"><span data-stu-id="7f40e-111">The subscription will time out if the client does not request information about events within ten minutes.</span></span> <span data-ttu-id="7f40e-112">Se a assinatura expirar, uma nova assinatura deve ser estabelecida para continuar solicitar notificações.</span><span class="sxs-lookup"><span data-stu-id="7f40e-112">If the subscription expires, a new subscription must be established to continue to request notifications.</span></span>
  
### <a name="code"></a><span data-ttu-id="7f40e-113">Código</span><span class="sxs-lookup"><span data-stu-id="7f40e-113">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Subscribe xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="pull-subscription-subscribe-request-elements"></a><span data-ttu-id="7f40e-114">Inscrição de recepção assine os elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7f40e-114">Pull Subscription Subscribe Request Elements</span></span>

<span data-ttu-id="7f40e-115">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="7f40e-115">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="7f40e-116">Inscrever-se</span><span class="sxs-lookup"><span data-stu-id="7f40e-116">Subscribe</span></span>](subscribe.md)
    
- [<span data-ttu-id="7f40e-117">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="7f40e-117">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md)
    
- [<span data-ttu-id="7f40e-118">FolderIds</span><span class="sxs-lookup"><span data-stu-id="7f40e-118">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="7f40e-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="7f40e-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="7f40e-120">EventTypes</span><span class="sxs-lookup"><span data-stu-id="7f40e-120">EventTypes</span></span>](eventtypes.md)
    
- [<span data-ttu-id="7f40e-121">EventType</span><span class="sxs-lookup"><span data-stu-id="7f40e-121">EventType</span></span>](eventtype.md)
    
- [<span data-ttu-id="7f40e-122">Timeout</span><span class="sxs-lookup"><span data-stu-id="7f40e-122">Timeout</span></span>](timeout.md)
    
<span data-ttu-id="7f40e-123">Para localizar outras opções para a mensagem de solicitação da operação Subscribe, explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="7f40e-123">To find other options for the request message of the Subscribe operation, explore the schema hierarchy.</span></span> <span data-ttu-id="7f40e-124">Inicie o elemento [PullSubscriptionRequest](pullsubscriptionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="7f40e-124">Start at the [PullSubscriptionRequest](pullsubscriptionrequest.md) element.</span></span> 
  
## <a name="successful-pull-subscription-subscribe-response-example"></a><span data-ttu-id="7f40e-125">Exemplo de resposta Pull assinatura assinar bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="7f40e-125">Successful Pull Subscription Subscribe response example</span></span>

### <a name="description"></a><span data-ttu-id="7f40e-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f40e-126">Description</span></span>

<span data-ttu-id="7f40e-127">O exemplo a seguir mostra uma resposta de inscrição de recepção bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="7f40e-127">The following example shows a successful pull subscription response.</span></span> <span data-ttu-id="7f40e-128">A resposta conterá o identificador de inscrição e marca d'água que é usada para obter a matriz de eventos que estão associados uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="7f40e-128">The response contains the subscription identifier and watermark that is used to get the array of events that are associated with a subscription.</span></span> <span data-ttu-id="7f40e-129">O identificador de inscrição também é usado para cancelar a assinatura de um cliente de uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="7f40e-129">The subscription identifier is also used to unsubscribe a client from a subscription.</span></span>
  
### <a name="code"></a><span data-ttu-id="7f40e-130">Código</span><span class="sxs-lookup"><span data-stu-id="7f40e-130">Code</span></span>

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
    <SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="pull-subscription-subscribe-response-elements"></a><span data-ttu-id="7f40e-131">Recepção de assinatura assinar elementos de resposta</span><span class="sxs-lookup"><span data-stu-id="7f40e-131">Pull Subscription Subscribe response elements</span></span>

<span data-ttu-id="7f40e-132">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="7f40e-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="7f40e-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7f40e-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="7f40e-134">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="7f40e-134">SubscribeResponse</span></span>](subscriberesponse.md)
    
- [<span data-ttu-id="7f40e-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7f40e-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="7f40e-136">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7f40e-136">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
    
- [<span data-ttu-id="7f40e-137">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7f40e-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7f40e-138">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="7f40e-138">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="7f40e-139">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="7f40e-139">Watermark</span></span>](watermark.md)
    
## <a name="pull-subscription-subscribe-error-response-example"></a><span data-ttu-id="7f40e-140">Exemplo de resposta de erro na assinatura assinar recepção</span><span class="sxs-lookup"><span data-stu-id="7f40e-140">Pull Subscription Subscribe Error response example</span></span>

### <a name="description"></a><span data-ttu-id="7f40e-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f40e-141">Description</span></span>

<span data-ttu-id="7f40e-142">O exemplo a seguir mostra uma resposta a uma solicitação Subscribe de erro.</span><span class="sxs-lookup"><span data-stu-id="7f40e-142">The following example shows an error response to a Subscribe request.</span></span> <span data-ttu-id="7f40e-143">O erro é causado por uma tentativa para assinar notificações usando o acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="7f40e-143">The error is caused by an attempt to subscribe to notifications by using delegate access.</span></span>
  
### <a name="code"></a><span data-ttu-id="7f40e-144">Código</span><span class="sxs-lookup"><span data-stu-id="7f40e-144">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="pull-subscription-error-response-elements"></a><span data-ttu-id="7f40e-145">Coloque os elementos de resposta de erro na assinatura</span><span class="sxs-lookup"><span data-stu-id="7f40e-145">Pull Subscription Error response elements</span></span>

<span data-ttu-id="7f40e-146">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="7f40e-146">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="7f40e-147">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7f40e-147">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="7f40e-148">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="7f40e-148">SubscribeResponse</span></span>](subscriberesponse.md)
    
- [<span data-ttu-id="7f40e-149">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7f40e-149">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="7f40e-150">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7f40e-150">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
    
- [<span data-ttu-id="7f40e-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="7f40e-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="7f40e-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7f40e-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7f40e-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7f40e-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="push-subscription-request-example"></a><span data-ttu-id="7f40e-154">Exemplo de solicitação de assinatura de push</span><span class="sxs-lookup"><span data-stu-id="7f40e-154">Push Subscription request example</span></span>

### <a name="description"></a><span data-ttu-id="7f40e-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f40e-155">Description</span></span>

<span data-ttu-id="7f40e-156">O exemplo de código a seguir mostra como se inscrever para uma inscrição de notificação de evento de envio.</span><span class="sxs-lookup"><span data-stu-id="7f40e-156">The following code example shows how to subscribe to a push event notification subscription.</span></span> <span data-ttu-id="7f40e-157">A solicitação identifica as pastas a serem monitorados, os tipos de eventos a serem monitorados, a frequência das notificações de status e a URL do serviço Web que escuta as notificações de push do cliente.</span><span class="sxs-lookup"><span data-stu-id="7f40e-157">The request identifies the folders to monitor, the types of events to monitor, the frequency of status notifications, and the URL of the client Web service that listens for the push notifications.</span></span>
  
### <a name="code"></a><span data-ttu-id="7f40e-158">Código</span><span class="sxs-lookup"><span data-stu-id="7f40e-158">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Subscribe xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <PushSubscriptionRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <FolderIds xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <DistinguishedFolderId Id="inbox" />
        </FolderIds>
        <EventTypes xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <EventType>NewMailEvent</EventType>
          <EventType>CopiedEvent</EventType>
          <EventType>CreatedEvent</EventType>
          <EventType>DeletedEvent</EventType>
          <EventType>ModifiedEvent</EventType>
          <EventType>MovedEvent</EventType>
        </EventTypes>
        <StatusFrequency xmlns="http://schemas.microsoft.com/exchange/services/2006/types">1</StatusFrequency>
        <URL xmlns="http://schemas.microsoft.com/exchange/services/2006/types">http://clientWebService/Service.asmx</URL>
      </PushSubscriptionRequest>
    </Subscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="7f40e-159">Comments</span><span class="sxs-lookup"><span data-stu-id="7f40e-159">Comments</span></span>

<span data-ttu-id="7f40e-160">O cliente do Web service deve ser configurada antes da notificação por push assine a solicitação é enviado; Caso contrário, a primeira notificação não será enviada para um ponto de extremidade válido e a notificação por push falhará.</span><span class="sxs-lookup"><span data-stu-id="7f40e-160">The client Web service must be set up before the push notification subscribe request is sent; otherwise, the first notification will not be sent to a valid endpoint and the push notification will fail.</span></span> <span data-ttu-id="7f40e-161">Para obter mais informações, consulte o [Aplicativo de amostra de notificação de Push](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="7f40e-161">For more information, see [Push Notification Sample Application](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx).</span></span>
  
<span data-ttu-id="7f40e-162">Um novo [SubscriptionId (GetEvents)](subscriptionid-getevents.md) é criado quando você inscrever-se novamente.</span><span class="sxs-lookup"><span data-stu-id="7f40e-162">A new [SubscriptionId (GetEvents)](subscriptionid-getevents.md) is created when you resubscribe.</span></span> <span data-ttu-id="7f40e-163">Use a marca d'água de uma assinatura anterior para inscrever-se novamente no ponto de onde a assinatura anterior terminou.</span><span class="sxs-lookup"><span data-stu-id="7f40e-163">Use the watermark of a previous subscription to resubscribe at the point where the previous subscription ended.</span></span> 
  
### <a name="push-subscription-request-elements"></a><span data-ttu-id="7f40e-164">Elementos de solicitação de assinatura de push</span><span class="sxs-lookup"><span data-stu-id="7f40e-164">Push Subscription Request Elements</span></span>

<span data-ttu-id="7f40e-165">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="7f40e-165">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="7f40e-166">Inscrever-se</span><span class="sxs-lookup"><span data-stu-id="7f40e-166">Subscribe</span></span>](subscribe.md)
    
- [<span data-ttu-id="7f40e-167">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="7f40e-167">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
    
- [<span data-ttu-id="7f40e-168">FolderIds</span><span class="sxs-lookup"><span data-stu-id="7f40e-168">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="7f40e-169">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="7f40e-169">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="7f40e-170">EventTypes</span><span class="sxs-lookup"><span data-stu-id="7f40e-170">EventTypes</span></span>](eventtypes.md)
    
- [<span data-ttu-id="7f40e-171">EventType</span><span class="sxs-lookup"><span data-stu-id="7f40e-171">EventType</span></span>](eventtype.md)
    
- [<span data-ttu-id="7f40e-172">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="7f40e-172">StatusFrequency</span></span>](statusfrequency.md)
    
- [<span data-ttu-id="7f40e-173">URL</span><span class="sxs-lookup"><span data-stu-id="7f40e-173">Url </span></span>](url-ex15websvcsotherref.md)
    
## <a name="successful-push-subscription-response-example"></a><span data-ttu-id="7f40e-174">Exemplo de resposta de assinatura Push bem-sucedidas</span><span class="sxs-lookup"><span data-stu-id="7f40e-174">Successful Push Subscription response example</span></span>

### <a name="description"></a><span data-ttu-id="7f40e-175">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f40e-175">Description</span></span>

<span data-ttu-id="7f40e-176">O exemplo a seguir mostra uma resposta de assinatura push bem-sucedidas.</span><span class="sxs-lookup"><span data-stu-id="7f40e-176">The following example shows a successful push subscription response.</span></span> 
  
### <a name="code"></a><span data-ttu-id="7f40e-177">Código</span><span class="sxs-lookup"><span data-stu-id="7f40e-177">Code</span></span>

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
    <SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="push-subscription-response-elements"></a><span data-ttu-id="7f40e-178">Elementos de resposta de assinatura de push</span><span class="sxs-lookup"><span data-stu-id="7f40e-178">Push Subscription response elements</span></span>

<span data-ttu-id="7f40e-179">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="7f40e-179">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="7f40e-180">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7f40e-180">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="7f40e-181">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="7f40e-181">SubscribeResponse</span></span>](subscriberesponse.md)
    
- [<span data-ttu-id="7f40e-182">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7f40e-182">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="7f40e-183">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7f40e-183">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
    
- [<span data-ttu-id="7f40e-184">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7f40e-184">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7f40e-185">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="7f40e-185">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="7f40e-186">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="7f40e-186">Watermark</span></span>](watermark.md)
    
## <a name="see-also"></a><span data-ttu-id="7f40e-187">Confira também</span><span class="sxs-lookup"><span data-stu-id="7f40e-187">See also</span></span>



[<span data-ttu-id="7f40e-188">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="7f40e-188">Unsubscribe operation</span></span>](unsubscribe-operation.md)
  
[<span data-ttu-id="7f40e-189">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="7f40e-189">GetEvents operation</span></span>](getevents-operation.md)


[<span data-ttu-id="7f40e-190">Usando inscrições de recepção</span><span class="sxs-lookup"><span data-stu-id="7f40e-190">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[<span data-ttu-id="7f40e-191">Aplicativo de amostra de notificação de push</span><span class="sxs-lookup"><span data-stu-id="7f40e-191">Push Notification Sample Application</span></span>](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

