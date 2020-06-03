---
title: MergedFreeBusy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MergedFreeBusy
api_type:
- schema
ms.assetid: ea45590d-476e-4b68-9fe8-ae392feadfea
description: O elemento MergedFreeBusy contém o fluxo de dados de disponibilidade mesclado.
ms.openlocfilehash: a1483449534f0d886e3c97a23d28c5d78f865042
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468723"
---
# <a name="mergedfreebusy"></a><span data-ttu-id="04288-103">MergedFreeBusy</span><span class="sxs-lookup"><span data-stu-id="04288-103">MergedFreeBusy</span></span>

<span data-ttu-id="04288-104">O elemento **MergedFreeBusy** contém o fluxo de dados de disponibilidade mesclado.</span><span class="sxs-lookup"><span data-stu-id="04288-104">The **MergedFreeBusy** element contains the merged free/busy stream of data.</span></span> 
  
[<span data-ttu-id="04288-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="04288-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="04288-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="04288-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="04288-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="04288-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="04288-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="04288-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="04288-109">MergedFreeBusy</span><span class="sxs-lookup"><span data-stu-id="04288-109">MergedFreeBusy</span></span>](mergedfreebusy.md)
  
```xml
<MergedFreeBusy>...</MergedFreeBusy>
```

 <span data-ttu-id="04288-110">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="04288-110">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="04288-111">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="04288-111">Attributes and elements</span></span>

<span data-ttu-id="04288-112">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="04288-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04288-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="04288-113">Attributes</span></span>

<span data-ttu-id="04288-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04288-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04288-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="04288-115">Child elements</span></span>

<span data-ttu-id="04288-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="04288-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="04288-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="04288-117">Parent elements</span></span>

|<span data-ttu-id="04288-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="04288-118">**Element**</span></span>|<span data-ttu-id="04288-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="04288-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04288-120">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="04288-120">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="04288-121">Contém informações de disponibilidade para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="04288-121">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="04288-122">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="04288-122">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="04288-123">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="04288-123">Text value</span></span>

<span data-ttu-id="04288-124">Um valor de texto é fornecido pelo servidor se o valor para o elemento [FreeBusyViewType](freebusyviewtype.md) for um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="04288-124">A text value is provided by the server if the value for the [FreeBusyViewType](freebusyviewtype.md) element is one of the following:</span></span> 
  
- <span data-ttu-id="04288-125">DetailedMerged</span><span class="sxs-lookup"><span data-stu-id="04288-125">DetailedMerged</span></span>
    
- <span data-ttu-id="04288-126">FreeBusyMerged</span><span class="sxs-lookup"><span data-stu-id="04288-126">FreeBusyMerged</span></span>
    
- <span data-ttu-id="04288-127">MergedOnly</span><span class="sxs-lookup"><span data-stu-id="04288-127">MergedOnly</span></span>
    
<span data-ttu-id="04288-128">O valor de texto é um fluxo de informações de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="04288-128">The text value is a stream of free/busy information.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="04288-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="04288-129">Remarks</span></span>

<span data-ttu-id="04288-130">O fluxo de dados fornecido por esse elemento é definido pelos elementos [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) e [TimeWindow](timewindow.md) .</span><span class="sxs-lookup"><span data-stu-id="04288-130">The stream of data provided by this element is defined by the [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) and [TimeWindow](timewindow.md) elements.</span></span> <span data-ttu-id="04288-131">O elemento [TimeWindow](timewindow.md) define o intervalo de tempo consultado para disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="04288-131">The [TimeWindow](timewindow.md) element defines the time span queried for availability.</span></span> <span data-ttu-id="04288-132">O elemento [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) define como o horário do elemento [TimeWindow](timewindow.md) é dividido em intervalos retornados no elemento **MergedFreeBusy** .</span><span class="sxs-lookup"><span data-stu-id="04288-132">The [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) element defines how the time from the [TimeWindow](timewindow.md) element is broken into intervals returned in the **MergedFreeBusy** element.</span></span> <span data-ttu-id="04288-133">Cada número no fluxo **MergedFreeBusy** representa um único intervalo definido pelo elemento [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) .</span><span class="sxs-lookup"><span data-stu-id="04288-133">Each number in the **MergedFreeBusy** stream represents a single interval defined by the [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) element.</span></span> <span data-ttu-id="04288-134">A tabela a seguir lista os valores possíveis para um intervalo individual.</span><span class="sxs-lookup"><span data-stu-id="04288-134">The following table lists the possible values for an individual interval.</span></span> 
  
|<span data-ttu-id="04288-135">**Dígitos**</span><span class="sxs-lookup"><span data-stu-id="04288-135">**Digit**</span></span>|<span data-ttu-id="04288-136">**Disponibilidade**</span><span class="sxs-lookup"><span data-stu-id="04288-136">**Availability**</span></span>|
|:-----|:-----|
|<span data-ttu-id="04288-137">,0</span><span class="sxs-lookup"><span data-stu-id="04288-137">0</span></span>  <br/> |<span data-ttu-id="04288-138">Disponível</span><span class="sxs-lookup"><span data-stu-id="04288-138">Free</span></span>  <br/> |
|<span data-ttu-id="04288-139">1 </span><span class="sxs-lookup"><span data-stu-id="04288-139">1</span></span>  <br/> |<span data-ttu-id="04288-140">Provisória</span><span class="sxs-lookup"><span data-stu-id="04288-140">Tentative</span></span>  <br/> |
|<span data-ttu-id="04288-141">duas</span><span class="sxs-lookup"><span data-stu-id="04288-141">2</span></span>  <br/> |<span data-ttu-id="04288-142">Ocupado</span><span class="sxs-lookup"><span data-stu-id="04288-142">Busy</span></span>  <br/> |
|<span data-ttu-id="04288-143">3D</span><span class="sxs-lookup"><span data-stu-id="04288-143">3</span></span>  <br/> |<span data-ttu-id="04288-144">Ausência Temporária</span><span class="sxs-lookup"><span data-stu-id="04288-144">Out of Office (OOF)</span></span>  <br/> |
|<span data-ttu-id="04288-145">4 </span><span class="sxs-lookup"><span data-stu-id="04288-145">4</span></span>  <br/> |<span data-ttu-id="04288-146">Nenhum dado</span><span class="sxs-lookup"><span data-stu-id="04288-146">No data</span></span>  <br/> |
   
<span data-ttu-id="04288-147">Por exemplo, uma solicitação de dados de disponibilidade inclui um elemento [TimeWindow](timewindow.md) que representa quatro horas e um elemento [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) que representa 60 minutos.</span><span class="sxs-lookup"><span data-stu-id="04288-147">For example, a request for free/busy data includes a [TimeWindow](timewindow.md) element that represents four hours and a [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) element that represents 60 minutes.</span></span> <span data-ttu-id="04288-148">Se o calendário do usuário solicitado for OOF para os primeiros 60 minutos, ocupado pelos seguintes 90 minutos e não tiver sido agendado para o final de 90 minutos na janela de tempo, o fluxo **MergedFreeBusy** será 3220.</span><span class="sxs-lookup"><span data-stu-id="04288-148">If the requested user's calendar is OOF for the first 60 minutes, busy for the following 90 minutes, and unscheduled for the final 90 minutes in the time window, the **MergedFreeBusy** stream will be 3220.</span></span> <span data-ttu-id="04288-149">Se um intervalo contiver mais de uma classificação de disponibilidade, o maior número será usado para classificar esse intervalo.</span><span class="sxs-lookup"><span data-stu-id="04288-149">If an interval contains more than one availability classification, the highest number is used to classify that interval.</span></span> 
  
<span data-ttu-id="04288-150">O nível de detalhes fornecido por esse elemento depende das permissões concedidas ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="04288-150">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="04288-151">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="04288-151">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04288-152">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="04288-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04288-153">Namespace</span><span class="sxs-lookup"><span data-stu-id="04288-153">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="04288-154">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="04288-154">Schema Name</span></span>  <br/> |<span data-ttu-id="04288-155">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="04288-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="04288-156">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="04288-156">Validation File</span></span>  <br/> |<span data-ttu-id="04288-157">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="04288-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="04288-158">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="04288-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="04288-159">False</span><span class="sxs-lookup"><span data-stu-id="04288-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04288-160">Confira também</span><span class="sxs-lookup"><span data-stu-id="04288-160">See also</span></span>



[<span data-ttu-id="04288-161">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="04288-161">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="04288-162">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="04288-162">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="04288-163">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="04288-163">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

