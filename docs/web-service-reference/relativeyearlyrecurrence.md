---
title: RelativeYearlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RelativeYearlyRecurrence
api_type:
- schema
ms.assetid: 25b67876-9979-4a30-a637-357ea10a93b8
description: O elemento RelativeYearlyRecurrence descreve um padrão relativo de recorrência anual.
ms.openlocfilehash: 2abe09ddfe52c24211ef5d0a392ddecaf15bf7bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456715"
---
# <a name="relativeyearlyrecurrence"></a><span data-ttu-id="13c30-103">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="13c30-103">RelativeYearlyRecurrence</span></span>

<span data-ttu-id="13c30-104">O elemento **RelativeYearlyRecurrence** descreve um padrão relativo de recorrência anual.</span><span class="sxs-lookup"><span data-stu-id="13c30-104">The **RelativeYearlyRecurrence** element describes a relative yearly recurrence pattern.</span></span> 
  
```xml
<RelativeYearlyRecurrence>
   <DaysOfWeek/>
   <DayOfWeekIndex/>
   <Month/>
</RelativeYearlyRecurrence>
```

 <span data-ttu-id="13c30-105">**RelativeYearlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="13c30-105">**RelativeYearlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="13c30-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="13c30-106">Attributes and elements</span></span>

<span data-ttu-id="13c30-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="13c30-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="13c30-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="13c30-108">Attributes</span></span>

<span data-ttu-id="13c30-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="13c30-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="13c30-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="13c30-110">Child elements</span></span>

|<span data-ttu-id="13c30-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="13c30-111">**Element**</span></span>|<span data-ttu-id="13c30-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="13c30-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13c30-113">DaysOfWeek (DayOfWeektype)</span><span class="sxs-lookup"><span data-stu-id="13c30-113">DaysOfWeek (DayOfWeekType)</span></span>](daysofweek-dayofweektype.md) <br/> |<span data-ttu-id="13c30-114">Descreve os dias da semana usados nos padrões de recorrência do item.</span><span class="sxs-lookup"><span data-stu-id="13c30-114">Describes the days of the week that are used in item recurrence patterns.</span></span>  <br/> |
|[<span data-ttu-id="13c30-115">DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="13c30-115">DayOfWeekIndex</span></span>](dayofweekindex.md) <br/> |<span data-ttu-id="13c30-116">Descreve qual semana em um mês é usada em um padrão relativo de recorrência anual.</span><span class="sxs-lookup"><span data-stu-id="13c30-116">Describes which week in a month is used in a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="13c30-117">Mês (recorrência do item)</span><span class="sxs-lookup"><span data-stu-id="13c30-117">Month (Item Recurrence)</span></span>](month-item-recurrence.md) <br/> |<span data-ttu-id="13c30-118">Descreve o mês em que ocorre um item recorrente anual.</span><span class="sxs-lookup"><span data-stu-id="13c30-118">Describes the month when a yearly recurring item occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="13c30-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="13c30-119">Parent elements</span></span>

|<span data-ttu-id="13c30-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="13c30-120">**Element**</span></span>|<span data-ttu-id="13c30-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="13c30-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13c30-122">Recorrência (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="13c30-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="13c30-123">Contém informações de recorrência para tarefas recorrentes.</span><span class="sxs-lookup"><span data-stu-id="13c30-123">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="13c30-124">Recurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="13c30-124">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="13c30-125">Contém o padrão de recorrência para itens de calendário e solicitações de reunião.</span><span class="sxs-lookup"><span data-stu-id="13c30-125">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="13c30-126">Standard</span><span class="sxs-lookup"><span data-stu-id="13c30-126">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="13c30-127">Representa a data e a hora em que o horário muda do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="13c30-127">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="13c30-128">Norte</span><span class="sxs-lookup"><span data-stu-id="13c30-128">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="13c30-129">Representa a data e a hora em que o horário muda do horário padrão para o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="13c30-129">Represents the date and time when the time changes from standard time to daylight saving time.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="13c30-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="13c30-130">Remarks</span></span>

<span data-ttu-id="13c30-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="13c30-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="13c30-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="13c30-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="13c30-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="13c30-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="13c30-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="13c30-134">Schema Name</span></span>  <br/> |<span data-ttu-id="13c30-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="13c30-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="13c30-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="13c30-136">Validation File</span></span>  <br/> |<span data-ttu-id="13c30-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="13c30-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="13c30-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="13c30-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="13c30-139">False</span><span class="sxs-lookup"><span data-stu-id="13c30-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="13c30-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="13c30-140">See also</span></span>



- [<span data-ttu-id="13c30-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="13c30-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

