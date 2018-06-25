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
description: O elemento RelativeMonthlyRecurrence descreve um padrão de recorrência mensal relativa.
ms.openlocfilehash: 9b695052c38e2693946837bf99f03baea093df08
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825053"
---
# <a name="relativemonthlyrecurrence"></a><span data-ttu-id="d9cb0-103">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="d9cb0-103">RelativeMonthlyRecurrence</span></span>

<span data-ttu-id="d9cb0-104">O elemento **RelativeMonthlyRecurrence** descreve um padrão de recorrência mensal relativa.</span><span class="sxs-lookup"><span data-stu-id="d9cb0-104">The **RelativeMonthlyRecurrence** element describes a relative monthly recurrence pattern.</span></span> 
  
```xml
<RelativeMonthlyRecurrence>
   <Interval/>
   <DaysOfWeek/>
   <DayOfWeekIndex/>
</RelativeMonthlyRecurrence>
```

 <span data-ttu-id="d9cb0-105">**RelativeMonthlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="d9cb0-105">**RelativeMonthlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d9cb0-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d9cb0-106">Attributes and elements</span></span>

<span data-ttu-id="d9cb0-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d9cb0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d9cb0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d9cb0-108">Attributes</span></span>

<span data-ttu-id="d9cb0-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d9cb0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d9cb0-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d9cb0-110">Child elements</span></span>

|<span data-ttu-id="d9cb0-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d9cb0-111">**Element**</span></span>|<span data-ttu-id="d9cb0-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d9cb0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9cb0-113">Intervalo</span><span class="sxs-lookup"><span data-stu-id="d9cb0-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="d9cb0-114">Define o intervalo entre dois itens padrão recorrente de mensal consecutivos.</span><span class="sxs-lookup"><span data-stu-id="d9cb0-114">Defines the interval between two consecutive monthly recurring pattern items.</span></span> <span data-ttu-id="d9cb0-115">O intervalo para esse valor é de 1 a 99.</span><span class="sxs-lookup"><span data-stu-id="d9cb0-115">The range for this value is 1 to 99.</span></span>  <br/> |
|[<span data-ttu-id="d9cb0-116">DaysOfWeek (DayOfWeekType)</span><span class="sxs-lookup"><span data-stu-id="d9cb0-116">DaysOfWeek (DayOfWeekType)</span></span>](daysofweek-dayofweektype.md) <br/> |<span data-ttu-id="d9cb0-117">Descreve quais dias da semana em que o padrão de recorrência mensal relativa.</span><span class="sxs-lookup"><span data-stu-id="d9cb0-117">Describes which days of the week are in the relative monthly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="d9cb0-118">DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="d9cb0-118">DayOfWeekIndex</span></span>](dayofweekindex.md) <br/> |<span data-ttu-id="d9cb0-119">Descreve qual semana é usada em um padrão de recorrência mensal relativa.</span><span class="sxs-lookup"><span data-stu-id="d9cb0-119">Describes which week is used in a relative monthly recurrence pattern.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d9cb0-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d9cb0-120">Parent elements</span></span>

|<span data-ttu-id="d9cb0-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d9cb0-121">**Element**</span></span>|<span data-ttu-id="d9cb0-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d9cb0-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9cb0-123">Recorrência (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="d9cb0-123">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="d9cb0-124">Contém o padrão de recorrência para itens de calendário e solicitações de reunião.</span><span class="sxs-lookup"><span data-stu-id="d9cb0-124">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="d9cb0-125">Recorrência (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="d9cb0-125">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="d9cb0-126">Contém informações de recorrência de tarefas recorrentes.</span><span class="sxs-lookup"><span data-stu-id="d9cb0-126">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d9cb0-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="d9cb0-127">Remarks</span></span>

<span data-ttu-id="d9cb0-128">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="d9cb0-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d9cb0-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d9cb0-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d9cb0-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="d9cb0-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d9cb0-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d9cb0-131">Schema Name</span></span>  <br/> |<span data-ttu-id="d9cb0-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d9cb0-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="d9cb0-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d9cb0-133">Validation File</span></span>  <br/> |<span data-ttu-id="d9cb0-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d9cb0-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d9cb0-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d9cb0-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="d9cb0-136">False</span><span class="sxs-lookup"><span data-stu-id="d9cb0-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d9cb0-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="d9cb0-137">See also</span></span>



- [<span data-ttu-id="d9cb0-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d9cb0-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

