---
title: Bias (UTC)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Bias
api_type:
- schema
ms.assetid: 15790d5a-5134-457b-8f2b-d9dee1f807a2
description: O elemento Bias representa o deslocamento geral do tempo Universal Coordenado (UTC). Este valor está em minutos.
ms.openlocfilehash: 43613593565ca15be97bd2a98dbe5c512dbe5fc7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751269"
---
# <a name="bias-utc"></a><span data-ttu-id="278f5-104">Bias (UTC)</span><span class="sxs-lookup"><span data-stu-id="278f5-104">Bias (UTC)</span></span>

<span data-ttu-id="278f5-105">O elemento **Bias** representa o deslocamento geral do tempo Universal Coordenado (UTC).</span><span class="sxs-lookup"><span data-stu-id="278f5-105">The **Bias** element represents the general offset from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="278f5-106">Este valor está em minutos.</span><span class="sxs-lookup"><span data-stu-id="278f5-106">This value is in minutes.</span></span> 
  
```xml
<TimeZone>
   <Bias>int</Bias>
</TimeZone>
```

<span data-ttu-id="278f5-107">**int**</span><span class="sxs-lookup"><span data-stu-id="278f5-107">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="278f5-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="278f5-108">Attributes and elements</span></span>

<span data-ttu-id="278f5-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="278f5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="278f5-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="278f5-110">Attributes</span></span>

<span data-ttu-id="278f5-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="278f5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="278f5-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="278f5-112">Child elements</span></span>

<span data-ttu-id="278f5-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="278f5-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="278f5-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="278f5-114">Parent elements</span></span>

|<span data-ttu-id="278f5-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="278f5-115">**Element**</span></span>|<span data-ttu-id="278f5-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="278f5-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="278f5-117">Fuso horário (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="278f5-117">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="278f5-118">O contêiner que identifica as informações de data / hora da solicitação.</span><span class="sxs-lookup"><span data-stu-id="278f5-118">The container that identifies the date-time information of the request.</span></span> <span data-ttu-id="278f5-119">Esse elemento contém informações sobre a transição entre o período padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="278f5-119">This element contains information about the transition between standard time and daylight saving time.</span></span>  <br/><br/><span data-ttu-id="278f5-120">A seguir estão as expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="278f5-120">The following are the XPath expressions to this element:</span></span><br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/><br/>`/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="278f5-121">Text value</span><span class="sxs-lookup"><span data-stu-id="278f5-121">Text value</span></span>

<span data-ttu-id="278f5-122">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="278f5-122">A text value is required.</span></span> <span data-ttu-id="278f5-123">O valor de texto representa um número inteiro.</span><span class="sxs-lookup"><span data-stu-id="278f5-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="278f5-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="278f5-124">Remarks</span></span>

<span data-ttu-id="278f5-125">Um segundo elemento [Bias](bias.md) no esquema representa o deslocamento do deslocamento de tempo Universal Coordenado (UTC).</span><span class="sxs-lookup"><span data-stu-id="278f5-125">A second [Bias](bias.md) element in the schema represents the offset from the Coordinated Universal Time (UTC) offset.</span></span> 
  
## <a name="example"></a><span data-ttu-id="278f5-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="278f5-126">Example</span></span>

<span data-ttu-id="278f5-127">O exemplo a seguir mostra a parte de uma solicitação XML que identifica um deslocamento de 8 horas do UTC no aplicativo cliente.</span><span class="sxs-lookup"><span data-stu-id="278f5-127">The following example shows part of an XML request that identifies an offset of 8 hours from UTC on the client application.</span></span>
  
```xml
<TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
  <Bias>480</Bias>
  <StandardTime>
    <Bias>0</Bias>
    <Time>02:00:00</Time>
    <DayOrder>5</DayOrder>
    <Month>10</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </StandardTime>
  <DaylightTime>
    <Bias>-60</Bias>
    <Time>02:00:00</Time>
    <DayOrder>1</DayOrder>
    <Month>4</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </DaylightTime>
</TimeZone>
```

## <a name="element-information"></a><span data-ttu-id="278f5-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="278f5-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="278f5-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="278f5-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="278f5-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="278f5-130">Schema Name</span></span>  <br/> |<span data-ttu-id="278f5-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="278f5-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="278f5-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="278f5-132">Validation File</span></span>  <br/> |<span data-ttu-id="278f5-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="278f5-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="278f5-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="278f5-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="278f5-135">False</span><span class="sxs-lookup"><span data-stu-id="278f5-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="278f5-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="278f5-136">See also</span></span>

- [<span data-ttu-id="278f5-137">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="278f5-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="278f5-138">Bias</span><span class="sxs-lookup"><span data-stu-id="278f5-138">Bias</span></span>](bias.md)
- [<span data-ttu-id="278f5-139">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="278f5-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

