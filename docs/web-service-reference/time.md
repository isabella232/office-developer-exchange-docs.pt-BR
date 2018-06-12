---
title: Hora
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Time
api_type:
- schema
ms.assetid: c4b98be7-141c-4ba8-97ef-9ad1ed19f61f
description: O elemento de tempo representa a hora de transição do dia de e para período padrão e o horário de verão.
ms.openlocfilehash: 716487fb7ed64dbaa6fa97caf1ea608e4673d2ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837724"
---
# <a name="time"></a><span data-ttu-id="38bd1-103">Hora</span><span class="sxs-lookup"><span data-stu-id="38bd1-103">Time</span></span>

<span data-ttu-id="38bd1-104">O elemento de **tempo** representa a hora de transição do dia de e para período padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="38bd1-104">The **Time** element represents the transition time of day to and from standard time and daylight saving time.</span></span> 
  
```xml
<Time>...</Time>
```

 <span data-ttu-id="38bd1-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="38bd1-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="38bd1-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="38bd1-106">Attributes and elements</span></span>

<span data-ttu-id="38bd1-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="38bd1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="38bd1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="38bd1-108">Attributes</span></span>

<span data-ttu-id="38bd1-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="38bd1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="38bd1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="38bd1-110">Child elements</span></span>

<span data-ttu-id="38bd1-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="38bd1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="38bd1-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="38bd1-112">Parent elements</span></span>

|<span data-ttu-id="38bd1-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="38bd1-113">**Element**</span></span>|<span data-ttu-id="38bd1-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="38bd1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38bd1-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="38bd1-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="38bd1-116">Representa um deslocamento, desde o momento em relação ao tempo Universal Coordenado (UTC) representado pelo elemento [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="38bd1-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="38bd1-117">Horário de verão em regiões onde o horário de verão é observado, esse elemento também contém informações sobre a transição para a hora padrão.</span><span class="sxs-lookup"><span data-stu-id="38bd1-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span>  <br/><br/>  <span data-ttu-id="38bd1-118">A seguir estão as expressões XPath ao elemento [StandardTime](standardtime.md) :</span><span class="sxs-lookup"><span data-stu-id="38bd1-118">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/> <br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="38bd1-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="38bd1-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="38bd1-120">Representa um deslocamento, desde o momento em relação ao UTC representado pelo [Bias (UTC)](bias-utc.md) elemento em regiões onde o horário de verão é observado.</span><span class="sxs-lookup"><span data-stu-id="38bd1-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="38bd1-121">Esse elemento também contém informações sobre como ocorre a transição do horário de verão do período padrão.</span><span class="sxs-lookup"><span data-stu-id="38bd1-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/><br/>  <span data-ttu-id="38bd1-122">A seguir estão as expressões XPath ao elemento [DaylightTime](daylighttime.md) :</span><span class="sxs-lookup"><span data-stu-id="38bd1-122">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span>  <br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="38bd1-123">Text value</span><span class="sxs-lookup"><span data-stu-id="38bd1-123">Text value</span></span>

<span data-ttu-id="38bd1-124">O valor de texto representa horas, minutos e segundos no seguinte formato: hh.</span><span class="sxs-lookup"><span data-stu-id="38bd1-124">The text value represents hours, minutes, and seconds in the following format: hh:mm:ss.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="38bd1-125">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="38bd1-125">Remarks</span></span>

<span data-ttu-id="38bd1-126">Quando o elemento de **tempo** ocorre no elemento [DaylightTime](daylighttime.md) , ela representa a hora do dia em que ocorre a transição de horário de verão para a hora padrão.</span><span class="sxs-lookup"><span data-stu-id="38bd1-126">When the **Time** element occurs in the [DaylightTime](daylighttime.md) element, it represents the time of day that the transition from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="38bd1-127">Quando o elemento de [tempo](time.md) ocorre no elemento [StandardTime](standardtime.md) , ela representa a hora do dia em que ocorre a transição da hora padrão para o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="38bd1-127">When the [Time](time.md) element occurs in the [StandardTime](standardtime.md) element, it represents the time of day that the transition from standard time to daylight saving time occurs.</span></span> 
  
<span data-ttu-id="38bd1-128">Este elemento tem uma ocorrência mínima de zero e uma ocorrência de máxima de um.</span><span class="sxs-lookup"><span data-stu-id="38bd1-128">This element has a minimum occurrence of zero and a maximum occurrence of one.</span></span>
  
## <a name="example"></a><span data-ttu-id="38bd1-129">Example</span><span class="sxs-lookup"><span data-stu-id="38bd1-129">Example</span></span>

<span data-ttu-id="38bd1-130">A seguinte parte de uma solicitação representa um tempo de transição de 2h da manhã</span><span class="sxs-lookup"><span data-stu-id="38bd1-130">The following part of a request represents a transition time of 2 A.M.</span></span> <span data-ttu-id="38bd1-131">da hora padrão para o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="38bd1-131">from standard time to daylight saving time.</span></span>
  
```xml
<StandardTime>
   <Bias>0</Bias>
   <Time>02:00:00</Time>
   <DayOrder>5</DayOrder>
   <Month>10</Month>
   <DayOfWeek>Sunday</DayOfWeek>
</StandardTime
```

## <a name="element-information"></a><span data-ttu-id="38bd1-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="38bd1-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="38bd1-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="38bd1-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="38bd1-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="38bd1-134">Schema Name</span></span>  <br/> |<span data-ttu-id="38bd1-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="38bd1-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="38bd1-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="38bd1-136">Validation File</span></span>  <br/> |<span data-ttu-id="38bd1-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="38bd1-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="38bd1-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="38bd1-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="38bd1-139">False</span><span class="sxs-lookup"><span data-stu-id="38bd1-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="38bd1-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="38bd1-140">See also</span></span>

- [<span data-ttu-id="38bd1-141">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="38bd1-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="38bd1-142">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="38bd1-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

