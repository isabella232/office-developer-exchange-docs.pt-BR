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
description: O elemento transições representa uma matriz de transições de fuso horário.
ms.openlocfilehash: df7cacdef71c3fdfaa3ecadb486843ea30e6109d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837795"
---
# <a name="transitions"></a><span data-ttu-id="0b988-103">Transições</span><span class="sxs-lookup"><span data-stu-id="0b988-103">Transitions</span></span>

<span data-ttu-id="0b988-104">O elemento **transições** representa uma matriz de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="0b988-104">The **Transitions** element represents an array of time zone transitions.</span></span> 
  
```xml
<Transitions Id="">
   <Transition/>
   <AbsoluteDateTransition/>
   <RecurringDayTransition/>
   <RecurringDateTransition/>
</Transitions>
```

 <span data-ttu-id="0b988-105">**ArrayOfTransitionsType**</span><span class="sxs-lookup"><span data-stu-id="0b988-105">**ArrayOfTransitionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0b988-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0b988-106">Attributes and elements</span></span>

<span data-ttu-id="0b988-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0b988-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b988-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0b988-108">Attributes</span></span>

|<span data-ttu-id="0b988-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="0b988-109">**Attribute**</span></span>|<span data-ttu-id="0b988-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0b988-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0b988-111">Id</span><span class="sxs-lookup"><span data-stu-id="0b988-111">Id</span></span>  <br/> |<span data-ttu-id="0b988-112">Representa o identificador exclusivo da definição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="0b988-112">Represents the unique identifier of the time zone definition.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0b988-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0b988-113">Child elements</span></span>

|<span data-ttu-id="0b988-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0b988-114">**Element**</span></span>|<span data-ttu-id="0b988-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0b988-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b988-116">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="0b988-116">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="0b988-117">Representa uma transição de fuso horário que ocorre em uma data específica e, em um momento específico.</span><span class="sxs-lookup"><span data-stu-id="0b988-117">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="0b988-118">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="0b988-118">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="0b988-119">Representa uma transição de fuso horário que ocorre no mesmo dia cada ano.</span><span class="sxs-lookup"><span data-stu-id="0b988-119">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="0b988-120">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="0b988-120">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="0b988-121">Representa uma transição de fuso horário que ocorre em um dia especificado do ano.</span><span class="sxs-lookup"><span data-stu-id="0b988-121">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
|[<span data-ttu-id="0b988-122">Transição</span><span class="sxs-lookup"><span data-stu-id="0b988-122">Transition</span></span>](transition.md) <br/> |<span data-ttu-id="0b988-123">Representa uma transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="0b988-123">Represents a time zone transition.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0b988-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0b988-124">Parent elements</span></span>

|<span data-ttu-id="0b988-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0b988-125">**Element**</span></span>|<span data-ttu-id="0b988-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0b988-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b988-127">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="0b988-127">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="0b988-128">Define o fuso horário para a hora de início de uma [CalendarItem](calendaritem.md) ou [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="0b988-128">Defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="0b988-129">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="0b988-129">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="0b988-130">Define o fuso horário para a hora de término de uma [CalendarItem](calendaritem.md) ou [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="0b988-130">Defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="0b988-131">Timezonedefinition pela última vez</span><span class="sxs-lookup"><span data-stu-id="0b988-131">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="0b988-132">Define um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="0b988-132">Defines a time zone.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0b988-133">Text value</span><span class="sxs-lookup"><span data-stu-id="0b988-133">Text value</span></span>

<span data-ttu-id="0b988-134">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0b988-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0b988-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="0b988-135">Remarks</span></span>

<span data-ttu-id="0b988-136">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0b988-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0b988-137">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0b988-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0b988-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="0b988-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0b988-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0b988-139">Schema Name</span></span>  <br/> |<span data-ttu-id="0b988-140">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0b988-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="0b988-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0b988-141">Validation File</span></span>  <br/> |<span data-ttu-id="0b988-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0b988-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0b988-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0b988-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="0b988-144">False</span><span class="sxs-lookup"><span data-stu-id="0b988-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0b988-145">Ver também</span><span class="sxs-lookup"><span data-stu-id="0b988-145">See also</span></span>



- [<span data-ttu-id="0b988-146">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0b988-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

