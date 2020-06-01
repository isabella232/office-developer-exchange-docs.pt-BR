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
description: O elemento DaylightTime representa um deslocamento do tempo relativo ao UTC (tempo Universal Coordenado) que é representado pelo elemento Bias (UTC) nas regiões onde o horário de verão é observado. Esse elemento também contém informações sobre quando ocorre a transição para o horário de Verão do horário padrão.
ms.openlocfilehash: 350fcb4ce278f423c62fcc5ecaa160eda71e4a2c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455650"
---
# <a name="daylighttime"></a><span data-ttu-id="2cd14-104">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="2cd14-104">DaylightTime</span></span>

<span data-ttu-id="2cd14-105">O elemento **DaylightTime** representa um deslocamento do tempo relativo ao UTC (tempo Universal Coordenado) que é representado pelo elemento [Bias (UTC)](bias-utc.md) nas regiões onde o horário de verão é observado.</span><span class="sxs-lookup"><span data-stu-id="2cd14-105">The **DaylightTime** element represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="2cd14-106">Esse elemento também contém informações sobre quando ocorre a transição para o horário de Verão do horário padrão.</span><span class="sxs-lookup"><span data-stu-id="2cd14-106">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span> 
  
- [<span data-ttu-id="2cd14-107">Fuso horário (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="2cd14-107">TimeZone (Availability)</span></span>](timezone-availability.md) 
- [<span data-ttu-id="2cd14-108">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="2cd14-108">DaylightTime</span></span>](daylighttime.md)
  
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

<span data-ttu-id="2cd14-109">**SerializableTimeZoneTime**</span><span class="sxs-lookup"><span data-stu-id="2cd14-109">**SerializableTimeZoneTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2cd14-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="2cd14-110">Attributes and elements</span></span>

<span data-ttu-id="2cd14-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2cd14-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2cd14-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="2cd14-112">Attributes</span></span>

<span data-ttu-id="2cd14-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2cd14-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2cd14-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2cd14-114">Child elements</span></span>

|<span data-ttu-id="2cd14-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2cd14-115">**Element**</span></span>|<span data-ttu-id="2cd14-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2cd14-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2cd14-117">Bias</span><span class="sxs-lookup"><span data-stu-id="2cd14-117">Bias</span></span>](bias.md) <br/> |<span data-ttu-id="2cd14-118">Representa o deslocamento do deslocamento UTC identificado pelo elemento [Bias (UTC)](bias-utc.md) para horário padrão e horário de verão.</span><span class="sxs-lookup"><span data-stu-id="2cd14-118">Represents the offset from the UTC offset that is identified by the [Bias (UTC)](bias-utc.md) element for standard time and daylight saving time.</span></span> <span data-ttu-id="2cd14-119">Este valor está em minutos.</span><span class="sxs-lookup"><span data-stu-id="2cd14-119">This value is in minutes.</span></span>  <br/> |
|[<span data-ttu-id="2cd14-120">Time</span><span class="sxs-lookup"><span data-stu-id="2cd14-120">Time</span></span>](time.md) <br/> |<span data-ttu-id="2cd14-121">Representa o horário de transição do dia para e a partir do horário padrão e do horário de verão.</span><span class="sxs-lookup"><span data-stu-id="2cd14-121">Represents the transition time of day to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="2cd14-122">DayOrder</span><span class="sxs-lookup"><span data-stu-id="2cd14-122">DayOrder</span></span>](dayorder.md) <br/> |<span data-ttu-id="2cd14-123">Representa a _n_th ocorrência do dia que é especificada no elemento [DayOfWeek (TimeZone)](dayofweek-timezone.md) que representa a data de transição de e para o horário padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="2cd14-123">Represents the  _n_th occurrence of the day that is specified in the [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that represents the date of transition from and to standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="2cd14-124">Month</span><span class="sxs-lookup"><span data-stu-id="2cd14-124">Month</span></span>](month.md) <br/> |<span data-ttu-id="2cd14-125">Representa o mês de transição do ano de e para hora padrão e horário de verão.</span><span class="sxs-lookup"><span data-stu-id="2cd14-125">Represents the transition month of the year to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="2cd14-126">DayOfWeek (fuso horário)</span><span class="sxs-lookup"><span data-stu-id="2cd14-126">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="2cd14-127">Representa o dia da semana em que ocorre a transição para e a hora padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="2cd14-127">Represents the day of the week when the transition to and from standard time and daylight saving time occurs.</span></span>  <br/> |
|[<span data-ttu-id="2cd14-128">Year</span><span class="sxs-lookup"><span data-stu-id="2cd14-128">Year</span></span>](year.md) <br/> |<span data-ttu-id="2cd14-129">Usado para definir um fuso horário que muda dependendo do ano.</span><span class="sxs-lookup"><span data-stu-id="2cd14-129">Used to define a time zone that changes depending on the year.</span></span> <span data-ttu-id="2cd14-130">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="2cd14-130">This element is optional.</span></span> <span data-ttu-id="2cd14-131">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2cd14-131">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2cd14-132">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2cd14-132">Parent elements</span></span>

|<span data-ttu-id="2cd14-133">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2cd14-133">**Element**</span></span>|<span data-ttu-id="2cd14-134">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2cd14-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2cd14-135">Fuso horário (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="2cd14-135">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="2cd14-136">Contém elementos que identificam informações de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="2cd14-136">Contains elements that identify time zone information.</span></span><br/><br/><span data-ttu-id="2cd14-137">Esse elemento também contém informações sobre a transição entre o horário padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="2cd14-137">This element also contains information about the transition between standard time and daylight saving time.</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/><br/>`/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="example"></a><span data-ttu-id="2cd14-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2cd14-138">Example</span></span>

<span data-ttu-id="2cd14-139">A solicitação parcial de GetUserAvailability a seguir representa um aplicativo cliente em um local que reconhece o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="2cd14-139">The following partial GetUserAvailability request represents a client application in a location that recognizes daylight saving time.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="2cd14-140">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="2cd14-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2cd14-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="2cd14-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2cd14-142">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2cd14-142">Schema Name</span></span>  <br/> |<span data-ttu-id="2cd14-143">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="2cd14-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="2cd14-144">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2cd14-144">Validation File</span></span>  <br/> |<span data-ttu-id="2cd14-145">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2cd14-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2cd14-146">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2cd14-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="2cd14-147">False</span><span class="sxs-lookup"><span data-stu-id="2cd14-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2cd14-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="2cd14-148">See also</span></span>

- [<span data-ttu-id="2cd14-149">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="2cd14-149">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="2cd14-150">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="2cd14-150">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

