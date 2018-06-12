---
title: Timezonedefinition pela última vez
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
description: O elemento timezonedefinition pela última vez Especifica os períodos e transições que definem um fuso horário.
ms.openlocfilehash: ffd5ed0c862af794e4aff2387f508849b1d5fd5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837760"
---
# <a name="timezonedefinition"></a><span data-ttu-id="42436-103">Timezonedefinition pela última vez</span><span class="sxs-lookup"><span data-stu-id="42436-103">TimeZoneDefinition</span></span>

<span data-ttu-id="42436-104">O elemento **timezonedefinition pela última vez** Especifica os períodos e transições que definem um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="42436-104">The **TimeZoneDefinition** element specifies the periods and transitions that define a time zone.</span></span> 
  
```XML
<TimeZoneDefinition Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</TimeZoneDefinition>

```

 <span data-ttu-id="42436-105">**TimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="42436-105">**TimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="42436-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="42436-106">Attributes and elements</span></span>

<span data-ttu-id="42436-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="42436-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="42436-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="42436-108">Attributes</span></span>

|<span data-ttu-id="42436-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="42436-109">**Attribute**</span></span>|<span data-ttu-id="42436-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="42436-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="42436-111">Id</span><span class="sxs-lookup"><span data-stu-id="42436-111">Id</span></span>  <br/> |<span data-ttu-id="42436-112">Representa o identificador exclusivo do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="42436-112">Represents the unique identifier of the time zone.</span></span>  <br/> |
|<span data-ttu-id="42436-113">Nome</span><span class="sxs-lookup"><span data-stu-id="42436-113">Name</span></span>  <br/> |<span data-ttu-id="42436-114">Representa o nome descritivo do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="42436-114">Represents the descriptive name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="42436-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="42436-115">Child elements</span></span>

|<span data-ttu-id="42436-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="42436-116">**Element**</span></span>|<span data-ttu-id="42436-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="42436-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="42436-118">Períodos</span><span class="sxs-lookup"><span data-stu-id="42436-118">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="42436-119">Representa uma matriz de elementos do [período](period.md) que definem o deslocamento de tempo em fases diferentes do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="42436-119">Represents an array of [Period](period.md) elements that define the time offset at different stages of the time zone.</span></span>  <br/> |
|[<span data-ttu-id="42436-120">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="42436-120">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="42436-121">Representa uma matriz de elementos de [TransitionsGroup](transitionsgroup.md) que especificam as transições do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="42436-121">Represents an array of [TransitionsGroup](transitionsgroup.md) elements that specify time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="42436-122">Transições</span><span class="sxs-lookup"><span data-stu-id="42436-122">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="42436-123">Representa uma matriz de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="42436-123">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="42436-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="42436-124">Parent elements</span></span>

|<span data-ttu-id="42436-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="42436-125">**Element**</span></span>|<span data-ttu-id="42436-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="42436-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="42436-127">TimeZoneDefinitions</span><span class="sxs-lookup"><span data-stu-id="42436-127">TimeZoneDefinitions</span></span>](timezonedefinitions.md) <br/> |<span data-ttu-id="42436-128">Representa uma matriz de definições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="42436-128">Represents an array of time zone definitions.</span></span>  <br/> |
|[<span data-ttu-id="42436-129">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="42436-129">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="42436-130">Representa a definição de fuso horário padrão que será usado para as propriedades de data/hora dos objetos que são criados, atualizados e recuperadas usando serviços Web do Exchange (EWS) de escopo.</span><span class="sxs-lookup"><span data-stu-id="42436-130">Represents the default time zone definition that is to be used for scoping the DateTime properties of objects that are created, updated, and retrieved by using Exchange Web Services (EWS).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="42436-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="42436-131">Remarks</span></span>

<span data-ttu-id="42436-132">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="42436-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="42436-133">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="42436-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="42436-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="42436-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="42436-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="42436-135">Schema Name</span></span>  <br/> |<span data-ttu-id="42436-136">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="42436-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="42436-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="42436-137">Validation File</span></span>  <br/> |<span data-ttu-id="42436-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="42436-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="42436-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="42436-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="42436-140">False</span><span class="sxs-lookup"><span data-stu-id="42436-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="42436-141">Ver também</span><span class="sxs-lookup"><span data-stu-id="42436-141">See also</span></span>



- [<span data-ttu-id="42436-142">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="42436-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

