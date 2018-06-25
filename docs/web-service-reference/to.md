---
title: Para
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
description: O elemento To Especifica o destino da transição fuso horário. O destino é um período de fuso horário ou um grupo de transições de fuso horário.
ms.openlocfilehash: dc7df8ed3ddd6a9b4222ffab4c2b47b00ee4ba0c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837754"
---
# <a name="to"></a><span data-ttu-id="41725-104">Para</span><span class="sxs-lookup"><span data-stu-id="41725-104">To</span></span>

<span data-ttu-id="41725-105">Elemento **To** Especifica o destino da transição fuso horário.</span><span class="sxs-lookup"><span data-stu-id="41725-105">The **To** element specifies the target of the time zone transition.</span></span> <span data-ttu-id="41725-106">O destino é um período de fuso horário ou um grupo de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="41725-106">The target is either a time zone period or a group of time zone transitions.</span></span> 
  
```xml
<To Kind=""/>
```

 <span data-ttu-id="41725-107">**TransitionTargetType**</span><span class="sxs-lookup"><span data-stu-id="41725-107">**TransitionTargetType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="41725-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="41725-108">Attributes and elements</span></span>

<span data-ttu-id="41725-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="41725-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="41725-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="41725-110">Attributes</span></span>

|<span data-ttu-id="41725-111">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="41725-111">**Attribute**</span></span>|<span data-ttu-id="41725-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="41725-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="41725-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="41725-113">Kind</span></span>  <br/> |<span data-ttu-id="41725-114">Indica se o destino de transição do fuso horário é um período de fuso horário ou de um grupo de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="41725-114">Indicates whether the time zone transition target is a time zone period or of a group of time zone transitions.</span></span>  <br/> |
   
#### <a name="kind-attribute-values"></a><span data-ttu-id="41725-115">Valores de atributo Kind</span><span class="sxs-lookup"><span data-stu-id="41725-115">Kind attribute values</span></span>

|<span data-ttu-id="41725-116">**Valor**</span><span class="sxs-lookup"><span data-stu-id="41725-116">**Value**</span></span>|<span data-ttu-id="41725-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="41725-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="41725-118">Ponto</span><span class="sxs-lookup"><span data-stu-id="41725-118">Period</span></span>  <br/> |<span data-ttu-id="41725-119">Especifica que o destino de transição do fuso horário é um período de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="41725-119">Specifies that the time zone transition target is a time zone period.</span></span>  <br/> |
|<span data-ttu-id="41725-120">Group</span><span class="sxs-lookup"><span data-stu-id="41725-120">Group</span></span>  <br/> |<span data-ttu-id="41725-121">Especifica que a meta de transição do fuso horário é um grupo de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="41725-121">Specifies that the time zone transition target is a group of time zone transitions.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="41725-122">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="41725-122">Child elements</span></span>

<span data-ttu-id="41725-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="41725-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="41725-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="41725-124">Parent elements</span></span>

|<span data-ttu-id="41725-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="41725-125">**Element**</span></span>|<span data-ttu-id="41725-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="41725-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41725-127">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="41725-127">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="41725-128">Representa uma transição de fuso horário que ocorre em uma data específica e, em um momento específico.</span><span class="sxs-lookup"><span data-stu-id="41725-128">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="41725-129">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="41725-129">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="41725-130">Representa uma transição de fuso horário que ocorre no mesmo dia cada ano.</span><span class="sxs-lookup"><span data-stu-id="41725-130">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="41725-131">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="41725-131">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="41725-132">Representa uma transição de fuso horário que ocorre em um dia especificado do ano.</span><span class="sxs-lookup"><span data-stu-id="41725-132">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
|[<span data-ttu-id="41725-133">Transição</span><span class="sxs-lookup"><span data-stu-id="41725-133">Transition</span></span>](transition.md) <br/> |<span data-ttu-id="41725-134">Representa uma transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="41725-134">Represents a time zone transition.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="41725-135">Text value</span><span class="sxs-lookup"><span data-stu-id="41725-135">Text value</span></span>

<span data-ttu-id="41725-136">O valor de texto é uma cadeia de caracteres que especifica o identificador exclusivo do [período](period.md) ou [TransitionsGroup](transitionsgroup.md) que é o destino da transição fuso horário.</span><span class="sxs-lookup"><span data-stu-id="41725-136">The text value is a string that specifies the unique identifier of the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="41725-137">Comentários</span><span class="sxs-lookup"><span data-stu-id="41725-137">Remarks</span></span>

<span data-ttu-id="41725-138">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="41725-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="41725-139">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="41725-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="41725-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="41725-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="41725-141">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="41725-141">Schema Name</span></span>  <br/> |<span data-ttu-id="41725-142">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="41725-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="41725-143">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="41725-143">Validation File</span></span>  <br/> |<span data-ttu-id="41725-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="41725-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="41725-145">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="41725-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="41725-146">False</span><span class="sxs-lookup"><span data-stu-id="41725-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="41725-147">Ver também</span><span class="sxs-lookup"><span data-stu-id="41725-147">See also</span></span>



- [<span data-ttu-id="41725-148">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="41725-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

