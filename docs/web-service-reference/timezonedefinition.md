---
title: TimeZoneDefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZoneDefinition
api_type:
- schema
ms.assetid: b005a80c-addb-4409-beff-e5162076752c
description: O elemento TimeZoneDefinition especifica os períodos e as transições que definem um fuso horário.
ms.openlocfilehash: 58d34556686bfc77244b5829798eada51a1df843
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466063"
---
# <a name="timezonedefinition"></a><span data-ttu-id="e1555-103">TimeZoneDefinition</span><span class="sxs-lookup"><span data-stu-id="e1555-103">TimeZoneDefinition</span></span>

<span data-ttu-id="e1555-104">O elemento **TimeZoneDefinition** especifica os períodos e as transições que definem um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="e1555-104">The **TimeZoneDefinition** element specifies the periods and transitions that define a time zone.</span></span> 
  
```XML
<TimeZoneDefinition Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</TimeZoneDefinition>

```

 <span data-ttu-id="e1555-105">**TimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="e1555-105">**TimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e1555-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e1555-106">Attributes and elements</span></span>

<span data-ttu-id="e1555-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e1555-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e1555-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e1555-108">Attributes</span></span>

|<span data-ttu-id="e1555-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="e1555-109">**Attribute**</span></span>|<span data-ttu-id="e1555-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e1555-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e1555-111">Id</span><span class="sxs-lookup"><span data-stu-id="e1555-111">Id</span></span>  <br/> |<span data-ttu-id="e1555-112">Representa o identificador exclusivo do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="e1555-112">Represents the unique identifier of the time zone.</span></span>  <br/> |
|<span data-ttu-id="e1555-113">Nome</span><span class="sxs-lookup"><span data-stu-id="e1555-113">Name</span></span>  <br/> |<span data-ttu-id="e1555-114">Representa o nome descritivo do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="e1555-114">Represents the descriptive name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e1555-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e1555-115">Child elements</span></span>

|<span data-ttu-id="e1555-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e1555-116">**Element**</span></span>|<span data-ttu-id="e1555-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e1555-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1555-118">Períodos</span><span class="sxs-lookup"><span data-stu-id="e1555-118">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="e1555-119">Representa uma matriz de elementos [period](period.md) que definem a diferença de tempo em diferentes estágios do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="e1555-119">Represents an array of [Period](period.md) elements that define the time offset at different stages of the time zone.</span></span>  <br/> |
|[<span data-ttu-id="e1555-120">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="e1555-120">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="e1555-121">Representa uma matriz de elementos [TransitionsGroup](transitionsgroup.md) que especificam transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="e1555-121">Represents an array of [TransitionsGroup](transitionsgroup.md) elements that specify time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="e1555-122">Transições</span><span class="sxs-lookup"><span data-stu-id="e1555-122">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="e1555-123">Representa uma matriz de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="e1555-123">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e1555-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e1555-124">Parent elements</span></span>

|<span data-ttu-id="e1555-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e1555-125">**Element**</span></span>|<span data-ttu-id="e1555-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e1555-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1555-127">TimeZoneDefinitions</span><span class="sxs-lookup"><span data-stu-id="e1555-127">TimeZoneDefinitions</span></span>](timezonedefinitions.md) <br/> |<span data-ttu-id="e1555-128">Representa uma matriz de definições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="e1555-128">Represents an array of time zone definitions.</span></span>  <br/> |
|[<span data-ttu-id="e1555-129">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="e1555-129">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="e1555-130">Representa a definição de fuso horário padrão que deve ser usada para definir o escopo das propriedades DateTime de objetos que são criados, atualizados e recuperados usando o EWS (serviços Web do Exchange).</span><span class="sxs-lookup"><span data-stu-id="e1555-130">Represents the default time zone definition that is to be used for scoping the DateTime properties of objects that are created, updated, and retrieved by using Exchange Web Services (EWS).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e1555-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="e1555-131">Remarks</span></span>

<span data-ttu-id="e1555-132">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e1555-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e1555-133">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e1555-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e1555-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="e1555-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e1555-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e1555-135">Schema Name</span></span>  <br/> |<span data-ttu-id="e1555-136">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e1555-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="e1555-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e1555-137">Validation File</span></span>  <br/> |<span data-ttu-id="e1555-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e1555-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e1555-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e1555-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="e1555-140">False</span><span class="sxs-lookup"><span data-stu-id="e1555-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e1555-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="e1555-141">See also</span></span>



- [<span data-ttu-id="e1555-142">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e1555-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

