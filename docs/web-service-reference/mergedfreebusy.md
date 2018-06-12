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
description: O elemento MergedFreeBusy contém mesclado livre/ocupado fluxo de dados.
ms.openlocfilehash: 542b9fae0c36b0236bd806e8a9117753968e812c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824449"
---
# <a name="mergedfreebusy"></a><span data-ttu-id="05cbe-103">MergedFreeBusy</span><span class="sxs-lookup"><span data-stu-id="05cbe-103">MergedFreeBusy</span></span>

<span data-ttu-id="05cbe-104">O elemento **MergedFreeBusy** contém mesclado livre/ocupado fluxo de dados.</span><span class="sxs-lookup"><span data-stu-id="05cbe-104">The **MergedFreeBusy** element contains the merged free/busy stream of data.</span></span> 
  
[<span data-ttu-id="05cbe-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="05cbe-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="05cbe-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="05cbe-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="05cbe-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="05cbe-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="05cbe-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="05cbe-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="05cbe-109">MergedFreeBusy</span><span class="sxs-lookup"><span data-stu-id="05cbe-109">MergedFreeBusy</span></span>](mergedfreebusy.md)
  
```xml
<MergedFreeBusy>...</MergedFreeBusy>
```

 <span data-ttu-id="05cbe-110">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="05cbe-110">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="05cbe-111">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="05cbe-111">Attributes and elements</span></span>

<span data-ttu-id="05cbe-112">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="05cbe-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05cbe-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="05cbe-113">Attributes</span></span>

<span data-ttu-id="05cbe-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="05cbe-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05cbe-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="05cbe-115">Child elements</span></span>

<span data-ttu-id="05cbe-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="05cbe-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="05cbe-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="05cbe-117">Parent elements</span></span>

|<span data-ttu-id="05cbe-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="05cbe-118">**Element**</span></span>|<span data-ttu-id="05cbe-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="05cbe-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05cbe-120">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="05cbe-120">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="05cbe-121">Contém informações de disponibilidade para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="05cbe-121">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="05cbe-122">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="05cbe-122">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="05cbe-123">Text value</span><span class="sxs-lookup"><span data-stu-id="05cbe-123">Text value</span></span>

<span data-ttu-id="05cbe-124">Um valor de texto for fornecido pelo servidor se o valor para o elemento [FreeBusyViewType](freebusyviewtype.md) for um destes procedimentos:</span><span class="sxs-lookup"><span data-stu-id="05cbe-124">A text value is provided by the server if the value for the [FreeBusyViewType](freebusyviewtype.md) element is one of the following:</span></span> 
  
- <span data-ttu-id="05cbe-125">DetailedMerged</span><span class="sxs-lookup"><span data-stu-id="05cbe-125">DetailedMerged</span></span>
    
- <span data-ttu-id="05cbe-126">FreeBusyMerged</span><span class="sxs-lookup"><span data-stu-id="05cbe-126">FreeBusyMerged</span></span>
    
- <span data-ttu-id="05cbe-127">MergedOnly</span><span class="sxs-lookup"><span data-stu-id="05cbe-127">MergedOnly</span></span>
    
<span data-ttu-id="05cbe-128">O valor de texto é um fluxo de informações de livre/ocupado.</span><span class="sxs-lookup"><span data-stu-id="05cbe-128">The text value is a stream of free/busy information.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="05cbe-129">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="05cbe-129">Remarks</span></span>

<span data-ttu-id="05cbe-130">Fluxo de dados fornecidos por esse elemento é definido pelos elementos [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) e [TimeWindow](timewindow.md) .</span><span class="sxs-lookup"><span data-stu-id="05cbe-130">The stream of data provided by this element is defined by the [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) and [TimeWindow](timewindow.md) elements.</span></span> <span data-ttu-id="05cbe-131">O elemento de [TimeWindow](timewindow.md) define o intervalo de tempo consultado para disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="05cbe-131">The [TimeWindow](timewindow.md) element defines the time span queried for availability.</span></span> <span data-ttu-id="05cbe-132">O elemento de [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) define como o tempo do elemento [TimeWindow](timewindow.md) é dividido em intervalos retornados no elemento **MergedFreeBusy** .</span><span class="sxs-lookup"><span data-stu-id="05cbe-132">The [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) element defines how the time from the [TimeWindow](timewindow.md) element is broken into intervals returned in the **MergedFreeBusy** element.</span></span> <span data-ttu-id="05cbe-133">Cada número no stream **MergedFreeBusy** representa um único intervalo definido pelo elemento [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) .</span><span class="sxs-lookup"><span data-stu-id="05cbe-133">Each number in the **MergedFreeBusy** stream represents a single interval defined by the [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) element.</span></span> <span data-ttu-id="05cbe-134">A tabela a seguir lista os valores possíveis para um intervalo individual.</span><span class="sxs-lookup"><span data-stu-id="05cbe-134">The following table lists the possible values for an individual interval.</span></span> 
  
|<span data-ttu-id="05cbe-135">**Dígito**</span><span class="sxs-lookup"><span data-stu-id="05cbe-135">**Digit**</span></span>|<span data-ttu-id="05cbe-136">**Disponibilidade**</span><span class="sxs-lookup"><span data-stu-id="05cbe-136">**Availability**</span></span>|
|:-----|:-----|
|<span data-ttu-id="05cbe-137">0</span><span class="sxs-lookup"><span data-stu-id="05cbe-137">0</span></span>  <br/> |<span data-ttu-id="05cbe-138">Disponível</span><span class="sxs-lookup"><span data-stu-id="05cbe-138">Free</span></span>  <br/> |
|<span data-ttu-id="05cbe-139">1</span><span class="sxs-lookup"><span data-stu-id="05cbe-139">1</span></span>  <br/> |<span data-ttu-id="05cbe-140">Provisório</span><span class="sxs-lookup"><span data-stu-id="05cbe-140">Tentative</span></span>  <br/> |
|<span data-ttu-id="05cbe-141">2</span><span class="sxs-lookup"><span data-stu-id="05cbe-141">2</span></span>  <br/> |<span data-ttu-id="05cbe-142">Ocupado</span><span class="sxs-lookup"><span data-stu-id="05cbe-142">Busy</span></span>  <br/> |
|<span data-ttu-id="05cbe-143">3</span><span class="sxs-lookup"><span data-stu-id="05cbe-143">3</span></span>  <br/> |<span data-ttu-id="05cbe-144">Out of Office (OOF)</span><span class="sxs-lookup"><span data-stu-id="05cbe-144">Out of Office (OOF)</span></span>  <br/> |
|<span data-ttu-id="05cbe-145">4</span><span class="sxs-lookup"><span data-stu-id="05cbe-145">4</span></span>  <br/> |<span data-ttu-id="05cbe-146">Nenhum dado</span><span class="sxs-lookup"><span data-stu-id="05cbe-146">No data</span></span>  <br/> |
   
<span data-ttu-id="05cbe-147">Por exemplo, uma solicitação de dados do tipo disponível/ocupado inclui um elemento [TimeWindow](timewindow.md) que representa as quatro horas e um elemento [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) que representa 60 minutos.</span><span class="sxs-lookup"><span data-stu-id="05cbe-147">For example, a request for free/busy data includes a [TimeWindow](timewindow.md) element that represents four hours and a [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) element that represents 60 minutes.</span></span> <span data-ttu-id="05cbe-148">Se calendário do usuário solicitado OOF nos primeiros 60 minutos, ocupada pelos seguintes 90 minutos e não agendada para os finais 90 minutos na janela de tempo, o fluxo de **MergedFreeBusy** será 3220.</span><span class="sxs-lookup"><span data-stu-id="05cbe-148">If the requested user's calendar is OOF for the first 60 minutes, busy for the following 90 minutes, and unscheduled for the final 90 minutes in the time window, the **MergedFreeBusy** stream will be 3220.</span></span> <span data-ttu-id="05cbe-149">Se um intervalo contiver mais de uma classificação de disponibilidade, o maior número é usado para classificar esse intervalo.</span><span class="sxs-lookup"><span data-stu-id="05cbe-149">If an interval contains more than one availability classification, the highest number is used to classify that interval.</span></span> 
  
<span data-ttu-id="05cbe-150">O nível de detalhes fornecidos por esse elemento depende as permissões concedidas para o solicitante.</span><span class="sxs-lookup"><span data-stu-id="05cbe-150">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="05cbe-151">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="05cbe-151">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05cbe-152">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="05cbe-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05cbe-153">Namespace</span><span class="sxs-lookup"><span data-stu-id="05cbe-153">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="05cbe-154">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="05cbe-154">Schema Name</span></span>  <br/> |<span data-ttu-id="05cbe-155">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="05cbe-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="05cbe-156">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="05cbe-156">Validation File</span></span>  <br/> |<span data-ttu-id="05cbe-157">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="05cbe-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="05cbe-158">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="05cbe-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="05cbe-159">False</span><span class="sxs-lookup"><span data-stu-id="05cbe-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="05cbe-160">Ver também</span><span class="sxs-lookup"><span data-stu-id="05cbe-160">See also</span></span>



[<span data-ttu-id="05cbe-161">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="05cbe-161">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="05cbe-162">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="05cbe-162">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="05cbe-163">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="05cbe-163">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

