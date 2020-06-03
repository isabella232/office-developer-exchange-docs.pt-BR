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
ms.openlocfilehash: 5006238590c4cd7556a92fb1fbe13292383412b8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530363"
---
# <a name="weeklyrecurrence"></a><span data-ttu-id="a627c-103">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="a627c-103">WeeklyRecurrence</span></span>

<span data-ttu-id="a627c-104">O elemento **WeeklyRecurrence** descreve um padrão de recorrência semanal.</span><span class="sxs-lookup"><span data-stu-id="a627c-104">The **WeeklyRecurrence** element describes a weekly recurrence pattern.</span></span> 
  
```XML
<WeeklyRecurrence>
   <Interval/>
   <DaysOfWeek/>
   <FirstDayOfWeek/>
</WeeklyRecurrence>
```

 <span data-ttu-id="a627c-105">**WeeklyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="a627c-105">**WeeklyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a627c-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a627c-106">Attributes and elements</span></span>

<span data-ttu-id="a627c-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a627c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a627c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a627c-108">Attributes</span></span>

<span data-ttu-id="a627c-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a627c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a627c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a627c-110">Child elements</span></span>

|<span data-ttu-id="a627c-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a627c-111">**Element**</span></span>|<span data-ttu-id="a627c-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a627c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a627c-113">Intervalo</span><span class="sxs-lookup"><span data-stu-id="a627c-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="a627c-114">Define o intervalo, em semanas, entre dois itens de padrão de recorrência semanal consecutivos.</span><span class="sxs-lookup"><span data-stu-id="a627c-114">Defines the interval, in weeks, between two consecutive weekly recurrence pattern items.</span></span> <span data-ttu-id="a627c-115">O valor pode estar no intervalo de 1 a 99.</span><span class="sxs-lookup"><span data-stu-id="a627c-115">The value can be in the range from 1 to 99.</span></span>  <br/> |
|[<span data-ttu-id="a627c-116">DaysOfWeek (DaysOfWeekType)</span><span class="sxs-lookup"><span data-stu-id="a627c-116">DaysOfWeek (DaysOfWeekType)</span></span>](daysofweek-daysofweektype.md) <br/> |<span data-ttu-id="a627c-117">Descreve quais dias da semana estão no padrão de recorrência semanal.</span><span class="sxs-lookup"><span data-stu-id="a627c-117">Describes which days of the week are in the weekly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="a627c-118">FirstDayOfWeek</span><span class="sxs-lookup"><span data-stu-id="a627c-118">FirstDayOfWeek</span></span>](firstdayofweek.md) <br/> |<span data-ttu-id="a627c-119">Especifica o primeiro dia da semana.</span><span class="sxs-lookup"><span data-stu-id="a627c-119">Specifies the first day of the week.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a627c-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a627c-120">Parent elements</span></span>

|<span data-ttu-id="a627c-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a627c-121">**Element**</span></span>|<span data-ttu-id="a627c-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a627c-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a627c-123">Recorrência (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="a627c-123">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="a627c-124">Contém informações de recorrência para tarefas recorrentes.</span><span class="sxs-lookup"><span data-stu-id="a627c-124">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="a627c-125">Recurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="a627c-125">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="a627c-126">Contém o padrão de recorrência para itens de calendário e solicitações de reunião.</span><span class="sxs-lookup"><span data-stu-id="a627c-126">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a627c-127">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="a627c-127">Text value</span></span>

<span data-ttu-id="a627c-128">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a627c-128">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a627c-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="a627c-129">Remarks</span></span>

<span data-ttu-id="a627c-130">As informações de deslocamento de fuso horário serão perdidas se as datas de [início](start.md) e [término](end-ex15websvcsotherref.md) do item mestre recorrente não tiverem uma data igual à primeira ocorrência de um padrão de recorrência semanal.</span><span class="sxs-lookup"><span data-stu-id="a627c-130">The time zone offset information is lost if the [Start](start.md) and [End ](end-ex15websvcsotherref.md) dates of the recurring master item do not have a date that is equal to the first occurrence of a weekly recurrence pattern.</span></span> 
  
<span data-ttu-id="a627c-131">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a627c-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a627c-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a627c-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a627c-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="a627c-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a627c-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a627c-134">Schema Name</span></span>  <br/> |<span data-ttu-id="a627c-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a627c-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="a627c-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a627c-136">Validation File</span></span>  <br/> |<span data-ttu-id="a627c-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a627c-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a627c-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a627c-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="a627c-139">False</span><span class="sxs-lookup"><span data-stu-id="a627c-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a627c-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="a627c-140">See also</span></span>



- [<span data-ttu-id="a627c-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a627c-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

