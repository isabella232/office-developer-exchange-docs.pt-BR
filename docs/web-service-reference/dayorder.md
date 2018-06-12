---
title: DayOrder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOrder
api_type:
- schema
ms.assetid: 3022f839-12a2-42a9-820e-3ea585ce8657
description: O elemento DayOrder representa a enésima ocorrência do dia especificado no elemento DayOfWeek (TimeZone) que representa a data de transição de e até o período padrão e o horário de verão.
ms.openlocfilehash: 03ee678611a6cf58a7256ded67ab4d0a8a06a7ee
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751708"
---
# <a name="dayorder"></a><span data-ttu-id="3dad9-103">DayOrder</span><span class="sxs-lookup"><span data-stu-id="3dad9-103">DayOrder</span></span>

<span data-ttu-id="3dad9-104">O elemento **DayOrder** representa a ocorrência de _n_th do dia especificado no elemento [DayOfWeek (TimeZone)](dayofweek-timezone.md) que representa a data de transição de e até o período padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="3dad9-104">The **DayOrder** element represents the  _n_th occurrence of the day specified in the [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that represents the date of transition from and to standard time and daylight saving time.</span></span> 
  
```xml
<DayOrder>...</DayOrder>
```

<span data-ttu-id="3dad9-105">**curto**</span><span class="sxs-lookup"><span data-stu-id="3dad9-105">**short**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="3dad9-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3dad9-106">Attributes and elements</span></span>

<span data-ttu-id="3dad9-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3dad9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3dad9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3dad9-108">Attributes</span></span>

<span data-ttu-id="3dad9-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3dad9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3dad9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3dad9-110">Child elements</span></span>

<span data-ttu-id="3dad9-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3dad9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3dad9-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3dad9-112">Parent elements</span></span>

|<span data-ttu-id="3dad9-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3dad9-113">**Element**</span></span>|<span data-ttu-id="3dad9-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3dad9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3dad9-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="3dad9-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="3dad9-116">Representa um deslocamento, desde o momento em relação ao tempo Universal Coordenado (UTC) representado pelo elemento [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="3dad9-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span><br/><br/><span data-ttu-id="3dad9-117">Horário de verão em regiões onde o horário de verão é observado, esse elemento também contém informações sobre a transição para a hora padrão.</span><span class="sxs-lookup"><span data-stu-id="3dad9-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="3dad9-118">A seguir estão as expressões XPath ao elemento [StandardTime](standardtime.md) :</span><span class="sxs-lookup"><span data-stu-id="3dad9-118">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="3dad9-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="3dad9-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="3dad9-120">Representa um deslocamento, desde o momento em relação ao UTC representado pelo [Bias (UTC)](bias-utc.md) elemento em regiões onde o horário de verão é observado.</span><span class="sxs-lookup"><span data-stu-id="3dad9-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="3dad9-121">Esse elemento também contém informações sobre como ocorre a transição do horário de verão do período padrão.</span><span class="sxs-lookup"><span data-stu-id="3dad9-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span><br/><br/><span data-ttu-id="3dad9-122">A seguir estão as expressões XPath ao elemento [DaylightTime](daylighttime.md) :</span><span class="sxs-lookup"><span data-stu-id="3dad9-122">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3dad9-123">Text value</span><span class="sxs-lookup"><span data-stu-id="3dad9-123">Text value</span></span>

<span data-ttu-id="3dad9-124">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="3dad9-124">A text value is required.</span></span> <span data-ttu-id="3dad9-125">O valor para o elemento **DayOrder** pode ser de 1 a 5.</span><span class="sxs-lookup"><span data-stu-id="3dad9-125">The value for the **DayOrder** element can be 1 through 5.</span></span> <span data-ttu-id="3dad9-126">O valor máximo para esse elemento pode ser 4 ou 5, dependendo do mês e ano.</span><span class="sxs-lookup"><span data-stu-id="3dad9-126">The maximum value for this element can be either 4 or 5, depending on the month and year.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3dad9-127">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="3dad9-127">Remarks</span></span>

<span data-ttu-id="3dad9-128">Um elemento de [StandardTime](standardtime.md) que contém um elemento **DayOrder** que tem um valor de 5, um elemento de [mês](month.md) que possui um valor de 10 e um elemento de [DayOfWeek (TimeZone)](dayofweek-timezone.md) que tem um valor de domingo significa que a transição da hora padrão para Horário de verão ocorre no domingo do mês décimo quinto.</span><span class="sxs-lookup"><span data-stu-id="3dad9-128">A [StandardTime](standardtime.md) element that contains a **DayOrder** element that has a value of 5, a [Month](month.md) element that has a value of 10, and a [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that has a value of Sunday means that the transition from standard time to daylight saving time occurs on the fifth Sunday of the tenth month.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="3dad9-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3dad9-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3dad9-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="3dad9-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3dad9-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3dad9-131">Schema Name</span></span>  <br/> |<span data-ttu-id="3dad9-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3dad9-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="3dad9-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3dad9-133">Validation File</span></span>  <br/> |<span data-ttu-id="3dad9-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3dad9-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3dad9-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3dad9-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="3dad9-136">False</span><span class="sxs-lookup"><span data-stu-id="3dad9-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3dad9-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="3dad9-137">See also</span></span>

- [<span data-ttu-id="3dad9-138">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="3dad9-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="3dad9-139">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="3dad9-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
