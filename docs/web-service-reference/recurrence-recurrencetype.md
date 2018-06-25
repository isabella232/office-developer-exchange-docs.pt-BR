---
title: Recorrência (RecurrenceType)
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
ms.openlocfilehash: f26ccf5912848a6d7fbbfa7d0a19d41635c896e0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825004"
---
# <a name="recurrence-recurrencetype"></a><span data-ttu-id="670ed-103">Recorrência (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="670ed-103">Recurrence (RecurrenceType)</span></span>

<span data-ttu-id="670ed-104">O elemento de **Recorrência** contém o padrão de recorrência para itens de calendário e solicitações de reunião.</span><span class="sxs-lookup"><span data-stu-id="670ed-104">The **Recurrence** element contains the recurrence pattern for calendar items and meeting requests.</span></span> 
  
```xml
<Recurrence>
      <RelativeYearlyRecurrence/>
      <NoEndRecurrence/>
</Recurrence>
```

 <span data-ttu-id="670ed-105">**RecurrenceType**</span><span class="sxs-lookup"><span data-stu-id="670ed-105">**RecurrenceType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="670ed-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="670ed-106">Attributes and elements</span></span>

<span data-ttu-id="670ed-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="670ed-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="670ed-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="670ed-108">Attributes</span></span>

<span data-ttu-id="670ed-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="670ed-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="670ed-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="670ed-110">Child elements</span></span>

|<span data-ttu-id="670ed-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="670ed-111">**Element**</span></span>|<span data-ttu-id="670ed-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="670ed-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="670ed-113">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="670ed-113">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="670ed-114">Descreve um padrão de recorrência anual relativa.</span><span class="sxs-lookup"><span data-stu-id="670ed-114">Describes a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="670ed-115">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="670ed-115">AbsoluteYearlyRecurrence</span></span>](absoluteyearlyrecurrence.md) <br/> |<span data-ttu-id="670ed-116">Representa um padrão de recorrência anual.</span><span class="sxs-lookup"><span data-stu-id="670ed-116">Represents a yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="670ed-117">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="670ed-117">RelativeMonthlyRecurrence</span></span>](relativemonthlyrecurrence.md) <br/> |<span data-ttu-id="670ed-118">Descreve um padrão de recorrência mensal relativa para um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="670ed-118">Describes a relative monthly recurrence pattern for a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="670ed-119">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="670ed-119">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="670ed-120">Representa um padrão de recorrência mensal.</span><span class="sxs-lookup"><span data-stu-id="670ed-120">Represents a monthly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="670ed-121">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="670ed-121">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="670ed-122">Descreve a frequência, em semanas e os dias em um item de calendário ou uma tarefa recorrente.</span><span class="sxs-lookup"><span data-stu-id="670ed-122">Describes the frequency, in weeks, and the days that a calendar item or task recurs.</span></span>  <br/> |
|[<span data-ttu-id="670ed-123">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="670ed-123">DailyRecurrence</span></span>](dailyrecurrence.md) <br/> |<span data-ttu-id="670ed-124">Descreve a frequência, em dias, no qual um item de calendário ou uma tarefa recorrente.</span><span class="sxs-lookup"><span data-stu-id="670ed-124">Describes the frequency, in days, in which a calendar item or task recurs.</span></span>  <br/> |
|[<span data-ttu-id="670ed-125">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="670ed-125">NoEndRecurrence</span></span>](noendrecurrence.md) <br/> |<span data-ttu-id="670ed-126">Descreve um padrão de recorrência que não tem uma data de término definidas.</span><span class="sxs-lookup"><span data-stu-id="670ed-126">Describes a recurrence pattern that does not have a defined end date.</span></span>  <br/> <span data-ttu-id="670ed-127">O uso deste elemento exclui o uso dos elementos [EndDateRecurrence](enddaterecurrence.md) e [NumberedRecurrence](numberedrecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="670ed-127">The use of this element excludes the use of the [EndDateRecurrence](enddaterecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="670ed-128">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="670ed-128">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="670ed-129">Descreve a data de início e a data final do padrão de recorrência de um item.</span><span class="sxs-lookup"><span data-stu-id="670ed-129">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> <span data-ttu-id="670ed-130">O uso deste elemento exclui o uso dos elementos [NoEndRecurrence](noendrecurrence.md) e [NumberedRecurrence](numberedrecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="670ed-130">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="670ed-131">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="670ed-131">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="670ed-132">Descreve a data de início e o número de ocorrências de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="670ed-132">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> <span data-ttu-id="670ed-133">O uso deste elemento exclui o uso dos elementos [NoEndRecurrence](noendrecurrence.md) e [EndDateRecurrence](enddaterecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="670ed-133">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [EndDateRecurrence](enddaterecurrence.md) elements.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="670ed-134">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="670ed-134">Parent elements</span></span>

|<span data-ttu-id="670ed-135">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="670ed-135">**Element**</span></span>|<span data-ttu-id="670ed-136">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="670ed-136">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="670ed-137">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="670ed-137">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="670ed-138">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="670ed-138">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="670ed-139">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="670ed-139">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="670ed-140">Representa uma solicitação de reunião no armazenamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="670ed-140">Represents a meeting request in the Exchange store</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="670ed-141">Comentários</span><span class="sxs-lookup"><span data-stu-id="670ed-141">Remarks</span></span>

<span data-ttu-id="670ed-142">Esse elemento é válido se [CalendarItemType](calendaritemtype.md) tem o valor de RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="670ed-142">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="670ed-143">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="670ed-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="670ed-144">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="670ed-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="670ed-145">Namespace</span><span class="sxs-lookup"><span data-stu-id="670ed-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="670ed-146">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="670ed-146">Schema name</span></span>  <br/> |<span data-ttu-id="670ed-147">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="670ed-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="670ed-148">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="670ed-148">Validation file</span></span>  <br/> |<span data-ttu-id="670ed-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="670ed-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="670ed-150">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="670ed-150">Can be empty</span></span>  <br/> |<span data-ttu-id="670ed-151">False</span><span class="sxs-lookup"><span data-stu-id="670ed-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="670ed-152">Ver também</span><span class="sxs-lookup"><span data-stu-id="670ed-152">See also</span></span>



- [<span data-ttu-id="670ed-153">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="670ed-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

