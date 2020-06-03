---
title: ChangeHighlights
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9bd7323-44db-4d2f-aaaa-94c2dfdeead6
description: O elemento ChangeHighlights especifica o que foi alterado entre duas versões de uma mensagem de solicitação de reunião.
ms.openlocfilehash: 6c78d2c96449ee41032859f90bf51d6e0faa92ae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463276"
---
# <a name="changehighlights"></a><span data-ttu-id="dcaa4-103">ChangeHighlights</span><span class="sxs-lookup"><span data-stu-id="dcaa4-103">ChangeHighlights</span></span>

<span data-ttu-id="dcaa4-104">O elemento **ChangeHighlights** especifica o que foi alterado entre duas versões de uma mensagem de solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="dcaa4-104">The **ChangeHighlights** element specifies what has changed between two versions of a meeting request message.</span></span> 
  
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

 <span data-ttu-id="dcaa4-105">**ChangeHighlightsType**</span><span class="sxs-lookup"><span data-stu-id="dcaa4-105">**ChangeHighlightsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dcaa4-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="dcaa4-106">Attributes and elements</span></span>

<span data-ttu-id="dcaa4-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="dcaa4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dcaa4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="dcaa4-108">Attributes</span></span>

<span data-ttu-id="dcaa4-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dcaa4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dcaa4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="dcaa4-110">Child elements</span></span>

|<span data-ttu-id="dcaa4-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dcaa4-111">**Element**</span></span>|<span data-ttu-id="dcaa4-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dcaa4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dcaa4-113">HasLocationChanged</span><span class="sxs-lookup"><span data-stu-id="dcaa4-113">HasLocationChanged</span></span>](haslocationchanged.md) <br/> |<span data-ttu-id="dcaa4-114">Especifica se a propriedade Location de uma reunião foi alterada.</span><span class="sxs-lookup"><span data-stu-id="dcaa4-114">Specifies whether the location property of a meeting has changed.</span></span>  <br/> |
|[<span data-ttu-id="dcaa4-115">Localização</span><span class="sxs-lookup"><span data-stu-id="dcaa4-115">Location</span></span>](location.md) <br/> |<span data-ttu-id="dcaa4-116">Representa o local de uma reunião ou compromisso.</span><span class="sxs-lookup"><span data-stu-id="dcaa4-116">Represents the location of a meeting or appointment.</span></span>  <br/> |
|[<span data-ttu-id="dcaa4-117">HasStartTimeChanged</span><span class="sxs-lookup"><span data-stu-id="dcaa4-117">HasStartTimeChanged</span></span>](hasstarttimechanged.md) <br/> |<span data-ttu-id="dcaa4-118">Especifica se a hora de início de uma reunião foi alterada.</span><span class="sxs-lookup"><span data-stu-id="dcaa4-118">Specifies whether the start time for a meeting has changed.</span></span>  <br/> |
|[<span data-ttu-id="dcaa4-119">Start</span><span class="sxs-lookup"><span data-stu-id="dcaa4-119">Start</span></span>](start.md) <br/> |<span data-ttu-id="dcaa4-120">Representa o início de uma duração.</span><span class="sxs-lookup"><span data-stu-id="dcaa4-120">Represents the start of a duration.</span></span>  <br/> |
|[<span data-ttu-id="dcaa4-121">HasEndTimeChanged</span><span class="sxs-lookup"><span data-stu-id="dcaa4-121">HasEndTimeChanged</span></span>](hasendtimechanged.md) <br/> |<span data-ttu-id="dcaa4-122">Especifica se a hora de término de uma reunião foi alterada.</span><span class="sxs-lookup"><span data-stu-id="dcaa4-122">Specifies whether the end time for a meeting has changed.</span></span>  <br/> |
|[<span data-ttu-id="dcaa4-123">Ponto</span><span class="sxs-lookup"><span data-stu-id="dcaa4-123">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="dcaa4-124">Representa o final de uma duração.</span><span class="sxs-lookup"><span data-stu-id="dcaa4-124">Represents the end of a duration.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dcaa4-125">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="dcaa4-125">Parent elements</span></span>

|<span data-ttu-id="dcaa4-126">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dcaa4-126">**Element**</span></span>|<span data-ttu-id="dcaa4-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dcaa4-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dcaa4-128">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="dcaa4-128">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="dcaa4-129">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="dcaa4-129">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dcaa4-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="dcaa4-130">Remarks</span></span>

<span data-ttu-id="dcaa4-131">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="dcaa4-131">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="dcaa4-132">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="dcaa4-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dcaa4-133">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="dcaa4-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dcaa4-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="dcaa4-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dcaa4-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="dcaa4-135">Schema Name</span></span>  <br/> |<span data-ttu-id="dcaa4-136">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="dcaa4-136">Type schema</span></span>  <br/> |
|<span data-ttu-id="dcaa4-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="dcaa4-137">Validation File</span></span>  <br/> |<span data-ttu-id="dcaa4-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="dcaa4-138">types.xsd</span></span>  <br/> |
|<span data-ttu-id="dcaa4-139">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="dcaa4-139">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="dcaa4-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="dcaa4-140">See also</span></span>



- [<span data-ttu-id="dcaa4-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="dcaa4-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

