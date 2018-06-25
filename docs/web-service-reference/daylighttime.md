---
title: DaylightTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DaylightTime
api_type:
- schema
ms.assetid: 9f551ee4-d945-477c-b981-9554b197d26d
description: O elemento DaylightTime representa um deslocamento, desde o momento em relação ao tempo Universal Coordenado (UTC) que é representado por um elemento Bias (UTC) em regiões onde o horário de verão é observado. Esse elemento também contém informações sobre como ocorre a transição do horário de verão do período padrão.
ms.openlocfilehash: 07ec4b1a5f84669aca33d46cdf1fa2e578f3b43b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751702"
---
# <a name="daylighttime"></a><span data-ttu-id="3703f-104">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="3703f-104">DaylightTime</span></span>

<span data-ttu-id="3703f-105">O elemento **DaylightTime** representa um deslocamento, desde o momento em relação ao tempo Universal Coordenado (UTC) que é representado por um elemento [Bias (UTC)](bias-utc.md) em regiões onde o horário de verão é observado.</span><span class="sxs-lookup"><span data-stu-id="3703f-105">The **DaylightTime** element represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="3703f-106">Esse elemento também contém informações sobre como ocorre a transição do horário de verão do período padrão.</span><span class="sxs-lookup"><span data-stu-id="3703f-106">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span> 
  
- [<span data-ttu-id="3703f-107">Fuso horário (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="3703f-107">TimeZone (Availability)</span></span>](timezone-availability.md) 
- [<span data-ttu-id="3703f-108">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="3703f-108">DaylightTime</span></span>](daylighttime.md)
  
```xml
<DaylightTime>
   <Bias>int</Bias>
   <Time>string</Time>
   <DayOrder>short</DayOrder>
   <Month>short</Month>
   <DayOfWeek>Sunday or Monday or Tuesday or Wednesday or Thursday or Friday or Saturday</DayOfWeek>
   <Year>string</Year>
</DaylightTime>
```

<span data-ttu-id="3703f-109">**SerializableTimeZoneTime**</span><span class="sxs-lookup"><span data-stu-id="3703f-109">**SerializableTimeZoneTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="3703f-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3703f-110">Attributes and elements</span></span>

<span data-ttu-id="3703f-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3703f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3703f-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="3703f-112">Attributes</span></span>

<span data-ttu-id="3703f-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3703f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3703f-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3703f-114">Child elements</span></span>

|<span data-ttu-id="3703f-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3703f-115">**Element**</span></span>|<span data-ttu-id="3703f-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3703f-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3703f-117">Bias</span><span class="sxs-lookup"><span data-stu-id="3703f-117">Bias</span></span>](bias.md) <br/> |<span data-ttu-id="3703f-118">Representa o deslocamento de deslocamento UTC é identificado pelo elemento [Bias (UTC)](bias-utc.md) para o período padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="3703f-118">Represents the offset from the UTC offset that is identified by the [Bias (UTC)](bias-utc.md) element for standard time and daylight saving time.</span></span> <span data-ttu-id="3703f-119">Este valor está em minutos.</span><span class="sxs-lookup"><span data-stu-id="3703f-119">This value is in minutes.</span></span>  <br/> |
|[<span data-ttu-id="3703f-120">Time</span><span class="sxs-lookup"><span data-stu-id="3703f-120">Time</span></span>](time.md) <br/> |<span data-ttu-id="3703f-121">Representa a hora de transição do dia de e para período padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="3703f-121">Represents the transition time of day to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="3703f-122">DayOrder</span><span class="sxs-lookup"><span data-stu-id="3703f-122">DayOrder</span></span>](dayorder.md) <br/> |<span data-ttu-id="3703f-123">Representa a ocorrência de _n_th do dia em que é especificado no elemento [DayOfWeek (TimeZone)](dayofweek-timezone.md) que representa a data de transição de e até o período padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="3703f-123">Represents the  _n_th occurrence of the day that is specified in the [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that represents the date of transition from and to standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="3703f-124">Month</span><span class="sxs-lookup"><span data-stu-id="3703f-124">Month</span></span>](month.md) <br/> |<span data-ttu-id="3703f-125">Representa o mês de transição do ano para e de período padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="3703f-125">Represents the transition month of the year to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="3703f-126">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="3703f-126">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="3703f-127">Representa o dia da semana em que ocorre a transição entre o horário padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="3703f-127">Represents the day of the week when the transition to and from standard time and daylight saving time occurs.</span></span>  <br/> |
|[<span data-ttu-id="3703f-128">Ano</span><span class="sxs-lookup"><span data-stu-id="3703f-128">Year</span></span>](year.md) <br/> |<span data-ttu-id="3703f-129">Usado para definir um fuso horário que mudam dependendo do ano.</span><span class="sxs-lookup"><span data-stu-id="3703f-129">Used to define a time zone that changes depending on the year.</span></span> <span data-ttu-id="3703f-130">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="3703f-130">This element is optional.</span></span> <span data-ttu-id="3703f-131">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="3703f-131">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3703f-132">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3703f-132">Parent elements</span></span>

|<span data-ttu-id="3703f-133">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3703f-133">**Element**</span></span>|<span data-ttu-id="3703f-134">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3703f-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3703f-135">Fuso horário (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="3703f-135">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="3703f-136">Contém os elementos que identificam as informações de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="3703f-136">Contains elements that identify time zone information.</span></span><br/><br/><span data-ttu-id="3703f-137">Esse elemento também contém informações sobre a transição entre o período padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="3703f-137">This element also contains information about the transition between standard time and daylight saving time.</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/><br/>`/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="example"></a><span data-ttu-id="3703f-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3703f-138">Example</span></span>

<span data-ttu-id="3703f-139">A solicitação de GetUserAvailability parcial seguinte representa um aplicativo cliente no local que reconheça o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="3703f-139">The following partial GetUserAvailability request represents a client application in a location that recognizes daylight saving time.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="3703f-140">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3703f-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3703f-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="3703f-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3703f-142">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3703f-142">Schema Name</span></span>  <br/> |<span data-ttu-id="3703f-143">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3703f-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="3703f-144">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3703f-144">Validation File</span></span>  <br/> |<span data-ttu-id="3703f-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3703f-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3703f-146">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3703f-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="3703f-147">False</span><span class="sxs-lookup"><span data-stu-id="3703f-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3703f-148">Ver também</span><span class="sxs-lookup"><span data-stu-id="3703f-148">See also</span></span>

- [<span data-ttu-id="3703f-149">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="3703f-149">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="3703f-150">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="3703f-150">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

