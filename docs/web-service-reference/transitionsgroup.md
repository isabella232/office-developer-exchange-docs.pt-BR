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
ms.openlocfilehash: e5991ad7f73a1694e0d4abadd8d252acc04970e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837798"
---
# <a name="transitionsgroup"></a><span data-ttu-id="96a76-103">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="96a76-103">TransitionsGroup</span></span>

<span data-ttu-id="96a76-104">O elemento **TransitionsGroup** representa uma matriz de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="96a76-104">The **TransitionsGroup** element represents an array of time zone transitions.</span></span> 
  
```xml
<TransitionsGroup Id="">
   <AbsoluteDateTransition/>
   <RecurringDayTransition/>
   <RecurringDateTransition/>
</TransitionsGroup>
```

 <span data-ttu-id="96a76-105">**ArrayOfTransitionsType**</span><span class="sxs-lookup"><span data-stu-id="96a76-105">**ArrayOfTransitionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="96a76-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="96a76-106">Attributes and elements</span></span>

<span data-ttu-id="96a76-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="96a76-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96a76-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="96a76-108">Attributes</span></span>

|<span data-ttu-id="96a76-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="96a76-109">**Attribute**</span></span>|<span data-ttu-id="96a76-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="96a76-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="96a76-111">Id</span><span class="sxs-lookup"><span data-stu-id="96a76-111">Id</span></span>  <br/> |<span data-ttu-id="96a76-112">Um valor string que representa o identificador exclusivo do grupo transições.</span><span class="sxs-lookup"><span data-stu-id="96a76-112">A string value that represents the unique identifier of the transitions group.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="96a76-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="96a76-113">Child elements</span></span>

|<span data-ttu-id="96a76-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="96a76-114">**Element**</span></span>|<span data-ttu-id="96a76-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="96a76-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96a76-116">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="96a76-116">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="96a76-117">Representa uma transição de fuso horário que ocorre em uma data específica e, em um momento específico.</span><span class="sxs-lookup"><span data-stu-id="96a76-117">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="96a76-118">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="96a76-118">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="96a76-119">Representa uma transição de fuso horário que ocorre no mesmo dia cada ano.</span><span class="sxs-lookup"><span data-stu-id="96a76-119">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="96a76-120">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="96a76-120">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="96a76-121">Representa uma transição de fuso horário que ocorre em um dia especificado do ano.</span><span class="sxs-lookup"><span data-stu-id="96a76-121">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="96a76-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="96a76-122">Parent elements</span></span>

|<span data-ttu-id="96a76-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="96a76-123">**Element**</span></span>|<span data-ttu-id="96a76-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="96a76-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="96a76-125">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="96a76-125">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="96a76-126">Representa uma matriz dos grupos de transição do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="96a76-126">Represents an array of time zone transition groups.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="96a76-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="96a76-127">Remarks</span></span>

<span data-ttu-id="96a76-128">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="96a76-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="96a76-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="96a76-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96a76-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="96a76-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="96a76-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="96a76-131">Schema Name</span></span>  <br/> |<span data-ttu-id="96a76-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="96a76-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="96a76-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="96a76-133">Validation File</span></span>  <br/> |<span data-ttu-id="96a76-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="96a76-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="96a76-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="96a76-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="96a76-136">False</span><span class="sxs-lookup"><span data-stu-id="96a76-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="96a76-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="96a76-137">See also</span></span>



- [<span data-ttu-id="96a76-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="96a76-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

