---
title: RecurringDayTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurringDayTransition
api_type:
- schema
ms.assetid: 1ae28d14-c2b8-4084-9e76-e2e347a884ce
description: O elemento RecurringDayTransition representa uma transição de fuso horário que ocorre no mesmo dia cada ano.
ms.openlocfilehash: 913345188547ce9903809fdc1cbbbe3e20ae7f36
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825012"
---
# <a name="recurringdaytransition"></a><span data-ttu-id="84591-103">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="84591-103">RecurringDayTransition</span></span>

<span data-ttu-id="84591-104">O elemento **RecurringDayTransition** representa uma transição de fuso horário que ocorre no mesmo dia cada ano.</span><span class="sxs-lookup"><span data-stu-id="84591-104">The **RecurringDayTransition** element represents a time zone transition that occurs on the same day each year.</span></span> 
  
```xml
<RecurringDayTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <DayOfWeek/>
   <Occurrence/>
</RecurringDayTransition>
```

 <span data-ttu-id="84591-105">**RecurringDayTransitionType**</span><span class="sxs-lookup"><span data-stu-id="84591-105">**RecurringDayTransitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="84591-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="84591-106">Attributes and elements</span></span>

<span data-ttu-id="84591-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="84591-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="84591-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="84591-108">Attributes</span></span>

<span data-ttu-id="84591-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="84591-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="84591-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="84591-110">Child elements</span></span>

|<span data-ttu-id="84591-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="84591-111">**Element**</span></span>|<span data-ttu-id="84591-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="84591-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="84591-113">To</span><span class="sxs-lookup"><span data-stu-id="84591-113">To</span></span>](to.md) <br/> |<span data-ttu-id="84591-114">Especifica o [período](period.md) ou [TransitionsGroup](transitionsgroup.md) que é o destino da transição fuso horário.</span><span class="sxs-lookup"><span data-stu-id="84591-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="84591-115">TimeOffset</span><span class="sxs-lookup"><span data-stu-id="84591-115">TimeOffset</span></span>](timeoffset.md) <br/> |<span data-ttu-id="84591-116">Representa o deslocamento de duração do tempo Universal Coordenado (UTC) para a transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="84591-116">Represents the duration offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="84591-117">Mês (transição de fuso horário)</span><span class="sxs-lookup"><span data-stu-id="84591-117">Month (Time Zone Transition)</span></span>](month-time-zone-transition.md) <br/> |<span data-ttu-id="84591-118">Representa o mês em que ocorre a transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="84591-118">Represents the month in which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="84591-119">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="84591-119">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="84591-120">Representa o dia da semana em que ocorre a transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="84591-120">Represents the day of the week on which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="84591-121">Ocorrência (transição de fuso horário)</span><span class="sxs-lookup"><span data-stu-id="84591-121">Occurrence (Time Zone Transition)</span></span>](occurrence-time-zone-transition.md) <br/> |<span data-ttu-id="84591-122">Representa a ocorrência do dia da semana do mês em que ocorre a transição do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="84591-122">Represents the occurrence of the day of the week in the month that the time zone transition occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="84591-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="84591-123">Parent elements</span></span>

|<span data-ttu-id="84591-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="84591-124">**Element**</span></span>|<span data-ttu-id="84591-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="84591-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="84591-126">Transições</span><span class="sxs-lookup"><span data-stu-id="84591-126">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="84591-127">Representa uma coleção de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="84591-127">Represents a collection of time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="84591-128">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="84591-128">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="84591-129">Representa uma coleção de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="84591-129">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="84591-130">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="84591-130">Remarks</span></span>

<span data-ttu-id="84591-131">Um exemplo de uma transição de fuso horário que poderia ser representado pelo elemento [RecurringDayTransition](recurringdaytransition.md) é uma transição que ocorre na segunda terça-feira de fevereiro a cada ano.</span><span class="sxs-lookup"><span data-stu-id="84591-131">An example of a time zone transition that could be represented by the [RecurringDayTransition](recurringdaytransition.md) element is a transition that occurs on the second Tuesday of February each year.</span></span> 
  
<span data-ttu-id="84591-132">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="84591-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="84591-133">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="84591-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="84591-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="84591-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="84591-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="84591-135">Schema Name</span></span>  <br/> |<span data-ttu-id="84591-136">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="84591-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="84591-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="84591-137">Validation File</span></span>  <br/> |<span data-ttu-id="84591-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="84591-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="84591-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="84591-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="84591-140">False</span><span class="sxs-lookup"><span data-stu-id="84591-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="84591-141">Ver também</span><span class="sxs-lookup"><span data-stu-id="84591-141">See also</span></span>



- [<span data-ttu-id="84591-142">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="84591-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

