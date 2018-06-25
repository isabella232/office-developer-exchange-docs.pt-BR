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
description: O elemento DayOfMonth descreve o dia de um mês em que ocorre um item recorrente.
ms.openlocfilehash: 0d0d95849a2562e06b88872b2857cc5e6ca67af3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751700"
---
# <a name="dayofmonth"></a><span data-ttu-id="91d7d-103">DayOfMonth</span><span class="sxs-lookup"><span data-stu-id="91d7d-103">DayOfMonth</span></span>

<span data-ttu-id="91d7d-104">O elemento **DayOfMonth** descreve o dia de um mês em que ocorre um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="91d7d-104">The **DayOfMonth** element describes the day in a month that a recurring item occurs.</span></span> 
  
```xml
<DayOfMonth/>
```

<span data-ttu-id="91d7d-105">**int**</span><span class="sxs-lookup"><span data-stu-id="91d7d-105">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="91d7d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="91d7d-106">Attributes and elements</span></span>

<span data-ttu-id="91d7d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="91d7d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="91d7d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="91d7d-108">Attributes</span></span>

<span data-ttu-id="91d7d-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="91d7d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="91d7d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="91d7d-110">Child elements</span></span>

<span data-ttu-id="91d7d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="91d7d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="91d7d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="91d7d-112">Parent elements</span></span>

|<span data-ttu-id="91d7d-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="91d7d-113">**Element**</span></span>|<span data-ttu-id="91d7d-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="91d7d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="91d7d-115">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="91d7d-115">AbsoluteYearlyRecurrence</span></span>](absoluteyearlyrecurrence.md) <br/> |<span data-ttu-id="91d7d-116">Representa um padrão de recorrência anual.</span><span class="sxs-lookup"><span data-stu-id="91d7d-116">Represents a yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="91d7d-117">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="91d7d-117">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="91d7d-118">Representa um padrão de recorrência mensal.</span><span class="sxs-lookup"><span data-stu-id="91d7d-118">Represents a monthly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="91d7d-119">Text value</span><span class="sxs-lookup"><span data-stu-id="91d7d-119">Text value</span></span>

<span data-ttu-id="91d7d-120">Um valor de texto que representa um inteiro no intervalo de 1 a 31 é necessário.</span><span class="sxs-lookup"><span data-stu-id="91d7d-120">A text value that represents an integer in the range of 1 to 31 is required.</span></span> <span data-ttu-id="91d7d-121">Se um determinado mês esse valor for maior que o número de dias no mês, o último dia do mês é assumido.</span><span class="sxs-lookup"><span data-stu-id="91d7d-121">If for a particular month this value is larger than the number of days in the month, the last day of the month is assumed.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="91d7d-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="91d7d-122">Remarks</span></span>

<span data-ttu-id="91d7d-123">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="91d7d-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="91d7d-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="91d7d-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="91d7d-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="91d7d-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="91d7d-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="91d7d-126">Schema name</span></span>  <br/> |<span data-ttu-id="91d7d-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="91d7d-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="91d7d-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="91d7d-128">Validation file</span></span>  <br/> |<span data-ttu-id="91d7d-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="91d7d-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="91d7d-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="91d7d-130">Can be empty</span></span>  <br/> |<span data-ttu-id="91d7d-131">False</span><span class="sxs-lookup"><span data-stu-id="91d7d-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="91d7d-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="91d7d-132">See also</span></span>

- [<span data-ttu-id="91d7d-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="91d7d-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

