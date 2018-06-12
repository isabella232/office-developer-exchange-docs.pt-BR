---
title: Marca d'água
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Watermark
api_type:
- schema
ms.assetid: e1545046-94f9-4ac7-af1c-ea81dfb6822c
description: O elemento de marca d'água representa um indicador de evento na fila de eventos de caixa de correio.
ms.openlocfilehash: 1867aa781bc24f5eb3bdb4648fa494a2a7ea396a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838047"
---
# <a name="watermark"></a><span data-ttu-id="7e8ee-103">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="7e8ee-103">Watermark</span></span>

<span data-ttu-id="7e8ee-104">O elemento de **marca d'água** representa um indicador de evento na fila de eventos de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7e8ee-104">The **Watermark** element represents an event bookmark in the mailbox event queue.</span></span> 
  
```xml
<Watermark/>
```

 <span data-ttu-id="7e8ee-105">**WatermarkType**</span><span class="sxs-lookup"><span data-stu-id="7e8ee-105">**WatermarkType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e8ee-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7e8ee-106">Attributes and elements</span></span>

<span data-ttu-id="7e8ee-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7e8ee-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e8ee-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7e8ee-108">Attributes</span></span>

<span data-ttu-id="7e8ee-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7e8ee-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e8ee-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7e8ee-110">Child elements</span></span>

<span data-ttu-id="7e8ee-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7e8ee-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7e8ee-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7e8ee-112">Parent elements</span></span>

|<span data-ttu-id="7e8ee-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7e8ee-113">**Element**</span></span>|<span data-ttu-id="7e8ee-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7e8ee-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e8ee-115">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="7e8ee-115">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="7e8ee-116">Representa uma assinatura para uma inscrição de notificação de evento baseado em extração.</span><span class="sxs-lookup"><span data-stu-id="7e8ee-116">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="7e8ee-117">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="7e8ee-117">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="7e8ee-118">Representa uma assinatura para uma inscrição de notificação de push com base no evento.</span><span class="sxs-lookup"><span data-stu-id="7e8ee-118">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="7e8ee-119">GetEvents</span><span class="sxs-lookup"><span data-stu-id="7e8ee-119">GetEvents</span></span>](getevents.md) <br/> |<span data-ttu-id="7e8ee-120">Representa a operação usada pelos clientes de recepção para notificações de solicitação do servidor.</span><span class="sxs-lookup"><span data-stu-id="7e8ee-120">Represents the operation used by pull clients to request notifications from the server.</span></span>  <br/> |
|[<span data-ttu-id="7e8ee-121">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="7e8ee-121">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="7e8ee-122">Representa um evento onde uma pasta ou um item é copiada.</span><span class="sxs-lookup"><span data-stu-id="7e8ee-122">Represents an event where an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="7e8ee-123">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="7e8ee-123">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="7e8ee-124">Representa um evento onde uma pasta ou um item é criada.</span><span class="sxs-lookup"><span data-stu-id="7e8ee-124">Represents an event where an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="7e8ee-125">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="7e8ee-125">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="7e8ee-126">Representa um evento onde uma pasta ou um item é excluída.</span><span class="sxs-lookup"><span data-stu-id="7e8ee-126">Represents an event where an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="7e8ee-127">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="7e8ee-127">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="7e8ee-128">Representa um evento onde um item ou pasta é modificada.</span><span class="sxs-lookup"><span data-stu-id="7e8ee-128">Represents an event where an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="7e8ee-129">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="7e8ee-129">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="7e8ee-130">Representa um evento onde uma pasta ou um item é movida da pasta pai de um para outra pasta pai.</span><span class="sxs-lookup"><span data-stu-id="7e8ee-130">Represents an event where an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="7e8ee-131">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="7e8ee-131">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="7e8ee-132">Representa um evento disparado por um novo item de email em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7e8ee-132">Represents an event triggered by a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="7e8ee-133">StatusEvent</span><span class="sxs-lookup"><span data-stu-id="7e8ee-133">StatusEvent</span></span>](statusevent.md) <br/> |<span data-ttu-id="7e8ee-134">Representa uma notificação que nenhuma nova atividade ocorreu na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7e8ee-134">Represents a notification that no new activity has occurred in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="7e8ee-135">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7e8ee-135">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md) <br/> |<span data-ttu-id="7e8ee-136">Contém o status e o resultado de uma solicitação Subscribe.</span><span class="sxs-lookup"><span data-stu-id="7e8ee-136">Contains the status and result of a Subscribe request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7e8ee-137">Text value</span><span class="sxs-lookup"><span data-stu-id="7e8ee-137">Text value</span></span>

<span data-ttu-id="7e8ee-138">Um valor de texto pode ser obrigatórias ou opcionais, dependendo de como esse elemento é usado.</span><span class="sxs-lookup"><span data-stu-id="7e8ee-138">A text value may be required or optional depending on how this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7e8ee-139">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="7e8ee-139">Remarks</span></span>

<span data-ttu-id="7e8ee-140">Se uma solicitação Subscribe contiver uma marca d'água, a assinatura é criada a partir de encaminhar a marca d'água.</span><span class="sxs-lookup"><span data-stu-id="7e8ee-140">If a Subscribe request contains a watermark, the subscription is created from the watermark forward.</span></span> <span data-ttu-id="7e8ee-141">Se a solicitação Subscribe contiver uma marca d'água que não foi encontrada na tabela de eventos de caixa de correio, uma `ErrorInvalidWatermark` erro será retornado para o aplicativo cliente.</span><span class="sxs-lookup"><span data-stu-id="7e8ee-141">If the Subscribe request contains a watermark that is not found in the mailbox events table, an  `ErrorInvalidWatermark` error is returned to the client application.</span></span> <span data-ttu-id="7e8ee-142">Isso pode ocorrer se a marca d'água é muito antiga e foi removida da janela de 30 dias de tabela eventos ou se a marca d'água não estava nunca presentes na tabela eventos.</span><span class="sxs-lookup"><span data-stu-id="7e8ee-142">This may occur if the watermark is too old and has been removed from the 30 day window of the events table or if the watermark was not ever present in the events table.</span></span> <span data-ttu-id="7e8ee-143">Isso pode acontecer, por exemplo, se uma marca d'água é obtida de uma assinatura diferente para uma caixa de correio em um banco de dados diferente.</span><span class="sxs-lookup"><span data-stu-id="7e8ee-143">This can happen, for example, if a watermark is obtained from a different subscription for a mailbox in a different database.</span></span> 
  
<span data-ttu-id="7e8ee-144">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="7e8ee-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e8ee-145">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7e8ee-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e8ee-146">Namespace</span><span class="sxs-lookup"><span data-stu-id="7e8ee-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7e8ee-147">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7e8ee-147">Schema name</span></span>  <br/> |<span data-ttu-id="7e8ee-148">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7e8ee-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="7e8ee-149">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7e8ee-149">Validation file</span></span>  <br/> |<span data-ttu-id="7e8ee-150">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7e8ee-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7e8ee-151">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="7e8ee-151">Can be empty</span></span>  <br/> |<span data-ttu-id="7e8ee-152">False</span><span class="sxs-lookup"><span data-stu-id="7e8ee-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e8ee-153">Ver também</span><span class="sxs-lookup"><span data-stu-id="7e8ee-153">See also</span></span>



[<span data-ttu-id="7e8ee-154">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="7e8ee-154">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="7e8ee-155">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="7e8ee-155">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="7e8ee-156">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="7e8ee-156">Unsubscribe operation</span></span>](unsubscribe-operation.md)

