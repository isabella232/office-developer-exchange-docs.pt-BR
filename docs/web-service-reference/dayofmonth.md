---
title: DayOfMonth
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfMonth
api_type:
- schema
ms.assetid: 09b7504e-08d8-42f9-88cc-a2a37a2e2b8b
description: O elemento DayOfMonth descreve o dia em um mês em que ocorre um item recorrente.
ms.openlocfilehash: dc333a46283d5e8eba3a79f62f8c22c22f56e190
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44442826"
---
# <a name="dayofmonth"></a><span data-ttu-id="99595-103">DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="99595-103">DayOfMonth</span></span>

<span data-ttu-id="99595-104">O elemento **DayOfMonth** descreve o dia em um mês em que ocorre um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="99595-104">The **DayOfMonth** element describes the day in a month that a recurring item occurs.</span></span> 
  
```xml
<DayOfMonth/>
```

<span data-ttu-id="99595-105">**int**</span><span class="sxs-lookup"><span data-stu-id="99595-105">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="99595-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="99595-106">Attributes and elements</span></span>

<span data-ttu-id="99595-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="99595-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="99595-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="99595-108">Attributes</span></span>

<span data-ttu-id="99595-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="99595-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="99595-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="99595-110">Child elements</span></span>

<span data-ttu-id="99595-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="99595-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="99595-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="99595-112">Parent elements</span></span>

|<span data-ttu-id="99595-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="99595-113">**Element**</span></span>|<span data-ttu-id="99595-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="99595-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="99595-115">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="99595-115">AbsoluteYearlyRecurrence</span></span>](absoluteyearlyrecurrence.md) <br/> |<span data-ttu-id="99595-116">Representa um padrão de recorrência anual.</span><span class="sxs-lookup"><span data-stu-id="99595-116">Represents a yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="99595-117">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="99595-117">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="99595-118">Representa um padrão de recorrência mensal.</span><span class="sxs-lookup"><span data-stu-id="99595-118">Represents a monthly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="99595-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="99595-119">Text value</span></span>

<span data-ttu-id="99595-120">Um valor de texto que representa um inteiro no intervalo de 1 a 31 é necessário.</span><span class="sxs-lookup"><span data-stu-id="99595-120">A text value that represents an integer in the range of 1 to 31 is required.</span></span> <span data-ttu-id="99595-121">Se for um mês específico, esse valor será maior do que o número de dias no mês, o último dia do mês será usado.</span><span class="sxs-lookup"><span data-stu-id="99595-121">If for a particular month this value is larger than the number of days in the month, the last day of the month is assumed.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="99595-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="99595-122">Remarks</span></span>

<span data-ttu-id="99595-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="99595-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="99595-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="99595-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="99595-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="99595-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="99595-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="99595-126">Schema name</span></span>  <br/> |<span data-ttu-id="99595-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="99595-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="99595-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="99595-128">Validation file</span></span>  <br/> |<span data-ttu-id="99595-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="99595-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="99595-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="99595-130">Can be empty</span></span>  <br/> |<span data-ttu-id="99595-131">False</span><span class="sxs-lookup"><span data-stu-id="99595-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="99595-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="99595-132">See also</span></span>

- [<span data-ttu-id="99595-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="99595-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

