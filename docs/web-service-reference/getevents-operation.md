---
title: Operação GetEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetEvents
api_type:
- schema
ms.assetid: f268efe5-9a1a-41a2-b6a6-51fcde7720a1
description: A operação GetEvents é usada por clientes de assinatura pull para solicitar notificações do servidor de acesso para cliente. A resposta da operação GetEvents retorna uma matriz de itens e eventos que ocorreram em uma caixa de correio desde a última notificação.
ms.openlocfilehash: 9258fd003c242911866aa7abbca5eba2b9582223
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462511"
---
# <a name="getevents-operation"></a><span data-ttu-id="120fb-104">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="120fb-104">GetEvents operation</span></span>

<span data-ttu-id="120fb-105">A operação **GetEvents** é usada por clientes de assinatura pull para solicitar notificações do servidor de acesso para cliente.</span><span class="sxs-lookup"><span data-stu-id="120fb-105">The **GetEvents** operation is used by pull subscription clients to request notifications from the Client Access server.</span></span> <span data-ttu-id="120fb-106">A resposta da operação **GetEvents** retorna uma matriz de itens e eventos que ocorreram em uma caixa de correio desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="120fb-106">The **GetEvents** operation response returns an array of items and events that have occurred in a mailbox since the last the notification.</span></span> 
  
> [!IMPORTANT]
> <span data-ttu-id="120fb-107">A operação **DeleteUserConfiguration** acionará um evento move para o sistema de notificação de eventos.</span><span class="sxs-lookup"><span data-stu-id="120fb-107">The **DeleteUserConfiguration** operation will trigger a move event for the event notification system.</span></span> <span data-ttu-id="120fb-108">O objeto de configuração do usuário será movido para o dumpster.</span><span class="sxs-lookup"><span data-stu-id="120fb-108">The user configuration object will be moved to the dumpster.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="120fb-109">Comentários</span><span class="sxs-lookup"><span data-stu-id="120fb-109">Remarks</span></span>

<span data-ttu-id="120fb-110">Alterações nos itens de calendário podem resultar na geração de vários eventos.</span><span class="sxs-lookup"><span data-stu-id="120fb-110">Changes to Calendar items may result in the generation of multiple events.</span></span> <span data-ttu-id="120fb-111">Esses eventos são o resultado de itens temporários sendo criados na caixa de correio, os itens de armazenamento de dados de disponibilidade estão sendo alterados como parte das operações normais do calendário ou ambos.</span><span class="sxs-lookup"><span data-stu-id="120fb-111">These events are the result of temporary items being created in the mailbox, free/busy data storage items being changed as part of the normal Calendar operations, or both.</span></span> <span data-ttu-id="120fb-112">Eventos de classe de item "IPM. SchedulePlus. FreeBusy. BinaryData "deve ser ignorado por clientes de serviço Web.</span><span class="sxs-lookup"><span data-stu-id="120fb-112">Events for item class "IPM.SchedulePlus.FreeBusy.BinaryData" should be ignored by Web service clients.</span></span> <span data-ttu-id="120fb-113">Esses itens temporários são excluídos após serem criados; Portanto, se for feita uma tentativa de recuperar esses itens, um erro será retornado afirmando que o item não foi encontrado.</span><span class="sxs-lookup"><span data-stu-id="120fb-113">These temporary items are deleted after they are created; therefore, if an attempt is made to retrieve these items, an error will be returned that states that the item was not found.</span></span>
  
## <a name="getevents-request-example"></a><span data-ttu-id="120fb-114">Exemplo de solicitação GetEvents</span><span class="sxs-lookup"><span data-stu-id="120fb-114">GetEvents request example</span></span>

### <a name="description"></a><span data-ttu-id="120fb-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="120fb-115">Description</span></span>

<span data-ttu-id="120fb-116">O exemplo a seguir mostra como solicitar os eventos e os itens que estão associados a uma assinatura identificada pelo identificador de assinatura e marca d' água.</span><span class="sxs-lookup"><span data-stu-id="120fb-116">The following example shows how to request the events and items that are associated with a subscription that is identified by the subscription identifier and watermark.</span></span>
  
### <a name="code"></a><span data-ttu-id="120fb-117">Código</span><span class="sxs-lookup"><span data-stu-id="120fb-117">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetEvents xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</SubscriptionId>
      <Watermark>AAAAAMAGAAAAAAAAAQ==</Watermark>
    </GetEvents>
  </soap:Body>
</soap:Envelope>
```

### <a name="getevents-request-elements"></a><span data-ttu-id="120fb-118">Elementos de solicitação GetEvents</span><span class="sxs-lookup"><span data-stu-id="120fb-118">GetEvents Request Elements</span></span>

<span data-ttu-id="120fb-119">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="120fb-119">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="120fb-120">GetEvents</span><span class="sxs-lookup"><span data-stu-id="120fb-120">GetEvents</span></span>](getevents.md)
    
- [<span data-ttu-id="120fb-121">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="120fb-121">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="120fb-122">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="120fb-122">Watermark</span></span>](watermark.md)
    
## <a name="successful-getevents-response-example"></a><span data-ttu-id="120fb-123">Exemplo de resposta de GetEvents bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="120fb-123">Successful GetEvents response example</span></span>

### <a name="description"></a><span data-ttu-id="120fb-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="120fb-124">Description</span></span>

<span data-ttu-id="120fb-125">O exemplo a seguir de uma resposta mostra uma notificação da existência de duas novas mensagens de email desde que a última solicitação de notificação foi enviada ao servidor.</span><span class="sxs-lookup"><span data-stu-id="120fb-125">The following example of a response shows a notification of the existence of two new mail messages since the last notification request was sent to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="120fb-126">Código</span><span class="sxs-lookup"><span data-stu-id="120fb-126">Code</span></span>

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
    <GetEventsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetEventsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Notification>
            <t:SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</t:SubscriptionId>
            <t:PreviousWatermark>AAAAAMAGAAAAAAAAAQ==</t:PreviousWatermark>
            <t:MoreEvents>false</t:MoreEvents>
            <t:NewMailEvent>
              <t:Watermark>AAAAAM4GAAAAAAAAAQ==</t:Watermark>
              <t:TimeStamp>2006-08-22T00:36:29Z</t:TimeStamp>
              <t:ItemId Id="AQApAHR" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQApAH" ChangeKey="AQAAAA==" />
            </t:NewMailEvent>
            <t:NewMailEvent>
              <t:Watermark>AAAAAOQGAAAAAAAAAQ==</t:Watermark>
              <t:TimeStamp>2006-08-22T01:00:50Z</t:TimeStamp>
              <t:ItemId Id="AQApAHRw" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQApAH" ChangeKey="AQAAAA==" />
            </t:NewMailEvent>
          </m:Notification>
        </m:GetEventsResponseMessage>
      </m:ResponseMessages>
    </GetEventsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="120fb-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="120fb-127">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="120fb-128">Os identificadores de item e de pasta foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="120fb-128">The item and folder identifiers have been shortened to preserve readability.</span></span> 
  
### <a name="getevents-response-elements"></a><span data-ttu-id="120fb-129">Elementos de resposta de GetEvents</span><span class="sxs-lookup"><span data-stu-id="120fb-129">GetEvents response elements</span></span>

<span data-ttu-id="120fb-130">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="120fb-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="120fb-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="120fb-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="120fb-132">GetEventsResponse</span><span class="sxs-lookup"><span data-stu-id="120fb-132">GetEventsResponse</span></span>](geteventsresponse.md)
    
- [<span data-ttu-id="120fb-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="120fb-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="120fb-134">GetEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="120fb-134">GetEventsResponseMessage</span></span>](geteventsresponsemessage.md)
    
- [<span data-ttu-id="120fb-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="120fb-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="120fb-136">Notificação</span><span class="sxs-lookup"><span data-stu-id="120fb-136">Notification</span></span>](notification-ex15websvcsotherref.md)
    
- [<span data-ttu-id="120fb-137">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="120fb-137">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="120fb-138">PreviousWatermark</span><span class="sxs-lookup"><span data-stu-id="120fb-138">PreviousWatermark</span></span>](previouswatermark.md)
    
- [<span data-ttu-id="120fb-139">MoreEvents</span><span class="sxs-lookup"><span data-stu-id="120fb-139">MoreEvents</span></span>](moreevents.md)
    
- [<span data-ttu-id="120fb-140">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="120fb-140">NewMailEvent</span></span>](newmailevent.md)
    
- [<span data-ttu-id="120fb-141">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="120fb-141">Watermark</span></span>](watermark.md)
    
- [<span data-ttu-id="120fb-142">Registra</span><span class="sxs-lookup"><span data-stu-id="120fb-142">TimeStamp</span></span>](timestamp.md)
    
- [<span data-ttu-id="120fb-143">ItemId</span><span class="sxs-lookup"><span data-stu-id="120fb-143">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="120fb-144">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="120fb-144">ParentFolderId</span></span>](parentfolderid.md)
    
<span data-ttu-id="120fb-145">Para encontrar outras opções para a mensagem de resposta da operação **GetEvents** , explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="120fb-145">To find other options for the response message of the **GetEvents** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="120fb-146">Inicie no elemento [Notification](notification-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="120fb-146">Start at the [Notification](notification-ex15websvcsotherref.md) element.</span></span> 
  
## <a name="getevents-error-response-example"></a><span data-ttu-id="120fb-147">Exemplo de resposta de erro GetEvents</span><span class="sxs-lookup"><span data-stu-id="120fb-147">GetEvents Error response example</span></span>

### <a name="description"></a><span data-ttu-id="120fb-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="120fb-148">Description</span></span>

<span data-ttu-id="120fb-149">O exemplo a seguir mostra uma resposta de erro a uma solicitação **GetEvents** .</span><span class="sxs-lookup"><span data-stu-id="120fb-149">The following example shows an error response to a **GetEvents** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="120fb-150">Código</span><span class="sxs-lookup"><span data-stu-id="120fb-150">Code</span></span>

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
    <GetEventsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetEventsResponseMessage ResponseClass="Error">
          <m:MessageText>Access is denied. Only the subscription owner may access the subscription.</m:MessageText>
          <m:ResponseCode>ErrorSubscriptionAccessDenied</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:GetEventsResponseMessage>
      </m:ResponseMessages>
    </GetEventsResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="remarks"></a><span data-ttu-id="120fb-151">Comentários</span><span class="sxs-lookup"><span data-stu-id="120fb-151">Remarks</span></span>

<span data-ttu-id="120fb-152">Durante o processamento de uma solicitação **GetEvents** , o servidor de acesso para cliente realiza as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="120fb-152">When processing a **GetEvents** request, the Client Access server performs the following steps:</span></span> 
  
1. <span data-ttu-id="120fb-153">A SubscriptionId da solicitação é confirmada como uma assinatura válida hospedada no servidor de acesso para cliente.</span><span class="sxs-lookup"><span data-stu-id="120fb-153">The SubscriptionID of the request is confirmed to be a valid subscription that is hosted on the Client Access server.</span></span> <span data-ttu-id="120fb-154">Se não for, a chamada **GetEvents** falhará.</span><span class="sxs-lookup"><span data-stu-id="120fb-154">If it is not, the **GetEvents** call fails.</span></span> 
    
2. <span data-ttu-id="120fb-155">O endereço SMTP do usuário autenticado para a solicitação é comparado com o endereço SMTP do usuário que criou a assinatura.</span><span class="sxs-lookup"><span data-stu-id="120fb-155">The SMTP address of the authenticated user for the request is compared to the SMTP address of the user who created the subscription.</span></span> <span data-ttu-id="120fb-156">Se eles não corresponderem, a solicitação **GetEvents** falhará.</span><span class="sxs-lookup"><span data-stu-id="120fb-156">If they do not match, the **GetEvents** request fails.</span></span> 
    
3. <span data-ttu-id="120fb-157">A fila de assinatura é consultada para eventos que estão aguardando para serem enviados para o cliente.</span><span class="sxs-lookup"><span data-stu-id="120fb-157">The subscription queue is queried for events that are waiting to be sent to the client.</span></span> <span data-ttu-id="120fb-158">Se a fila não estiver vazia, os primeiros eventos 50 da fila são retirados da fila e codificados em uma notificação.</span><span class="sxs-lookup"><span data-stu-id="120fb-158">If the queue is not empty, the first 50 events from the queue are pulled from the queue and encoded into a notification.</span></span>
    
4. <span data-ttu-id="120fb-159">Se nenhum evento for encontrado na fila, um StatusEvent é gerado e codificado em uma resposta de notificação.</span><span class="sxs-lookup"><span data-stu-id="120fb-159">If no events are found in the queue, a StatusEvent is generated and encoded into a notification response.</span></span>
    
5. <span data-ttu-id="120fb-160">A resposta de notificação é retornada ao cliente.</span><span class="sxs-lookup"><span data-stu-id="120fb-160">The notification response is returned to the client.</span></span>
    
6. <span data-ttu-id="120fb-161">Os eventos incluídos na notificação são removidos da fila de assinatura e o servidor de acesso para cliente última marca d' água local da assinatura é definida como a marca d' água do último evento retornado.</span><span class="sxs-lookup"><span data-stu-id="120fb-161">The events that are included in the notification are removed from the subscription queue and the Client Access server local last watermark for the subscription is set to the watermark of the last event that is returned.</span></span>
    
7. <span data-ttu-id="120fb-162">O temporizador de tempo limite da assinatura é redefinido.</span><span class="sxs-lookup"><span data-stu-id="120fb-162">The timeout timer for the subscription is reset.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="120fb-163">Confira também</span><span class="sxs-lookup"><span data-stu-id="120fb-163">See also</span></span>



[<span data-ttu-id="120fb-164">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="120fb-164">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="120fb-165">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="120fb-165">Unsubscribe operation</span></span>](unsubscribe-operation.md)


[<span data-ttu-id="120fb-166">Usando assinaturas pull</span><span class="sxs-lookup"><span data-stu-id="120fb-166">Using Pull Subscriptions</span></span>](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)

