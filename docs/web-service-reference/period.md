---
title: Ponto
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
description: O elemento de período define o nome, a diferença de horário e o identificador exclusivo de um estágio específico do fuso horário.
ms.openlocfilehash: 3b5d5877e6d9baffdfe536a0feec3b25b6d2883f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824726"
---
# <a name="period"></a><span data-ttu-id="8622c-103">Ponto</span><span class="sxs-lookup"><span data-stu-id="8622c-103">Period</span></span>

<span data-ttu-id="8622c-104">O elemento de **período** define o nome, a diferença de horário e o identificador exclusivo de um estágio específico do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="8622c-104">The **Period** element defines the name, time offset, and unique identifier for a specific stage of the time zone.</span></span> 
  
```xml
<Period Bias="" Name="" Id=""/>
```

 <span data-ttu-id="8622c-105">**PeriodType**</span><span class="sxs-lookup"><span data-stu-id="8622c-105">**PeriodType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8622c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8622c-106">Attributes and elements</span></span>

<span data-ttu-id="8622c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8622c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8622c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8622c-108">Attributes</span></span>

|<span data-ttu-id="8622c-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="8622c-109">**Attribute**</span></span>|<span data-ttu-id="8622c-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8622c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8622c-111">Bias</span><span class="sxs-lookup"><span data-stu-id="8622c-111">Bias</span></span>  <br/> |<span data-ttu-id="8622c-112">Um valor de Duration que representa o deslocamento de tempo do tempo Universal Coordenado (UTC) para o período.</span><span class="sxs-lookup"><span data-stu-id="8622c-112">An xs:duration value that represents the time offset from Coordinated Universal Time (UTC) for the period.</span></span>  <br/> |
|<span data-ttu-id="8622c-113">Nome</span><span class="sxs-lookup"><span data-stu-id="8622c-113">Name</span></span>  <br/> |<span data-ttu-id="8622c-114">Um valor string que representa o nome descritivo do período.</span><span class="sxs-lookup"><span data-stu-id="8622c-114">A string value that represents the descriptive name of the period.</span></span>  <br/> |
|<span data-ttu-id="8622c-115">Id</span><span class="sxs-lookup"><span data-stu-id="8622c-115">Id</span></span>  <br/> |<span data-ttu-id="8622c-116">Um valor string que representa o identificador para o período.</span><span class="sxs-lookup"><span data-stu-id="8622c-116">A string value that represents the identifier for the period.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8622c-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8622c-117">Child elements</span></span>

<span data-ttu-id="8622c-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8622c-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8622c-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8622c-119">Parent elements</span></span>

|<span data-ttu-id="8622c-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8622c-120">**Element**</span></span>|<span data-ttu-id="8622c-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8622c-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8622c-122">Períodos</span><span class="sxs-lookup"><span data-stu-id="8622c-122">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="8622c-123">Representa uma matriz de períodos que definem o deslocamento de tempo em fases diferentes do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="8622c-123">Represents an array of periods that define the time offset at different stages of the time zone.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8622c-124">Text value</span><span class="sxs-lookup"><span data-stu-id="8622c-124">Text value</span></span>

<span data-ttu-id="8622c-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8622c-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8622c-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="8622c-126">Remarks</span></span>

<span data-ttu-id="8622c-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8622c-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8622c-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8622c-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8622c-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="8622c-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8622c-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8622c-130">Schema Name</span></span>  <br/> |<span data-ttu-id="8622c-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8622c-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="8622c-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8622c-132">Validation File</span></span>  <br/> |<span data-ttu-id="8622c-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8622c-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8622c-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8622c-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="8622c-135">False</span><span class="sxs-lookup"><span data-stu-id="8622c-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8622c-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="8622c-136">See also</span></span>



- [<span data-ttu-id="8622c-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8622c-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

