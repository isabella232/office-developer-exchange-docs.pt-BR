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
description: O elemento DayOfWeekIndex descreve qual semana em um mês é usada em um padrão de recorrência relativo.
ms.openlocfilehash: c9235d83a944f9c8883439dd2adf190b88977f16
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529207"
---
# <a name="dayofweekindex"></a><span data-ttu-id="2700b-103">DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="2700b-103">DayOfWeekIndex</span></span>

<span data-ttu-id="2700b-104">O elemento **DayOfWeekIndex** descreve qual semana em um mês é usada em um padrão de recorrência relativo.</span><span class="sxs-lookup"><span data-stu-id="2700b-104">The **DayOfWeekIndex** element describes which week in a month is used in a relative recurrence pattern.</span></span> 
  
```xml
<DayOfWeekIndex/>
```

<span data-ttu-id="2700b-105">**DayOfWeekIndexType**</span><span class="sxs-lookup"><span data-stu-id="2700b-105">**DayOfWeekIndexType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2700b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="2700b-106">Attributes and elements</span></span>

<span data-ttu-id="2700b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2700b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2700b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2700b-108">Attributes</span></span>

<span data-ttu-id="2700b-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2700b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2700b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2700b-110">Child elements</span></span>

<span data-ttu-id="2700b-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2700b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2700b-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2700b-112">Parent elements</span></span>

|<span data-ttu-id="2700b-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2700b-113">**Element**</span></span>|<span data-ttu-id="2700b-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2700b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2700b-115">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="2700b-115">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="2700b-116">Descreve um padrão relativo de recorrência anual.</span><span class="sxs-lookup"><span data-stu-id="2700b-116">Describes a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="2700b-117">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="2700b-117">RelativeMonthlyRecurrence</span></span>](relativemonthlyrecurrence.md) <br/> |<span data-ttu-id="2700b-118">Descreve um padrão relativo de recorrência mensal.</span><span class="sxs-lookup"><span data-stu-id="2700b-118">Describes a relative monthly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2700b-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="2700b-119">Text value</span></span>

<span data-ttu-id="2700b-120">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2700b-120">A text value is required.</span></span> <span data-ttu-id="2700b-121">Veja a seguir os valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="2700b-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="2700b-122">Primeiro</span><span class="sxs-lookup"><span data-stu-id="2700b-122">First</span></span>    
- <span data-ttu-id="2700b-123">Segundo</span><span class="sxs-lookup"><span data-stu-id="2700b-123">Second</span></span>    
- <span data-ttu-id="2700b-124">Terceira</span><span class="sxs-lookup"><span data-stu-id="2700b-124">Third</span></span>    
- <span data-ttu-id="2700b-125">Etapa</span><span class="sxs-lookup"><span data-stu-id="2700b-125">Fourth</span></span>    
- <span data-ttu-id="2700b-126">Último</span><span class="sxs-lookup"><span data-stu-id="2700b-126">Last</span></span>
    
## <a name="remarks"></a><span data-ttu-id="2700b-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="2700b-127">Remarks</span></span>

<span data-ttu-id="2700b-128">Por exemplo, a segunda segunda-feira de um mês pode ocorrer na terceira semana desse mês.</span><span class="sxs-lookup"><span data-stu-id="2700b-128">For example, the second Monday of a month may occur in the third week of that month.</span></span> <span data-ttu-id="2700b-129">Se um mês iniciar em uma sexta-feira, a primeira semana do mês conterá apenas alguns dias e não conterá uma segunda-feira.</span><span class="sxs-lookup"><span data-stu-id="2700b-129">If a month starts on a Friday, the first week of the month only contains a few days and does not contain a Monday.</span></span> <span data-ttu-id="2700b-130">Portanto, a primeira segunda-feira deve ocorrer na segunda semana.</span><span class="sxs-lookup"><span data-stu-id="2700b-130">Therefore, the first Monday would have to occur in the second week.</span></span>
  
<span data-ttu-id="2700b-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="2700b-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2700b-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="2700b-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2700b-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="2700b-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2700b-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2700b-134">Schema name</span></span>  <br/> |<span data-ttu-id="2700b-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="2700b-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="2700b-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2700b-136">Validation file</span></span>  <br/> |<span data-ttu-id="2700b-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2700b-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2700b-138">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="2700b-138">Can be empty</span></span>  <br/> |<span data-ttu-id="2700b-139">False</span><span class="sxs-lookup"><span data-stu-id="2700b-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2700b-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="2700b-140">See also</span></span>

- [<span data-ttu-id="2700b-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2700b-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

