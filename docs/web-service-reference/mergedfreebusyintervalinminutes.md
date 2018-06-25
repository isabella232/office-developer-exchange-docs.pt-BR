---
title: MergedFreeBusyIntervalInMinutes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MergedFreeBusyIntervalInMinutes
api_type:
- schema
ms.assetid: 481cdbc6-d5aa-49fa-a3fa-9d119d3dca99
description: O elemento MergedFreeBusyIntervalInMinutes representa a diferença de horário entre dois slots sucessivos no modo de exibição FreeBusyMerged.
ms.openlocfilehash: 99c8c69424a0a9d9594005fdf6b2ceba53e6288a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824451"
---
# <a name="mergedfreebusyintervalinminutes"></a><span data-ttu-id="38c23-103">MergedFreeBusyIntervalInMinutes</span><span class="sxs-lookup"><span data-stu-id="38c23-103">MergedFreeBusyIntervalInMinutes</span></span>

<span data-ttu-id="38c23-104">O elemento **MergedFreeBusyIntervalInMinutes** representa a diferença de horário entre dois slots sucessivos no modo de exibição **FreeBusyMerged** .</span><span class="sxs-lookup"><span data-stu-id="38c23-104">The **MergedFreeBusyIntervalInMinutes** element represents the time difference between two successive slots in the **FreeBusyMerged** view.</span></span> 
  
[<span data-ttu-id="38c23-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="38c23-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="38c23-106">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="38c23-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
[<span data-ttu-id="38c23-107">MergedFreeBusyIntervalInMinutes</span><span class="sxs-lookup"><span data-stu-id="38c23-107">MergedFreeBusyIntervalInMinutes</span></span>](mergedfreebusyintervalinminutes.md)
  
```xml
<MergedFreeBusyIntervalInMinutes>...</MergedFreeBusyIntervalInMinutes>
```

 <span data-ttu-id="38c23-108">**int**</span><span class="sxs-lookup"><span data-stu-id="38c23-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="38c23-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="38c23-109">Attributes and elements</span></span>

<span data-ttu-id="38c23-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="38c23-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="38c23-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="38c23-111">Attributes</span></span>

<span data-ttu-id="38c23-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="38c23-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="38c23-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="38c23-113">Child elements</span></span>

<span data-ttu-id="38c23-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="38c23-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="38c23-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="38c23-115">Parent elements</span></span>

|<span data-ttu-id="38c23-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="38c23-116">**Element**</span></span>|<span data-ttu-id="38c23-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="38c23-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38c23-118">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="38c23-118">FreeBusyViewOptions</span></span>](freebusyviewoptions.md) <br/> |<span data-ttu-id="38c23-119">Especifica o tipo de informações de disponibilidade retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="38c23-119">Specifies the type of free/busy information returned in the response.</span></span>  <br/> <span data-ttu-id="38c23-120">Este é o XPath a este elemento:</span><span class="sxs-lookup"><span data-stu-id="38c23-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="38c23-121">Text value</span><span class="sxs-lookup"><span data-stu-id="38c23-121">Text value</span></span>

<span data-ttu-id="38c23-122">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="38c23-122">A text value is required.</span></span> <span data-ttu-id="38c23-123">O valor de texto representa o tempo em minutos.</span><span class="sxs-lookup"><span data-stu-id="38c23-123">The text value represents time in minutes.</span></span> <span data-ttu-id="38c23-124">O valor padrão é 30 minutos.</span><span class="sxs-lookup"><span data-stu-id="38c23-124">The default value is 30 minutes.</span></span> <span data-ttu-id="38c23-125">Seis minutos é o intervalo mínimo e um dia (1440 minutos) é o intervalo máximo para esse elemento.</span><span class="sxs-lookup"><span data-stu-id="38c23-125">Six minutes is the minimum interval and one day (1440 minutes) is the maximum interval for this element.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="38c23-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="38c23-126">Remarks</span></span>

<span data-ttu-id="38c23-127">Esse valor é usado somente se o elemento [RequestedView](requestedview.md) for igual a **MergedOnly**, **FreeBusyMerged**ou **DetailedMerge**.</span><span class="sxs-lookup"><span data-stu-id="38c23-127">This value is used only if the [RequestedView](requestedview.md) element is equal to **MergedOnly**, **FreeBusyMerged**, or **DetailedMerge**.</span></span> <span data-ttu-id="38c23-128">Este é um tipo de dados inteiro.</span><span class="sxs-lookup"><span data-stu-id="38c23-128">This is an integer data type.</span></span> <span data-ttu-id="38c23-129">O fluxo que contém os intervalos definidos por esse elemento é retornado no elemento [MergedFreeBusy](mergedfreebusy.md) .</span><span class="sxs-lookup"><span data-stu-id="38c23-129">The stream that contains the intervals defined by this element is returned in the [MergedFreeBusy](mergedfreebusy.md) element.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="38c23-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="38c23-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="38c23-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="38c23-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="38c23-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="38c23-132">Schema Name</span></span>  <br/> |<span data-ttu-id="38c23-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="38c23-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="38c23-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="38c23-134">Validation File</span></span>  <br/> |<span data-ttu-id="38c23-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="38c23-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="38c23-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="38c23-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="38c23-137">False</span><span class="sxs-lookup"><span data-stu-id="38c23-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="38c23-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="38c23-138">See also</span></span>



[<span data-ttu-id="38c23-139">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="38c23-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="38c23-140">Operação GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="38c23-140">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)


[<span data-ttu-id="38c23-141">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="38c23-141">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

