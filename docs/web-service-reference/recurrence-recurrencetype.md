---
title: Recurrence (RecurrenceType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recurrence
api_type:
- schema
ms.assetid: 3d1c2c1c-4103-47ce-ad3c-ad16ec6e9b12
description: O elemento de recorrência contém o padrão de recorrência para itens de calendário e solicitações de reunião.
ms.openlocfilehash: d9c6009e11eb5b66cdd749b8e085935060f99ab7
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353347"
---
# <a name="recurrence-recurrencetype"></a><span data-ttu-id="dd4d9-103">Recurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="dd4d9-103">Recurrence (RecurrenceType)</span></span>

<span data-ttu-id="dd4d9-104">O elemento de **Recorrência** contém o padrão de recorrência para itens de calendário e solicitações de reunião.</span><span class="sxs-lookup"><span data-stu-id="dd4d9-104">The **Recurrence** element contains the recurrence pattern for calendar items and meeting requests.</span></span> 
  
```xml
<Recurrence>
      <RelativeYearlyRecurrence/>
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteMonthlyRecurrence/>
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <RelativeMonthlyRecurrence/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <RelativeYearlyRecurrence/> 
      <EndDateRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <RelativeYearlyRecurrence/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <DailyRecurrence/> 
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteYearlyRecurrence/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <DailyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteYearlyRecurrence/> 
      <NumberedRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <DailyRecurrence/> 
      <NumberedRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteMonthlyRecurrence/> 
      <EndDateRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteMonthlyRecurrence/> 
      <NumberedRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <RelativeMonthlyRecurrence/> 
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <NumberedRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteYearlyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <RelativeMonthlyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

<span data-ttu-id="dd4d9-105">**RecurrenceType**</span><span class="sxs-lookup"><span data-stu-id="dd4d9-105">**RecurrenceType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="dd4d9-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="dd4d9-106">Attributes and elements</span></span>

<span data-ttu-id="dd4d9-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="dd4d9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd4d9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="dd4d9-108">Attributes</span></span>

<span data-ttu-id="dd4d9-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="dd4d9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dd4d9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="dd4d9-110">Child elements</span></span>

|<span data-ttu-id="dd4d9-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dd4d9-111">**Element**</span></span>|<span data-ttu-id="dd4d9-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dd4d9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd4d9-113">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="dd4d9-113">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="dd4d9-114">Descreve um padrão de recorrência anual relativa.</span><span class="sxs-lookup"><span data-stu-id="dd4d9-114">Describes a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="dd4d9-115">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="dd4d9-115">AbsoluteYearlyRecurrence</span></span>](absoluteyearlyrecurrence.md) <br/> |<span data-ttu-id="dd4d9-116">Representa um padrão de recorrência anual.</span><span class="sxs-lookup"><span data-stu-id="dd4d9-116">Represents a yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="dd4d9-117">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="dd4d9-117">RelativeMonthlyRecurrence</span></span>](relativemonthlyrecurrence.md) <br/> |<span data-ttu-id="dd4d9-118">Descreve um padrão de recorrência mensal relativa para um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="dd4d9-118">Describes a relative monthly recurrence pattern for a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="dd4d9-119">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="dd4d9-119">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="dd4d9-120">Representa um padrão de recorrência mensal.</span><span class="sxs-lookup"><span data-stu-id="dd4d9-120">Represents a monthly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="dd4d9-121">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="dd4d9-121">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="dd4d9-122">Descreve a frequência, em semanas e os dias em um item de calendário ou uma tarefa recorrente.</span><span class="sxs-lookup"><span data-stu-id="dd4d9-122">Describes the frequency, in weeks, and the days that a calendar item or task recurs.</span></span>  <br/> |
|[<span data-ttu-id="dd4d9-123">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="dd4d9-123">DailyRecurrence</span></span>](dailyrecurrence.md) <br/> |<span data-ttu-id="dd4d9-124">Descreve a frequência, em dias, no qual um item de calendário ou uma tarefa recorrente.</span><span class="sxs-lookup"><span data-stu-id="dd4d9-124">Describes the frequency, in days, in which a calendar item or task recurs.</span></span>  <br/> |
|[<span data-ttu-id="dd4d9-125">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="dd4d9-125">NoEndRecurrence</span></span>](noendrecurrence.md) <br/> |<span data-ttu-id="dd4d9-126">Descreve um padrão de recorrência que não tem uma data de término definidas.</span><span class="sxs-lookup"><span data-stu-id="dd4d9-126">Describes a recurrence pattern that does not have a defined end date.</span></span>  <br/> <span data-ttu-id="dd4d9-127">O uso deste elemento exclui o uso dos elementos [EndDateRecurrence](enddaterecurrence.md) e [NumberedRecurrence](numberedrecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="dd4d9-127">The use of this element excludes the use of the [EndDateRecurrence](enddaterecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="dd4d9-128">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="dd4d9-128">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="dd4d9-129">Descreve a data de início e a data final do padrão de recorrência de um item.</span><span class="sxs-lookup"><span data-stu-id="dd4d9-129">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> <span data-ttu-id="dd4d9-130">O uso deste elemento exclui o uso dos elementos [NoEndRecurrence](noendrecurrence.md) e [NumberedRecurrence](numberedrecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="dd4d9-130">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="dd4d9-131">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="dd4d9-131">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="dd4d9-132">Descreve a data de início e o número de ocorrências de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="dd4d9-132">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> <span data-ttu-id="dd4d9-133">O uso deste elemento exclui o uso dos elementos [NoEndRecurrence](noendrecurrence.md) e [EndDateRecurrence](enddaterecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="dd4d9-133">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [EndDateRecurrence](enddaterecurrence.md) elements.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dd4d9-134">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="dd4d9-134">Parent elements</span></span>

|<span data-ttu-id="dd4d9-135">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dd4d9-135">**Element**</span></span>|<span data-ttu-id="dd4d9-136">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dd4d9-136">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd4d9-137">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="dd4d9-137">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="dd4d9-138">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="dd4d9-138">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="dd4d9-139">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="dd4d9-139">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="dd4d9-140">Representa uma solicitação de reunião no armazenamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="dd4d9-140">Represents a meeting request in the Exchange store</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dd4d9-141">Comentários</span><span class="sxs-lookup"><span data-stu-id="dd4d9-141">Remarks</span></span>

<span data-ttu-id="dd4d9-142">Esse elemento é válido se [CalendarItemType](calendaritemtype.md) tem o valor de RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="dd4d9-142">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="dd4d9-143">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="dd4d9-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dd4d9-144">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="dd4d9-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dd4d9-145">Namespace</span><span class="sxs-lookup"><span data-stu-id="dd4d9-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dd4d9-146">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="dd4d9-146">Schema name</span></span>  <br/> |<span data-ttu-id="dd4d9-147">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="dd4d9-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="dd4d9-148">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="dd4d9-148">Validation file</span></span>  <br/> |<span data-ttu-id="dd4d9-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dd4d9-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dd4d9-150">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="dd4d9-150">Can be empty</span></span>  <br/> |<span data-ttu-id="dd4d9-151">False</span><span class="sxs-lookup"><span data-stu-id="dd4d9-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dd4d9-152">Ver também</span><span class="sxs-lookup"><span data-stu-id="dd4d9-152">See also</span></span>

- [<span data-ttu-id="dd4d9-153">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="dd4d9-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

