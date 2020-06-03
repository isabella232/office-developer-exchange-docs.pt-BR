---
title: To
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- To
api_type:
- schema
ms.assetid: d14e46da-14bd-4a33-a78e-8ee314d9c1d8
description: O elemento to especifica o destino da transição de fuso horário. O destino é um período de fuso horário ou um grupo de transições de fuso horário.
ms.openlocfilehash: 8cce700eedd64035f2e21be4db6b517f3f85d98d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44468793"
---
# <a name="to"></a><span data-ttu-id="7876e-104">To</span><span class="sxs-lookup"><span data-stu-id="7876e-104">To</span></span>

<span data-ttu-id="7876e-105">O elemento **to** especifica o destino da transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="7876e-105">The **To** element specifies the target of the time zone transition.</span></span> <span data-ttu-id="7876e-106">O destino é um período de fuso horário ou um grupo de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="7876e-106">The target is either a time zone period or a group of time zone transitions.</span></span> 
  
```xml
<To Kind=""/>
```

 <span data-ttu-id="7876e-107">**TransitionTargetType**</span><span class="sxs-lookup"><span data-stu-id="7876e-107">**TransitionTargetType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7876e-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="7876e-108">Attributes and elements</span></span>

<span data-ttu-id="7876e-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7876e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7876e-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="7876e-110">Attributes</span></span>

|<span data-ttu-id="7876e-111">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="7876e-111">**Attribute**</span></span>|<span data-ttu-id="7876e-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7876e-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7876e-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="7876e-113">Kind</span></span>  <br/> |<span data-ttu-id="7876e-114">Indica se o destino de transição de fuso horário é um período de fuso horário ou de um grupo de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="7876e-114">Indicates whether the time zone transition target is a time zone period or of a group of time zone transitions.</span></span>  <br/> |
   
#### <a name="kind-attribute-values"></a><span data-ttu-id="7876e-115">Valores de atributo Kind</span><span class="sxs-lookup"><span data-stu-id="7876e-115">Kind attribute values</span></span>

|<span data-ttu-id="7876e-116">**Valor**</span><span class="sxs-lookup"><span data-stu-id="7876e-116">**Value**</span></span>|<span data-ttu-id="7876e-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7876e-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7876e-118">Período</span><span class="sxs-lookup"><span data-stu-id="7876e-118">Period</span></span>  <br/> |<span data-ttu-id="7876e-119">Especifica que o destino de transição de fuso horário é um período de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="7876e-119">Specifies that the time zone transition target is a time zone period.</span></span>  <br/> |
|<span data-ttu-id="7876e-120">Group</span><span class="sxs-lookup"><span data-stu-id="7876e-120">Group</span></span>  <br/> |<span data-ttu-id="7876e-121">Especifica que o destino de transição de fuso horário é um grupo de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="7876e-121">Specifies that the time zone transition target is a group of time zone transitions.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7876e-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7876e-122">Child elements</span></span>

<span data-ttu-id="7876e-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7876e-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7876e-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7876e-124">Parent elements</span></span>

|<span data-ttu-id="7876e-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7876e-125">**Element**</span></span>|<span data-ttu-id="7876e-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7876e-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7876e-127">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="7876e-127">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="7876e-128">Representa uma transição de fuso horário que ocorre em uma data específica e em uma hora específica.</span><span class="sxs-lookup"><span data-stu-id="7876e-128">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="7876e-129">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="7876e-129">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="7876e-130">Representa uma transição de fuso horário que ocorre no mesmo dia a cada ano.</span><span class="sxs-lookup"><span data-stu-id="7876e-130">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="7876e-131">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="7876e-131">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="7876e-132">Representa uma transição de fuso horário que ocorre em um dia do ano especificado.</span><span class="sxs-lookup"><span data-stu-id="7876e-132">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
|[<span data-ttu-id="7876e-133">Transição</span><span class="sxs-lookup"><span data-stu-id="7876e-133">Transition</span></span>](transition.md) <br/> |<span data-ttu-id="7876e-134">Representa uma transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="7876e-134">Represents a time zone transition.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7876e-135">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="7876e-135">Text value</span></span>

<span data-ttu-id="7876e-136">O valor de texto é uma cadeia de caracteres que especifica o identificador exclusivo do [período](period.md) ou [TransitionsGroup](transitionsgroup.md) que é o destino da transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="7876e-136">The text value is a string that specifies the unique identifier of the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7876e-137">Comentários</span><span class="sxs-lookup"><span data-stu-id="7876e-137">Remarks</span></span>

<span data-ttu-id="7876e-138">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="7876e-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7876e-139">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="7876e-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7876e-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="7876e-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7876e-141">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7876e-141">Schema Name</span></span>  <br/> |<span data-ttu-id="7876e-142">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7876e-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="7876e-143">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7876e-143">Validation File</span></span>  <br/> |<span data-ttu-id="7876e-144">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7876e-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7876e-145">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7876e-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="7876e-146">False</span><span class="sxs-lookup"><span data-stu-id="7876e-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7876e-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="7876e-147">See also</span></span>



- [<span data-ttu-id="7876e-148">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7876e-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

