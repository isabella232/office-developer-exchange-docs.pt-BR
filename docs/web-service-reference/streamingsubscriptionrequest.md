---
title: StreamingSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StreamingSubscriptionRequest
api_type:
- schema
ms.assetid: d18f3b60-ebb6-4133-b895-a6ec8942d039
description: O elemento StreamingSubscriptionRequest representa uma assinatura para uma inscrição de notificação de evento streaming.
ms.openlocfilehash: 088ec3b8048d70803b4837548ca918c0005d91bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825601"
---
# <a name="streamingsubscriptionrequest"></a><span data-ttu-id="913fa-103">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="913fa-103">StreamingSubscriptionRequest</span></span>

<span data-ttu-id="913fa-104">O elemento **StreamingSubscriptionRequest** representa uma assinatura para uma inscrição de notificação de evento streaming.</span><span class="sxs-lookup"><span data-stu-id="913fa-104">The **StreamingSubscriptionRequest** element represents a subscription to a streaming event notification subscription.</span></span> 
  
[<span data-ttu-id="913fa-105">Inscrever-se</span><span class="sxs-lookup"><span data-stu-id="913fa-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="913fa-106">StreamingSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="913fa-106">StreamingSubscriptionRequest</span></span>](streamingsubscriptionrequest.md)
  
```xml
<StreamingSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
</StreamingSubscriptionRequest>
```

 <span data-ttu-id="913fa-107">**StreamingSubscriptionRequest**</span><span class="sxs-lookup"><span data-stu-id="913fa-107">**StreamingSubscriptionRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="913fa-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="913fa-108">Attributes and elements</span></span>

<span data-ttu-id="913fa-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="913fa-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="913fa-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="913fa-110">Attributes</span></span>

|<span data-ttu-id="913fa-111">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="913fa-111">**Attribute**</span></span>|<span data-ttu-id="913fa-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="913fa-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="913fa-113">**SubscribeToAllFolders**</span><span class="sxs-lookup"><span data-stu-id="913fa-113">**SubscribeToAllFolders**</span></span> <br/> |<span data-ttu-id="913fa-114">Indica se o servidor se inscreverá a todas as pastas na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="913fa-114">Indicates whether the server will subscribe to all folders in the user's mailbox.</span></span> <span data-ttu-id="913fa-115">Um valor **true** indica que o servidor inscreverá.</span><span class="sxs-lookup"><span data-stu-id="913fa-115">A value of **true** indicates that the server will subscribe.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="913fa-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="913fa-116">Child elements</span></span>

|<span data-ttu-id="913fa-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="913fa-117">**Element**</span></span>|<span data-ttu-id="913fa-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="913fa-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="913fa-119">FolderIds</span><span class="sxs-lookup"><span data-stu-id="913fa-119">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="913fa-120">Contém uma matriz de identificadores de pasta que são usados para identificar pastas para monitorar as notificações de eventos.</span><span class="sxs-lookup"><span data-stu-id="913fa-120">Contains an array of folder identifiers that are used to identify folders to monitor for event notifications.</span></span>  <br/> |
|[<span data-ttu-id="913fa-121">EventTypes</span><span class="sxs-lookup"><span data-stu-id="913fa-121">EventTypes</span></span>](eventtypes.md) <br/> |<span data-ttu-id="913fa-122">Contém uma coleção de notificações de eventos que são usados para criar uma assinatura.</span><span class="sxs-lookup"><span data-stu-id="913fa-122">Contains a collection of event notifications that are used to create a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="913fa-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="913fa-123">Parent elements</span></span>

|<span data-ttu-id="913fa-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="913fa-124">**Element**</span></span>|<span data-ttu-id="913fa-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="913fa-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="913fa-126">Inscrever-se</span><span class="sxs-lookup"><span data-stu-id="913fa-126">Subscribe</span></span>](subscribe.md) <br/> |<span data-ttu-id="913fa-127">Contém as propriedades que são usadas para criar assinaturas.</span><span class="sxs-lookup"><span data-stu-id="913fa-127">Contains the properties that are used to create subscriptions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="913fa-128">Text value</span><span class="sxs-lookup"><span data-stu-id="913fa-128">Text value</span></span>

<span data-ttu-id="913fa-129">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="913fa-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="913fa-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="913fa-130">Remarks</span></span>

<span data-ttu-id="913fa-131">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="913fa-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="913fa-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="913fa-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="913fa-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="913fa-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="913fa-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="913fa-134">Schema name</span></span>  <br/> |<span data-ttu-id="913fa-135">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="913fa-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="913fa-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="913fa-136">Validation file</span></span>  <br/> |<span data-ttu-id="913fa-137">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="913fa-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="913fa-138">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="913fa-138">Can be empty</span></span>  <br/> |<span data-ttu-id="913fa-139">False</span><span class="sxs-lookup"><span data-stu-id="913fa-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="913fa-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="913fa-140">See also</span></span>



[<span data-ttu-id="913fa-141">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="913fa-141">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="913fa-142">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="913fa-142">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="913fa-143">Operação GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="913fa-143">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)
  
[<span data-ttu-id="913fa-144">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="913fa-144">Unsubscribe operation</span></span>](unsubscribe-operation.md)

