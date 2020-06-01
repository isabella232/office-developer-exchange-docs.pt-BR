---
title: PushSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PushSubscriptionRequest
api_type:
- schema
ms.assetid: 70caa0ca-40a1-421f-b4e6-0658f22d0b8e
description: O elemento PushSubscriptionRequest representa uma assinatura para uma assinatura de notificação de eventos baseada em push.
ms.openlocfilehash: dcdb767ed175468aa4ec940f3147c164e4707e40
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465510"
---
# <a name="pushsubscriptionrequest"></a><span data-ttu-id="90e07-103">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="90e07-103">PushSubscriptionRequest</span></span>

<span data-ttu-id="90e07-104">O elemento **PushSubscriptionRequest** representa uma assinatura para uma assinatura de notificação de eventos baseada em push.</span><span class="sxs-lookup"><span data-stu-id="90e07-104">The **PushSubscriptionRequest** element represents a subscription to a push-based event notification subscription.</span></span> 
  
[<span data-ttu-id="90e07-105">Assinar</span><span class="sxs-lookup"><span data-stu-id="90e07-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="90e07-106">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="90e07-106">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
```XML
<PushSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <StatusFrequency/>
   <URL/>
</PushSubscriptionRequest>
```

 <span data-ttu-id="90e07-107">**PushSubscriptionRequestType**</span><span class="sxs-lookup"><span data-stu-id="90e07-107">**PushSubscriptionRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="90e07-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="90e07-108">Attributes and elements</span></span>

<span data-ttu-id="90e07-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="90e07-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="90e07-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="90e07-110">Attributes</span></span>

|<span data-ttu-id="90e07-111">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="90e07-111">**Attribute**</span></span>|<span data-ttu-id="90e07-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="90e07-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="90e07-113">**SubscribeToAllFolders**</span><span class="sxs-lookup"><span data-stu-id="90e07-113">**SubscribeToAllFolders**</span></span> <br/> |<span data-ttu-id="90e07-114">Indica se é para se inscrever em todas as pastas disponíveis.</span><span class="sxs-lookup"><span data-stu-id="90e07-114">Indicates whether to subscribe to all available folders.</span></span> <span data-ttu-id="90e07-115">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="90e07-115">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="90e07-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="90e07-116">Child elements</span></span>

|<span data-ttu-id="90e07-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="90e07-117">**Element**</span></span>|<span data-ttu-id="90e07-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="90e07-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90e07-119">FolderIds</span><span class="sxs-lookup"><span data-stu-id="90e07-119">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="90e07-120">Contém uma matriz de identificadores de pasta que são usados para identificar as pastas a serem monitoradas para notificações de eventos.</span><span class="sxs-lookup"><span data-stu-id="90e07-120">Contains an array of folder identifiers that are used to identify folders to monitor for event notifications.</span></span>  <br/> |
|[<span data-ttu-id="90e07-121">EventType</span><span class="sxs-lookup"><span data-stu-id="90e07-121">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="90e07-122">Contém uma coleção de notificações de eventos que são usadas para criar uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="90e07-122">Contains a collection of event notifications that are used to create a subscription.</span></span>  <br/> |
|[<span data-ttu-id="90e07-123">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="90e07-123">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="90e07-124">Representa um indicador de evento na tabela de eventos de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="90e07-124">Represents an event bookmark in the mailbox events table.</span></span> <span data-ttu-id="90e07-125">Isso é usado para criar uma assinatura começando em um evento representado pela marca d' água.</span><span class="sxs-lookup"><span data-stu-id="90e07-125">This is used to create a subscription starting at an event represented by the watermark.</span></span> <span data-ttu-id="90e07-126">Se a marca d' água de uma solicitação de assinatura não for encontrada, uma resposta de erro será retornada ao cliente.</span><span class="sxs-lookup"><span data-stu-id="90e07-126">If the watermark from a Subscribe request is not found, an error response will be returned to the client.</span></span> <span data-ttu-id="90e07-127">Isso pode ocorrer se a marca d' água for mais antiga que 30 dias ou se a marca d' água nunca estiver presente na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="90e07-127">This may occur if the watermark is older than 30 days or if the watermark was never present in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="90e07-128">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="90e07-128">StatusFrequency</span></span>](statusfrequency.md) <br/> |<span data-ttu-id="90e07-129">Representa a frequência, especificada em minutos, em que as mensagens de notificação serão enviadas ao cliente quando nenhum evento tiver ocorrido.</span><span class="sxs-lookup"><span data-stu-id="90e07-129">Represents the frequency, specified in minutes, at which notification messages will be sent to the client when no events have occurred.</span></span>  <br/> |
|[<span data-ttu-id="90e07-130">Endereço</span><span class="sxs-lookup"><span data-stu-id="90e07-130">Url </span></span>](url-ex15websvcsotherref.md) <br/> |<span data-ttu-id="90e07-131">Representa o local do serviço Web cliente para notificações por push.</span><span class="sxs-lookup"><span data-stu-id="90e07-131">Represents the location of the client Web service for push notifications.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="90e07-132">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="90e07-132">Parent elements</span></span>

|<span data-ttu-id="90e07-133">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="90e07-133">**Element**</span></span>|<span data-ttu-id="90e07-134">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="90e07-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90e07-135">Assinar</span><span class="sxs-lookup"><span data-stu-id="90e07-135">Subscribe</span></span>](subscribe.md) <br/> |<span data-ttu-id="90e07-136">Contém as propriedades usadas para criar assinaturas.</span><span class="sxs-lookup"><span data-stu-id="90e07-136">Contains the properties used to create subscriptions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="90e07-137">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="90e07-137">Text value</span></span>

<span data-ttu-id="90e07-138">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="90e07-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="90e07-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="90e07-139">Remarks</span></span>

<span data-ttu-id="90e07-140">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="90e07-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="90e07-141">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="90e07-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="90e07-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="90e07-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="90e07-143">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="90e07-143">Schema name</span></span>  <br/> |<span data-ttu-id="90e07-144">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="90e07-144">Messages schema</span></span>  <br/> |
|<span data-ttu-id="90e07-145">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="90e07-145">Validation file</span></span>  <br/> |<span data-ttu-id="90e07-146">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="90e07-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="90e07-147">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="90e07-147">Can be empty</span></span>  <br/> |<span data-ttu-id="90e07-148">False</span><span class="sxs-lookup"><span data-stu-id="90e07-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="90e07-149">Confira também</span><span class="sxs-lookup"><span data-stu-id="90e07-149">See also</span></span>



[<span data-ttu-id="90e07-150">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="90e07-150">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="90e07-151">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="90e07-151">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="90e07-152">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="90e07-152">Unsubscribe operation</span></span>](unsubscribe-operation.md)

