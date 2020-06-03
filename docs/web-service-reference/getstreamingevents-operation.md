---
title: Operação GetStreamingEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetStreamingEvents
api_type:
- schema
ms.assetid: 8da95423-72bc-4034-90a8-162eedcd059b
description: Encontre informações sobre a operação do EWS do GetStreamingEvents.
ms.openlocfilehash: 27744ec40d7c7cb551f35ed5f6fcb726f23d4865
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530166"
---
# <a name="getstreamingevents-operation"></a><span data-ttu-id="cabf2-103">Operação GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="cabf2-103">GetStreamingEvents operation</span></span>

<span data-ttu-id="cabf2-104">Encontre informações sobre a operação do EWS do **GetStreamingEvents** .</span><span class="sxs-lookup"><span data-stu-id="cabf2-104">Find information about the **GetStreamingEvents** EWS operation.</span></span> 
  
<span data-ttu-id="cabf2-105">A operação **GetStreamingEvents** é usada por clientes de assinatura de streaming para solicitar notificações do servidor de acesso para cliente.</span><span class="sxs-lookup"><span data-stu-id="cabf2-105">The **GetStreamingEvents** operation is used by streaming subscription clients to request notifications from the Client Access server.</span></span> <span data-ttu-id="cabf2-106">A resposta **GetStreamingEvents** retorna uma matriz de itens e eventos que ocorreram em uma caixa de correio desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="cabf2-106">The **GetStreamingEvents** response returns an array of items and events that have occurred in a mailbox since the last the notification.</span></span> 
  
## <a name="getstreamingevents-request-example"></a><span data-ttu-id="cabf2-107">Exemplo de solicitação GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="cabf2-107">GetStreamingEvents request example</span></span>

### <a name="description"></a><span data-ttu-id="cabf2-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="cabf2-108">Description</span></span>

<span data-ttu-id="cabf2-109">O exemplo a seguir de uma operação **GetStreamingEvents** mostra como solicitar os eventos e os itens que estão associados a uma assinatura identificada pelo identificador de assinatura.</span><span class="sxs-lookup"><span data-stu-id="cabf2-109">The following example of a **GetStreamingEvents** operation shows how to request the events and items that are associated with a subscription that is identified by the subscription identifier.</span></span> 
  
### <a name="code"></a><span data-ttu-id="cabf2-110">Código</span><span class="sxs-lookup"><span data-stu-id="cabf2-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
  xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Body>
    <GetStreamingEvents xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</SubscriptionId>
      <ConnectionTimeout>30</ConnectionTimeout>
    </GetStreamingEvents>
  </soap:Body>
</soap:Envelope>
```

### <a name="getstreamingevents-request-elements"></a><span data-ttu-id="cabf2-111">Elementos de solicitação GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="cabf2-111">GetStreamingEvents request elements</span></span>

<span data-ttu-id="cabf2-112">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="cabf2-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="cabf2-113">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="cabf2-113">GetStreamingEvents</span></span>](getstreamingevents.md)
    
- [<span data-ttu-id="cabf2-114">SubscriptionId (GetStreamingEvents)</span><span class="sxs-lookup"><span data-stu-id="cabf2-114">SubscriptionId (GetStreamingEvents)</span></span>](subscriptionid-getstreamingevents.md)
    
- [<span data-ttu-id="cabf2-115">ConnectionTimeout</span><span class="sxs-lookup"><span data-stu-id="cabf2-115">ConnectionTimeout</span></span>](connectiontimeout.md)
    
## <a name="successful-getstreamingevents-response-example"></a><span data-ttu-id="cabf2-116">Exemplo de resposta GetStreamingEvents bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="cabf2-116">Successful GetStreamingEvents response example</span></span>

### <a name="description"></a><span data-ttu-id="cabf2-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="cabf2-117">Description</span></span>

<span data-ttu-id="cabf2-118">O exemplo a seguir de uma resposta **GetStreamingEvents** mostra as notificações enviadas para o cliente quando uma nova mensagem de email é recebida.</span><span class="sxs-lookup"><span data-stu-id="cabf2-118">The following example of a **GetStreamingEvents** response shows the notifications that are sent to the client when a new email message is received.</span></span> <span data-ttu-id="cabf2-119">Ele inclui notificações para os seguintes eventos: CreatedEvent, NewMail e ModifiedEvent.</span><span class="sxs-lookup"><span data-stu-id="cabf2-119">It includes notifications for the following events: CreatedEvent, NewMail, and ModifiedEvent.</span></span> 
  
### <a name="code"></a><span data-ttu-id="cabf2-120">Código</span><span class="sxs-lookup"><span data-stu-id="cabf2-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Header xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <ServerVersionInfo xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" />
</soap:Header>
<soap:Body xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <m:GetStreamingEventsResponse xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
    <m:ResponseMessages>
      <m:GetStreamingEventsResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:Notifications>
          <m:Notification>
            <t:SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</t:SubscriptionId>
            <t:CreatedEvent>
              <t:TimeStamp>2013-09-16T04:31:29Z</t:TimeStamp>
              <t:ItemId Id="AAMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwBGAAAAAABSSWVKrmGUTJE+MVIvofglBwDZGACZQpSgSpyNkexYe2b7AAAAAAENAADZGACZQpSgSpyNkexYe2b7AAANGFYwAAA=" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgENAAAA" ChangeKey="AQAAAA==" />
            </t:CreatedEvent>
            <t:NewMailEvent>
              <t:TimeStamp>2013-09-16T04:31:29Z</t:TimeStamp>
              <t:ItemId Id="AAMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwBGAAAAAABSSWVKrmGUTJE+MVIvofglBwDZGACZQpSgSpyNkexYe2b7AAAAAAENAADZGACZQpSgSpyNkexYe2b7AAANGFYwAAA=" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgENAAAA" ChangeKey="AQAAAA==" />
            </t:NewMailEvent>
            <t:ModifiedEvent>
              <t:TimeStamp>2013-09-16T04:31:29Z</t:TimeStamp>
              <t:FolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgENAAAA" ChangeKey="AQAAAA==" />
              <t:ParentFolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgEJAAAA" ChangeKey="AQAAAA==" />
              <t:UnreadCount>1</t:UnreadCount>
            </t:ModifiedEvent>
          </m:Notification>
        </m:Notifications>
      </m:GetStreamingEventsResponseMessage>
    </m:ResponseMessages>
  </m:GetStreamingEventsResponse>
</soap:Body>
```

### <a name="getstreamingevents-response-elements"></a><span data-ttu-id="cabf2-121">Elementos de resposta GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="cabf2-121">GetStreamingEvents response elements</span></span>

<span data-ttu-id="cabf2-122">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="cabf2-122">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="cabf2-123">GetStreamingEventsResponse</span><span class="sxs-lookup"><span data-stu-id="cabf2-123">GetStreamingEventsResponse</span></span>](getstreamingeventsresponse.md)
    
- [<span data-ttu-id="cabf2-124">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="cabf2-124">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="cabf2-125">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="cabf2-125">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md)
    
- [<span data-ttu-id="cabf2-126">NotesFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="cabf2-126">NotesFolderPermissionLevel</span></span>](notesfolderpermissionlevel.md)
    
- [<span data-ttu-id="cabf2-127">Notificação</span><span class="sxs-lookup"><span data-stu-id="cabf2-127">Notification</span></span>](notification-ex15websvcsotherref.md)
    
- [<span data-ttu-id="cabf2-128">SubscriptionId (GetStreamingEvents)</span><span class="sxs-lookup"><span data-stu-id="cabf2-128">SubscriptionId (GetStreamingEvents)</span></span>](subscriptionid-getstreamingevents.md)
    
<span data-ttu-id="cabf2-129">Para encontrar outras opções para a mensagem de resposta da operação **GetStreamingEvents** , explore a hierarquia do esquema.</span><span class="sxs-lookup"><span data-stu-id="cabf2-129">To find other options for the response message of the **GetStreamingEvents** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="cabf2-130">Inicie no elemento [Notification](notification-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="cabf2-130">Start at the [Notification](notification-ex15websvcsotherref.md) element.</span></span> 
  
## <a name="getstreamingevents-error-response-example"></a><span data-ttu-id="cabf2-131">Exemplo de resposta de erro GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="cabf2-131">GetStreamingEvents error response example</span></span>

### <a name="description"></a><span data-ttu-id="cabf2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cabf2-132">Description</span></span>

<span data-ttu-id="cabf2-133">O exemplo a seguir mostra uma resposta de erro a uma solicitação **GetStreamingEvents** .</span><span class="sxs-lookup"><span data-stu-id="cabf2-133">The following example shows an error response to a **GetStreamingEvents** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="cabf2-134">Código</span><span class="sxs-lookup"><span data-stu-id="cabf2-134">Code</span></span>

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
    <GetStreamingEventsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetStreamingEventsResponseMessage ResponseClass="Error">
        <m:MessageText></m:MessageText>
        <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        <m:ResponseCode>ErrorInvalidSubscription</m:ResponseCode>
        <m:ConnectionStatus>Closed</m:ConnectionStatus>
      </m:ResponseMessages>
    </GetStreamingEventsResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="remarks"></a><span data-ttu-id="cabf2-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="cabf2-135">Remarks</span></span>

<span data-ttu-id="cabf2-136">Durante o processamento de uma solicitação **GetStreamingEvents** , o servidor de acesso para cliente realiza as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="cabf2-136">When processing a **GetStreamingEvents** request, the Client Access server performs the following steps:</span></span> 
  
1. <span data-ttu-id="cabf2-137">O [SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md) da solicitação é confirmado como uma assinatura válida hospedada no servidor de acesso para cliente.</span><span class="sxs-lookup"><span data-stu-id="cabf2-137">The [SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md) of the request is confirmed to be a valid subscription that is hosted on the Client Access server.</span></span> <span data-ttu-id="cabf2-138">Se não for, a chamada **GetStreamingEvents** falhará.</span><span class="sxs-lookup"><span data-stu-id="cabf2-138">If it is not, the **GetStreamingEvents** call fails.</span></span> 
    
2. <span data-ttu-id="cabf2-139">O endereço SMTP do usuário autenticado para a solicitação é validado para ter direitos de representação.</span><span class="sxs-lookup"><span data-stu-id="cabf2-139">The SMTP address of the authenticated user for the request is validated to have impersonation rights.</span></span> <span data-ttu-id="cabf2-140">Caso contrário, a solicitação **GetStreamingEvents** falhará.</span><span class="sxs-lookup"><span data-stu-id="cabf2-140">If they do not, the **GetStreamingEvents** request fails.</span></span> 
    
3. <span data-ttu-id="cabf2-141">A fila de assinatura é consultada para eventos que estão aguardando para serem enviados para o cliente.</span><span class="sxs-lookup"><span data-stu-id="cabf2-141">The subscription queue is queried for events that are waiting to be sent to the client.</span></span> <span data-ttu-id="cabf2-142">Se a fila não estiver vazia, os primeiros eventos 50 da fila são retirados da fila e codificados em uma notificação.</span><span class="sxs-lookup"><span data-stu-id="cabf2-142">If the queue is not empty, the first 50 events from the queue are pulled from the queue and encoded into a notification.</span></span>
    
4. <span data-ttu-id="cabf2-143">Se nenhum evento for encontrado na fila, um [StatusEvent](statusevent.md) é gerado e codificado em uma resposta de notificação.</span><span class="sxs-lookup"><span data-stu-id="cabf2-143">If no events are found in the queue, a [StatusEvent](statusevent.md) is generated and encoded into a notification response.</span></span> 
    
5. <span data-ttu-id="cabf2-144">A resposta de notificação é retornada ao cliente.</span><span class="sxs-lookup"><span data-stu-id="cabf2-144">The notification response is returned to the client.</span></span>
    
6. <span data-ttu-id="cabf2-145">Os eventos incluídos na notificação são removidos da fila de assinatura e o servidor de acesso para cliente – a última marca d' água local da assinatura é definida como a marca d' água do último evento retornado.</span><span class="sxs-lookup"><span data-stu-id="cabf2-145">The events that are included in the notification are removed from the subscription queue and the Client Access server-local last watermark for the subscription is set to the watermark of the last event that is returned.</span></span>
    
7. <span data-ttu-id="cabf2-146">O temporizador de tempo limite da assinatura é redefinido.</span><span class="sxs-lookup"><span data-stu-id="cabf2-146">The timeout timer for the subscription is reset.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="cabf2-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="cabf2-147">See also</span></span>



[<span data-ttu-id="cabf2-148">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="cabf2-148">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="cabf2-149">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="cabf2-149">Unsubscribe operation</span></span>](unsubscribe-operation.md)

