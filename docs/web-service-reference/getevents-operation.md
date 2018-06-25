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
description: A operação GetEvents é usada pelos clientes de inscrição de recepção para notificações de solicitação do servidor de acesso para cliente. A resposta de operação GetEvents retorna uma matriz de itens e os eventos que ocorreram em uma caixa de correio desde a última notificação.
ms.openlocfilehash: 1a23a9d570a4554e54becb7927f25dff89888c74
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752473"
---
# <a name="getevents-operation"></a><span data-ttu-id="b054b-104">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="b054b-104">GetEvents operation</span></span>

<span data-ttu-id="b054b-105">A operação **GetEvents** é usada pelos clientes de inscrição de recepção para notificações de solicitação do servidor de acesso para cliente.</span><span class="sxs-lookup"><span data-stu-id="b054b-105">The **GetEvents** operation is used by pull subscription clients to request notifications from the Client Access server.</span></span> <span data-ttu-id="b054b-106">A resposta de operação **GetEvents** retorna uma matriz de itens e os eventos que ocorreram em uma caixa de correio desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="b054b-106">The **GetEvents** operation response returns an array of items and events that have occurred in a mailbox since the last the notification.</span></span> 
  
> [!IMPORTANT]
> <span data-ttu-id="b054b-107">A operação **DeleteUserConfiguration** irá disparar um evento de movimentação para o sistema de notificação de evento.</span><span class="sxs-lookup"><span data-stu-id="b054b-107">The **DeleteUserConfiguration** operation will trigger a move event for the event notification system.</span></span> <span data-ttu-id="b054b-108">O objeto de configuração do usuário será movido para o dumpster.</span><span class="sxs-lookup"><span data-stu-id="b054b-108">The user configuration object will be moved to the dumpster.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b054b-109">Comentários</span><span class="sxs-lookup"><span data-stu-id="b054b-109">Remarks</span></span>

<span data-ttu-id="b054b-110">Alterações nos itens de calendário podem resultar na geração de vários eventos.</span><span class="sxs-lookup"><span data-stu-id="b054b-110">Changes to Calendar items may result in the generation of multiple events.</span></span> <span data-ttu-id="b054b-111">Esses eventos são o resultado de itens temporários que está sendo criada na caixa de correio, itens de armazenamento de dados de livre/ocupado sendo alteradas como parte das operações normais do calendário, ou ambos.</span><span class="sxs-lookup"><span data-stu-id="b054b-111">These events are the result of temporary items being created in the mailbox, free/busy data storage items being changed as part of the normal Calendar operations, or both.</span></span> <span data-ttu-id="b054b-112">Classe de eventos para o item "IPM. SchedulePlus.FreeBusy.BinaryData"devem ser ignorados pelo clientes de serviço Web.</span><span class="sxs-lookup"><span data-stu-id="b054b-112">Events for item class "IPM.SchedulePlus.FreeBusy.BinaryData" should be ignored by Web service clients.</span></span> <span data-ttu-id="b054b-113">Esses itens temporários são excluídos depois que eles são criados; Portanto, se for feita uma tentativa para recuperar esses itens, um erro será retornado que afirma que o item não foi encontrado.</span><span class="sxs-lookup"><span data-stu-id="b054b-113">These temporary items are deleted after they are created; therefore, if an attempt is made to retrieve these items, an error will be returned that states that the item was not found.</span></span>
  
## <a name="getevents-request-example"></a><span data-ttu-id="b054b-114">Exemplo de solicitação GetEvents</span><span class="sxs-lookup"><span data-stu-id="b054b-114">GetEvents request example</span></span>

### <a name="description"></a><span data-ttu-id="b054b-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="b054b-115">Description</span></span>

<span data-ttu-id="b054b-116">O exemplo a seguir mostra como solicitar os eventos e os itens que estão associados uma assinatura que é identificada pela marca d'água e do identificador de inscrição.</span><span class="sxs-lookup"><span data-stu-id="b054b-116">The following example shows how to request the events and items that are associated with a subscription that is identified by the subscription identifier and watermark.</span></span>
  
### <a name="code"></a><span data-ttu-id="b054b-117">Código</span><span class="sxs-lookup"><span data-stu-id="b054b-117">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetEvents xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</SubscriptionId>
      <Watermark>AAAAAMAGAAAAAAAAAQ==</Watermark>
    </GetEvents>
  </soap:Body>
</soap:Envelope>
```

### <a name="getevents-request-elements"></a><span data-ttu-id="b054b-118">Elementos de solicitação GetEvents</span><span class="sxs-lookup"><span data-stu-id="b054b-118">GetEvents Request Elements</span></span>

<span data-ttu-id="b054b-119">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="b054b-119">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="b054b-120">GetEvents</span><span class="sxs-lookup"><span data-stu-id="b054b-120">GetEvents</span></span>](getevents.md)
    
- [<span data-ttu-id="b054b-121">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="b054b-121">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="b054b-122">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="b054b-122">Watermark</span></span>](watermark.md)
    
## <a name="successful-getevents-response-example"></a><span data-ttu-id="b054b-123">Exemplo de resposta bem-sucedida GetEvents</span><span class="sxs-lookup"><span data-stu-id="b054b-123">Successful GetEvents response example</span></span>

### <a name="description"></a><span data-ttu-id="b054b-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b054b-124">Description</span></span>

<span data-ttu-id="b054b-125">O exemplo de uma resposta a seguir mostra uma notificação da existência de duas novas mensagens de email desde a última solicitação de notificação foi enviada para o servidor.</span><span class="sxs-lookup"><span data-stu-id="b054b-125">The following example of a response shows a notification of the existence of two new mail messages since the last notification request was sent to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="b054b-126">Código</span><span class="sxs-lookup"><span data-stu-id="b054b-126">Code</span></span>

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
    <GetEventsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="b054b-127">Comments</span><span class="sxs-lookup"><span data-stu-id="b054b-127">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="b054b-128">Os identificadores de item e pasta foram diminuídos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b054b-128">The item and folder identifiers have been shortened to preserve readability.</span></span> 
  
### <a name="getevents-response-elements"></a><span data-ttu-id="b054b-129">Elementos de resposta GetEvents</span><span class="sxs-lookup"><span data-stu-id="b054b-129">GetEvents response elements</span></span>

<span data-ttu-id="b054b-130">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="b054b-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="b054b-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b054b-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="b054b-132">GetEventsResponse</span><span class="sxs-lookup"><span data-stu-id="b054b-132">GetEventsResponse</span></span>](geteventsresponse.md)
    
- [<span data-ttu-id="b054b-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b054b-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b054b-134">GetEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b054b-134">GetEventsResponseMessage</span></span>](geteventsresponsemessage.md)
    
- [<span data-ttu-id="b054b-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b054b-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b054b-136">Notificação</span><span class="sxs-lookup"><span data-stu-id="b054b-136">Notification</span></span>](notification-ex15websvcsotherref.md)
    
- [<span data-ttu-id="b054b-137">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="b054b-137">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="b054b-138">PreviousWatermark</span><span class="sxs-lookup"><span data-stu-id="b054b-138">PreviousWatermark</span></span>](previouswatermark.md)
    
- [<span data-ttu-id="b054b-139">MoreEvents</span><span class="sxs-lookup"><span data-stu-id="b054b-139">MoreEvents</span></span>](moreevents.md)
    
- [<span data-ttu-id="b054b-140">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="b054b-140">NewMailEvent</span></span>](newmailevent.md)
    
- [<span data-ttu-id="b054b-141">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="b054b-141">Watermark</span></span>](watermark.md)
    
- [<span data-ttu-id="b054b-142">Carimbo de hora</span><span class="sxs-lookup"><span data-stu-id="b054b-142">TimeStamp</span></span>](timestamp.md)
    
- [<span data-ttu-id="b054b-143">ItemId</span><span class="sxs-lookup"><span data-stu-id="b054b-143">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="b054b-144">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="b054b-144">ParentFolderId</span></span>](parentfolderid.md)
    
<span data-ttu-id="b054b-145">Para localizar outras opções para a mensagem de resposta da operação **GetEvents** , explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="b054b-145">To find other options for the response message of the **GetEvents** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="b054b-146">Inicie o elemento de [notificação](notification-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="b054b-146">Start at the [Notification](notification-ex15websvcsotherref.md) element.</span></span> 
  
## <a name="getevents-error-response-example"></a><span data-ttu-id="b054b-147">Exemplo de resposta de erro GetEvents</span><span class="sxs-lookup"><span data-stu-id="b054b-147">GetEvents Error response example</span></span>

### <a name="description"></a><span data-ttu-id="b054b-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="b054b-148">Description</span></span>

<span data-ttu-id="b054b-149">O exemplo a seguir mostra uma resposta de erro a uma solicitação de **GetEvents** .</span><span class="sxs-lookup"><span data-stu-id="b054b-149">The following example shows an error response to a **GetEvents** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b054b-150">Código</span><span class="sxs-lookup"><span data-stu-id="b054b-150">Code</span></span>

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
    <GetEventsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="remarks"></a><span data-ttu-id="b054b-151">Comentários</span><span class="sxs-lookup"><span data-stu-id="b054b-151">Remarks</span></span>

<span data-ttu-id="b054b-152">Ao processar uma solicitação de **GetEvents** , o servidor de acesso para cliente executa as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="b054b-152">When processing a **GetEvents** request, the Client Access server performs the following steps:</span></span> 
  
1. <span data-ttu-id="b054b-153">A SubscriptionID da solicitação for confirmada seja uma assinatura válida que está hospedada no servidor de acesso para cliente.</span><span class="sxs-lookup"><span data-stu-id="b054b-153">The SubscriptionID of the request is confirmed to be a valid subscription that is hosted on the Client Access server.</span></span> <span data-ttu-id="b054b-154">Se não for, a chamada **GetEvents** falha.</span><span class="sxs-lookup"><span data-stu-id="b054b-154">If it is not, the **GetEvents** call fails.</span></span> 
    
2. <span data-ttu-id="b054b-155">O endereço SMTP do usuário autenticado para a solicitação é comparado com o endereço SMTP do usuário que criou a assinatura.</span><span class="sxs-lookup"><span data-stu-id="b054b-155">The SMTP address of the authenticated user for the request is compared to the SMTP address of the user who created the subscription.</span></span> <span data-ttu-id="b054b-156">Se eles não coincidirem, a solicitação de **GetEvents** falhará.</span><span class="sxs-lookup"><span data-stu-id="b054b-156">If they do not match, the **GetEvents** request fails.</span></span> 
    
3. <span data-ttu-id="b054b-157">A fila de inscrição é consultada para eventos que estão em espera a serem enviados para o cliente.</span><span class="sxs-lookup"><span data-stu-id="b054b-157">The subscription queue is queried for events that are waiting to be sent to the client.</span></span> <span data-ttu-id="b054b-158">Se a fila não está vazia, os 50 primeiros eventos da fila são retirados da fila e codificados em uma notificação.</span><span class="sxs-lookup"><span data-stu-id="b054b-158">If the queue is not empty, the first 50 events from the queue are pulled from the queue and encoded into a notification.</span></span>
    
4. <span data-ttu-id="b054b-159">Se nenhum evento forem encontrado na fila, um StatusEvent será gerado e codificado em uma resposta de notificação.</span><span class="sxs-lookup"><span data-stu-id="b054b-159">If no events are found in the queue, a StatusEvent is generated and encoded into a notification response.</span></span>
    
5. <span data-ttu-id="b054b-160">A resposta de notificação é retornada para o cliente.</span><span class="sxs-lookup"><span data-stu-id="b054b-160">The notification response is returned to the client.</span></span>
    
6. <span data-ttu-id="b054b-161">Os eventos que estão incluídos na notificação são removidos da fila de inscrição e a acesso para cliente local última marca d'água server para a assinatura é definida como a marca d'água do último evento que é retornado.</span><span class="sxs-lookup"><span data-stu-id="b054b-161">The events that are included in the notification are removed from the subscription queue and the Client Access server local last watermark for the subscription is set to the watermark of the last event that is returned.</span></span>
    
7. <span data-ttu-id="b054b-162">O timer de tempo limite para a assinatura é redefinido.</span><span class="sxs-lookup"><span data-stu-id="b054b-162">The timeout timer for the subscription is reset.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="b054b-163">Confira também</span><span class="sxs-lookup"><span data-stu-id="b054b-163">See also</span></span>



[<span data-ttu-id="b054b-164">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="b054b-164">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="b054b-165">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="b054b-165">Unsubscribe operation</span></span>](unsubscribe-operation.md)


[<span data-ttu-id="b054b-166">Usando inscrições de recepção</span><span class="sxs-lookup"><span data-stu-id="b054b-166">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)

