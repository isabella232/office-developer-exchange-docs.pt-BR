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
description: O elemento MergedFreeBusyIntervalInMinutes representa a diferença de tempo entre dois slots sucessivos no modo de exibição FreeBusyMerged.
ms.openlocfilehash: 6228ee5b66202634e6bb3b6c1ad6b8897a109d58
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468786"
---
# <a name="mergedfreebusyintervalinminutes"></a><span data-ttu-id="e1872-103">MergedFreeBusyIntervalInMinutes</span><span class="sxs-lookup"><span data-stu-id="e1872-103">MergedFreeBusyIntervalInMinutes</span></span>

<span data-ttu-id="e1872-104">O elemento **MergedFreeBusyIntervalInMinutes** representa a diferença de tempo entre dois slots sucessivos no modo de exibição **FreeBusyMerged** .</span><span class="sxs-lookup"><span data-stu-id="e1872-104">The **MergedFreeBusyIntervalInMinutes** element represents the time difference between two successive slots in the **FreeBusyMerged** view.</span></span> 
  
[<span data-ttu-id="e1872-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="e1872-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="e1872-106">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="e1872-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
[<span data-ttu-id="e1872-107">MergedFreeBusyIntervalInMinutes</span><span class="sxs-lookup"><span data-stu-id="e1872-107">MergedFreeBusyIntervalInMinutes</span></span>](mergedfreebusyintervalinminutes.md)
  
```xml
<MergedFreeBusyIntervalInMinutes>...</MergedFreeBusyIntervalInMinutes>
```

 <span data-ttu-id="e1872-108">**int**</span><span class="sxs-lookup"><span data-stu-id="e1872-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e1872-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e1872-109">Attributes and elements</span></span>

<span data-ttu-id="e1872-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e1872-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e1872-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="e1872-111">Attributes</span></span>

<span data-ttu-id="e1872-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1872-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e1872-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e1872-113">Child elements</span></span>

<span data-ttu-id="e1872-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e1872-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e1872-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e1872-115">Parent elements</span></span>

|<span data-ttu-id="e1872-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e1872-116">**Element**</span></span>|<span data-ttu-id="e1872-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e1872-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1872-118">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="e1872-118">FreeBusyViewOptions</span></span>](freebusyviewoptions.md) <br/> |<span data-ttu-id="e1872-119">Especifica o tipo de informações de disponibilidade retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="e1872-119">Specifies the type of free/busy information returned in the response.</span></span>  <br/> <span data-ttu-id="e1872-120">Este é o XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="e1872-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e1872-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="e1872-121">Text value</span></span>

<span data-ttu-id="e1872-122">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1872-122">A text value is required.</span></span> <span data-ttu-id="e1872-123">O valor de texto representa o tempo em minutos.</span><span class="sxs-lookup"><span data-stu-id="e1872-123">The text value represents time in minutes.</span></span> <span data-ttu-id="e1872-124">O valor-padrão é 30 minutos.</span><span class="sxs-lookup"><span data-stu-id="e1872-124">The default value is 30 minutes.</span></span> <span data-ttu-id="e1872-125">Seis minutos é o intervalo mínimo e um dia (1440 minutos) é o intervalo máximo para este elemento.</span><span class="sxs-lookup"><span data-stu-id="e1872-125">Six minutes is the minimum interval and one day (1440 minutes) is the maximum interval for this element.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e1872-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="e1872-126">Remarks</span></span>

<span data-ttu-id="e1872-127">Esse valor é usado somente se o elemento [RequestedView](requestedview.md) for igual a **MergedOnly**, **FreeBusyMerged**ou **DetailedMerge**.</span><span class="sxs-lookup"><span data-stu-id="e1872-127">This value is used only if the [RequestedView](requestedview.md) element is equal to **MergedOnly**, **FreeBusyMerged**, or **DetailedMerge**.</span></span> <span data-ttu-id="e1872-128">Este é um tipo de dados Integer.</span><span class="sxs-lookup"><span data-stu-id="e1872-128">This is an integer data type.</span></span> <span data-ttu-id="e1872-129">O Stream que contém os intervalos definidos por esse elemento é retornado no elemento [MergedFreeBusy](mergedfreebusy.md) .</span><span class="sxs-lookup"><span data-stu-id="e1872-129">The stream that contains the intervals defined by this element is returned in the [MergedFreeBusy](mergedfreebusy.md) element.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="e1872-130">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e1872-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e1872-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="e1872-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e1872-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e1872-132">Schema Name</span></span>  <br/> |<span data-ttu-id="e1872-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e1872-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="e1872-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e1872-134">Validation File</span></span>  <br/> |<span data-ttu-id="e1872-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e1872-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e1872-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e1872-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="e1872-137">False</span><span class="sxs-lookup"><span data-stu-id="e1872-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e1872-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="e1872-138">See also</span></span>



[<span data-ttu-id="e1872-139">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="e1872-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="e1872-140">Operação GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="e1872-140">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)


[<span data-ttu-id="e1872-141">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="e1872-141">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

