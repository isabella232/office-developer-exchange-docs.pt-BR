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
ms.openlocfilehash: 19b617dfd5c0a3d206d62439c880da084fd5f5f0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460411"
---
# <a name="absoluteyearlyrecurrence"></a><span data-ttu-id="b98cb-103">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="b98cb-103">AbsoluteYearlyRecurrence</span></span>

<span data-ttu-id="b98cb-104">O elemento **AbsoluteYearlyRecurrence** representa um padrão de recorrência anual.</span><span class="sxs-lookup"><span data-stu-id="b98cb-104">The **AbsoluteYearlyRecurrence** element represents a yearly recurrence pattern.</span></span> 
  
```xml
<AbsoluteYearlyRecurrence>
   <DayOfMonth/>
   <Month/>
</AbsoluteYearlyRecurrence>
```

 <span data-ttu-id="b98cb-105">**AbsoluteYearlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="b98cb-105">**AbsoluteYearlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b98cb-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b98cb-106">Attributes and elements</span></span>

<span data-ttu-id="b98cb-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b98cb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b98cb-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b98cb-108">Attributes</span></span>

<span data-ttu-id="b98cb-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b98cb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b98cb-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b98cb-110">Child elements</span></span>

|<span data-ttu-id="b98cb-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b98cb-111">**Element**</span></span>|<span data-ttu-id="b98cb-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b98cb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b98cb-113">DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="b98cb-113">DayOfMonth</span></span>](dayofmonth.md) <br/> |<span data-ttu-id="b98cb-114">Descreve o dia em um mês em que ocorre um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="b98cb-114">Describes the day in a month on which a recurring item occurs.</span></span> <span data-ttu-id="b98cb-115">O intervalo de valores para essa propriedade é de 1 a 31.</span><span class="sxs-lookup"><span data-stu-id="b98cb-115">The range of values for this property is 1 to 31.</span></span> <span data-ttu-id="b98cb-116">Se for um mês específico, esse valor será maior do que o número de dias no mês, o último dia do mês será assumido para essa propriedade.</span><span class="sxs-lookup"><span data-stu-id="b98cb-116">If for a particular month this value is larger than the number of days in the month, the last day of the month is assumed for this property.</span></span>  <br/> |
|[<span data-ttu-id="b98cb-117">Mês (recorrência do item)</span><span class="sxs-lookup"><span data-stu-id="b98cb-117">Month (Item Recurrence)</span></span>](month-item-recurrence.md) <br/> |<span data-ttu-id="b98cb-118">Descreve o mês em que ocorre um item recorrente anual.</span><span class="sxs-lookup"><span data-stu-id="b98cb-118">Describes the month in which a yearly recurring item occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b98cb-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b98cb-119">Parent elements</span></span>

|<span data-ttu-id="b98cb-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b98cb-120">**Element**</span></span>|<span data-ttu-id="b98cb-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b98cb-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b98cb-122">Recorrência (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="b98cb-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="b98cb-123">Contém informações de recorrência para tarefas recorrentes.</span><span class="sxs-lookup"><span data-stu-id="b98cb-123">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="b98cb-124">Recurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="b98cb-124">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="b98cb-125">Contém o padrão de recorrência para itens de calendário e solicitações de reunião.</span><span class="sxs-lookup"><span data-stu-id="b98cb-125">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b98cb-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="b98cb-126">Remarks</span></span>

<span data-ttu-id="b98cb-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="b98cb-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b98cb-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b98cb-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b98cb-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="b98cb-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b98cb-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b98cb-130">Schema Name</span></span>  <br/> |<span data-ttu-id="b98cb-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b98cb-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="b98cb-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b98cb-132">Validation File</span></span>  <br/> |<span data-ttu-id="b98cb-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b98cb-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b98cb-134">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b98cb-134">Can Be Empty</span></span>  <br/> |<span data-ttu-id="b98cb-135">False</span><span class="sxs-lookup"><span data-stu-id="b98cb-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b98cb-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="b98cb-136">See also</span></span>

- [<span data-ttu-id="b98cb-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b98cb-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

