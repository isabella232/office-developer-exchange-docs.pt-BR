---
title: StandardTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StandardTime
api_type:
- schema
ms.assetid: 13084726-ab24-4009-be99-c4a4273c9e05
description: O elemento StandardTime representa um deslocamento, desde o momento em relação ao tempo Universal Coordenado (UTC) que é representado por um elemento Bias (UTC). Horário de verão em regiões onde o horário de verão é observado, esse elemento também contém informações sobre a transição para a hora padrão.
ms.openlocfilehash: 726c31ffba06c1c437711b88444ec5eba45b520d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825546"
---
# <a name="standardtime"></a><span data-ttu-id="6a38e-104">StandardTime</span><span class="sxs-lookup"><span data-stu-id="6a38e-104">StandardTime</span></span>

<span data-ttu-id="6a38e-105">O elemento **StandardTime** representa um deslocamento, desde o momento em relação ao tempo Universal Coordenado (UTC) que é representado por um elemento [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="6a38e-105">The **StandardTime** element represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="6a38e-106">Horário de verão em regiões onde o horário de verão é observado, esse elemento também contém informações sobre a transição para a hora padrão.</span><span class="sxs-lookup"><span data-stu-id="6a38e-106">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span> 
  
- [<span data-ttu-id="6a38e-107">Fuso horário (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="6a38e-107">TimeZone (Availability)</span></span>](timezone-availability.md)
- [<span data-ttu-id="6a38e-108">StandardTime</span><span class="sxs-lookup"><span data-stu-id="6a38e-108">StandardTime</span></span>](standardtime.md)
  
```xml
<StandardTime>
   <Bias>int</Bias>
   <Time>string</Time>
   <DayOrder>short</DayOrder>
   <Month>short</Month>
   <DayOfWeek>Sunday or Monday or Tuesday or Wednesday or Thursday or Friday or Saturday</DayOfWeek>
   <Year>string</Year>
</StandardTime>
```

 <span data-ttu-id="6a38e-109">**SerializableTimeZoneTime**</span><span class="sxs-lookup"><span data-stu-id="6a38e-109">**SerializableTimeZoneTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6a38e-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6a38e-110">Attributes and elements</span></span>

<span data-ttu-id="6a38e-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6a38e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a38e-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="6a38e-112">Attributes</span></span>

<span data-ttu-id="6a38e-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6a38e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6a38e-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6a38e-114">Child elements</span></span>

|<span data-ttu-id="6a38e-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6a38e-115">**Element**</span></span>|<span data-ttu-id="6a38e-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6a38e-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a38e-117">Bias</span><span class="sxs-lookup"><span data-stu-id="6a38e-117">Bias</span></span>](bias.md) <br/> |<span data-ttu-id="6a38e-118">Representa o deslocamento de deslocamento UTC é identificado pelo elemento [Bias (UTC)](bias-utc.md) para o período padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="6a38e-118">Represents the offset from the UTC offset that is identified by the [Bias (UTC)](bias-utc.md) element for standard time and daylight saving time.</span></span> <span data-ttu-id="6a38e-119">Este valor está em minutos.</span><span class="sxs-lookup"><span data-stu-id="6a38e-119">This value is in minutes.</span></span>  <br/> |
|[<span data-ttu-id="6a38e-120">Time</span><span class="sxs-lookup"><span data-stu-id="6a38e-120">Time</span></span>](time.md) <br/> |<span data-ttu-id="6a38e-121">Representa a hora de transição do dia de e para período padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="6a38e-121">Represents the transition time of day to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="6a38e-122">DayOrder</span><span class="sxs-lookup"><span data-stu-id="6a38e-122">DayOrder</span></span>](dayorder.md) <br/> |<span data-ttu-id="6a38e-123">Representa a ocorrência de _n_th do dia em que é especificado no elemento [DayOfWeek (TimeZone)](dayofweek-timezone.md) que representa a data de transição de e até o período padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="6a38e-123">Represents the  _n_th occurrence of the day that is specified in the [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that represents the date of transition from and to standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="6a38e-124">Month</span><span class="sxs-lookup"><span data-stu-id="6a38e-124">Month</span></span>](month.md) <br/> |<span data-ttu-id="6a38e-125">Representa o mês de transição do ano para e de período padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="6a38e-125">Represents the transition month of the year to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="6a38e-126">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="6a38e-126">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="6a38e-127">Representa o dia da semana em que ocorre a transição entre o horário padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="6a38e-127">Represents the day of the week when the transition to and from standard time and daylight saving time occurs.</span></span>  <br/> |
|[<span data-ttu-id="6a38e-128">Ano</span><span class="sxs-lookup"><span data-stu-id="6a38e-128">Year</span></span>](year.md) <br/> |<span data-ttu-id="6a38e-129">Define um fuso horário que mudam dependendo do ano.</span><span class="sxs-lookup"><span data-stu-id="6a38e-129">Defines a time zone that changes depending on the year.</span></span> <span data-ttu-id="6a38e-130">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="6a38e-130">This element is optional.</span></span> <span data-ttu-id="6a38e-131">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6a38e-131">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6a38e-132">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6a38e-132">Parent elements</span></span>

|<span data-ttu-id="6a38e-133">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6a38e-133">**Element**</span></span>|<span data-ttu-id="6a38e-134">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6a38e-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a38e-135">Fuso horário (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="6a38e-135">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="6a38e-136">Contém os elementos que identificam as informações de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="6a38e-136">Contains elements that identify time zone information.</span></span> <span data-ttu-id="6a38e-137">Esse elemento também contém informações sobre a transição entre o período padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="6a38e-137">This element also contains information about the transition between standard time and daylight saving time.</span></span> <br/><br/><span data-ttu-id="6a38e-138">A seguir estão as expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="6a38e-138">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/> <br/> `/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6a38e-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="6a38e-139">Remarks</span></span>

<span data-ttu-id="6a38e-140">O elemento **StandardTime** representa um tempo de deslocamento é representado por um elemento [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="6a38e-140">The **StandardTime** element represents an offset time that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="6a38e-141">Quando o elemento filho [Bias](bias.md) for igual a 0, o tempo padrão é igual ao deslocamento bias de UTC representado pelo elemento [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="6a38e-141">When the child [Bias](bias.md) element equals 0, the standard time is equal to the bias offset from UTC that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="6a38e-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6a38e-142">Example</span></span>

<span data-ttu-id="6a38e-143">O exemplo a seguir mostra uma região em que o horário de verão é observado.</span><span class="sxs-lookup"><span data-stu-id="6a38e-143">The following example shows a region where daylight saving time is observed.</span></span> <span data-ttu-id="6a38e-144">A transição de horário de verão para a hora padrão é observada às 2h</span><span class="sxs-lookup"><span data-stu-id="6a38e-144">The transition from daylight saving time to standard time is observed at 2 A.M.</span></span> <span data-ttu-id="6a38e-145">no quinto domingo do mês décimo.</span><span class="sxs-lookup"><span data-stu-id="6a38e-145">on the fifth Sunday of the tenth month.</span></span>
  
```xml
<TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
  <Bias>480</Bias>
  <StandardTime>
    <Bias>0</Bias>
    <Time>02:00:00</Time>
    <DayOrder>5</DayOrder>
    <Month>10</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </StandardTime>
  <DaylightTime>
    <Bias>-60</Bias>
    <Time>02:00:00</Time>
    <DayOrder>1</DayOrder>
    <Month>4</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </DaylightTime>
</TimeZone>
```

## <a name="element-information"></a><span data-ttu-id="6a38e-146">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6a38e-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6a38e-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="6a38e-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6a38e-148">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6a38e-148">Schema Name</span></span>  <br/> |<span data-ttu-id="6a38e-149">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="6a38e-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="6a38e-150">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6a38e-150">Validation File</span></span>  <br/> |<span data-ttu-id="6a38e-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6a38e-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6a38e-152">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6a38e-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="6a38e-153">False</span><span class="sxs-lookup"><span data-stu-id="6a38e-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6a38e-154">Ver também</span><span class="sxs-lookup"><span data-stu-id="6a38e-154">See also</span></span>

- [<span data-ttu-id="6a38e-155">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="6a38e-155">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="6a38e-156">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="6a38e-156">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

