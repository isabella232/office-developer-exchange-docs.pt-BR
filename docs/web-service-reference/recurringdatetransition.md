---
title: RecurringDateTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurringDateTransition
api_type:
- schema
ms.assetid: 52fe1e05-3c50-40a1-8752-5c3c64c9f1ed
description: O elemento RecurringDateTransition representa uma transição de fuso horário que ocorre em uma data específica de cada ano.
ms.openlocfilehash: 7cd8f3452a744e0c9a98fd3698dffb9ed8721a6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825014"
---
# <a name="recurringdatetransition"></a><span data-ttu-id="51907-103">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="51907-103">RecurringDateTransition</span></span>

<span data-ttu-id="51907-104">O elemento **RecurringDateTransition** representa uma transição de fuso horário que ocorre em uma data específica de cada ano.</span><span class="sxs-lookup"><span data-stu-id="51907-104">The **RecurringDateTransition** element represents a time zone transition that occurs on a specific date each year.</span></span> 
  
```xml
<RecurringDateTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <Day/>
</RecurringDateTransition>
```

 <span data-ttu-id="51907-105">**RecurringDateTransitionType**</span><span class="sxs-lookup"><span data-stu-id="51907-105">**RecurringDateTransitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="51907-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="51907-106">Attributes and elements</span></span>

<span data-ttu-id="51907-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="51907-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="51907-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="51907-108">Attributes</span></span>

<span data-ttu-id="51907-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="51907-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="51907-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="51907-110">Child elements</span></span>

|<span data-ttu-id="51907-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="51907-111">**Element**</span></span>|<span data-ttu-id="51907-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="51907-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="51907-113">To</span><span class="sxs-lookup"><span data-stu-id="51907-113">To</span></span>](to.md) <br/> |<span data-ttu-id="51907-114">Especifica o [período](period.md) ou [TransitionsGroup](transitionsgroup.md) que é o destino da transição fuso horário.</span><span class="sxs-lookup"><span data-stu-id="51907-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="51907-115">TimeOffset</span><span class="sxs-lookup"><span data-stu-id="51907-115">TimeOffset</span></span>](timeoffset.md) <br/> |<span data-ttu-id="51907-116">Representa o deslocamento de duração do tempo Universal Coordenado (UTC) para a transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="51907-116">Represents the duration offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="51907-117">Mês (transição de fuso horário)</span><span class="sxs-lookup"><span data-stu-id="51907-117">Month (Time Zone Transition)</span></span>](month-time-zone-transition.md) <br/> |<span data-ttu-id="51907-118">Representa o mês em que ocorre a transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="51907-118">Represents the month in which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="51907-119">Dia</span><span class="sxs-lookup"><span data-stu-id="51907-119">Day</span></span>](day.md) <br/> |<span data-ttu-id="51907-120">Representa o dia do mês em que ocorre a transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="51907-120">Represents the day of the month on which the time zone transition occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="51907-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="51907-121">Parent elements</span></span>

|<span data-ttu-id="51907-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="51907-122">**Element**</span></span>|<span data-ttu-id="51907-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="51907-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="51907-124">Transições</span><span class="sxs-lookup"><span data-stu-id="51907-124">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="51907-125">Representa uma coleção de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="51907-125">Represents a collection of time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="51907-126">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="51907-126">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="51907-127">Representa uma coleção de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="51907-127">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="51907-128">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="51907-128">Remarks</span></span>

<span data-ttu-id="51907-129">Um exemplo de uma transição de fuso horário que poderia ser representado pelo elemento [RecurringDateTransition](recurringdatetransition.md) é uma transição que ocorre em 15 de março de cada ano.</span><span class="sxs-lookup"><span data-stu-id="51907-129">An example of a time zone transition that could be represented by the [RecurringDateTransition](recurringdatetransition.md) element is a transition that occurs on March 15 each year.</span></span> 
  
<span data-ttu-id="51907-130">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="51907-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="51907-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="51907-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="51907-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="51907-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="51907-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="51907-133">Schema Name</span></span>  <br/> |<span data-ttu-id="51907-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="51907-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="51907-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="51907-135">Validation File</span></span>  <br/> |<span data-ttu-id="51907-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="51907-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="51907-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="51907-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="51907-138">False</span><span class="sxs-lookup"><span data-stu-id="51907-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="51907-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="51907-139">See also</span></span>



- [<span data-ttu-id="51907-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="51907-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

