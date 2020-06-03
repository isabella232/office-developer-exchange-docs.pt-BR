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
description: O elemento Bias representa o deslocamento geral do tempo universal coordenado (UTC). Este valor está em minutos.
ms.openlocfilehash: d95284aa28e59542d1a1ee40686163138b015702
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460243"
---
# <a name="bias-utc"></a><span data-ttu-id="3dc68-104">Bias (UTC)</span><span class="sxs-lookup"><span data-stu-id="3dc68-104">Bias (UTC)</span></span>

<span data-ttu-id="3dc68-105">O elemento **Bias** representa o deslocamento geral do tempo universal coordenado (UTC).</span><span class="sxs-lookup"><span data-stu-id="3dc68-105">The **Bias** element represents the general offset from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="3dc68-106">Este valor está em minutos.</span><span class="sxs-lookup"><span data-stu-id="3dc68-106">This value is in minutes.</span></span> 
  
```xml
<TimeZone>
   <Bias>int</Bias>
</TimeZone>
```

<span data-ttu-id="3dc68-107">**int**</span><span class="sxs-lookup"><span data-stu-id="3dc68-107">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="3dc68-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3dc68-108">Attributes and elements</span></span>

<span data-ttu-id="3dc68-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3dc68-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3dc68-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="3dc68-110">Attributes</span></span>

<span data-ttu-id="3dc68-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3dc68-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3dc68-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3dc68-112">Child elements</span></span>

<span data-ttu-id="3dc68-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3dc68-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3dc68-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3dc68-114">Parent elements</span></span>

|<span data-ttu-id="3dc68-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3dc68-115">**Element**</span></span>|<span data-ttu-id="3dc68-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3dc68-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3dc68-117">Fuso horário (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="3dc68-117">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="3dc68-118">O contêiner que identifica as informações de data e hora da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3dc68-118">The container that identifies the date-time information of the request.</span></span> <span data-ttu-id="3dc68-119">Este elemento contém informações sobre a transição entre o horário padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="3dc68-119">This element contains information about the transition between standard time and daylight saving time.</span></span>  <br/><br/><span data-ttu-id="3dc68-120">A seguir estão as expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="3dc68-120">The following are the XPath expressions to this element:</span></span><br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/><br/>`/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3dc68-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="3dc68-121">Text value</span></span>

<span data-ttu-id="3dc68-122">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3dc68-122">A text value is required.</span></span> <span data-ttu-id="3dc68-123">O valor de texto representa um inteiro.</span><span class="sxs-lookup"><span data-stu-id="3dc68-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3dc68-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="3dc68-124">Remarks</span></span>

<span data-ttu-id="3dc68-125">Um segundo elemento [Bias](bias.md) no esquema representa o deslocamento do deslocamento UTC (tempo Universal Coordenado).</span><span class="sxs-lookup"><span data-stu-id="3dc68-125">A second [Bias](bias.md) element in the schema represents the offset from the Coordinated Universal Time (UTC) offset.</span></span> 
  
## <a name="example"></a><span data-ttu-id="3dc68-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3dc68-126">Example</span></span>

<span data-ttu-id="3dc68-127">O exemplo a seguir mostra parte de uma solicitação XML que identifica um deslocamento de 8 horas do UTC no aplicativo cliente.</span><span class="sxs-lookup"><span data-stu-id="3dc68-127">The following example shows part of an XML request that identifies an offset of 8 hours from UTC on the client application.</span></span>
  
```xml
<TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="3dc68-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3dc68-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3dc68-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="3dc68-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3dc68-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3dc68-130">Schema Name</span></span>  <br/> |<span data-ttu-id="3dc68-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3dc68-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="3dc68-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3dc68-132">Validation File</span></span>  <br/> |<span data-ttu-id="3dc68-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3dc68-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3dc68-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3dc68-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="3dc68-135">False</span><span class="sxs-lookup"><span data-stu-id="3dc68-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3dc68-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="3dc68-136">See also</span></span>

- [<span data-ttu-id="3dc68-137">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="3dc68-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="3dc68-138">Bias</span><span class="sxs-lookup"><span data-stu-id="3dc68-138">Bias</span></span>](bias.md)
- [<span data-ttu-id="3dc68-139">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="3dc68-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

