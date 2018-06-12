---
title: AbsoluteYearlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AbsoluteYearlyRecurrence
api_type:
- schema
ms.assetid: 96f53e2c-3893-4f6e-a78a-ac179f45c5db
description: O elemento AbsoluteYearlyRecurrence representa um padrão de recorrência anual.
ms.openlocfilehash: 205da336a6a6ca4fd39120e83ab264e1543354e8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752178"
---
# <a name="absoluteyearlyrecurrence"></a><span data-ttu-id="4dd1e-103">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="4dd1e-103">AbsoluteYearlyRecurrence</span></span>

<span data-ttu-id="4dd1e-104">O elemento **AbsoluteYearlyRecurrence** representa um padrão de recorrência anual.</span><span class="sxs-lookup"><span data-stu-id="4dd1e-104">The **AbsoluteYearlyRecurrence** element represents a yearly recurrence pattern.</span></span> 
  
```xml
<AbsoluteYearlyRecurrence>
   <DayOfMonth/>
   <Month/>
</AbsoluteYearlyRecurrence>
```

 <span data-ttu-id="4dd1e-105">**AbsoluteYearlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="4dd1e-105">**AbsoluteYearlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4dd1e-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4dd1e-106">Attributes and elements</span></span>

<span data-ttu-id="4dd1e-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4dd1e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4dd1e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4dd1e-108">Attributes</span></span>

<span data-ttu-id="4dd1e-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4dd1e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4dd1e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4dd1e-110">Child elements</span></span>

|<span data-ttu-id="4dd1e-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4dd1e-111">**Element**</span></span>|<span data-ttu-id="4dd1e-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4dd1e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4dd1e-113">DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="4dd1e-113">DayOfMonth</span></span>](dayofmonth.md) <br/> |<span data-ttu-id="4dd1e-114">Descreve o dia de um mês em que um item recorrente ocorre.</span><span class="sxs-lookup"><span data-stu-id="4dd1e-114">Describes the day in a month on which a recurring item occurs.</span></span> <span data-ttu-id="4dd1e-115">O intervalo de valores para essa propriedade é de 1 a 31.</span><span class="sxs-lookup"><span data-stu-id="4dd1e-115">The range of values for this property is 1 to 31.</span></span> <span data-ttu-id="4dd1e-116">Se um determinado mês esse valor for maior que o número de dias no mês, o último dia do mês, será adotado para essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="4dd1e-116">If for a particular month this value is larger than the number of days in the month, the last day of the month is assumed for this property.</span></span>  <br/> |
|[<span data-ttu-id="4dd1e-117">Mês (recorrência do Item)</span><span class="sxs-lookup"><span data-stu-id="4dd1e-117">Month (Item Recurrence)</span></span>](month-item-recurrence.md) <br/> |<span data-ttu-id="4dd1e-118">Descreve o mês em que um item recorrente anual ocorre.</span><span class="sxs-lookup"><span data-stu-id="4dd1e-118">Describes the month in which a yearly recurring item occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4dd1e-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4dd1e-119">Parent elements</span></span>

|<span data-ttu-id="4dd1e-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4dd1e-120">**Element**</span></span>|<span data-ttu-id="4dd1e-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4dd1e-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4dd1e-122">Recorrência (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="4dd1e-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="4dd1e-123">Contém informações de recorrência de tarefas recorrentes.</span><span class="sxs-lookup"><span data-stu-id="4dd1e-123">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="4dd1e-124">Recorrência (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="4dd1e-124">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="4dd1e-125">Contém o padrão de recorrência para itens de calendário e solicitações de reunião.</span><span class="sxs-lookup"><span data-stu-id="4dd1e-125">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4dd1e-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="4dd1e-126">Remarks</span></span>

<span data-ttu-id="4dd1e-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="4dd1e-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4dd1e-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4dd1e-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4dd1e-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="4dd1e-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4dd1e-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4dd1e-130">Schema Name</span></span>  <br/> |<span data-ttu-id="4dd1e-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="4dd1e-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="4dd1e-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4dd1e-132">Validation File</span></span>  <br/> |<span data-ttu-id="4dd1e-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4dd1e-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4dd1e-134">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="4dd1e-134">Can Be Empty</span></span>  <br/> |<span data-ttu-id="4dd1e-135">False</span><span class="sxs-lookup"><span data-stu-id="4dd1e-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4dd1e-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="4dd1e-136">See also</span></span>

- [<span data-ttu-id="4dd1e-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4dd1e-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

