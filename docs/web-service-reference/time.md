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
description: O elemento time representa o horário de transição do dia para e de horário padrão e horário de verão.
ms.openlocfilehash: 97c89fbcbdb85fcdd4d32a1d44075ac42adef053
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460292"
---
# <a name="time"></a><span data-ttu-id="c060a-103">Hora</span><span class="sxs-lookup"><span data-stu-id="c060a-103">Time</span></span>

<span data-ttu-id="c060a-104">O elemento **time** representa o horário de transição do dia para e de horário padrão e horário de verão.</span><span class="sxs-lookup"><span data-stu-id="c060a-104">The **Time** element represents the transition time of day to and from standard time and daylight saving time.</span></span> 
  
```xml
<Time>...</Time>
```

 <span data-ttu-id="c060a-105">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="c060a-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c060a-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c060a-106">Attributes and elements</span></span>

<span data-ttu-id="c060a-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c060a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c060a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c060a-108">Attributes</span></span>

<span data-ttu-id="c060a-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c060a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c060a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c060a-110">Child elements</span></span>

<span data-ttu-id="c060a-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c060a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c060a-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c060a-112">Parent elements</span></span>

|<span data-ttu-id="c060a-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c060a-113">**Element**</span></span>|<span data-ttu-id="c060a-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c060a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c060a-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="c060a-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="c060a-116">Representa um deslocamento do tempo relativo ao UTC (tempo Universal Coordenado) representado pelo elemento [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="c060a-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="c060a-117">Esse elemento também contém informações sobre a transição para o horário padrão do horário de verão nas regiões nas quais o horário de verão é observado.</span><span class="sxs-lookup"><span data-stu-id="c060a-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span>  <br/><br/>  <span data-ttu-id="c060a-118">A seguir estão as expressões XPath para o elemento [StandardTime](standardtime.md) :</span><span class="sxs-lookup"><span data-stu-id="c060a-118">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/> <br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="c060a-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="c060a-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="c060a-120">Representa um deslocamento do tempo relativo ao UTC representado pelo elemento [Bias (UTC)](bias-utc.md) nas regiões em que o horário de verão é observado.</span><span class="sxs-lookup"><span data-stu-id="c060a-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="c060a-121">Esse elemento também contém informações sobre quando ocorre a transição para o horário de Verão do horário padrão.</span><span class="sxs-lookup"><span data-stu-id="c060a-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/><br/>  <span data-ttu-id="c060a-122">A seguir estão as expressões XPath para o elemento [DaylightTime](daylighttime.md) :</span><span class="sxs-lookup"><span data-stu-id="c060a-122">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span>  <br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c060a-123">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c060a-123">Text value</span></span>

<span data-ttu-id="c060a-124">O valor de texto representa horas, minutos e segundos no seguinte formato: hh: mm: SS.</span><span class="sxs-lookup"><span data-stu-id="c060a-124">The text value represents hours, minutes, and seconds in the following format: hh:mm:ss.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c060a-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="c060a-125">Remarks</span></span>

<span data-ttu-id="c060a-126">Quando o elemento **time** ocorre no elemento [DaylightTime](daylighttime.md) , ele representa a hora do dia em que ocorre a transição do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="c060a-126">When the **Time** element occurs in the [DaylightTime](daylighttime.md) element, it represents the time of day that the transition from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="c060a-127">Quando o elemento [time](time.md) ocorre no elemento [StandardTime](standardtime.md) , ele representa a hora do dia em que ocorre a transição do horário padrão para o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="c060a-127">When the [Time](time.md) element occurs in the [StandardTime](standardtime.md) element, it represents the time of day that the transition from standard time to daylight saving time occurs.</span></span> 
  
<span data-ttu-id="c060a-128">Esse elemento tem uma ocorrência mínima de zero e uma ocorrência máxima de um.</span><span class="sxs-lookup"><span data-stu-id="c060a-128">This element has a minimum occurrence of zero and a maximum occurrence of one.</span></span>
  
## <a name="example"></a><span data-ttu-id="c060a-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c060a-129">Example</span></span>

<span data-ttu-id="c060a-130">A parte a seguir de uma solicitação representa um tempo de transição de 2 A.M.</span><span class="sxs-lookup"><span data-stu-id="c060a-130">The following part of a request represents a transition time of 2 A.M.</span></span> <span data-ttu-id="c060a-131">do horário padrão para o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="c060a-131">from standard time to daylight saving time.</span></span>
  
```xml
<StandardTime>
   <Bias>0</Bias>
   <Time>02:00:00</Time>
   <DayOrder>5</DayOrder>
   <Month>10</Month>
   <DayOfWeek>Sunday</DayOfWeek>
</StandardTime
```

## <a name="element-information"></a><span data-ttu-id="c060a-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c060a-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c060a-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="c060a-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c060a-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c060a-134">Schema Name</span></span>  <br/> |<span data-ttu-id="c060a-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c060a-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="c060a-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c060a-136">Validation File</span></span>  <br/> |<span data-ttu-id="c060a-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c060a-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c060a-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c060a-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="c060a-139">False</span><span class="sxs-lookup"><span data-stu-id="c060a-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c060a-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="c060a-140">See also</span></span>

- [<span data-ttu-id="c060a-141">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="c060a-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="c060a-142">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="c060a-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

