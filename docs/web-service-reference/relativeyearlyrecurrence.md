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
description: O elemento RelativeYearlyRecurrence descreve um padrão de recorrência anual relativa.
ms.openlocfilehash: ce8d2b134ce1fa34cbce8bd2fa921cab18d908a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825057"
---
# <a name="relativeyearlyrecurrence"></a><span data-ttu-id="f5a07-103">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="f5a07-103">RelativeYearlyRecurrence</span></span>

<span data-ttu-id="f5a07-104">O elemento **RelativeYearlyRecurrence** descreve um padrão de recorrência anual relativa.</span><span class="sxs-lookup"><span data-stu-id="f5a07-104">The **RelativeYearlyRecurrence** element describes a relative yearly recurrence pattern.</span></span> 
  
```xml
<RelativeYearlyRecurrence>
   <DaysOfWeek/>
   <DayOfWeekIndex/>
   <Month/>
</RelativeYearlyRecurrence>
```

 <span data-ttu-id="f5a07-105">**RelativeYearlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="f5a07-105">**RelativeYearlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f5a07-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f5a07-106">Attributes and elements</span></span>

<span data-ttu-id="f5a07-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f5a07-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f5a07-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f5a07-108">Attributes</span></span>

<span data-ttu-id="f5a07-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f5a07-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f5a07-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f5a07-110">Child elements</span></span>

|<span data-ttu-id="f5a07-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f5a07-111">**Element**</span></span>|<span data-ttu-id="f5a07-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f5a07-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5a07-113">DaysOfWeek (DayOfWeekType)</span><span class="sxs-lookup"><span data-stu-id="f5a07-113">DaysOfWeek (DayOfWeekType)</span></span>](daysofweek-dayofweektype.md) <br/> |<span data-ttu-id="f5a07-114">Descreve os dias da semana que são usados em padrões de recorrência do item.</span><span class="sxs-lookup"><span data-stu-id="f5a07-114">Describes the days of the week that are used in item recurrence patterns.</span></span>  <br/> |
|[<span data-ttu-id="f5a07-115">DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="f5a07-115">DayOfWeekIndex</span></span>](dayofweekindex.md) <br/> |<span data-ttu-id="f5a07-116">Descreve qual semana em um mês é usada em um padrão de recorrência anual relativa.</span><span class="sxs-lookup"><span data-stu-id="f5a07-116">Describes which week in a month is used in a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="f5a07-117">Mês (recorrência do Item)</span><span class="sxs-lookup"><span data-stu-id="f5a07-117">Month (Item Recurrence)</span></span>](month-item-recurrence.md) <br/> |<span data-ttu-id="f5a07-118">Descreve o mês quando um item recorrente anual ocorre.</span><span class="sxs-lookup"><span data-stu-id="f5a07-118">Describes the month when a yearly recurring item occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f5a07-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f5a07-119">Parent elements</span></span>

|<span data-ttu-id="f5a07-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f5a07-120">**Element**</span></span>|<span data-ttu-id="f5a07-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f5a07-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5a07-122">Recorrência (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="f5a07-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="f5a07-123">Contém informações de recorrência de tarefas recorrentes.</span><span class="sxs-lookup"><span data-stu-id="f5a07-123">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="f5a07-124">Recorrência (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="f5a07-124">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="f5a07-125">Contém o padrão de recorrência para itens de calendário e solicitações de reunião.</span><span class="sxs-lookup"><span data-stu-id="f5a07-125">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="f5a07-126">Standard</span><span class="sxs-lookup"><span data-stu-id="f5a07-126">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="f5a07-127">Representa a data e hora de quando o tempo é alterado de horário de verão para a hora padrão.</span><span class="sxs-lookup"><span data-stu-id="f5a07-127">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="f5a07-128">Horário de verão</span><span class="sxs-lookup"><span data-stu-id="f5a07-128">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="f5a07-129">Representa a data e hora de quando o tempo é alterado do período padrão para o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="f5a07-129">Represents the date and time when the time changes from standard time to daylight saving time.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f5a07-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="f5a07-130">Remarks</span></span>

<span data-ttu-id="f5a07-131">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f5a07-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f5a07-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f5a07-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f5a07-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="f5a07-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f5a07-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f5a07-134">Schema Name</span></span>  <br/> |<span data-ttu-id="f5a07-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f5a07-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="f5a07-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f5a07-136">Validation File</span></span>  <br/> |<span data-ttu-id="f5a07-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f5a07-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f5a07-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f5a07-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="f5a07-139">False</span><span class="sxs-lookup"><span data-stu-id="f5a07-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f5a07-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="f5a07-140">See also</span></span>



- [<span data-ttu-id="f5a07-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f5a07-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

