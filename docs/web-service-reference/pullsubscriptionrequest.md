---
title: PullSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PullSubscriptionRequest
api_type:
- schema
ms.assetid: 145c5cc7-a894-4f0b-a6ea-358cddfb5c33
description: O elemento PullSubscriptionRequest representa uma assinatura para uma assinatura de notificação de eventos baseada em pull.
ms.openlocfilehash: fb9712c9e1481678c2821ee344052783d5c25bf9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468863"
---
# <a name="pullsubscriptionrequest"></a><span data-ttu-id="d493f-103">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="d493f-103">PullSubscriptionRequest</span></span>

<span data-ttu-id="d493f-104">O elemento **PullSubscriptionRequest** representa uma assinatura para uma assinatura de notificação de eventos baseada em pull.</span><span class="sxs-lookup"><span data-stu-id="d493f-104">The **PullSubscriptionRequest** element represents a subscription to a pull-based event notification subscription.</span></span> 
  
[<span data-ttu-id="d493f-105">Assinar</span><span class="sxs-lookup"><span data-stu-id="d493f-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="d493f-106">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="d493f-106">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md)
  
```XML
<PullSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <Timeout/>
</PullSubscriptionRequest>
```

 <span data-ttu-id="d493f-107">**PullSubscriptionRequestType**</span><span class="sxs-lookup"><span data-stu-id="d493f-107">**PullSubscriptionRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d493f-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d493f-108">Attributes and elements</span></span>

<span data-ttu-id="d493f-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d493f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d493f-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="d493f-110">Attributes</span></span>

|<span data-ttu-id="d493f-111">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="d493f-111">**Attribute**</span></span>|<span data-ttu-id="d493f-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d493f-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d493f-113">**SubscribeToAllFolders**</span><span class="sxs-lookup"><span data-stu-id="d493f-113">**SubscribeToAllFolders**</span></span> <br/> |<span data-ttu-id="d493f-114">Indica se é para se inscrever em todas as pastas disponíveis.</span><span class="sxs-lookup"><span data-stu-id="d493f-114">Indicates whether to subscribe to all available folders.</span></span> <span data-ttu-id="d493f-115">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="d493f-115">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d493f-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d493f-116">Child elements</span></span>

|<span data-ttu-id="d493f-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d493f-117">**Element**</span></span>|<span data-ttu-id="d493f-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d493f-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d493f-119">FolderIds</span><span class="sxs-lookup"><span data-stu-id="d493f-119">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="d493f-120">Contém uma matriz de identificadores de pasta que são usados para identificar as pastas a serem monitoradas para notificações de eventos.</span><span class="sxs-lookup"><span data-stu-id="d493f-120">Contains an array of folder identifiers that are used to identify folders to monitor for event notifications.</span></span>  <br/> |
|[<span data-ttu-id="d493f-121">EventType</span><span class="sxs-lookup"><span data-stu-id="d493f-121">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="d493f-122">Contém uma coleção de notificações de eventos que são usadas para criar uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="d493f-122">Contains a collection of event notifications that are used to create a subscription.</span></span>  <br/> |
|[<span data-ttu-id="d493f-123">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="d493f-123">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="d493f-124">Representa um indicador de evento na tabela de eventos de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d493f-124">Represents an event bookmark in the mailbox events table.</span></span> <span data-ttu-id="d493f-125">Isso é usado para criar uma assinatura que começa em um evento que é representado pela marca d' água.</span><span class="sxs-lookup"><span data-stu-id="d493f-125">This is used to create a subscription that starts at an event that is represented by the watermark.</span></span> <span data-ttu-id="d493f-126">Se a marca d' água de uma solicitação de assinatura não for encontrada, uma resposta de erro será retornada ao cliente.</span><span class="sxs-lookup"><span data-stu-id="d493f-126">If the watermark from a Subscribe request is not found, an error response will be returned to the client.</span></span> <span data-ttu-id="d493f-127">Esse erro pode ocorrer se a marca d' água for mais antiga que 30 dias ou se a marca d' água nunca estiver presente na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d493f-127">This error may occur if the watermark is older than 30 days or if the watermark was never present in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d493f-128">Timeout</span><span class="sxs-lookup"><span data-stu-id="d493f-128">Timeout</span></span>](timeout.md) <br/> |<span data-ttu-id="d493f-129">Representa a duração, em minutos, que a assinatura pode permanecer ociosa sem uma solicitação de GetEvents do cliente.</span><span class="sxs-lookup"><span data-stu-id="d493f-129">Represents the duration, in minutes, that the subscription can remain idle without a GetEvents request from the client.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d493f-130">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d493f-130">Parent elements</span></span>

|<span data-ttu-id="d493f-131">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d493f-131">**Element**</span></span>|<span data-ttu-id="d493f-132">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d493f-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d493f-133">Assinar</span><span class="sxs-lookup"><span data-stu-id="d493f-133">Subscribe</span></span>](subscribe.md) <br/> |<span data-ttu-id="d493f-134">Contém as propriedades que são usadas para criar assinaturas.</span><span class="sxs-lookup"><span data-stu-id="d493f-134">Contains the properties that are used to create subscriptions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d493f-135">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="d493f-135">Text value</span></span>

<span data-ttu-id="d493f-136">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d493f-136">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d493f-137">Comentários</span><span class="sxs-lookup"><span data-stu-id="d493f-137">Remarks</span></span>

<span data-ttu-id="d493f-138">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d493f-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d493f-139">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d493f-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d493f-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="d493f-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d493f-141">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d493f-141">Schema name</span></span>  <br/> |<span data-ttu-id="d493f-142">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="d493f-142">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d493f-143">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d493f-143">Validation file</span></span>  <br/> |<span data-ttu-id="d493f-144">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d493f-144">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d493f-145">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d493f-145">Can be empty</span></span>  <br/> |<span data-ttu-id="d493f-146">False</span><span class="sxs-lookup"><span data-stu-id="d493f-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d493f-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="d493f-147">See also</span></span>



[<span data-ttu-id="d493f-148">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="d493f-148">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
[<span data-ttu-id="d493f-149">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="d493f-149">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="d493f-150">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="d493f-150">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="d493f-151">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="d493f-151">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="d493f-152">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d493f-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

