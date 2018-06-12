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
description: O elemento StatusFrequency representa o valor de tempo limite máximo, em minutos, no qual as repetições são tentadas pelo servidor.
ms.openlocfilehash: 402f8978c0ec6b377dfa020f23595c8954509a07
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825589"
---
# <a name="statusfrequency"></a><span data-ttu-id="f8a4b-103">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="f8a4b-103">StatusFrequency</span></span>

<span data-ttu-id="f8a4b-104">O elemento **StatusFrequency** representa o valor de tempo limite máximo, em minutos, no qual as repetições são tentadas pelo servidor.</span><span class="sxs-lookup"><span data-stu-id="f8a4b-104">The **StatusFrequency** element represents the maximum timeout value, in minutes, in which retries are attempted by the server.</span></span> 
  
[<span data-ttu-id="f8a4b-105">Inscrever-se</span><span class="sxs-lookup"><span data-stu-id="f8a4b-105">Subscribe</span></span>](subscribe.md)
  
[<span data-ttu-id="f8a4b-106">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="f8a4b-106">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
  
[<span data-ttu-id="f8a4b-107">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="f8a4b-107">StatusFrequency</span></span>](statusfrequency.md)
  
```XML
<StatusFrequency/>
```

 <span data-ttu-id="f8a4b-108">**SubscriptionStatusFrequencyType**</span><span class="sxs-lookup"><span data-stu-id="f8a4b-108">**SubscriptionStatusFrequencyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f8a4b-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f8a4b-109">Attributes and elements</span></span>

<span data-ttu-id="f8a4b-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f8a4b-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f8a4b-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="f8a4b-111">Attributes</span></span>

<span data-ttu-id="f8a4b-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f8a4b-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f8a4b-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f8a4b-113">Child elements</span></span>

<span data-ttu-id="f8a4b-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f8a4b-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f8a4b-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f8a4b-115">Parent elements</span></span>

|<span data-ttu-id="f8a4b-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f8a4b-116">**Element**</span></span>|<span data-ttu-id="f8a4b-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f8a4b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f8a4b-118">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="f8a4b-118">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md) <br/> |<span data-ttu-id="f8a4b-119">Representa uma assinatura para uma inscrição de notificação de push com base no evento.</span><span class="sxs-lookup"><span data-stu-id="f8a4b-119">Represents a subscription to a push-based event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f8a4b-120">Text value</span><span class="sxs-lookup"><span data-stu-id="f8a4b-120">Text value</span></span>

<span data-ttu-id="f8a4b-121">Se este elemento for usado, será necessário um valor de texto que representa um número inteiro.</span><span class="sxs-lookup"><span data-stu-id="f8a4b-121">A text value that represents an integer is required if this element is used.</span></span> <span data-ttu-id="f8a4b-122">Os valores possíveis para esse elemento são de 1 a 1440, inclusive.</span><span class="sxs-lookup"><span data-stu-id="f8a4b-122">The possible values for this element are 1 to 1440, inclusive.</span></span> <span data-ttu-id="f8a4b-123">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="f8a4b-123">This element is optional.</span></span> <span data-ttu-id="f8a4b-124">O valor padrão é 30 minutos.</span><span class="sxs-lookup"><span data-stu-id="f8a4b-124">The default value is 30 minutes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f8a4b-125">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="f8a4b-125">Remarks</span></span>

<span data-ttu-id="f8a4b-126">O valor de **StatusFrequency** é usado pelo servidor para repetir uma notificação de push quando ele não recebe uma resposta a uma notificação de push ou ping de status do cliente.</span><span class="sxs-lookup"><span data-stu-id="f8a4b-126">The **StatusFrequency** value is used by the server to retry a push notification when it does not receive a response to a push notification or status ping from the client.</span></span> <span data-ttu-id="f8a4b-127">Se o servidor não recebe uma resposta, ele repete enviando a notificação várias vezes, antes de parar enviar a notificação.</span><span class="sxs-lookup"><span data-stu-id="f8a4b-127">If the server does not receive a response, it retries sending the notification several times before it stops sending the notification.</span></span> <span data-ttu-id="f8a4b-128">No EWS, o intervalo de repetição padrão é 30 segundos e tentativas subsequentes são sempre double a hora do último intervalo de repetição.</span><span class="sxs-lookup"><span data-stu-id="f8a4b-128">In EWS, the default retry interval is 30 seconds and subsequent retries are always double the time of the last retry interval.</span></span> <span data-ttu-id="f8a4b-129">Número de repetições não é exato, pois eles podem ser atrasados devido aos outros carregamentos no servidor.</span><span class="sxs-lookup"><span data-stu-id="f8a4b-129">Retry times are not exact as they can be delayed due to other loads on the server.</span></span> <span data-ttu-id="f8a4b-130">A tabela a seguir mostra como os intervalos de repetição ocorrerem nos 30 minutos alocados pelo valor **StatusFrequency** padrão (supondo que o servidor não o encontrou qualquer atrasos).</span><span class="sxs-lookup"><span data-stu-id="f8a4b-130">The following table shows how the retry intervals occur in the 30 minutes allotted by the default **StatusFrequency** value (assuming the server did not encounter any delays).</span></span> 
  
|<span data-ttu-id="f8a4b-131">**Retry**</span><span class="sxs-lookup"><span data-stu-id="f8a4b-131">**Retry**</span></span>|<span data-ttu-id="f8a4b-132">**Segundos**</span><span class="sxs-lookup"><span data-stu-id="f8a4b-132">**Seconds**</span></span>|<span data-ttu-id="f8a4b-133">**Time**</span><span class="sxs-lookup"><span data-stu-id="f8a4b-133">**Time**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f8a4b-134">0</span><span class="sxs-lookup"><span data-stu-id="f8a4b-134">0</span></span>  <br/> |<span data-ttu-id="f8a4b-135">0</span><span class="sxs-lookup"><span data-stu-id="f8a4b-135">0</span></span>  <br/> |<span data-ttu-id="f8a4b-136">Sincronização inicial</span><span class="sxs-lookup"><span data-stu-id="f8a4b-136">Initial sync</span></span>  <br/> |
|<span data-ttu-id="f8a4b-137">1</span><span class="sxs-lookup"><span data-stu-id="f8a4b-137">1</span></span>  <br/> |<span data-ttu-id="f8a4b-138">30</span><span class="sxs-lookup"><span data-stu-id="f8a4b-138">30</span></span>  <br/> |<span data-ttu-id="f8a4b-139">00:30</span><span class="sxs-lookup"><span data-stu-id="f8a4b-139">00:30</span></span>  <br/> |
|<span data-ttu-id="f8a4b-140">2</span><span class="sxs-lookup"><span data-stu-id="f8a4b-140">2</span></span>  <br/> |<span data-ttu-id="f8a4b-141">60</span><span class="sxs-lookup"><span data-stu-id="f8a4b-141">60</span></span>  <br/> |<span data-ttu-id="f8a4b-142">01:00</span><span class="sxs-lookup"><span data-stu-id="f8a4b-142">01:00</span></span>  <br/> |
|<span data-ttu-id="f8a4b-143">3</span><span class="sxs-lookup"><span data-stu-id="f8a4b-143">3</span></span>  <br/> |<span data-ttu-id="f8a4b-144">120</span><span class="sxs-lookup"><span data-stu-id="f8a4b-144">120</span></span>  <br/> |<span data-ttu-id="f8a4b-145">02:00</span><span class="sxs-lookup"><span data-stu-id="f8a4b-145">02:00</span></span>  <br/> |
|<span data-ttu-id="f8a4b-146">4</span><span class="sxs-lookup"><span data-stu-id="f8a4b-146">4</span></span>  <br/> |<span data-ttu-id="f8a4b-147">240</span><span class="sxs-lookup"><span data-stu-id="f8a4b-147">240</span></span>  <br/> |<span data-ttu-id="f8a4b-148">04:00</span><span class="sxs-lookup"><span data-stu-id="f8a4b-148">04:00</span></span>  <br/> |
|<span data-ttu-id="f8a4b-149">5</span><span class="sxs-lookup"><span data-stu-id="f8a4b-149">5</span></span>  <br/> |<span data-ttu-id="f8a4b-150">480</span><span class="sxs-lookup"><span data-stu-id="f8a4b-150">480</span></span>  <br/> |<span data-ttu-id="f8a4b-151">08:00</span><span class="sxs-lookup"><span data-stu-id="f8a4b-151">08:00</span></span>  <br/> |
|<span data-ttu-id="f8a4b-152">6</span><span class="sxs-lookup"><span data-stu-id="f8a4b-152">6</span></span>  <br/> |<span data-ttu-id="f8a4b-153">960</span><span class="sxs-lookup"><span data-stu-id="f8a4b-153">960</span></span>  <br/> |<span data-ttu-id="f8a4b-154">16:00</span><span class="sxs-lookup"><span data-stu-id="f8a4b-154">16:00</span></span>  <br/> |
|<span data-ttu-id="f8a4b-155">7</span><span class="sxs-lookup"><span data-stu-id="f8a4b-155">7</span></span>  <br/> |<span data-ttu-id="f8a4b-156">1920</span><span class="sxs-lookup"><span data-stu-id="f8a4b-156">1920</span></span>  <br/> |<span data-ttu-id="f8a4b-157">32:00 - o valor padrão de **StatusFrequency** de 30 excedido, repetir não enviado</span><span class="sxs-lookup"><span data-stu-id="f8a4b-157">32:00 - **StatusFrequency** default value of 30 exceeded, retry not sent</span></span>  <br/> |
   
<span data-ttu-id="f8a4b-158">Se o cliente não receber mensagens de notificação do servidor por um período de tempo que excede o dobro do tempo especificado pela **StatusFrequency**, o cliente deve executar uma ação, como recriar a assinatura.</span><span class="sxs-lookup"><span data-stu-id="f8a4b-158">If the client does not receive notification messages from the server for a period of time that exceeds twice the time specified by **StatusFrequency**, the client should take an action such as recreating the subscription.</span></span> 
  
<span data-ttu-id="f8a4b-159">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f8a4b-159">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f8a4b-160">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f8a4b-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f8a4b-161">Namespace</span><span class="sxs-lookup"><span data-stu-id="f8a4b-161">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f8a4b-162">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f8a4b-162">Schema name</span></span>  <br/> |<span data-ttu-id="f8a4b-163">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f8a4b-163">Types schema</span></span>  <br/> |
|<span data-ttu-id="f8a4b-164">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f8a4b-164">Validation file</span></span>  <br/> |<span data-ttu-id="f8a4b-165">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f8a4b-165">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f8a4b-166">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="f8a4b-166">Can be empty</span></span>  <br/> |<span data-ttu-id="f8a4b-167">False</span><span class="sxs-lookup"><span data-stu-id="f8a4b-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f8a4b-168">Ver também</span><span class="sxs-lookup"><span data-stu-id="f8a4b-168">See also</span></span>



[<span data-ttu-id="f8a4b-169">Inscrever-se a operação</span><span class="sxs-lookup"><span data-stu-id="f8a4b-169">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="f8a4b-170">Operação GetEvents</span><span class="sxs-lookup"><span data-stu-id="f8a4b-170">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="f8a4b-171">Cancelar a operação</span><span class="sxs-lookup"><span data-stu-id="f8a4b-171">Unsubscribe operation</span></span>](unsubscribe-operation.md)
  
[<span data-ttu-id="f8a4b-172">Marca d'água</span><span class="sxs-lookup"><span data-stu-id="f8a4b-172">Watermark</span></span>](watermark.md)

