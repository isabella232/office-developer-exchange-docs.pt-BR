---
title: DayOfWeek (TimeZone)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfWeek
api_type:
- schema
ms.assetid: 416e8892-ebb1-4fac-82cf-e27549a6c175
description: O elemento DayOfWeek representa o dia da semana em que ocorre a transição de fuso horário.
ms.openlocfilehash: 7816b90000be36cf3a3354d26d978684bfdcfe40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751703"
---
# <a name="dayofweek-timezone"></a><span data-ttu-id="91e74-103">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="91e74-103">DayOfWeek (TimeZone)</span></span>

<span data-ttu-id="91e74-104">O elemento **DayOfWeek** representa o dia da semana em que ocorre a transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="91e74-104">The **DayOfWeek** element represents the day of the week on which the time zone transition occurs.</span></span> 
  
```xml
<DayOfWeek>...</DayOfWeek>
```

<span data-ttu-id="91e74-105">**DayOfWeekType**</span><span class="sxs-lookup"><span data-stu-id="91e74-105">**DayOfWeekType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="91e74-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="91e74-106">Attributes and elements</span></span>

<span data-ttu-id="91e74-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="91e74-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="91e74-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="91e74-108">Attributes</span></span>

<span data-ttu-id="91e74-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="91e74-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="91e74-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="91e74-110">Child elements</span></span>

<span data-ttu-id="91e74-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="91e74-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="91e74-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="91e74-112">Parent elements</span></span>

|<span data-ttu-id="91e74-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="91e74-113">**Element**</span></span>|<span data-ttu-id="91e74-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="91e74-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="91e74-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="91e74-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="91e74-116">Representa um deslocamento, desde o momento em relação ao tempo Universal Coordenado (UTC) representado pelo elemento [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="91e74-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span><br/><br/><span data-ttu-id="91e74-117">Horário de verão em regiões onde o horário de verão é observado, esse elemento também contém informações sobre a transição para a hora padrão.</span><span class="sxs-lookup"><span data-stu-id="91e74-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="91e74-118">A seguir estão as expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="91e74-118">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="91e74-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="91e74-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="91e74-120">Representa um deslocamento, desde o momento em relação ao UTC representado pelo [Bias (UTC)](bias-utc.md) elemento em regiões onde o horário de verão é observado.</span><span class="sxs-lookup"><span data-stu-id="91e74-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="91e74-121">Esse elemento também contém informações sobre como ocorre a transição do horário de verão do período padrão.</span><span class="sxs-lookup"><span data-stu-id="91e74-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span><br/><br/><span data-ttu-id="91e74-122">A seguir estão as expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="91e74-122">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
|[<span data-ttu-id="91e74-123">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="91e74-123">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="91e74-124">Representa uma transição de fuso horário que ocorre no mesmo dia cada ano.</span><span class="sxs-lookup"><span data-stu-id="91e74-124">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="91e74-125">Text value</span><span class="sxs-lookup"><span data-stu-id="91e74-125">Text value</span></span>

<span data-ttu-id="91e74-126">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="91e74-126">A text value is required.</span></span> <span data-ttu-id="91e74-127">O valor de texto é representado por uma enumeração que tem os seguintes valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="91e74-127">The text value is represented by an enumeration that has the following possible values:</span></span>
  
- <span data-ttu-id="91e74-128">Domingo</span><span class="sxs-lookup"><span data-stu-id="91e74-128">Sunday</span></span>    
- <span data-ttu-id="91e74-129">Segunda-feira</span><span class="sxs-lookup"><span data-stu-id="91e74-129">Monday</span></span>    
- <span data-ttu-id="91e74-130">Terça-feira</span><span class="sxs-lookup"><span data-stu-id="91e74-130">Tuesday</span></span>    
- <span data-ttu-id="91e74-131">Quarta-feira</span><span class="sxs-lookup"><span data-stu-id="91e74-131">Wednesday</span></span>    
- <span data-ttu-id="91e74-132">Quinta-feira</span><span class="sxs-lookup"><span data-stu-id="91e74-132">Thursday</span></span>    
- <span data-ttu-id="91e74-133">Sexta-feira</span><span class="sxs-lookup"><span data-stu-id="91e74-133">Friday</span></span>    
- <span data-ttu-id="91e74-134">Sábado</span><span class="sxs-lookup"><span data-stu-id="91e74-134">Saturday</span></span>    
- <span data-ttu-id="91e74-135">Dia</span><span class="sxs-lookup"><span data-stu-id="91e74-135">Day</span></span>    
- <span data-ttu-id="91e74-136">Dia da semana</span><span class="sxs-lookup"><span data-stu-id="91e74-136">Weekday</span></span>   
- <span data-ttu-id="91e74-137">WeekendDay</span><span class="sxs-lookup"><span data-stu-id="91e74-137">WeekendDay</span></span>
    
## <a name="remarks"></a><span data-ttu-id="91e74-138">Comentários</span><span class="sxs-lookup"><span data-stu-id="91e74-138">Remarks</span></span>

<span data-ttu-id="91e74-139">Um elemento de [StandardTime](standardtime.md) que contém um elemento [DayOrder](dayorder.md) que tem um valor de 5, um elemento de [mês](month.md) que possui um valor de 10 e um elemento de **DayOfWeek** que tem um valor de domingo significa que a transição da hora padrão para o horário de verão economia de tempo ocorre no domingo do mês décimo quinto.</span><span class="sxs-lookup"><span data-stu-id="91e74-139">A [StandardTime](standardtime.md) element that contains a [DayOrder](dayorder.md) element that has a value of 5, a [Month](month.md) element that has a value of 10, and a **DayOfWeek** element that has a value of Sunday means that the transition from standard time to daylight saving time occurs on the fifth Sunday of the tenth month.</span></span> 
  
<span data-ttu-id="91e74-140">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="91e74-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="91e74-141">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="91e74-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="91e74-142">Namespace</span><span class="sxs-lookup"><span data-stu-id="91e74-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="91e74-143">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="91e74-143">Schema Name</span></span>  <br/> |<span data-ttu-id="91e74-144">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="91e74-144">Types schema</span></span>  <br/> |
|<span data-ttu-id="91e74-145">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="91e74-145">Validation File</span></span>  <br/> |<span data-ttu-id="91e74-146">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="91e74-146">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="91e74-147">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="91e74-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="91e74-148">False</span><span class="sxs-lookup"><span data-stu-id="91e74-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="91e74-149">Ver também</span><span class="sxs-lookup"><span data-stu-id="91e74-149">See also</span></span>

- [<span data-ttu-id="91e74-150">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="91e74-150">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="91e74-151">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="91e74-151">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

