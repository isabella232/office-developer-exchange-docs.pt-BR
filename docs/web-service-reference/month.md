---
title: Mês
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Month
api_type:
- schema
ms.assetid: b12ac64f-b230-4573-be05-c86a428c4965
description: O elemento de mês representa o mês de transição do ano para e de período padrão e o horário de verão.
ms.openlocfilehash: 73d052ef16bc51cd574eb8b04e21546f97347258
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824476"
---
# <a name="month"></a><span data-ttu-id="dd1de-103">Mês</span><span class="sxs-lookup"><span data-stu-id="dd1de-103">Month</span></span>

<span data-ttu-id="dd1de-104">O elemento de **mês** representa o mês de transição do ano para e de período padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="dd1de-104">The **Month** element represents the transition month of the year to and from standard time and daylight saving time.</span></span> 
  
```xml
<Month>...</Month>
```

 <span data-ttu-id="dd1de-105">**Curto**</span><span class="sxs-lookup"><span data-stu-id="dd1de-105">**Short**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dd1de-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="dd1de-106">Attributes and elements</span></span>

<span data-ttu-id="dd1de-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="dd1de-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd1de-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="dd1de-108">Attributes</span></span>

<span data-ttu-id="dd1de-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="dd1de-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dd1de-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="dd1de-110">Child elements</span></span>

<span data-ttu-id="dd1de-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="dd1de-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dd1de-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="dd1de-112">Parent elements</span></span>

|<span data-ttu-id="dd1de-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dd1de-113">**Element**</span></span>|<span data-ttu-id="dd1de-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dd1de-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd1de-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="dd1de-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="dd1de-116">Representa um deslocamento, desde o momento em relação ao tempo Universal Coordenado (UTC) representado pelo elemento [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="dd1de-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="dd1de-117">Horário de verão em regiões onde o horário de verão é observado, esse elemento também contém informações sobre a transição para a hora padrão.</span><span class="sxs-lookup"><span data-stu-id="dd1de-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span> <br/> <br/>  <span data-ttu-id="dd1de-118">A seguir estão as expressões XPath ao elemento [StandardTime](standardtime.md) :</span><span class="sxs-lookup"><span data-stu-id="dd1de-118">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="dd1de-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="dd1de-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="dd1de-120">Representa um deslocamento, desde o momento em relação ao UTC representado pelo [Bias (UTC)](bias-utc.md) elemento em regiões onde o horário de verão é observado.</span><span class="sxs-lookup"><span data-stu-id="dd1de-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="dd1de-121">Esse elemento também contém informações sobre como ocorre a transição do horário de verão do período padrão.</span><span class="sxs-lookup"><span data-stu-id="dd1de-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/><br/>  <span data-ttu-id="dd1de-122">A seguir estão as expressões XPath ao elemento [DaylightTime](daylighttime.md) :</span><span class="sxs-lookup"><span data-stu-id="dd1de-122">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span>  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dd1de-123">Text value</span><span class="sxs-lookup"><span data-stu-id="dd1de-123">Text value</span></span>

<span data-ttu-id="dd1de-124">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="dd1de-124">A text value is required.</span></span> <span data-ttu-id="dd1de-125">O valor representa a posição ordinal do mês pela ocorrência e deve ser um número entre 1 e 12.</span><span class="sxs-lookup"><span data-stu-id="dd1de-125">The value represents the ordinal rank of the month by occurrence and must be a number between 1 and 12.</span></span> <span data-ttu-id="dd1de-126">Este é um tipo de dados de inteiro curto.</span><span class="sxs-lookup"><span data-stu-id="dd1de-126">This is a short integer data type.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dd1de-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="dd1de-127">Remarks</span></span>

<span data-ttu-id="dd1de-128">Um elemento de [StandardTime](standardtime.md) que contém um elemento [DayOrder](dayorder.md) que tem um valor de 5, um elemento de **mês** que possui um valor de 10 e um elemento de [DayOfWeek (TimeZone)](dayofweek-timezone.md) que tem um valor de domingo significa que a transição da hora padrão para Horário de verão ocorre no domingo do mês décimo quinto.</span><span class="sxs-lookup"><span data-stu-id="dd1de-128">A [StandardTime](standardtime.md) element that contains a [DayOrder](dayorder.md) element that has a value of 5, a **Month** element that has a value of 10, and a [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that has a value of Sunday means that the transition from standard time to daylight saving time occurs on the fifth Sunday of the tenth month.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="dd1de-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="dd1de-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dd1de-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="dd1de-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dd1de-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="dd1de-131">Schema Name</span></span>  <br/> |<span data-ttu-id="dd1de-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="dd1de-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="dd1de-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="dd1de-133">Validation File</span></span>  <br/> |<span data-ttu-id="dd1de-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dd1de-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dd1de-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="dd1de-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="dd1de-136">False</span><span class="sxs-lookup"><span data-stu-id="dd1de-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dd1de-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="dd1de-137">See also</span></span>

- [<span data-ttu-id="dd1de-138">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="dd1de-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="dd1de-139">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="dd1de-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

