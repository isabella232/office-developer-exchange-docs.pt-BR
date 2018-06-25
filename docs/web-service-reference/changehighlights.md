---
title: ChangeHighlights
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9bd7323-44db-4d2f-aaaa-94c2dfdeead6
description: Mensagem de solicitação de ChangeHighlights elemento Especifica o que mudou entre duas versões de uma reunião.
ms.openlocfilehash: 5fe7aa95f60ae95f1af24e8f7a0463ad49716f65
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751385"
---
# <a name="changehighlights"></a><span data-ttu-id="659cb-103">ChangeHighlights</span><span class="sxs-lookup"><span data-stu-id="659cb-103">ChangeHighlights</span></span>

<span data-ttu-id="659cb-104">O elemento **ChangeHighlights** Especifica o que mudou entre duas versões de uma reunião mensagem de solicitação.</span><span class="sxs-lookup"><span data-stu-id="659cb-104">The **ChangeHighlights** element specifies what has changed between two versions of a meeting request message.</span></span> 
  
```XML
<ChangeHighlights>
    <HasLocationChanged></HasLocationChanged>
    <Location></Location>
    <HasStartTimeChanged></HasStartTimeChanged>
    <Start></Start>
    <HasEndTimeChanged></HasEndTimeChanged>
    <End></End>
</ChangeHighlights>
```

 <span data-ttu-id="659cb-105">**ChangeHighlightsType**</span><span class="sxs-lookup"><span data-stu-id="659cb-105">**ChangeHighlightsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="659cb-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="659cb-106">Attributes and elements</span></span>

<span data-ttu-id="659cb-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="659cb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="659cb-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="659cb-108">Attributes</span></span>

<span data-ttu-id="659cb-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="659cb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="659cb-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="659cb-110">Child elements</span></span>

|<span data-ttu-id="659cb-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="659cb-111">**Element**</span></span>|<span data-ttu-id="659cb-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="659cb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="659cb-113">HasLocationChanged</span><span class="sxs-lookup"><span data-stu-id="659cb-113">HasLocationChanged</span></span>](haslocationchanged.md) <br/> |<span data-ttu-id="659cb-114">Especifica se a propriedade location de uma reunião foi alterada.</span><span class="sxs-lookup"><span data-stu-id="659cb-114">Specifies whether the location property of a meeting has changed.</span></span>  <br/> |
|[<span data-ttu-id="659cb-115">Location</span><span class="sxs-lookup"><span data-stu-id="659cb-115">Location</span></span>](location.md) <br/> |<span data-ttu-id="659cb-116">Representa o local de uma reunião ou compromisso.</span><span class="sxs-lookup"><span data-stu-id="659cb-116">Represents the location of a meeting or appointment.</span></span>  <br/> |
|[<span data-ttu-id="659cb-117">HasStartTimeChanged</span><span class="sxs-lookup"><span data-stu-id="659cb-117">HasStartTimeChanged</span></span>](hasstarttimechanged.md) <br/> |<span data-ttu-id="659cb-118">Especifica se a hora de início para uma reunião foi alterada.</span><span class="sxs-lookup"><span data-stu-id="659cb-118">Specifies whether the start time for a meeting has changed.</span></span>  <br/> |
|[<span data-ttu-id="659cb-119">Start</span><span class="sxs-lookup"><span data-stu-id="659cb-119">Start</span></span>](start.md) <br/> |<span data-ttu-id="659cb-120">Representa o início de uma duração.</span><span class="sxs-lookup"><span data-stu-id="659cb-120">Represents the start of a duration.</span></span>  <br/> |
|[<span data-ttu-id="659cb-121">HasEndTimeChanged</span><span class="sxs-lookup"><span data-stu-id="659cb-121">HasEndTimeChanged</span></span>](hasendtimechanged.md) <br/> |<span data-ttu-id="659cb-122">Especifica se a hora de término para uma reunião foi alterada.</span><span class="sxs-lookup"><span data-stu-id="659cb-122">Specifies whether the end time for a meeting has changed.</span></span>  <br/> |
|[<span data-ttu-id="659cb-123">End</span><span class="sxs-lookup"><span data-stu-id="659cb-123">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="659cb-124">Representa o fim de uma duração.</span><span class="sxs-lookup"><span data-stu-id="659cb-124">Represents the end of a duration.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="659cb-125">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="659cb-125">Parent elements</span></span>

|<span data-ttu-id="659cb-126">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="659cb-126">**Element**</span></span>|<span data-ttu-id="659cb-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="659cb-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="659cb-128">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="659cb-128">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="659cb-129">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="659cb-129">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="659cb-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="659cb-130">Remarks</span></span>

<span data-ttu-id="659cb-131">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="659cb-131">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="659cb-132">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="659cb-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="659cb-133">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="659cb-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="659cb-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="659cb-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="659cb-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="659cb-135">Schema Name</span></span>  <br/> |<span data-ttu-id="659cb-136">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="659cb-136">Type schema</span></span>  <br/> |
|<span data-ttu-id="659cb-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="659cb-137">Validation File</span></span>  <br/> |<span data-ttu-id="659cb-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="659cb-138">types.xsd</span></span>  <br/> |
|<span data-ttu-id="659cb-139">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="659cb-139">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="659cb-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="659cb-140">See also</span></span>



- [<span data-ttu-id="659cb-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="659cb-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

