---
title: Ano
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Year
api_type:
- schema
ms.assetid: 93bf2847-53fa-496c-9a1e-dc9a9ffd0b9f
description: O elemento de ano é usado para definir um fuso horário que mudam dependendo do ano. Esse elemento é opcional. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 95d75f9c6166fc26e86534346fb07292a7fb3dcd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838101"
---
# <a name="year"></a><span data-ttu-id="8e787-105">Ano</span><span class="sxs-lookup"><span data-stu-id="8e787-105">Year</span></span>

<span data-ttu-id="8e787-106">O elemento de **ano** é usado para definir um fuso horário que mudam dependendo do ano.</span><span class="sxs-lookup"><span data-stu-id="8e787-106">The **Year** element is used to define a time zone that changes depending on the year.</span></span> <span data-ttu-id="8e787-107">Esse elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="8e787-107">This element is optional.</span></span> <span data-ttu-id="8e787-108">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="8e787-108">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<Year/>
```

<span data-ttu-id="8e787-109">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="8e787-109">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8e787-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8e787-110">Attributes and elements</span></span>

<span data-ttu-id="8e787-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8e787-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8e787-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="8e787-112">Attributes</span></span>

<span data-ttu-id="8e787-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8e787-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8e787-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8e787-114">Child elements</span></span>

<span data-ttu-id="8e787-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8e787-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8e787-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8e787-116">Parent elements</span></span>

|<span data-ttu-id="8e787-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8e787-117">**Element**</span></span>|<span data-ttu-id="8e787-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8e787-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8e787-119">StandardTime</span><span class="sxs-lookup"><span data-stu-id="8e787-119">StandardTime</span></span>](standardtime.md) <br/> |<span data-ttu-id="8e787-120">Representa um deslocamento, desde o momento em relação ao tempo Universal Coordenado (UTC) que é representado por um elemento [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="8e787-120">Represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span>  <br/> |
|[<span data-ttu-id="8e787-121">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="8e787-121">DaylightTime</span></span>](daylighttime.md) <br/> |<span data-ttu-id="8e787-122">Representa um deslocamento, desde o momento em relação ao tempo Universal Coordenado (UTC) que é representado por um elemento [Bias (UTC)](bias-utc.md) em regiões onde o horário de verão é observado.</span><span class="sxs-lookup"><span data-stu-id="8e787-122">Represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8e787-123">Text value</span><span class="sxs-lookup"><span data-stu-id="8e787-123">Text value</span></span>

<span data-ttu-id="8e787-124">O elemento de ano aceita uma cadeia de caracteres que representa um ano.</span><span class="sxs-lookup"><span data-stu-id="8e787-124">The Year element accepts a string that represents a year.</span></span> <span data-ttu-id="8e787-125">O formato de ano é aaaa.</span><span class="sxs-lookup"><span data-stu-id="8e787-125">The year format is YYYY.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8e787-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="8e787-126">Remarks</span></span>

<span data-ttu-id="8e787-127">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="8e787-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8e787-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8e787-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8e787-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="8e787-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8e787-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8e787-130">Schema Name</span></span>  <br/> |<span data-ttu-id="8e787-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8e787-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="8e787-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8e787-132">Validation File</span></span>  <br/> |<span data-ttu-id="8e787-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8e787-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8e787-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8e787-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="8e787-135">False</span><span class="sxs-lookup"><span data-stu-id="8e787-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8e787-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="8e787-136">See also</span></span>

- [<span data-ttu-id="8e787-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8e787-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

