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
description: O elemento year é usado para definir um fuso horário que muda dependendo do ano. Este elemento é opcional. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: cc83f9b2137f151f3f8ef0ceaf603ec036989961
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465167"
---
# <a name="year"></a><span data-ttu-id="a8494-105">Ano</span><span class="sxs-lookup"><span data-stu-id="a8494-105">Year</span></span>

<span data-ttu-id="a8494-106">O elemento **year** é usado para definir um fuso horário que muda dependendo do ano.</span><span class="sxs-lookup"><span data-stu-id="a8494-106">The **Year** element is used to define a time zone that changes depending on the year.</span></span> <span data-ttu-id="a8494-107">Este elemento é opcional.</span><span class="sxs-lookup"><span data-stu-id="a8494-107">This element is optional.</span></span> <span data-ttu-id="a8494-108">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a8494-108">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<Year/>
```

<span data-ttu-id="a8494-109">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="a8494-109">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a8494-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a8494-110">Attributes and elements</span></span>

<span data-ttu-id="a8494-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a8494-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8494-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="a8494-112">Attributes</span></span>

<span data-ttu-id="a8494-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a8494-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a8494-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a8494-114">Child elements</span></span>

<span data-ttu-id="a8494-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a8494-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a8494-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a8494-116">Parent elements</span></span>

|<span data-ttu-id="a8494-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a8494-117">**Element**</span></span>|<span data-ttu-id="a8494-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a8494-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8494-119">StandardTime</span><span class="sxs-lookup"><span data-stu-id="a8494-119">StandardTime</span></span>](standardtime.md) <br/> |<span data-ttu-id="a8494-120">Representa um deslocamento do tempo relativo ao UTC (tempo Universal Coordenado) que é representado pelo elemento [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="a8494-120">Represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span>  <br/> |
|[<span data-ttu-id="a8494-121">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="a8494-121">DaylightTime</span></span>](daylighttime.md) <br/> |<span data-ttu-id="a8494-122">Representa um deslocamento da hora relativa ao UTC (tempo Universal Coordenado) que é representado pelo elemento [Bias (UTC)](bias-utc.md) nas regiões onde o horário de verão é observado.</span><span class="sxs-lookup"><span data-stu-id="a8494-122">Represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a8494-123">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="a8494-123">Text value</span></span>

<span data-ttu-id="a8494-124">O elemento year aceita uma cadeia de caracteres que representa um ano.</span><span class="sxs-lookup"><span data-stu-id="a8494-124">The Year element accepts a string that represents a year.</span></span> <span data-ttu-id="a8494-125">O formato de ano é aaaa.</span><span class="sxs-lookup"><span data-stu-id="a8494-125">The year format is YYYY.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a8494-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="a8494-126">Remarks</span></span>

<span data-ttu-id="a8494-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="a8494-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8494-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a8494-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8494-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="a8494-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a8494-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a8494-130">Schema Name</span></span>  <br/> |<span data-ttu-id="a8494-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a8494-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="a8494-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a8494-132">Validation File</span></span>  <br/> |<span data-ttu-id="a8494-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a8494-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a8494-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a8494-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="a8494-135">False</span><span class="sxs-lookup"><span data-stu-id="a8494-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a8494-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="a8494-136">See also</span></span>

- [<span data-ttu-id="a8494-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a8494-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

