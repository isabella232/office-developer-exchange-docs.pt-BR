---
title: StatusFrequency
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StatusFrequency
api_type:
- schema
ms.assetid: 917474e2-a426-4166-b825-53783a41dad4
description: O elemento StatusFrequency representa o valor de tempo limite máximo, em minutos, em que as tentativas são tentadas pelo servidor.
ms.openlocfilehash: db14ecfd54584188b3da16bb369db6c8089c70f4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468240"
---
# <a name="statusfrequency"></a><span data-ttu-id="c2007-103">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="c2007-103">StatusFrequency</span></span>

<span data-ttu-id="c2007-104">O elemento **StatusFrequency** representa o valor de tempo limite máximo, em minutos, em que as tentativas são tentadas pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="c2007-104">The **StatusFrequency** element represents the maximum timeout value, in minutes, in which retries are attempted by the server.</span></span> 
  
[<span data-ttu-id="c2007-105">Assinar</span><span class="sxs-lookup"><span data-stu-id="c2007-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="c2007-106">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="c2007-106">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
[<span data-ttu-id="c2007-107">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="c2007-107">StatusFrequency</span></span>](statusfrequency.md)
  
```XML
<StatusFrequency/>
```

 <span data-ttu-id="c2007-108">**SubscriptionStatusFrequencyType**</span><span class="sxs-lookup"><span data-stu-id="c2007-108">**SubscriptionStatusFrequencyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c2007-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c2007-109">Attributes and elements</span></span>

<span data-ttu-id="c2007-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c2007-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2007-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="c2007-111">Attributes</span></span>

<span data-ttu-id="c2007-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c2007-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c2007-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c2007-113">Child elements</span></span>

<span data-ttu-id="c2007-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c2007-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c2007-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c2007-115">Parent elements</span></span>

|<span data-ttu-id="c2007-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c2007-116">**Element**</span></span>|<span data-ttu-id="c2007-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c2007-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2007-118">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="c2007-118">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="c2007-119">Representa uma assinatura para uma assinatura de notificação de eventos baseada em push.</span><span class="sxs-lookup"><span data-stu-id="c2007-119">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c2007-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c2007-120">Text value</span></span>

<span data-ttu-id="c2007-121">Um valor de texto que representa um inteiro será necessário se esse elemento for usado.</span><span class="sxs-lookup"><span data-stu-id="c2007-121">A text value that represents an integer is required if this element is used.</span></span> <span data-ttu-id="c2007-122">Os valores possíveis para esse elemento são 1 a 1440, inclusive.</span><span class="sxs-lookup"><span data-stu-id="c2007-122">The possible values for this element are 1 to 1440, inclusive.</span></span> <span data-ttu-id="c2007-123">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="c2007-123">This element is optional.</span></span> <span data-ttu-id="c2007-124">O valor-padrão é 30 minutos.</span><span class="sxs-lookup"><span data-stu-id="c2007-124">The default value is 30 minutes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c2007-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="c2007-125">Remarks</span></span>

<span data-ttu-id="c2007-126">O valor **StatusFrequency** é usado pelo servidor para repetir uma notificação por push quando não recebe uma resposta para uma notificação por Push ou o status ping do cliente.</span><span class="sxs-lookup"><span data-stu-id="c2007-126">The **StatusFrequency** value is used by the server to retry a push notification when it does not receive a response to a push notification or status ping from the client.</span></span> <span data-ttu-id="c2007-127">Se o servidor não receber uma resposta, ele tentará enviar a notificação várias vezes antes de parar de enviar a notificação.</span><span class="sxs-lookup"><span data-stu-id="c2007-127">If the server does not receive a response, it retries sending the notification several times before it stops sending the notification.</span></span> <span data-ttu-id="c2007-128">No EWS, o intervalo de repetição padrão é de 30 segundos e as novas tentativas subsequentes sempre têm o dobro da hora do último intervalo de repetição.</span><span class="sxs-lookup"><span data-stu-id="c2007-128">In EWS, the default retry interval is 30 seconds and subsequent retries are always double the time of the last retry interval.</span></span> <span data-ttu-id="c2007-129">Horários de tentativas não são exatos, já que podem ser atrasados devido a outras cargas no servidor.</span><span class="sxs-lookup"><span data-stu-id="c2007-129">Retry times are not exact as they can be delayed due to other loads on the server.</span></span> <span data-ttu-id="c2007-130">A tabela a seguir mostra como os intervalos de repetição ocorrem nos 30 minutos alocados pelo valor padrão do **StatusFrequency** (supondo que o servidor não encontrou atrasos).</span><span class="sxs-lookup"><span data-stu-id="c2007-130">The following table shows how the retry intervals occur in the 30 minutes allotted by the default **StatusFrequency** value (assuming the server did not encounter any delays).</span></span> 
  
|<span data-ttu-id="c2007-131">repetir</span><span class="sxs-lookup"><span data-stu-id="c2007-131">**Retry**</span></span>|<span data-ttu-id="c2007-132">**Segundos**</span><span class="sxs-lookup"><span data-stu-id="c2007-132">**Seconds**</span></span>|<span data-ttu-id="c2007-133">**Time**</span><span class="sxs-lookup"><span data-stu-id="c2007-133">**Time**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c2007-134">,0</span><span class="sxs-lookup"><span data-stu-id="c2007-134">0</span></span>  <br/> |<span data-ttu-id="c2007-135">,0</span><span class="sxs-lookup"><span data-stu-id="c2007-135">0</span></span>  <br/> |<span data-ttu-id="c2007-136">Sincronização inicial</span><span class="sxs-lookup"><span data-stu-id="c2007-136">Initial sync</span></span>  <br/> |
|<span data-ttu-id="c2007-137">1 </span><span class="sxs-lookup"><span data-stu-id="c2007-137">1</span></span>  <br/> |<span data-ttu-id="c2007-138">até</span><span class="sxs-lookup"><span data-stu-id="c2007-138">30</span></span>  <br/> |<span data-ttu-id="c2007-139">00:30</span><span class="sxs-lookup"><span data-stu-id="c2007-139">00:30</span></span>  <br/> |
|<span data-ttu-id="c2007-140">duas</span><span class="sxs-lookup"><span data-stu-id="c2007-140">2</span></span>  <br/> |<span data-ttu-id="c2007-141">60</span><span class="sxs-lookup"><span data-stu-id="c2007-141">60</span></span>  <br/> |<span data-ttu-id="c2007-142">01:00</span><span class="sxs-lookup"><span data-stu-id="c2007-142">01:00</span></span>  <br/> |
|<span data-ttu-id="c2007-143">3D</span><span class="sxs-lookup"><span data-stu-id="c2007-143">3</span></span>  <br/> |<span data-ttu-id="c2007-144">120</span><span class="sxs-lookup"><span data-stu-id="c2007-144">120</span></span>  <br/> |<span data-ttu-id="c2007-145">02:00</span><span class="sxs-lookup"><span data-stu-id="c2007-145">02:00</span></span>  <br/> |
|<span data-ttu-id="c2007-146">4 </span><span class="sxs-lookup"><span data-stu-id="c2007-146">4</span></span>  <br/> |<span data-ttu-id="c2007-147">240</span><span class="sxs-lookup"><span data-stu-id="c2007-147">240</span></span>  <br/> |<span data-ttu-id="c2007-148">04:00</span><span class="sxs-lookup"><span data-stu-id="c2007-148">04:00</span></span>  <br/> |
|<span data-ttu-id="c2007-149">5 </span><span class="sxs-lookup"><span data-stu-id="c2007-149">5</span></span>  <br/> |<span data-ttu-id="c2007-150">480</span><span class="sxs-lookup"><span data-stu-id="c2007-150">480</span></span>  <br/> |<span data-ttu-id="c2007-151">08:00</span><span class="sxs-lookup"><span data-stu-id="c2007-151">08:00</span></span>  <br/> |
|<span data-ttu-id="c2007-152">6 </span><span class="sxs-lookup"><span data-stu-id="c2007-152">6</span></span>  <br/> |<span data-ttu-id="c2007-153">960</span><span class="sxs-lookup"><span data-stu-id="c2007-153">960</span></span>  <br/> |<span data-ttu-id="c2007-154">16:00</span><span class="sxs-lookup"><span data-stu-id="c2007-154">16:00</span></span>  <br/> |
|<span data-ttu-id="c2007-155">7 </span><span class="sxs-lookup"><span data-stu-id="c2007-155">7</span></span>  <br/> |<span data-ttu-id="c2007-156">1920</span><span class="sxs-lookup"><span data-stu-id="c2007-156">1920</span></span>  <br/> |<span data-ttu-id="c2007-157">32:00- **StatusFrequency** valor padrão de 30 excedido, repetir não enviado</span><span class="sxs-lookup"><span data-stu-id="c2007-157">32:00 - **StatusFrequency** default value of 30 exceeded, retry not sent</span></span>  <br/> |
   
<span data-ttu-id="c2007-158">Se o cliente não receber mensagens de notificação do servidor por um período de tempo que exceder o tempo especificado por **StatusFrequency**, o cliente deverá executar uma ação, como recriar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="c2007-158">If the client does not receive notification messages from the server for a period of time that exceeds twice the time specified by **StatusFrequency**, the client should take an action such as recreating the subscription.</span></span> 
  
<span data-ttu-id="c2007-159">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c2007-159">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2007-160">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c2007-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2007-161">Namespace</span><span class="sxs-lookup"><span data-stu-id="c2007-161">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c2007-162">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c2007-162">Schema name</span></span>  <br/> |<span data-ttu-id="c2007-163">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c2007-163">Types schema</span></span>  <br/> |
|<span data-ttu-id="c2007-164">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c2007-164">Validation file</span></span>  <br/> |<span data-ttu-id="c2007-165">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c2007-165">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c2007-166">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="c2007-166">Can be empty</span></span>  <br/> |<span data-ttu-id="c2007-167">False</span><span class="sxs-lookup"><span data-stu-id="c2007-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c2007-168">Confira também</span><span class="sxs-lookup"><span data-stu-id="c2007-168">See also</span></span>



[<span data-ttu-id="c2007-169">Operação Subscribe</span><span class="sxs-lookup"><span data-stu-id="c2007-169">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="c2007-170">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="c2007-170">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="c2007-171">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="c2007-171">Unsubscribe operation</span></span>](unsubscribe-operation.md)
  
[<span data-ttu-id="c2007-172">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="c2007-172">Watermark</span></span>](watermark.md)

