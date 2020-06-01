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
description: O elemento StandardTime representa um deslocamento do tempo relativo ao UTC (tempo Universal Coordenado) que é representado pelo elemento Bias (UTC). Esse elemento também contém informações sobre a transição para o horário padrão do horário de verão nas regiões nas quais o horário de verão é observado.
ms.openlocfilehash: 793f058840d4fd9216f03e660f5be0f7564906cf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456399"
---
# <a name="standardtime"></a><span data-ttu-id="0c66c-104">StandardTime</span><span class="sxs-lookup"><span data-stu-id="0c66c-104">StandardTime</span></span>

<span data-ttu-id="0c66c-105">O elemento **StandardTime** representa um deslocamento do tempo relativo ao UTC (tempo Universal Coordenado) que é representado pelo elemento [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="0c66c-105">The **StandardTime** element represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="0c66c-106">Esse elemento também contém informações sobre a transição para o horário padrão do horário de verão nas regiões nas quais o horário de verão é observado.</span><span class="sxs-lookup"><span data-stu-id="0c66c-106">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span> 
  
- [<span data-ttu-id="0c66c-107">Fuso horário (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="0c66c-107">TimeZone (Availability)</span></span>](timezone-availability.md)
- [<span data-ttu-id="0c66c-108">StandardTime</span><span class="sxs-lookup"><span data-stu-id="0c66c-108">StandardTime</span></span>](standardtime.md)
  
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

 <span data-ttu-id="0c66c-109">**SerializableTimeZoneTime**</span><span class="sxs-lookup"><span data-stu-id="0c66c-109">**SerializableTimeZoneTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0c66c-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0c66c-110">Attributes and elements</span></span>

<span data-ttu-id="0c66c-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0c66c-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0c66c-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="0c66c-112">Attributes</span></span>

<span data-ttu-id="0c66c-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0c66c-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0c66c-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0c66c-114">Child elements</span></span>

|<span data-ttu-id="0c66c-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0c66c-115">**Element**</span></span>|<span data-ttu-id="0c66c-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0c66c-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c66c-117">Bias</span><span class="sxs-lookup"><span data-stu-id="0c66c-117">Bias</span></span>](bias.md) <br/> |<span data-ttu-id="0c66c-118">Representa o deslocamento do deslocamento UTC identificado pelo elemento [Bias (UTC)](bias-utc.md) para horário padrão e horário de verão.</span><span class="sxs-lookup"><span data-stu-id="0c66c-118">Represents the offset from the UTC offset that is identified by the [Bias (UTC)](bias-utc.md) element for standard time and daylight saving time.</span></span> <span data-ttu-id="0c66c-119">Este valor está em minutos.</span><span class="sxs-lookup"><span data-stu-id="0c66c-119">This value is in minutes.</span></span>  <br/> |
|[<span data-ttu-id="0c66c-120">Time</span><span class="sxs-lookup"><span data-stu-id="0c66c-120">Time</span></span>](time.md) <br/> |<span data-ttu-id="0c66c-121">Representa o horário de transição do dia para e a partir do horário padrão e do horário de verão.</span><span class="sxs-lookup"><span data-stu-id="0c66c-121">Represents the transition time of day to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="0c66c-122">DayOrder</span><span class="sxs-lookup"><span data-stu-id="0c66c-122">DayOrder</span></span>](dayorder.md) <br/> |<span data-ttu-id="0c66c-123">Representa a _n_th ocorrência do dia que é especificada no elemento [DayOfWeek (TimeZone)](dayofweek-timezone.md) que representa a data de transição de e para o horário padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="0c66c-123">Represents the  _n_th occurrence of the day that is specified in the [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that represents the date of transition from and to standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="0c66c-124">Month</span><span class="sxs-lookup"><span data-stu-id="0c66c-124">Month</span></span>](month.md) <br/> |<span data-ttu-id="0c66c-125">Representa o mês de transição do ano de e para hora padrão e horário de verão.</span><span class="sxs-lookup"><span data-stu-id="0c66c-125">Represents the transition month of the year to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="0c66c-126">DayOfWeek (fuso horário)</span><span class="sxs-lookup"><span data-stu-id="0c66c-126">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="0c66c-127">Representa o dia da semana em que ocorre a transição para e a hora padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="0c66c-127">Represents the day of the week when the transition to and from standard time and daylight saving time occurs.</span></span>  <br/> |
|[<span data-ttu-id="0c66c-128">Year</span><span class="sxs-lookup"><span data-stu-id="0c66c-128">Year</span></span>](year.md) <br/> |<span data-ttu-id="0c66c-129">Define um fuso horário que muda dependendo do ano.</span><span class="sxs-lookup"><span data-stu-id="0c66c-129">Defines a time zone that changes depending on the year.</span></span> <span data-ttu-id="0c66c-130">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="0c66c-130">This element is optional.</span></span> <span data-ttu-id="0c66c-131">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0c66c-131">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0c66c-132">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0c66c-132">Parent elements</span></span>

|<span data-ttu-id="0c66c-133">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0c66c-133">**Element**</span></span>|<span data-ttu-id="0c66c-134">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0c66c-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c66c-135">Fuso horário (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="0c66c-135">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="0c66c-136">Contém elementos que identificam informações de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="0c66c-136">Contains elements that identify time zone information.</span></span> <span data-ttu-id="0c66c-137">Esse elemento também contém informações sobre a transição entre o horário padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="0c66c-137">This element also contains information about the transition between standard time and daylight saving time.</span></span> <br/><br/><span data-ttu-id="0c66c-138">A seguir estão as expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="0c66c-138">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/> <br/> `/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0c66c-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="0c66c-139">Remarks</span></span>

<span data-ttu-id="0c66c-140">O elemento **StandardTime** representa um tempo de deslocamento que é representado pelo elemento [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="0c66c-140">The **StandardTime** element represents an offset time that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="0c66c-141">Quando o elemento de [polar](bias.md) filho é igual a 0, o horário padrão é igual ao deslocamento de polaridade do UTC que é representado pelo elemento [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="0c66c-141">When the child [Bias](bias.md) element equals 0, the standard time is equal to the bias offset from UTC that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="0c66c-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0c66c-142">Example</span></span>

<span data-ttu-id="0c66c-143">O exemplo a seguir mostra uma região onde o horário de verão é observado.</span><span class="sxs-lookup"><span data-stu-id="0c66c-143">The following example shows a region where daylight saving time is observed.</span></span> <span data-ttu-id="0c66c-144">A transição do horário de verão para o horário padrão é observada às 6:00</span><span class="sxs-lookup"><span data-stu-id="0c66c-144">The transition from daylight saving time to standard time is observed at 2 A.M.</span></span> <span data-ttu-id="0c66c-145">no quinto domingo do décimo mês.</span><span class="sxs-lookup"><span data-stu-id="0c66c-145">on the fifth Sunday of the tenth month.</span></span>
  
```xml
<TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="0c66c-146">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0c66c-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0c66c-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="0c66c-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0c66c-148">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0c66c-148">Schema Name</span></span>  <br/> |<span data-ttu-id="0c66c-149">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0c66c-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="0c66c-150">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0c66c-150">Validation File</span></span>  <br/> |<span data-ttu-id="0c66c-151">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0c66c-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0c66c-152">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0c66c-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="0c66c-153">False</span><span class="sxs-lookup"><span data-stu-id="0c66c-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0c66c-154">Confira também</span><span class="sxs-lookup"><span data-stu-id="0c66c-154">See also</span></span>

- [<span data-ttu-id="0c66c-155">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="0c66c-155">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="0c66c-156">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="0c66c-156">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

