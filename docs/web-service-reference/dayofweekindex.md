---
title: DayOfWeekIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfWeekIndex
api_type:
- schema
ms.assetid: 82420338-a1f7-4887-b338-b2d93b2c2bf1
description: O elemento DayOfWeekIndex descreve qual semana em um mês é usada em um padrão de recorrência relativa.
ms.openlocfilehash: 4987685d0c3cefdfad4f5be1368776a5b859bf94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751709"
---
# <a name="dayofweekindex"></a><span data-ttu-id="24a67-103">DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="24a67-103">DayOfWeekIndex</span></span>

<span data-ttu-id="24a67-104">O elemento **DayOfWeekIndex** descreve qual semana em um mês é usada em um padrão de recorrência relativa.</span><span class="sxs-lookup"><span data-stu-id="24a67-104">The **DayOfWeekIndex** element describes which week in a month is used in a relative recurrence pattern.</span></span> 
  
```xml
<DayOfWeekIndex/>
```

<span data-ttu-id="24a67-105">**DayOfWeekIndexType**</span><span class="sxs-lookup"><span data-stu-id="24a67-105">**DayOfWeekIndexType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="24a67-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="24a67-106">Attributes and elements</span></span>

<span data-ttu-id="24a67-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="24a67-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="24a67-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="24a67-108">Attributes</span></span>

<span data-ttu-id="24a67-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="24a67-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="24a67-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="24a67-110">Child elements</span></span>

<span data-ttu-id="24a67-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="24a67-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="24a67-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="24a67-112">Parent elements</span></span>

|<span data-ttu-id="24a67-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="24a67-113">**Element**</span></span>|<span data-ttu-id="24a67-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="24a67-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24a67-115">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="24a67-115">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="24a67-116">Descreve um padrão de recorrência anual relativa.</span><span class="sxs-lookup"><span data-stu-id="24a67-116">Describes a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="24a67-117">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="24a67-117">RelativeMonthlyRecurrence</span></span>](relativemonthlyrecurrence.md) <br/> |<span data-ttu-id="24a67-118">Descreve um padrão de recorrência mensal relativa.</span><span class="sxs-lookup"><span data-stu-id="24a67-118">Describes a relative monthly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="24a67-119">Text value</span><span class="sxs-lookup"><span data-stu-id="24a67-119">Text value</span></span>

<span data-ttu-id="24a67-120">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="24a67-120">A text value is required.</span></span> <span data-ttu-id="24a67-121">Veja a seguir os valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="24a67-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="24a67-122">Primeira</span><span class="sxs-lookup"><span data-stu-id="24a67-122">First</span></span>    
- <span data-ttu-id="24a67-123">Segunda</span><span class="sxs-lookup"><span data-stu-id="24a67-123">Second</span></span>    
- <span data-ttu-id="24a67-124">Terceira</span><span class="sxs-lookup"><span data-stu-id="24a67-124">Third</span></span>    
- <span data-ttu-id="24a67-125">Quarto</span><span class="sxs-lookup"><span data-stu-id="24a67-125">Fourth</span></span>    
- <span data-ttu-id="24a67-126">Last</span><span class="sxs-lookup"><span data-stu-id="24a67-126">Last</span></span>
    
## <a name="remarks"></a><span data-ttu-id="24a67-127">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="24a67-127">Remarks</span></span>

<span data-ttu-id="24a67-128">Por exemplo, a segunda segunda-feira de um mês pode ocorrer na terceira semana do mês.</span><span class="sxs-lookup"><span data-stu-id="24a67-128">For example, the second Monday of a month may occur in the third week of that month.</span></span> <span data-ttu-id="24a67-129">Se um mês inicia em uma sexta-feira, a primeira semana do mês contém alguns dias apenas e não contém segunda-feira.</span><span class="sxs-lookup"><span data-stu-id="24a67-129">If a month starts on a Friday, the first week of the month only contains a few days and does not contain a Monday.</span></span> <span data-ttu-id="24a67-130">Portanto, a primeira segunda-feira teria ocorrer na segunda semana.</span><span class="sxs-lookup"><span data-stu-id="24a67-130">Therefore, the first Monday would have to occur in the second week.</span></span>
  
<span data-ttu-id="24a67-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="24a67-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="24a67-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="24a67-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="24a67-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="24a67-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="24a67-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="24a67-134">Schema name</span></span>  <br/> |<span data-ttu-id="24a67-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="24a67-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="24a67-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="24a67-136">Validation file</span></span>  <br/> |<span data-ttu-id="24a67-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="24a67-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="24a67-138">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="24a67-138">Can be empty</span></span>  <br/> |<span data-ttu-id="24a67-139">False</span><span class="sxs-lookup"><span data-stu-id="24a67-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="24a67-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="24a67-140">See also</span></span>

- [<span data-ttu-id="24a67-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="24a67-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

