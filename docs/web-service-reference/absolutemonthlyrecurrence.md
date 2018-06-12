---
title: AbsoluteMonthlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AbsoluteMonthlyRecurrence
api_type:
- schema
ms.assetid: 178fa0ae-9dfc-417f-933c-d657d31c2161
description: O elemento AbsoluteMonthlyRecurrence representa um padrão de recorrência mensal.
ms.openlocfilehash: f4613fa71a9164c45b60a82f675959817cd4bdd5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752183"
---
# <a name="absolutemonthlyrecurrence"></a><span data-ttu-id="3875c-103">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="3875c-103">AbsoluteMonthlyRecurrence</span></span>

<span data-ttu-id="3875c-104">O elemento **AbsoluteMonthlyRecurrence** representa um padrão de recorrência mensal.</span><span class="sxs-lookup"><span data-stu-id="3875c-104">The **AbsoluteMonthlyRecurrence** element represents a monthly recurrence pattern.</span></span> 
  
```xml
<AbsoluteMonthlyRecurrence>
   <Interval/>
   <DayOfMonth/>
</AbsoluteMonthlyRecurrence>
```

 <span data-ttu-id="3875c-105">**AbsoluteMonthlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="3875c-105">**AbsoluteMonthlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3875c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3875c-106">Attributes and elements</span></span>

<span data-ttu-id="3875c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3875c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3875c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3875c-108">Attributes</span></span>

<span data-ttu-id="3875c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3875c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3875c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3875c-110">Child elements</span></span>

|<span data-ttu-id="3875c-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3875c-111">**Element**</span></span>|<span data-ttu-id="3875c-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3875c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3875c-113">DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="3875c-113">DayOfMonth</span></span>](dayofmonth.md) <br/> |<span data-ttu-id="3875c-114">Descreve o dia de um mês em que ocorre um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="3875c-114">Describes the day in a month that a recurring item occurs.</span></span> <span data-ttu-id="3875c-115">O intervalo de valores para essa propriedade é de 1 a 31.</span><span class="sxs-lookup"><span data-stu-id="3875c-115">The range of values for this property is 1 to 31.</span></span> <span data-ttu-id="3875c-116">Se um determinado mês esse valor for maior que o número de dias no mês, o último dia do mês, será adotado para essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="3875c-116">If for a particular month this value is larger than the number of days in the month, the last day of the month is assumed for this property.</span></span>  <br/> |
|[<span data-ttu-id="3875c-117">Intervalo</span><span class="sxs-lookup"><span data-stu-id="3875c-117">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="3875c-118">Define o intervalo entre dois itens recorrentes consecutivos.</span><span class="sxs-lookup"><span data-stu-id="3875c-118">Defines the interval between two consecutive recurring items.</span></span> <span data-ttu-id="3875c-119">Por exemplo, se o elemento de **intervalo** tem um valor de 5, o item recorrente ocorre a cada 5 meses.</span><span class="sxs-lookup"><span data-stu-id="3875c-119">For example, if the **Interval** element has a value of 5, the recurring item occurs every 5 months.</span></span> <span data-ttu-id="3875c-120">O intervalo de valores válidos é de 1 a 99.</span><span class="sxs-lookup"><span data-stu-id="3875c-120">The range of valid values is from 1 to 99.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3875c-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3875c-121">Parent elements</span></span>

|<span data-ttu-id="3875c-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3875c-122">**Element**</span></span>|<span data-ttu-id="3875c-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3875c-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3875c-124">Recorrência (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="3875c-124">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="3875c-125">Contém informações de recorrência de tarefas recorrentes.</span><span class="sxs-lookup"><span data-stu-id="3875c-125">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="3875c-126">Recorrência (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="3875c-126">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="3875c-127">Contém o padrão de recorrência para itens de calendário e solicitações de reunião.</span><span class="sxs-lookup"><span data-stu-id="3875c-127">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3875c-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="3875c-128">Remarks</span></span>

<span data-ttu-id="3875c-129">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="3875c-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3875c-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3875c-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3875c-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="3875c-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3875c-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3875c-132">Schema Name</span></span>  <br/> |<span data-ttu-id="3875c-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3875c-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="3875c-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3875c-134">Validation File</span></span>  <br/> |<span data-ttu-id="3875c-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3875c-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3875c-136">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="3875c-136">Can Be Empty</span></span>  <br/> |<span data-ttu-id="3875c-137">False</span><span class="sxs-lookup"><span data-stu-id="3875c-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3875c-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="3875c-138">See also</span></span>

- [<span data-ttu-id="3875c-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3875c-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

