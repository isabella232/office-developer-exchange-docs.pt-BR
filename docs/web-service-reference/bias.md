---
title: Tendência
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Bias
api_type:
- schema
ms.assetid: ae10aa44-e6d3-483d-a3e6-bb9c45966810
description: O elemento Bias representa o deslocamento do deslocamento de tempo universal coordenado (UTC) identificado pelo elemento Bias (UTC) para horário padrão e horário de verão. Este valor está em minutos.
ms.openlocfilehash: 6c9dce88f3eece9c793fb018114f07a85c7cb89b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460236"
---
# <a name="bias"></a><span data-ttu-id="540c0-104">Tendência</span><span class="sxs-lookup"><span data-stu-id="540c0-104">Bias</span></span>

<span data-ttu-id="540c0-105">O elemento **Bias** representa o deslocamento do deslocamento de tempo universal coordenado (UTC) identificado pelo elemento [Bias (UTC)](bias-utc.md) para horário padrão e horário de verão.</span><span class="sxs-lookup"><span data-stu-id="540c0-105">The **Bias** element represents the offset from the Coordinated Universal Time (UTC) offset identified by the [Bias (UTC)](bias-utc.md) element for standard time and daylight saving time.</span></span> <span data-ttu-id="540c0-106">Este valor está em minutos.</span><span class="sxs-lookup"><span data-stu-id="540c0-106">This value is in minutes.</span></span> 
  
```xml
<Bias>...</Bias>
```

<span data-ttu-id="540c0-107">**int**</span><span class="sxs-lookup"><span data-stu-id="540c0-107">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="540c0-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="540c0-108">Attributes and elements</span></span>

<span data-ttu-id="540c0-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="540c0-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="540c0-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="540c0-110">Attributes</span></span>

<span data-ttu-id="540c0-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="540c0-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="540c0-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="540c0-112">Child elements</span></span>

<span data-ttu-id="540c0-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="540c0-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="540c0-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="540c0-114">Parent elements</span></span>

|<span data-ttu-id="540c0-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="540c0-115">**Element**</span></span>|<span data-ttu-id="540c0-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="540c0-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="540c0-117">StandardTime</span><span class="sxs-lookup"><span data-stu-id="540c0-117">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="540c0-118">Representa um deslocamento do tempo relativo ao UTC representado pelo elemento [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="540c0-118">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="540c0-119">Esse elemento também contém informações sobre a transição para o horário padrão do horário de verão nas regiões nas quais o horário de verão é observado.</span><span class="sxs-lookup"><span data-stu-id="540c0-119">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="540c0-120">A seguir estão as expressões XPath para o elemento [StandardTime](standardtime.md) :</span><span class="sxs-lookup"><span data-stu-id="540c0-120">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span><br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="540c0-121">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="540c0-121">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="540c0-122">Representa um deslocamento do tempo relativo ao UTC representado pelo elemento [Bias (UTC)](bias-utc.md) nas regiões em que o horário de verão é observado.</span><span class="sxs-lookup"><span data-stu-id="540c0-122">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="540c0-123">Esse elemento também contém informações sobre quando ocorre a transição para o horário de Verão do horário padrão.</span><span class="sxs-lookup"><span data-stu-id="540c0-123">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/><br/><span data-ttu-id="540c0-124">A seguir estão as expressões XPath para o elemento [DaylightTime](daylighttime.md) :</span><span class="sxs-lookup"><span data-stu-id="540c0-124">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span><br/><br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="540c0-125">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="540c0-125">Text value</span></span>

<span data-ttu-id="540c0-126">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="540c0-126">A text value is required.</span></span> <span data-ttu-id="540c0-127">O valor de texto representa um inteiro.</span><span class="sxs-lookup"><span data-stu-id="540c0-127">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="540c0-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="540c0-128">Remarks</span></span>

<span data-ttu-id="540c0-129">O deslocamento usado para determinar a hora local só pode ser fornecido por um dos elementos **Bias** .</span><span class="sxs-lookup"><span data-stu-id="540c0-129">The offset used to determine the local time can only be provided by one of the **Bias** elements.</span></span> <span data-ttu-id="540c0-130">A soma dos valores do elemento Bias fornecido pelo elemento [DaylightTime](daylighttime.md) ou o elemento [StandardTime](standardtime.md) mais o elemento [Bias (UTC)](bias-utc.md) identifica a hora local.</span><span class="sxs-lookup"><span data-stu-id="540c0-130">The sum of the values of the Bias element provided by the [DaylightTime](daylighttime.md) element or the [StandardTime](standardtime.md) element plus the [Bias (UTC)](bias-utc.md) element identifies the local time.</span></span> 
  
## <a name="example"></a><span data-ttu-id="540c0-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="540c0-131">Example</span></span>

<span data-ttu-id="540c0-132">O exemplo a seguir mostra parte de uma solicitação XML que identifica um usuário que observa o horário de verão ajustando o deslocamento do UTC por-60 minutos.</span><span class="sxs-lookup"><span data-stu-id="540c0-132">The following example shows part of an XML request that identifies a user who observes daylight saving time by adjusting the offset from UTC by -60 minutes.</span></span> <span data-ttu-id="540c0-133">Isso torna efetivamente a diferença de 420 minutos do UTC.</span><span class="sxs-lookup"><span data-stu-id="540c0-133">This effectively makes the bias 420 minutes from UTC.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="540c0-134">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="540c0-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="540c0-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="540c0-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="540c0-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="540c0-136">Schema Name</span></span>  <br/> |<span data-ttu-id="540c0-137">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="540c0-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="540c0-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="540c0-138">Validation File</span></span>  <br/> |<span data-ttu-id="540c0-139">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="540c0-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="540c0-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="540c0-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="540c0-141">False</span><span class="sxs-lookup"><span data-stu-id="540c0-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="540c0-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="540c0-142">See also</span></span>

- [<span data-ttu-id="540c0-143">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="540c0-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="540c0-144">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="540c0-144">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

