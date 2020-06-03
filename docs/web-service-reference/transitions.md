---
title: Transições
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Transitions
api_type:
- schema
ms.assetid: 26f38f1c-96a3-440e-805c-1437886d11c5
description: O elemento Transitions representa uma matriz de transições de fuso horário.
ms.openlocfilehash: d48fb8872b2f7e052f733c32e5dd1c9b4d04d898
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467435"
---
# <a name="transitions"></a><span data-ttu-id="b01be-103">Transições</span><span class="sxs-lookup"><span data-stu-id="b01be-103">Transitions</span></span>

<span data-ttu-id="b01be-104">O elemento **Transitions** representa uma matriz de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="b01be-104">The **Transitions** element represents an array of time zone transitions.</span></span> 
  
```xml
<Transitions Id="">
   <Transition/>
   <AbsoluteDateTransition/>
   <RecurringDayTransition/>
   <RecurringDateTransition/>
</Transitions>
```

 <span data-ttu-id="b01be-105">**ArrayOfTransitionsType**</span><span class="sxs-lookup"><span data-stu-id="b01be-105">**ArrayOfTransitionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b01be-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b01be-106">Attributes and elements</span></span>

<span data-ttu-id="b01be-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b01be-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b01be-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b01be-108">Attributes</span></span>

|<span data-ttu-id="b01be-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="b01be-109">**Attribute**</span></span>|<span data-ttu-id="b01be-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b01be-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b01be-111">Id</span><span class="sxs-lookup"><span data-stu-id="b01be-111">Id</span></span>  <br/> |<span data-ttu-id="b01be-112">Representa o identificador exclusivo da definição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="b01be-112">Represents the unique identifier of the time zone definition.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b01be-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b01be-113">Child elements</span></span>

|<span data-ttu-id="b01be-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b01be-114">**Element**</span></span>|<span data-ttu-id="b01be-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b01be-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b01be-116">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="b01be-116">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="b01be-117">Representa uma transição de fuso horário que ocorre em uma data específica e em uma hora específica.</span><span class="sxs-lookup"><span data-stu-id="b01be-117">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="b01be-118">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="b01be-118">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="b01be-119">Representa uma transição de fuso horário que ocorre no mesmo dia a cada ano.</span><span class="sxs-lookup"><span data-stu-id="b01be-119">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="b01be-120">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="b01be-120">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="b01be-121">Representa uma transição de fuso horário que ocorre em um dia do ano especificado.</span><span class="sxs-lookup"><span data-stu-id="b01be-121">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
|[<span data-ttu-id="b01be-122">Transição</span><span class="sxs-lookup"><span data-stu-id="b01be-122">Transition</span></span>](transition.md) <br/> |<span data-ttu-id="b01be-123">Representa uma transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="b01be-123">Represents a time zone transition.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b01be-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b01be-124">Parent elements</span></span>

|<span data-ttu-id="b01be-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b01be-125">**Element**</span></span>|<span data-ttu-id="b01be-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b01be-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b01be-127">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="b01be-127">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="b01be-128">Define o fuso horário para a hora de início de um [CalendarItem](calendaritem.md) ou [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="b01be-128">Defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="b01be-129">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="b01be-129">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="b01be-130">Define o fuso horário para a hora de término de um [CalendarItem](calendaritem.md) ou [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="b01be-130">Defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="b01be-131">TimeZoneDefinition</span><span class="sxs-lookup"><span data-stu-id="b01be-131">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="b01be-132">Define um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="b01be-132">Defines a time zone.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b01be-133">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="b01be-133">Text value</span></span>

<span data-ttu-id="b01be-134">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b01be-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b01be-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="b01be-135">Remarks</span></span>

<span data-ttu-id="b01be-136">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b01be-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b01be-137">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b01be-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b01be-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="b01be-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b01be-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b01be-139">Schema Name</span></span>  <br/> |<span data-ttu-id="b01be-140">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b01be-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="b01be-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b01be-141">Validation File</span></span>  <br/> |<span data-ttu-id="b01be-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b01be-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b01be-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b01be-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="b01be-144">False</span><span class="sxs-lookup"><span data-stu-id="b01be-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b01be-145">Confira também</span><span class="sxs-lookup"><span data-stu-id="b01be-145">See also</span></span>



- [<span data-ttu-id="b01be-146">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b01be-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

