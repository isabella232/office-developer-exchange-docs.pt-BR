---
title: Recorrência (TaskRecurrenceType)
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
ms.assetid: 99f8414a-9110-4721-a6e5-ebf225d7ed0a
description: O elemento de recorrência contém informações de recorrência de tarefas recorrentes.
ms.openlocfilehash: ae2bb35e89a0a50c7ca67cb0e580427150afb99e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825006"
---
# <a name="recurrence-taskrecurrencetype"></a><span data-ttu-id="a5a64-103">Recorrência (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="a5a64-103">Recurrence (TaskRecurrenceType)</span></span>

<span data-ttu-id="a5a64-104">O elemento de **Recorrência** contém informações de recorrência de tarefas recorrentes.</span><span class="sxs-lookup"><span data-stu-id="a5a64-104">The **Recurrence** element contains recurrence information for recurring tasks.</span></span> 
  
```xml
<Recurrence>
      <RelativeYearlyRecurrence/>
      <NoEndRecurrence/>
</Recurrence>
```

 <span data-ttu-id="a5a64-105">**TaskRecurrenceType**</span><span class="sxs-lookup"><span data-stu-id="a5a64-105">**TaskRecurrenceType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a5a64-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a5a64-106">Attributes and elements</span></span>

<span data-ttu-id="a5a64-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a5a64-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a5a64-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a5a64-108">Attributes</span></span>

<span data-ttu-id="a5a64-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a5a64-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a5a64-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a5a64-110">Child elements</span></span>

|<span data-ttu-id="a5a64-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a5a64-111">**Element**</span></span>|<span data-ttu-id="a5a64-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a5a64-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5a64-113">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="a5a64-113">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="a5a64-114">Descreve um padrão de recorrência anual relativa de uma tarefa recorrente.</span><span class="sxs-lookup"><span data-stu-id="a5a64-114">Describes a relative yearly recurrence pattern for a recurring task.</span></span>  <br/> |
|[<span data-ttu-id="a5a64-115">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="a5a64-115">AbsoluteYearlyRecurrence</span></span>](absoluteyearlyrecurrence.md) <br/> |<span data-ttu-id="a5a64-116">Representa um padrão de recorrência anual de uma tarefa recorrente.</span><span class="sxs-lookup"><span data-stu-id="a5a64-116">Represents a yearly recurrence pattern for a recurring task.</span></span>  <br/> |
|[<span data-ttu-id="a5a64-117">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="a5a64-117">RelativeMonthlyRecurrence</span></span>](relativemonthlyrecurrence.md) <br/> |<span data-ttu-id="a5a64-118">Descreve um padrão de recorrência mensal relativa de uma tarefa recorrente.</span><span class="sxs-lookup"><span data-stu-id="a5a64-118">Describes a relative monthly recurrence pattern for a recurring task.</span></span>  <br/> |
|[<span data-ttu-id="a5a64-119">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="a5a64-119">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="a5a64-120">Representa um padrão de recorrência mensal para uma tarefa recorrente.</span><span class="sxs-lookup"><span data-stu-id="a5a64-120">Represents a monthly recurrence pattern for a recurring task.</span></span>  <br/> |
|[<span data-ttu-id="a5a64-121">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="a5a64-121">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="a5a64-122">Descreve a frequência, em semanas e os dias em que é uma tarefa recorrente.</span><span class="sxs-lookup"><span data-stu-id="a5a64-122">Describes the frequency, in weeks, and the days on which a task recurs.</span></span>  <br/> |
|[<span data-ttu-id="a5a64-123">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="a5a64-123">DailyRecurrence</span></span>](dailyrecurrence.md) <br/> |<span data-ttu-id="a5a64-124">Descreve a frequência, em dias, em que é uma tarefa recorrente.</span><span class="sxs-lookup"><span data-stu-id="a5a64-124">Describes the frequency, in days, in which a task recurs.</span></span>  <br/> |
|[<span data-ttu-id="a5a64-125">DailyRegeneration</span><span class="sxs-lookup"><span data-stu-id="a5a64-125">DailyRegeneration</span></span>](dailyregeneration.md) <br/> |<span data-ttu-id="a5a64-126">Descreve o número de dias após a conclusão da tarefa a próxima ocorrência atual será vencimento.</span><span class="sxs-lookup"><span data-stu-id="a5a64-126">Describes how many days after the completion of the current task the next occurrence will be due.</span></span>  <br/> |
|[<span data-ttu-id="a5a64-127">WeeklyRegeneration</span><span class="sxs-lookup"><span data-stu-id="a5a64-127">WeeklyRegeneration</span></span>](weeklyregeneration.md) <br/> |<span data-ttu-id="a5a64-128">Descreve quantos semanas após a conclusão da tarefa a próxima ocorrência atual será vencimento.</span><span class="sxs-lookup"><span data-stu-id="a5a64-128">Describes how many weeks after the completion of the current task the next occurrence will be due.</span></span>  <br/> |
|[<span data-ttu-id="a5a64-129">MonthlyRegeneration</span><span class="sxs-lookup"><span data-stu-id="a5a64-129">MonthlyRegeneration</span></span>](monthlyregeneration.md) <br/> |<span data-ttu-id="a5a64-130">Descreve quantos meses após a conclusão da tarefa a próxima ocorrência atual será vencimento.</span><span class="sxs-lookup"><span data-stu-id="a5a64-130">Describes how many months after the completion of the current task the next occurrence will be due.</span></span>  <br/> |
|[<span data-ttu-id="a5a64-131">YearlyRegeneration</span><span class="sxs-lookup"><span data-stu-id="a5a64-131">YearlyRegeneration</span></span>](yearlyregeneration.md) <br/> |<span data-ttu-id="a5a64-132">Descreve quantos anos após a conclusão da tarefa a próxima ocorrência atual será vencimento.</span><span class="sxs-lookup"><span data-stu-id="a5a64-132">Describes how many years after the completion of the current task the next occurrence will be due.</span></span>  <br/> |
|[<span data-ttu-id="a5a64-133">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="a5a64-133">NoEndRecurrence</span></span>](noendrecurrence.md) <br/> |<span data-ttu-id="a5a64-134">Descreve um padrão de recorrência que não tem uma data de término definidas.</span><span class="sxs-lookup"><span data-stu-id="a5a64-134">Describes a recurrence pattern that does not have a defined end date.</span></span>  <br/> <span data-ttu-id="a5a64-135">O uso deste elemento exclui o uso dos elementos [EndDateRecurrence](enddaterecurrence.md) e [NumberedRecurrence](numberedrecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="a5a64-135">The use of this element excludes the use of the [EndDateRecurrence](enddaterecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="a5a64-136">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="a5a64-136">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="a5a64-137">Descreve a data de início e a data final do padrão de recorrência de um item.</span><span class="sxs-lookup"><span data-stu-id="a5a64-137">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> <span data-ttu-id="a5a64-138">O uso deste elemento exclui o uso dos elementos [NoEndRecurrence](noendrecurrence.md) e [NumberedRecurrence](numberedrecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="a5a64-138">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> <span data-ttu-id="a5a64-139">[EndDateRecurrence](enddaterecurrence.md) não pode ser usado em conjunto com um padrão de regeneração.</span><span class="sxs-lookup"><span data-stu-id="a5a64-139">[EndDateRecurrence](enddaterecurrence.md) cannot be used together with a regeneration pattern.</span></span>  <br/> |
|[<span data-ttu-id="a5a64-140">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="a5a64-140">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="a5a64-141">Descreve a data de início e o número de ocorrências de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="a5a64-141">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> <span data-ttu-id="a5a64-142">O uso deste elemento exclui o uso dos elementos [NoEndRecurrence](noendrecurrence.md) e [EndDateRecurrence](enddaterecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="a5a64-142">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [EndDateRecurrence](enddaterecurrence.md) elements.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a5a64-143">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a5a64-143">Parent elements</span></span>

|<span data-ttu-id="a5a64-144">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a5a64-144">**Element**</span></span>|<span data-ttu-id="a5a64-145">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a5a64-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5a64-146">Task</span><span class="sxs-lookup"><span data-stu-id="a5a64-146">Task</span></span>](task.md) <br/> |<span data-ttu-id="a5a64-147">Representa uma tarefa no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a5a64-147">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a5a64-148">Comentários</span><span class="sxs-lookup"><span data-stu-id="a5a64-148">Remarks</span></span>

<span data-ttu-id="a5a64-149">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="a5a64-149">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a5a64-150">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a5a64-150">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a5a64-151">Namespace</span><span class="sxs-lookup"><span data-stu-id="a5a64-151">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a5a64-152">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a5a64-152">Schema name</span></span>  <br/> |<span data-ttu-id="a5a64-153">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a5a64-153">Types schema</span></span>  <br/> |
|<span data-ttu-id="a5a64-154">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a5a64-154">Validation file</span></span>  <br/> |<span data-ttu-id="a5a64-155">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a5a64-155">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a5a64-156">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="a5a64-156">Can be empty</span></span>  <br/> |<span data-ttu-id="a5a64-157">False</span><span class="sxs-lookup"><span data-stu-id="a5a64-157">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a5a64-158">Ver também</span><span class="sxs-lookup"><span data-stu-id="a5a64-158">See also</span></span>



- [<span data-ttu-id="a5a64-159">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a5a64-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

