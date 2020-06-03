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
description: O elemento Month representa o mês do ano de transição de e para hora padrão e horário de verão.
ms.openlocfilehash: f102dca4ed9e833b9742844cfd612c81dfd05e70
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468618"
---
# <a name="month"></a><span data-ttu-id="5dd64-103">Mês</span><span class="sxs-lookup"><span data-stu-id="5dd64-103">Month</span></span>

<span data-ttu-id="5dd64-104">O elemento **month** representa o mês do ano de transição de e para hora padrão e horário de verão.</span><span class="sxs-lookup"><span data-stu-id="5dd64-104">The **Month** element represents the transition month of the year to and from standard time and daylight saving time.</span></span> 
  
```xml
<Month>...</Month>
```

 <span data-ttu-id="5dd64-105">**Rápido**</span><span class="sxs-lookup"><span data-stu-id="5dd64-105">**Short**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5dd64-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5dd64-106">Attributes and elements</span></span>

<span data-ttu-id="5dd64-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5dd64-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5dd64-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5dd64-108">Attributes</span></span>

<span data-ttu-id="5dd64-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5dd64-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5dd64-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5dd64-110">Child elements</span></span>

<span data-ttu-id="5dd64-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5dd64-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5dd64-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5dd64-112">Parent elements</span></span>

|<span data-ttu-id="5dd64-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5dd64-113">**Element**</span></span>|<span data-ttu-id="5dd64-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5dd64-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5dd64-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="5dd64-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="5dd64-116">Representa um deslocamento do tempo relativo ao UTC (tempo Universal Coordenado) representado pelo elemento [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="5dd64-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="5dd64-117">Esse elemento também contém informações sobre a transição para o horário padrão do horário de verão nas regiões nas quais o horário de verão é observado.</span><span class="sxs-lookup"><span data-stu-id="5dd64-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span> <br/> <br/>  <span data-ttu-id="5dd64-118">A seguir estão as expressões XPath para o elemento [StandardTime](standardtime.md) :</span><span class="sxs-lookup"><span data-stu-id="5dd64-118">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="5dd64-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="5dd64-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="5dd64-120">Representa um deslocamento do tempo relativo ao UTC representado pelo elemento [Bias (UTC)](bias-utc.md) nas regiões em que o horário de verão é observado.</span><span class="sxs-lookup"><span data-stu-id="5dd64-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="5dd64-121">Esse elemento também contém informações sobre quando ocorre a transição para o horário de Verão do horário padrão.</span><span class="sxs-lookup"><span data-stu-id="5dd64-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/><br/>  <span data-ttu-id="5dd64-122">A seguir estão as expressões XPath para o elemento [DaylightTime](daylighttime.md) :</span><span class="sxs-lookup"><span data-stu-id="5dd64-122">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span>  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5dd64-123">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="5dd64-123">Text value</span></span>

<span data-ttu-id="5dd64-124">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5dd64-124">A text value is required.</span></span> <span data-ttu-id="5dd64-125">O valor representa a classificação ordinal do mês por ocorrência e deve ser um número entre 1 e 12.</span><span class="sxs-lookup"><span data-stu-id="5dd64-125">The value represents the ordinal rank of the month by occurrence and must be a number between 1 and 12.</span></span> <span data-ttu-id="5dd64-126">Este é um tipo de dados inteiro curto.</span><span class="sxs-lookup"><span data-stu-id="5dd64-126">This is a short integer data type.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5dd64-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="5dd64-127">Remarks</span></span>

<span data-ttu-id="5dd64-128">Um elemento [StandardTime](standardtime.md) que contém um elemento [DayOrder](dayorder.md) que tem um valor de 5, um elemento **month** que tem um valor de 10, e um elemento [DayOfWeek (TimeZone)](dayofweek-timezone.md) que tem um valor de domingo significa que a transição do horário padrão para o horário de Verão ocorre no quinto domingo do décimo mês.</span><span class="sxs-lookup"><span data-stu-id="5dd64-128">A [StandardTime](standardtime.md) element that contains a [DayOrder](dayorder.md) element that has a value of 5, a **Month** element that has a value of 10, and a [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that has a value of Sunday means that the transition from standard time to daylight saving time occurs on the fifth Sunday of the tenth month.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="5dd64-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5dd64-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5dd64-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="5dd64-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5dd64-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5dd64-131">Schema Name</span></span>  <br/> |<span data-ttu-id="5dd64-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5dd64-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="5dd64-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5dd64-133">Validation File</span></span>  <br/> |<span data-ttu-id="5dd64-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5dd64-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5dd64-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5dd64-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="5dd64-136">False</span><span class="sxs-lookup"><span data-stu-id="5dd64-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5dd64-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="5dd64-137">See also</span></span>

- [<span data-ttu-id="5dd64-138">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="5dd64-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="5dd64-139">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="5dd64-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

