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
description: O elemento RecurringDateTransition representa uma transição de fuso horário que ocorre em uma data específica por ano.
ms.openlocfilehash: 2acbd3afb50a92d4e4f3d7b552eecb36fe59be8b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461573"
---
# <a name="recurringdatetransition"></a><span data-ttu-id="87d76-103">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="87d76-103">RecurringDateTransition</span></span>

<span data-ttu-id="87d76-104">O elemento **RecurringDateTransition** representa uma transição de fuso horário que ocorre em uma data específica por ano.</span><span class="sxs-lookup"><span data-stu-id="87d76-104">The **RecurringDateTransition** element represents a time zone transition that occurs on a specific date each year.</span></span> 
  
```xml
<RecurringDateTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <Day/>
</RecurringDateTransition>
```

 <span data-ttu-id="87d76-105">**RecurringDateTransitionType**</span><span class="sxs-lookup"><span data-stu-id="87d76-105">**RecurringDateTransitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="87d76-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="87d76-106">Attributes and elements</span></span>

<span data-ttu-id="87d76-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="87d76-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="87d76-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="87d76-108">Attributes</span></span>

<span data-ttu-id="87d76-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="87d76-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="87d76-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="87d76-110">Child elements</span></span>

|<span data-ttu-id="87d76-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="87d76-111">**Element**</span></span>|<span data-ttu-id="87d76-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="87d76-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="87d76-113">To</span><span class="sxs-lookup"><span data-stu-id="87d76-113">To</span></span>](to.md) <br/> |<span data-ttu-id="87d76-114">Especifica o [período](period.md) ou [TransitionsGroup](transitionsgroup.md) que é o destino da transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="87d76-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="87d76-115">Timeoffset</span><span class="sxs-lookup"><span data-stu-id="87d76-115">TimeOffset</span></span>](timeoffset.md) <br/> |<span data-ttu-id="87d76-116">Representa a diferença de duração do tempo universal coordenado (UTC) para a transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="87d76-116">Represents the duration offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="87d76-117">Month (transição de fuso horário)</span><span class="sxs-lookup"><span data-stu-id="87d76-117">Month (Time Zone Transition)</span></span>](month-time-zone-transition.md) <br/> |<span data-ttu-id="87d76-118">Representa o mês em que ocorre a transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="87d76-118">Represents the month in which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="87d76-119">Day</span><span class="sxs-lookup"><span data-stu-id="87d76-119">Day</span></span>](day.md) <br/> |<span data-ttu-id="87d76-120">Representa o dia do mês em que ocorre a transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="87d76-120">Represents the day of the month on which the time zone transition occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="87d76-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="87d76-121">Parent elements</span></span>

|<span data-ttu-id="87d76-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="87d76-122">**Element**</span></span>|<span data-ttu-id="87d76-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="87d76-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="87d76-124">Transições</span><span class="sxs-lookup"><span data-stu-id="87d76-124">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="87d76-125">Representa uma coleção de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="87d76-125">Represents a collection of time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="87d76-126">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="87d76-126">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="87d76-127">Representa uma coleção de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="87d76-127">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="87d76-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="87d76-128">Remarks</span></span>

<span data-ttu-id="87d76-129">Um exemplo de uma transição de fuso horário que pode ser representada pelo elemento [RecurringDateTransition](recurringdatetransition.md) é uma transição que ocorre em 15 de março a cada ano.</span><span class="sxs-lookup"><span data-stu-id="87d76-129">An example of a time zone transition that could be represented by the [RecurringDateTransition](recurringdatetransition.md) element is a transition that occurs on March 15 each year.</span></span> 
  
<span data-ttu-id="87d76-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="87d76-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="87d76-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="87d76-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="87d76-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="87d76-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="87d76-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="87d76-133">Schema Name</span></span>  <br/> |<span data-ttu-id="87d76-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="87d76-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="87d76-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="87d76-135">Validation File</span></span>  <br/> |<span data-ttu-id="87d76-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="87d76-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="87d76-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="87d76-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="87d76-138">False</span><span class="sxs-lookup"><span data-stu-id="87d76-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="87d76-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="87d76-139">See also</span></span>



- [<span data-ttu-id="87d76-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="87d76-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

