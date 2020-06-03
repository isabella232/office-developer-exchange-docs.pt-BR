---
title: RelativeMonthlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RelativeMonthlyRecurrence
api_type:
- schema
ms.assetid: a76595db-7460-44ac-ac2a-53241caa33a7
description: O elemento RelativeMonthlyRecurrence descreve um padrão relativo de recorrência mensal.
ms.openlocfilehash: 90aa0e43684bfb09a3e13cf86ec96f680e80a714
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457505"
---
# <a name="relativemonthlyrecurrence"></a><span data-ttu-id="027d7-103">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="027d7-103">RelativeMonthlyRecurrence</span></span>

<span data-ttu-id="027d7-104">O elemento **RelativeMonthlyRecurrence** descreve um padrão relativo de recorrência mensal.</span><span class="sxs-lookup"><span data-stu-id="027d7-104">The **RelativeMonthlyRecurrence** element describes a relative monthly recurrence pattern.</span></span> 
  
```xml
<RelativeMonthlyRecurrence>
   <Interval/>
   <DaysOfWeek/>
   <DayOfWeekIndex/>
</RelativeMonthlyRecurrence>
```

 <span data-ttu-id="027d7-105">**RelativeMonthlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="027d7-105">**RelativeMonthlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="027d7-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="027d7-106">Attributes and elements</span></span>

<span data-ttu-id="027d7-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="027d7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="027d7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="027d7-108">Attributes</span></span>

<span data-ttu-id="027d7-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="027d7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="027d7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="027d7-110">Child elements</span></span>

|<span data-ttu-id="027d7-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="027d7-111">**Element**</span></span>|<span data-ttu-id="027d7-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="027d7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="027d7-113">Intervalo</span><span class="sxs-lookup"><span data-stu-id="027d7-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="027d7-114">Define o intervalo entre dois itens padrão consecutivos de padrão recorrentes.</span><span class="sxs-lookup"><span data-stu-id="027d7-114">Defines the interval between two consecutive monthly recurring pattern items.</span></span> <span data-ttu-id="027d7-115">O intervalo desse valor é de 1 a 99.</span><span class="sxs-lookup"><span data-stu-id="027d7-115">The range for this value is 1 to 99.</span></span>  <br/> |
|[<span data-ttu-id="027d7-116">DaysOfWeek (DayOfWeektype)</span><span class="sxs-lookup"><span data-stu-id="027d7-116">DaysOfWeek (DayOfWeekType)</span></span>](daysofweek-dayofweektype.md) <br/> |<span data-ttu-id="027d7-117">Descreve quais dias da semana estão no padrão de recorrência mensal relativo.</span><span class="sxs-lookup"><span data-stu-id="027d7-117">Describes which days of the week are in the relative monthly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="027d7-118">DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="027d7-118">DayOfWeekIndex</span></span>](dayofweekindex.md) <br/> |<span data-ttu-id="027d7-119">Descreve qual semana é usada em um padrão relativo de recorrência mensal.</span><span class="sxs-lookup"><span data-stu-id="027d7-119">Describes which week is used in a relative monthly recurrence pattern.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="027d7-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="027d7-120">Parent elements</span></span>

|<span data-ttu-id="027d7-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="027d7-121">**Element**</span></span>|<span data-ttu-id="027d7-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="027d7-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="027d7-123">Recurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="027d7-123">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="027d7-124">Contém o padrão de recorrência para itens de calendário e solicitações de reunião.</span><span class="sxs-lookup"><span data-stu-id="027d7-124">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="027d7-125">Recorrência (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="027d7-125">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="027d7-126">Contém informações de recorrência para tarefas recorrentes.</span><span class="sxs-lookup"><span data-stu-id="027d7-126">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="027d7-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="027d7-127">Remarks</span></span>

<span data-ttu-id="027d7-128">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="027d7-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="027d7-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="027d7-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="027d7-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="027d7-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="027d7-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="027d7-131">Schema Name</span></span>  <br/> |<span data-ttu-id="027d7-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="027d7-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="027d7-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="027d7-133">Validation File</span></span>  <br/> |<span data-ttu-id="027d7-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="027d7-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="027d7-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="027d7-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="027d7-136">False</span><span class="sxs-lookup"><span data-stu-id="027d7-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="027d7-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="027d7-137">See also</span></span>



- [<span data-ttu-id="027d7-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="027d7-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

