---
title: WeeklyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WeeklyRecurrence
api_type:
- schema
ms.assetid: 69c41dd5-597c-45bc-be3f-e2f2b5615aa3
description: O elemento WeeklyRecurrence descreve um padrão de recorrência semanal.
ms.openlocfilehash: 78bc76dd63c6737786df02f336217dc8de9a3a67
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838065"
---
# <a name="weeklyrecurrence"></a><span data-ttu-id="984a5-103">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="984a5-103">WeeklyRecurrence</span></span>

<span data-ttu-id="984a5-104">O elemento **WeeklyRecurrence** descreve um padrão de recorrência semanal.</span><span class="sxs-lookup"><span data-stu-id="984a5-104">The **WeeklyRecurrence** element describes a weekly recurrence pattern.</span></span> 
  
```XML
<WeeklyRecurrence>
   <Interval/>
   <DaysOfWeek/>
   <FirstDayOfWeek/>
</WeeklyRecurrence>
```

 <span data-ttu-id="984a5-105">**WeeklyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="984a5-105">**WeeklyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="984a5-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="984a5-106">Attributes and elements</span></span>

<span data-ttu-id="984a5-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="984a5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="984a5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="984a5-108">Attributes</span></span>

<span data-ttu-id="984a5-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="984a5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="984a5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="984a5-110">Child elements</span></span>

|<span data-ttu-id="984a5-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="984a5-111">**Element**</span></span>|<span data-ttu-id="984a5-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="984a5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="984a5-113">Intervalo</span><span class="sxs-lookup"><span data-stu-id="984a5-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="984a5-114">Define o intervalo, em semanas, entre dois consecutivos semanal recorrência padrão itens.</span><span class="sxs-lookup"><span data-stu-id="984a5-114">Defines the interval, in weeks, between two consecutive weekly recurrence pattern items.</span></span> <span data-ttu-id="984a5-115">O valor pode ser no intervalo de 1 a 99.</span><span class="sxs-lookup"><span data-stu-id="984a5-115">The value can be in the range from 1 to 99.</span></span>  <br/> |
|[<span data-ttu-id="984a5-116">DaysOfWeek (DaysOfWeekType)</span><span class="sxs-lookup"><span data-stu-id="984a5-116">DaysOfWeek (DaysOfWeekType)</span></span>](daysofweek-daysofweektype.md) <br/> |<span data-ttu-id="984a5-117">Descreve quais dias da semana em que o padrão de recorrência semanal.</span><span class="sxs-lookup"><span data-stu-id="984a5-117">Describes which days of the week are in the weekly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="984a5-118">Primeiro_dia_semana</span><span class="sxs-lookup"><span data-stu-id="984a5-118">FirstDayOfWeek</span></span>](firstdayofweek.md) <br/> |<span data-ttu-id="984a5-119">Especifica o primeiro dia da semana.</span><span class="sxs-lookup"><span data-stu-id="984a5-119">Specifies the first day of the week.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="984a5-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="984a5-120">Parent elements</span></span>

|<span data-ttu-id="984a5-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="984a5-121">**Element**</span></span>|<span data-ttu-id="984a5-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="984a5-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="984a5-123">Recorrência (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="984a5-123">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="984a5-124">Contém informações de recorrência de tarefas recorrentes.</span><span class="sxs-lookup"><span data-stu-id="984a5-124">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="984a5-125">Recorrência (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="984a5-125">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="984a5-126">Contém o padrão de recorrência para itens de calendário e solicitações de reunião.</span><span class="sxs-lookup"><span data-stu-id="984a5-126">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="984a5-127">Text value</span><span class="sxs-lookup"><span data-stu-id="984a5-127">Text value</span></span>

<span data-ttu-id="984a5-128">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="984a5-128">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="984a5-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="984a5-129">Remarks</span></span>

<span data-ttu-id="984a5-130">As informações de deslocamento do fuso horário serão perdidas se as datas de [início](start.md) e [término](end-ex15websvcsotherref.md) do item mestre recorrente não tiver uma data que é igual a primeira ocorrência de um padrão de recorrência semanal.</span><span class="sxs-lookup"><span data-stu-id="984a5-130">The time zone offset information is lost if the [Start](start.md) and [End ](end-ex15websvcsotherref.md) dates of the recurring master item do not have a date that is equal to the first occurrence of a weekly recurrence pattern.</span></span> 
  
<span data-ttu-id="984a5-131">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="984a5-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="984a5-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="984a5-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="984a5-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="984a5-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="984a5-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="984a5-134">Schema Name</span></span>  <br/> |<span data-ttu-id="984a5-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="984a5-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="984a5-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="984a5-136">Validation File</span></span>  <br/> |<span data-ttu-id="984a5-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="984a5-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="984a5-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="984a5-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="984a5-139">False</span><span class="sxs-lookup"><span data-stu-id="984a5-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="984a5-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="984a5-140">See also</span></span>



- [<span data-ttu-id="984a5-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="984a5-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

