---
title: TransitionsGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TransitionsGroup
api_type:
- schema
ms.assetid: 19d56080-546a-4d53-929e-363d56186759
description: O elemento TransitionsGroup representa uma matriz de transições de fuso horário.
ms.openlocfilehash: 9f08dec048d410dadab9580e7886b2499d943176
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467414"
---
# <a name="transitionsgroup"></a><span data-ttu-id="ef6a8-103">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="ef6a8-103">TransitionsGroup</span></span>

<span data-ttu-id="ef6a8-104">O elemento **TransitionsGroup** representa uma matriz de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="ef6a8-104">The **TransitionsGroup** element represents an array of time zone transitions.</span></span> 
  
```xml
<TransitionsGroup Id="">
   <AbsoluteDateTransition/>
   <RecurringDayTransition/>
   <RecurringDateTransition/>
</TransitionsGroup>
```

 <span data-ttu-id="ef6a8-105">**ArrayOfTransitionsType**</span><span class="sxs-lookup"><span data-stu-id="ef6a8-105">**ArrayOfTransitionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ef6a8-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ef6a8-106">Attributes and elements</span></span>

<span data-ttu-id="ef6a8-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ef6a8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ef6a8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ef6a8-108">Attributes</span></span>

|<span data-ttu-id="ef6a8-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="ef6a8-109">**Attribute**</span></span>|<span data-ttu-id="ef6a8-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ef6a8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ef6a8-111">Id</span><span class="sxs-lookup"><span data-stu-id="ef6a8-111">Id</span></span>  <br/> |<span data-ttu-id="ef6a8-112">Um valor String que representa o identificador exclusivo do grupo de transições.</span><span class="sxs-lookup"><span data-stu-id="ef6a8-112">A string value that represents the unique identifier of the transitions group.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ef6a8-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ef6a8-113">Child elements</span></span>

|<span data-ttu-id="ef6a8-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ef6a8-114">**Element**</span></span>|<span data-ttu-id="ef6a8-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ef6a8-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ef6a8-116">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="ef6a8-116">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="ef6a8-117">Representa uma transição de fuso horário que ocorre em uma data específica e em uma hora específica.</span><span class="sxs-lookup"><span data-stu-id="ef6a8-117">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="ef6a8-118">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="ef6a8-118">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="ef6a8-119">Representa uma transição de fuso horário que ocorre no mesmo dia a cada ano.</span><span class="sxs-lookup"><span data-stu-id="ef6a8-119">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="ef6a8-120">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="ef6a8-120">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="ef6a8-121">Representa uma transição de fuso horário que ocorre em um dia do ano especificado.</span><span class="sxs-lookup"><span data-stu-id="ef6a8-121">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ef6a8-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ef6a8-122">Parent elements</span></span>

|<span data-ttu-id="ef6a8-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ef6a8-123">**Element**</span></span>|<span data-ttu-id="ef6a8-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ef6a8-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ef6a8-125">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="ef6a8-125">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="ef6a8-126">Representa uma matriz de grupos de transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="ef6a8-126">Represents an array of time zone transition groups.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ef6a8-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="ef6a8-127">Remarks</span></span>

<span data-ttu-id="ef6a8-128">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="ef6a8-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ef6a8-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ef6a8-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ef6a8-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="ef6a8-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ef6a8-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ef6a8-131">Schema Name</span></span>  <br/> |<span data-ttu-id="ef6a8-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ef6a8-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="ef6a8-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ef6a8-133">Validation File</span></span>  <br/> |<span data-ttu-id="ef6a8-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ef6a8-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ef6a8-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ef6a8-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="ef6a8-136">False</span><span class="sxs-lookup"><span data-stu-id="ef6a8-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ef6a8-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="ef6a8-137">See also</span></span>



- [<span data-ttu-id="ef6a8-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ef6a8-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

