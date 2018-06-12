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
description: O elemento PushSubscriptionRequest representa uma assinatura para uma inscrição de notificação de push com base no evento.
ms.openlocfilehash: 34717d37b8e5bb50c927e57088299fbcb18a2514
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824929"
---
# <a name="pushsubscriptionrequest"></a><span data-ttu-id="02251-103">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="02251-103">PushSubscriptionRequest</span></span>

<span data-ttu-id="02251-104">O elemento **PushSubscriptionRequest** representa uma assinatura para uma inscrição de notificação de push com base no evento.</span><span class="sxs-lookup"><span data-stu-id="02251-104">The **PushSubscriptionRequest** element represents a subscription to a push-based event notification subscription.</span></span> 
  
[<span data-ttu-id="02251-105">Inscrever-se</span><span class="sxs-lookup"><span data-stu-id="02251-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="02251-106">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="02251-106">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
```XML
<PushSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <StatusFrequency/>
   <URL/>
</PushSubscriptionRequest>
```

 <span data-ttu-id="02251-107">**PushSubscriptionRequestType**</span><span class="sxs-lookup"><span data-stu-id="02251-107">**PushSubscriptionRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="02251-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="02251-108">Attributes and elements</span></span>

<span data-ttu-id="02251-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="02251-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="02251-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="02251-110">Attributes</span></span>

|<span data-ttu-id="02251-111">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="02251-111">**Attribute**</span></span>|<span data-ttu-id="02251-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="02251-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="02251-113">**SubscribeToAllFolders**</span><span class="sxs-lookup"><span data-stu-id="02251-113">**SubscribeToAllFolders**</span></span> <br/> |<span data-ttu-id="02251-114">Indica se deve se inscrever para todas as pastas disponíveis.</span><span class="sxs-lookup"><span data-stu-id="02251-114">Indicates whether to subscribe to all available folders.</span></span> <span data-ttu-id="02251-115">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="02251-115">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="02251-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="02251-116">Child elements</span></span>

|<span data-ttu-id="02251-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="02251-117">**Element**</span></span>|<span data-ttu-id="02251-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="02251-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02251-119">FolderIds</span><span class="sxs-lookup"><span data-stu-id="02251-119">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="02251-120">Contém uma matriz de identificadores de pasta que são usados para identificar pastas para monitorar as notificações de eventos.</span><span class="sxs-lookup"><span data-stu-id="02251-120">Contains an array of folder identifiers that are used to identify folders to monitor for event notifications.</span></span>  <br/> |
|[<span data-ttu-id="02251-121">EventTypes</span><span class="sxs-lookup"><span data-stu-id="02251-121">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="02251-122">Contém uma coleção de notificações de eventos que são usados para criar uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="02251-122">Contains a collection of event notifications that are used to create a subscription.</span></span>  <br/> |
|[<span data-ttu-id="02251-123">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="02251-123">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="02251-124">Representa um indicador de evento na tabela de eventos de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="02251-124">Represents an event bookmark in the mailbox events table.</span></span> <span data-ttu-id="02251-125">Isso é usado para criar uma assinatura começando um evento representado por marca d'água.</span><span class="sxs-lookup"><span data-stu-id="02251-125">This is used to create a subscription starting at an event represented by the watermark.</span></span> <span data-ttu-id="02251-126">Se a marca d'água de uma solicitação Subscribe não for encontrada, uma resposta de erro será retornada ao cliente.</span><span class="sxs-lookup"><span data-stu-id="02251-126">If the watermark from a Subscribe request is not found, an error response will be returned to the client.</span></span> <span data-ttu-id="02251-127">Isso poderá ocorrer se a marca d'água tem mais de 30 dias ou se a marca d'água nunca estava presente na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="02251-127">This may occur if the watermark is older than 30 days or if the watermark was never present in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="02251-128">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="02251-128">StatusFrequency</span></span>](statusfrequency.md) <br/> |<span data-ttu-id="02251-129">Representa a frequência, especificada em minutos, na qual notificação mensagens serão enviadas para o cliente quando nenhum evento ocorreu.</span><span class="sxs-lookup"><span data-stu-id="02251-129">Represents the frequency, specified in minutes, at which notification messages will be sent to the client when no events have occurred.</span></span>  <br/> |
|[<span data-ttu-id="02251-130">URL</span><span class="sxs-lookup"><span data-stu-id="02251-130">Url </span></span>](url-ex15websvcsotherref.md) <br/> |<span data-ttu-id="02251-131">Representa o local do cliente do serviço Web para notificações de push.</span><span class="sxs-lookup"><span data-stu-id="02251-131">Represents the location of the client Web service for push notifications.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="02251-132">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="02251-132">Parent elements</span></span>

|<span data-ttu-id="02251-133">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="02251-133">**Element**</span></span>|<span data-ttu-id="02251-134">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="02251-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02251-135">Inscrever-se</span><span class="sxs-lookup"><span data-stu-id="02251-135">Subscribe</span></span>](subscribe.md) <br/> |<span data-ttu-id="02251-136">Contém as propriedades usadas para criar inscrições.</span><span class="sxs-lookup"><span data-stu-id="02251-136">Contains the properties used to create subscriptions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="02251-137">Text value</span><span class="sxs-lookup"><span data-stu-id="02251-137">Text value</span></span>

<span data-ttu-id="02251-138">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="02251-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="02251-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="02251-139">Remarks</span></span>

<span data-ttu-id="02251-140">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="02251-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="02251-141">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="02251-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="02251-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="02251-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="02251-143">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="02251-143">Schema name</span></span>  <br/> |<span data-ttu-id="02251-144">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="02251-144">Messages schema</span></span>  <br/> |
|<span data-ttu-id="02251-145">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="02251-145">Validation file</span></span>  <br/> |<span data-ttu-id="02251-146">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="02251-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="02251-147">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="02251-147">Can be empty</span></span>  <br/> |<span data-ttu-id="02251-148">False</span><span class="sxs-lookup"><span data-stu-id="02251-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="02251-149">Ver também</span><span class="sxs-lookup"><span data-stu-id="02251-149">See also</span></span>



[<span data-ttu-id="02251-150">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="02251-150">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="02251-151">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="02251-151">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="02251-152">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="02251-152">Unsubscribe operation</span></span>](unsubscribe-operation.md)

