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
description: Encontre informações sobre o EWS GetStreamingEvents operação.
ms.openlocfilehash: 0e93be7b14cb1ca6a2a9821b016f7bdc0e8d7772
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823673"
---
# <a name="getstreamingevents-operation"></a><span data-ttu-id="14509-103">Operação GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="14509-103">GetStreamingEvents operation</span></span>

<span data-ttu-id="14509-104">Encontre informações sobre a operação de EWS **GetStreamingEvents** .</span><span class="sxs-lookup"><span data-stu-id="14509-104">Find information about the **GetStreamingEvents** EWS operation.</span></span> 
  
<span data-ttu-id="14509-105">A operação **GetStreamingEvents** é usada por clientes de assinatura de streaming para solicitar notificações de servidor acesso para cliente.</span><span class="sxs-lookup"><span data-stu-id="14509-105">The **GetStreamingEvents** operation is used by streaming subscription clients to request notifications from the Client Access server.</span></span> <span data-ttu-id="14509-106">A resposta **GetStreamingEvents** retorna uma matriz de itens e os eventos que ocorreram em uma caixa de correio desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="14509-106">The **GetStreamingEvents** response returns an array of items and events that have occurred in a mailbox since the last the notification.</span></span> 
  
## <a name="getstreamingevents-request-example"></a><span data-ttu-id="14509-107">Exemplo de solicitação de GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="14509-107">GetStreamingEvents request example</span></span>

### <a name="description"></a><span data-ttu-id="14509-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="14509-108">Description</span></span>

<span data-ttu-id="14509-109">O exemplo a seguir de uma operação **GetStreamingEvents** mostra como solicitar os eventos e os itens que estão associados uma assinatura que é identificada pelo identificador de inscrição.</span><span class="sxs-lookup"><span data-stu-id="14509-109">The following example of a **GetStreamingEvents** operation shows how to request the events and items that are associated with a subscription that is identified by the subscription identifier.</span></span> 
  
### <a name="code"></a><span data-ttu-id="14509-110">Código</span><span class="sxs-lookup"><span data-stu-id="14509-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
  xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Body>
    <GetStreamingEvents xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</SubscriptionId>
      <ConnectionTimeout>30</ConnectionTimeout>
    </GetStreamingEvents>
  </soap:Body>
</soap:Envelope>
```

### <a name="getstreamingevents-request-elements"></a><span data-ttu-id="14509-111">Elementos de solicitação de GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="14509-111">GetStreamingEvents request elements</span></span>

<span data-ttu-id="14509-112">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="14509-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="14509-113">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="14509-113">GetStreamingEvents</span></span>](getstreamingevents.md)
    
- [<span data-ttu-id="14509-114">SubscriptionId (GetStreamingEvents)</span><span class="sxs-lookup"><span data-stu-id="14509-114">SubscriptionId (GetStreamingEvents)</span></span>](subscriptionid-getstreamingevents.md)
    
- [<span data-ttu-id="14509-115">ConnectionTimeout</span><span class="sxs-lookup"><span data-stu-id="14509-115">ConnectionTimeout</span></span>](connectiontimeout.md)
    
## <a name="successful-getstreamingevents-response-example"></a><span data-ttu-id="14509-116">Exemplo de resposta bem-sucedida GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="14509-116">Successful GetStreamingEvents response example</span></span>

### <a name="description"></a><span data-ttu-id="14509-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="14509-117">Description</span></span>

<span data-ttu-id="14509-118">O exemplo a seguir de uma resposta **GetStreamingEvents** mostra as notificações que são enviadas para o cliente quando uma nova mensagem de email é recebida.</span><span class="sxs-lookup"><span data-stu-id="14509-118">The following example of a **GetStreamingEvents** response shows the notifications that are sent to the client when a new email message is received.</span></span> <span data-ttu-id="14509-119">Ele inclui notificações para os seguintes eventos: CreatedEvent, NewMail e ModifiedEvent.</span><span class="sxs-lookup"><span data-stu-id="14509-119">It includes notifications for the following events: CreatedEvent, NewMail, and ModifiedEvent.</span></span> 
  
### <a name="code"></a><span data-ttu-id="14509-120">Código</span><span class="sxs-lookup"><span data-stu-id="14509-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Header xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <ServerVersionInfo xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" />
</soap:Header>
<soap:Body xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <m:GetStreamingEventsResponse xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="getstreamingevents-response-elements"></a><span data-ttu-id="14509-121">Elementos de resposta GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="14509-121">GetStreamingEvents response elements</span></span>

<span data-ttu-id="14509-122">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="14509-122">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="14509-123">GetStreamingEventsResponse</span><span class="sxs-lookup"><span data-stu-id="14509-123">GetStreamingEventsResponse</span></span>](getstreamingeventsresponse.md)
    
- [<span data-ttu-id="14509-124">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="14509-124">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="14509-125">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="14509-125">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md)
    
- [<span data-ttu-id="14509-126">NotesFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="14509-126">NotesFolderPermissionLevel</span></span>](notesfolderpermissionlevel.md)
    
- [<span data-ttu-id="14509-127">Notificação</span><span class="sxs-lookup"><span data-stu-id="14509-127">Notification</span></span>](notification-ex15websvcsotherref.md)
    
- [<span data-ttu-id="14509-128">SubscriptionId (GetStreamingEvents)</span><span class="sxs-lookup"><span data-stu-id="14509-128">SubscriptionId (GetStreamingEvents)</span></span>](subscriptionid-getstreamingevents.md)
    
<span data-ttu-id="14509-129">Para localizar outras opções para a mensagem de resposta da operação **GetStreamingEvents** , explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="14509-129">To find other options for the response message of the **GetStreamingEvents** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="14509-130">Inicie o elemento de [notificação](notification-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="14509-130">Start at the [Notification](notification-ex15websvcsotherref.md) element.</span></span> 
  
## <a name="getstreamingevents-error-response-example"></a><span data-ttu-id="14509-131">Exemplo de resposta de erro GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="14509-131">GetStreamingEvents error response example</span></span>

### <a name="description"></a><span data-ttu-id="14509-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="14509-132">Description</span></span>

<span data-ttu-id="14509-133">O exemplo a seguir mostra uma resposta de erro a uma solicitação **GetStreamingEvents** .</span><span class="sxs-lookup"><span data-stu-id="14509-133">The following example shows an error response to a **GetStreamingEvents** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="14509-134">Código</span><span class="sxs-lookup"><span data-stu-id="14509-134">Code</span></span>

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
    <GetStreamingEventsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="remarks"></a><span data-ttu-id="14509-135">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="14509-135">Remarks</span></span>

<span data-ttu-id="14509-136">Ao processar uma solicitação de **GetStreamingEvents** , o servidor de acesso para cliente executa as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="14509-136">When processing a **GetStreamingEvents** request, the Client Access server performs the following steps:</span></span> 
  
1. <span data-ttu-id="14509-137">A [SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md) da solicitação é confirmada seja uma assinatura válida que está hospedada no servidor de acesso para cliente.</span><span class="sxs-lookup"><span data-stu-id="14509-137">The [SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md) of the request is confirmed to be a valid subscription that is hosted on the Client Access server.</span></span> <span data-ttu-id="14509-138">Se não for, a chamada de **GetStreamingEvents** falhar.</span><span class="sxs-lookup"><span data-stu-id="14509-138">If it is not, the **GetStreamingEvents** call fails.</span></span> 
    
2. <span data-ttu-id="14509-139">O endereço SMTP do usuário autenticado para a solicitação é validado para ter direitos de representação.</span><span class="sxs-lookup"><span data-stu-id="14509-139">The SMTP address of the authenticated user for the request is validated to have impersonation rights.</span></span> <span data-ttu-id="14509-140">Se não tiverem, a solicitação de **GetStreamingEvents** falhará.</span><span class="sxs-lookup"><span data-stu-id="14509-140">If they do not, the **GetStreamingEvents** request fails.</span></span> 
    
3. <span data-ttu-id="14509-141">A fila de inscrição é consultada para eventos que estão em espera a serem enviados para o cliente.</span><span class="sxs-lookup"><span data-stu-id="14509-141">The subscription queue is queried for events that are waiting to be sent to the client.</span></span> <span data-ttu-id="14509-142">Se a fila não está vazia, os 50 primeiros eventos da fila são retirados da fila e codificados em uma notificação.</span><span class="sxs-lookup"><span data-stu-id="14509-142">If the queue is not empty, the first 50 events from the queue are pulled from the queue and encoded into a notification.</span></span>
    
4. <span data-ttu-id="14509-143">Se nenhum evento forem encontrado na fila, um [StatusEvent](statusevent.md) será gerado e codificada em uma resposta de notificação.</span><span class="sxs-lookup"><span data-stu-id="14509-143">If no events are found in the queue, a [StatusEvent](statusevent.md) is generated and encoded into a notification response.</span></span> 
    
5. <span data-ttu-id="14509-144">A resposta de notificação é retornada para o cliente.</span><span class="sxs-lookup"><span data-stu-id="14509-144">The notification response is returned to the client.</span></span>
    
6. <span data-ttu-id="14509-145">Os eventos que estão incluídos na notificação são removidos da fila de assinatura e acesso para cliente local de servidor última marca d'água para a assinatura é definida como a marca d'água do último evento que é retornado.</span><span class="sxs-lookup"><span data-stu-id="14509-145">The events that are included in the notification are removed from the subscription queue and the Client Access server-local last watermark for the subscription is set to the watermark of the last event that is returned.</span></span>
    
7. <span data-ttu-id="14509-146">O timer de tempo limite para a assinatura é redefinido.</span><span class="sxs-lookup"><span data-stu-id="14509-146">The timeout timer for the subscription is reset.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="14509-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="14509-147">See also</span></span>



[<span data-ttu-id="14509-148">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="14509-148">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="14509-149">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="14509-149">Unsubscribe operation</span></span>](unsubscribe-operation.md)

