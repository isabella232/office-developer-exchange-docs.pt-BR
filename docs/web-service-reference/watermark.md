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
description: O elemento Watermark representa um indicador de evento na fila de eventos de caixa de correio.
ms.openlocfilehash: a717196101fea698b0b8c66f92a3d420fda9a421
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459760"
---
# <a name="watermark"></a><span data-ttu-id="0a579-103">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="0a579-103">Watermark</span></span>

<span data-ttu-id="0a579-104">O elemento **Watermark** representa um indicador de evento na fila de eventos de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0a579-104">The **Watermark** element represents an event bookmark in the mailbox event queue.</span></span> 
  
```xml
<Watermark/>
```

 <span data-ttu-id="0a579-105">**Marca d' água**</span><span class="sxs-lookup"><span data-stu-id="0a579-105">**WatermarkType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0a579-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0a579-106">Attributes and elements</span></span>

<span data-ttu-id="0a579-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0a579-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0a579-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0a579-108">Attributes</span></span>

<span data-ttu-id="0a579-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0a579-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0a579-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0a579-110">Child elements</span></span>

<span data-ttu-id="0a579-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0a579-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0a579-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0a579-112">Parent elements</span></span>

|<span data-ttu-id="0a579-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0a579-113">**Element**</span></span>|<span data-ttu-id="0a579-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0a579-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a579-115">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="0a579-115">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="0a579-116">Representa uma assinatura para uma assinatura de notificação de eventos baseada em pull.</span><span class="sxs-lookup"><span data-stu-id="0a579-116">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="0a579-117">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="0a579-117">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="0a579-118">Representa uma assinatura para uma assinatura de notificação de eventos baseada em push.</span><span class="sxs-lookup"><span data-stu-id="0a579-118">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
|[<span data-ttu-id="0a579-119">GetEvents</span><span class="sxs-lookup"><span data-stu-id="0a579-119">GetEvents</span></span>](getevents.md) <br/> |<span data-ttu-id="0a579-120">Representa a operação usada por clientes de recebimento para solicitar notificações do servidor.</span><span class="sxs-lookup"><span data-stu-id="0a579-120">Represents the operation used by pull clients to request notifications from the server.</span></span>  <br/> |
|[<span data-ttu-id="0a579-121">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="0a579-121">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="0a579-122">Representa um evento em que um item ou pasta é copiado.</span><span class="sxs-lookup"><span data-stu-id="0a579-122">Represents an event where an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="0a579-123">CreatedEvent</span><span class="sxs-lookup"><span data-stu-id="0a579-123">CreatedEvent</span></span>](createdevent.md) <br/> |<span data-ttu-id="0a579-124">Representa um evento em que um item ou pasta é criado.</span><span class="sxs-lookup"><span data-stu-id="0a579-124">Represents an event where an item or folder is created.</span></span>  <br/> |
|[<span data-ttu-id="0a579-125">DeletedEvent</span><span class="sxs-lookup"><span data-stu-id="0a579-125">DeletedEvent</span></span>](deletedevent.md) <br/> |<span data-ttu-id="0a579-126">Representa um evento em que um item ou pasta é excluído.</span><span class="sxs-lookup"><span data-stu-id="0a579-126">Represents an event where an item or folder is deleted.</span></span>  <br/> |
|[<span data-ttu-id="0a579-127">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="0a579-127">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="0a579-128">Representa um evento em que um item ou pasta é modificado.</span><span class="sxs-lookup"><span data-stu-id="0a579-128">Represents an event where an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="0a579-129">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="0a579-129">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="0a579-130">Representa um evento em que um item ou pasta é movido de uma pasta pai para outra pasta pai.</span><span class="sxs-lookup"><span data-stu-id="0a579-130">Represents an event where an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
|[<span data-ttu-id="0a579-131">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="0a579-131">NewMailEvent</span></span>](newmailevent.md) <br/> |<span data-ttu-id="0a579-132">Representa um evento disparado por um novo item de email em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0a579-132">Represents an event triggered by a new mail item in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0a579-133">StatusEvent</span><span class="sxs-lookup"><span data-stu-id="0a579-133">StatusEvent</span></span>](statusevent.md) <br/> |<span data-ttu-id="0a579-134">Representa uma notificação de que nenhuma atividade nova ocorreu na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0a579-134">Represents a notification that no new activity has occurred in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0a579-135">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0a579-135">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md) <br/> |<span data-ttu-id="0a579-136">Contém o status e o resultado de uma solicitação de assinatura.</span><span class="sxs-lookup"><span data-stu-id="0a579-136">Contains the status and result of a Subscribe request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0a579-137">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="0a579-137">Text value</span></span>

<span data-ttu-id="0a579-138">Um valor de texto pode ser obrigatório ou opcional, dependendo de como esse elemento é usado.</span><span class="sxs-lookup"><span data-stu-id="0a579-138">A text value may be required or optional depending on how this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0a579-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="0a579-139">Remarks</span></span>

<span data-ttu-id="0a579-140">Se uma solicitação de assinatura contiver uma marca d' água, a assinatura será criada a partir da marca d' água para frente.</span><span class="sxs-lookup"><span data-stu-id="0a579-140">If a Subscribe request contains a watermark, the subscription is created from the watermark forward.</span></span> <span data-ttu-id="0a579-141">Se a solicitação de assinatura contiver uma marca d' água que não seja encontrada na tabela de eventos de caixa de correio, um `ErrorInvalidWatermark` erro será retornado para o aplicativo cliente.</span><span class="sxs-lookup"><span data-stu-id="0a579-141">If the Subscribe request contains a watermark that is not found in the mailbox events table, an  `ErrorInvalidWatermark` error is returned to the client application.</span></span> <span data-ttu-id="0a579-142">Isso pode ocorrer se a marca d' água for muito antiga e tiver sido removida da janela de 30 dias da tabela de eventos ou se a marca d' água ainda não estiver presente na tabela de eventos.</span><span class="sxs-lookup"><span data-stu-id="0a579-142">This may occur if the watermark is too old and has been removed from the 30 day window of the events table or if the watermark was not ever present in the events table.</span></span> <span data-ttu-id="0a579-143">Isso pode acontecer, por exemplo, se uma marca d' água for Obtida de uma assinatura diferente para uma caixa de correio em um banco de dados diferente.</span><span class="sxs-lookup"><span data-stu-id="0a579-143">This can happen, for example, if a watermark is obtained from a different subscription for a mailbox in a different database.</span></span> 
  
<span data-ttu-id="0a579-144">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="0a579-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0a579-145">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0a579-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0a579-146">Namespace</span><span class="sxs-lookup"><span data-stu-id="0a579-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0a579-147">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0a579-147">Schema name</span></span>  <br/> |<span data-ttu-id="0a579-148">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0a579-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="0a579-149">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0a579-149">Validation file</span></span>  <br/> |<span data-ttu-id="0a579-150">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0a579-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0a579-151">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="0a579-151">Can be empty</span></span>  <br/> |<span data-ttu-id="0a579-152">False</span><span class="sxs-lookup"><span data-stu-id="0a579-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0a579-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="0a579-153">See also</span></span>



[<span data-ttu-id="0a579-154">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="0a579-154">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="0a579-155">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="0a579-155">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="0a579-156">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="0a579-156">Unsubscribe operation</span></span>](unsubscribe-operation.md)

