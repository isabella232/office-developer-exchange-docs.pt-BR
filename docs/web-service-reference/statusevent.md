---
title: StatusEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StatusEvent
api_type:
- schema
ms.assetid: d3901818-2640-4bed-aad8-21a61aee62a1
description: O elemento StatusEvent representa uma notificação de que nenhuma atividade nova ocorreu na caixa de correio.
ms.openlocfilehash: 8158a47937a810be2ea22346384b4e61da56ac48
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468254"
---
# <a name="statusevent"></a><span data-ttu-id="30df9-103">StatusEvent</span><span class="sxs-lookup"><span data-stu-id="30df9-103">StatusEvent</span></span>

<span data-ttu-id="30df9-104">O elemento **StatusEvent** representa uma notificação de que nenhuma atividade nova ocorreu na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="30df9-104">The **StatusEvent** element represents a notification that no new activity has occurred in the mailbox.</span></span> 
  
```xml
<StatusEvent>
   <Watermark/>
</StatusEvent>
```

 <span data-ttu-id="30df9-105">**BaseNotificationEventType**</span><span class="sxs-lookup"><span data-stu-id="30df9-105">**BaseNotificationEventType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="30df9-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="30df9-106">Attributes and elements</span></span>

<span data-ttu-id="30df9-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="30df9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="30df9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="30df9-108">Attributes</span></span>

<span data-ttu-id="30df9-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="30df9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="30df9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="30df9-110">Child elements</span></span>

|<span data-ttu-id="30df9-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="30df9-111">**Element**</span></span>|<span data-ttu-id="30df9-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="30df9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30df9-113">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="30df9-113">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="30df9-114">Representa a última marca d' água válida para uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="30df9-114">Represents the last valid watermark for a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="30df9-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="30df9-115">Parent elements</span></span>

|<span data-ttu-id="30df9-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="30df9-116">**Element**</span></span>|<span data-ttu-id="30df9-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="30df9-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30df9-118">Notificação</span><span class="sxs-lookup"><span data-stu-id="30df9-118">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="30df9-119">Contém informações sobre a assinatura e os eventos que ocorreram desde a última notificação.</span><span class="sxs-lookup"><span data-stu-id="30df9-119">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="30df9-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="30df9-120">Remarks</span></span>

<span data-ttu-id="30df9-121">O elemento **StatusEvent** é retornado em uma notificação por uma das seguintes razões:</span><span class="sxs-lookup"><span data-stu-id="30df9-121">The **StatusEvent** element is returned in a notification for one of the following reasons:</span></span> 
  
- <span data-ttu-id="30df9-122">Um cliente de recepção emite uma solicitação GetEvents em uma assinatura sem atividade.</span><span class="sxs-lookup"><span data-stu-id="30df9-122">A pull client issues a GetEvents request on a subscription that has no activity.</span></span>
    
- <span data-ttu-id="30df9-123">Um cliente de envio não tem eventos na fila quando o [StatusFrequency](statusfrequency.md) foi alcançado.</span><span class="sxs-lookup"><span data-stu-id="30df9-123">A push client has no events in the queue when the [StatusFrequency](statusfrequency.md) has been reached.</span></span> 
    
<span data-ttu-id="30df9-124">A **StatusEvent**[marca d' água](watermark.md) StatusEvent é usada por um aplicativo cliente da mesma maneira que as marcas d' água de outro tipo de evento.</span><span class="sxs-lookup"><span data-stu-id="30df9-124">The **StatusEvent**[Watermark](watermark.md) is used by a client application in the same manner as the other event type watermarks.</span></span> <span data-ttu-id="30df9-125">No entanto, a marca d' água de **StatusEvent** não é a mesma que as marcas d' água usadas para outros eventos.</span><span class="sxs-lookup"><span data-stu-id="30df9-125">However, the watermark for the **StatusEvent** is not the same as the watermarks used for other events.</span></span> <span data-ttu-id="30df9-126">Por exemplo, uma assinatura tem eventos com marcas d' água 1, 2 e 3, e esses eventos foram comunicados com êxito em uma notificação.</span><span class="sxs-lookup"><span data-stu-id="30df9-126">For example, a subscription has events with watermarks 1, 2, and 3 and those events have been successfully communicated in a notification.</span></span> <span data-ttu-id="30df9-127">Um período de inatividade ocorre e uma solicitação **GetEvents** é enviada.</span><span class="sxs-lookup"><span data-stu-id="30df9-127">A period of inactivity occurs and a **GetEvents** request is sent.</span></span> <span data-ttu-id="30df9-128">O servidor de acesso para cliente (CAS) retorna um evento de status e inclui a última marca d' água, 3, como [PreviousWatermark](previouswatermark.md) e a [marca d' água](watermark.md)atual.</span><span class="sxs-lookup"><span data-stu-id="30df9-128">The Client Access server (CAS) returns a status event and includes the last watermark, 3, as both the [PreviousWatermark](previouswatermark.md) and the current [Watermark](watermark.md).</span></span>
  
<span data-ttu-id="30df9-129">A marca d' água não permanecerá a mesma em todos os casos.</span><span class="sxs-lookup"><span data-stu-id="30df9-129">The watermark will not remain the same in all cases.</span></span> <span data-ttu-id="30df9-130">As entradas de evento são mantidas por 30 dias.</span><span class="sxs-lookup"><span data-stu-id="30df9-130">Event entries are maintained for 30 days.</span></span> <span data-ttu-id="30df9-131">Para manter uma assinatura ativa, o CAS atualiza periodicamente as marcas d' água das filas de assinatura.</span><span class="sxs-lookup"><span data-stu-id="30df9-131">To maintain an active subscription, the CAS periodically updates the watermarks for subscription queues.</span></span> <span data-ttu-id="30df9-132">As marcas d' água atualizadas são enviadas aos clientes para manter uma assinatura ativa.</span><span class="sxs-lookup"><span data-stu-id="30df9-132">The updated watermarks are sent to clients to maintain an active subscription.</span></span>
  
<span data-ttu-id="30df9-133">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="30df9-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="30df9-134">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="30df9-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30df9-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="30df9-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="30df9-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="30df9-136">Schema name</span></span>  <br/> |<span data-ttu-id="30df9-137">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="30df9-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="30df9-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="30df9-138">Validation file</span></span>  <br/> |<span data-ttu-id="30df9-139">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="30df9-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="30df9-140">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="30df9-140">Can be empty</span></span>  <br/> |<span data-ttu-id="30df9-141">False</span><span class="sxs-lookup"><span data-stu-id="30df9-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="30df9-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="30df9-142">See also</span></span>



[<span data-ttu-id="30df9-143">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="30df9-143">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="30df9-144">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="30df9-144">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="30df9-145">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="30df9-145">Unsubscribe operation</span></span>](unsubscribe-operation.md)

