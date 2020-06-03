---
title: Período
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Period
api_type:
- schema
ms.assetid: 2f9cf6af-c531-4d7d-90c9-1a1db504d890
description: O elemento period define o nome, o deslocamento de tempo e o identificador exclusivo de um estágio específico do fuso horário.
ms.openlocfilehash: a7c36a9de01fd0484a7df75de3b5525992ef7ee7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459718"
---
# <a name="period"></a><span data-ttu-id="b6fec-103">Período</span><span class="sxs-lookup"><span data-stu-id="b6fec-103">Period</span></span>

<span data-ttu-id="b6fec-104">O elemento **period** define o nome, o deslocamento de tempo e o identificador exclusivo de um estágio específico do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="b6fec-104">The **Period** element defines the name, time offset, and unique identifier for a specific stage of the time zone.</span></span> 
  
```xml
<Period Bias="" Name="" Id=""/>
```

 <span data-ttu-id="b6fec-105">**Periodtype**</span><span class="sxs-lookup"><span data-stu-id="b6fec-105">**PeriodType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b6fec-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b6fec-106">Attributes and elements</span></span>

<span data-ttu-id="b6fec-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b6fec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b6fec-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b6fec-108">Attributes</span></span>

|<span data-ttu-id="b6fec-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="b6fec-109">**Attribute**</span></span>|<span data-ttu-id="b6fec-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b6fec-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b6fec-111">Tendência</span><span class="sxs-lookup"><span data-stu-id="b6fec-111">Bias</span></span>  <br/> |<span data-ttu-id="b6fec-112">Um valor de duração xs: que representa a diferença de tempo do UTC (tempo Universal Coordenado) para o período.</span><span class="sxs-lookup"><span data-stu-id="b6fec-112">An xs:duration value that represents the time offset from Coordinated Universal Time (UTC) for the period.</span></span>  <br/> |
|<span data-ttu-id="b6fec-113">Nome</span><span class="sxs-lookup"><span data-stu-id="b6fec-113">Name</span></span>  <br/> |<span data-ttu-id="b6fec-114">Um valor String que representa o nome descritivo do período.</span><span class="sxs-lookup"><span data-stu-id="b6fec-114">A string value that represents the descriptive name of the period.</span></span>  <br/> |
|<span data-ttu-id="b6fec-115">Id</span><span class="sxs-lookup"><span data-stu-id="b6fec-115">Id</span></span>  <br/> |<span data-ttu-id="b6fec-116">Um valor String que representa o identificador para o período.</span><span class="sxs-lookup"><span data-stu-id="b6fec-116">A string value that represents the identifier for the period.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b6fec-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b6fec-117">Child elements</span></span>

<span data-ttu-id="b6fec-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b6fec-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b6fec-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b6fec-119">Parent elements</span></span>

|<span data-ttu-id="b6fec-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b6fec-120">**Element**</span></span>|<span data-ttu-id="b6fec-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b6fec-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6fec-122">Períodos</span><span class="sxs-lookup"><span data-stu-id="b6fec-122">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="b6fec-123">Representa uma matriz de períodos que definem a diferença de tempo em diferentes estágios do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="b6fec-123">Represents an array of periods that define the time offset at different stages of the time zone.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b6fec-124">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="b6fec-124">Text value</span></span>

<span data-ttu-id="b6fec-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b6fec-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b6fec-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="b6fec-126">Remarks</span></span>

<span data-ttu-id="b6fec-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b6fec-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b6fec-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b6fec-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b6fec-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="b6fec-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b6fec-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b6fec-130">Schema Name</span></span>  <br/> |<span data-ttu-id="b6fec-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b6fec-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="b6fec-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b6fec-132">Validation File</span></span>  <br/> |<span data-ttu-id="b6fec-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b6fec-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b6fec-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b6fec-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="b6fec-135">False</span><span class="sxs-lookup"><span data-stu-id="b6fec-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b6fec-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="b6fec-136">See also</span></span>



- [<span data-ttu-id="b6fec-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b6fec-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

