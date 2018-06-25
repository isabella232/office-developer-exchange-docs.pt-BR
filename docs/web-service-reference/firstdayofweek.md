---
title: Primeiro_dia_semana
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FirstDayOfWeek
api_type:
- schema
ms.assetid: d6cf1bd3-a19b-4d5f-9e25-8e337a4939e0
description: O elemento Primeiro_dia_semana Especifica o primeiro dia da semana.
ms.openlocfilehash: 99858d17213d077ce7c51ad1c746588f2f3939a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752312"
---
# <a name="firstdayofweek"></a><span data-ttu-id="275e3-103">Primeiro_dia_semana</span><span class="sxs-lookup"><span data-stu-id="275e3-103">FirstDayOfWeek</span></span>

<span data-ttu-id="275e3-104">O elemento **Primeiro_dia_semana** Especifica o primeiro dia da semana.</span><span class="sxs-lookup"><span data-stu-id="275e3-104">The **FirstDayOfWeek** element specifies the first day of the week.</span></span> 
  
```XML
<FirstDayOfWeek> Sunday | Monday | Tuesday | Wednesday | Thursday | Friday | Saturday</FirstDayOfWeek>
```

 <span data-ttu-id="275e3-105">**DayOfWeekType**</span><span class="sxs-lookup"><span data-stu-id="275e3-105">**DayOfWeekType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="275e3-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="275e3-106">Attributes and elements</span></span>

<span data-ttu-id="275e3-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="275e3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="275e3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="275e3-108">Attributes</span></span>

<span data-ttu-id="275e3-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="275e3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="275e3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="275e3-110">Child elements</span></span>

<span data-ttu-id="275e3-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="275e3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="275e3-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="275e3-112">Parent elements</span></span>

|<span data-ttu-id="275e3-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="275e3-113">**Element**</span></span>|<span data-ttu-id="275e3-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="275e3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="275e3-115">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="275e3-115">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="275e3-116">Descreve um padrão de recorrência semanal.</span><span class="sxs-lookup"><span data-stu-id="275e3-116">Describes a weekly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="275e3-117">Text value</span><span class="sxs-lookup"><span data-stu-id="275e3-117">Text value</span></span>

<span data-ttu-id="275e3-118">O valor de texto do elemento **Primeiro_dia_semana** indica qual dia da semana é usado como o primeiro dia da semana.</span><span class="sxs-lookup"><span data-stu-id="275e3-118">The text value of the **FirstDayOfWeek** element indicates which day of the week is used as the first day of the week.</span></span> <span data-ttu-id="275e3-119">Estes são os valores de texto possíveis:</span><span class="sxs-lookup"><span data-stu-id="275e3-119">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="275e3-120">Domingo</span><span class="sxs-lookup"><span data-stu-id="275e3-120">Sunday</span></span>
    
- <span data-ttu-id="275e3-121">Segunda-feira</span><span class="sxs-lookup"><span data-stu-id="275e3-121">Monday</span></span>
    
- <span data-ttu-id="275e3-122">Terça-feira</span><span class="sxs-lookup"><span data-stu-id="275e3-122">Tuesday</span></span>
    
- <span data-ttu-id="275e3-123">Quarta-feira</span><span class="sxs-lookup"><span data-stu-id="275e3-123">Wednesday</span></span>
    
- <span data-ttu-id="275e3-124">Quinta-feira</span><span class="sxs-lookup"><span data-stu-id="275e3-124">Thursday</span></span>
    
- <span data-ttu-id="275e3-125">Sexta-feira</span><span class="sxs-lookup"><span data-stu-id="275e3-125">Friday</span></span>
    
- <span data-ttu-id="275e3-126">Sábado</span><span class="sxs-lookup"><span data-stu-id="275e3-126">Saturday</span></span>
    
## <a name="remarks"></a><span data-ttu-id="275e3-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="275e3-127">Remarks</span></span>

<span data-ttu-id="275e3-128">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="275e3-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="275e3-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="275e3-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="275e3-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="275e3-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="275e3-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="275e3-131">Schema Name</span></span>  <br/> |<span data-ttu-id="275e3-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="275e3-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="275e3-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="275e3-133">Validation File</span></span>  <br/> |<span data-ttu-id="275e3-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="275e3-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="275e3-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="275e3-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="275e3-136">False</span><span class="sxs-lookup"><span data-stu-id="275e3-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="275e3-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="275e3-137">See also</span></span>



- [<span data-ttu-id="275e3-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="275e3-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

