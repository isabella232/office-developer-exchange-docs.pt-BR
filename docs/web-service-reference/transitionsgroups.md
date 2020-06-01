---
title: TransitionsGroups
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TransitionsGroups
api_type:
- schema
ms.assetid: ad0849f8-5158-4a23-9c36-a49f5be1d1e1
description: O elemento TransitionsGroups representa uma matriz de grupos de transição de fuso horário.
ms.openlocfilehash: 35244e122ee31045359afd0833459bbb94fd0aa1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467407"
---
# <a name="transitionsgroups"></a><span data-ttu-id="c9de8-103">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="c9de8-103">TransitionsGroups</span></span>

<span data-ttu-id="c9de8-104">O elemento **TransitionsGroups** representa uma matriz de grupos de transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="c9de8-104">The **TransitionsGroups** element represents an array of time zone transition groups.</span></span> 
  
```XML
<TransitionsGroups>
   <TransitionsGroup/>
</TransitionsGroups>
```

 <span data-ttu-id="c9de8-105">**ArrayOfTransitionsGroupsType**</span><span class="sxs-lookup"><span data-stu-id="c9de8-105">**ArrayOfTransitionsGroupsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c9de8-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c9de8-106">Attributes and elements</span></span>

<span data-ttu-id="c9de8-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c9de8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9de8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c9de8-108">Attributes</span></span>

<span data-ttu-id="c9de8-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c9de8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9de8-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c9de8-110">Child elements</span></span>

|<span data-ttu-id="c9de8-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c9de8-111">**Element**</span></span>|<span data-ttu-id="c9de8-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c9de8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9de8-113">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="c9de8-113">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="c9de8-114">Representa uma matriz de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="c9de8-114">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c9de8-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c9de8-115">Parent elements</span></span>

|<span data-ttu-id="c9de8-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c9de8-116">**Element**</span></span>|<span data-ttu-id="c9de8-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c9de8-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9de8-118">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="c9de8-118">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="c9de8-119">Define o fuso horário para a hora de início de um [CalendarItem](calendaritem.md) ou [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="c9de8-119">Defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="c9de8-120">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="c9de8-120">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="c9de8-121">Define o fuso horário para a hora de término de um [CalendarItem](calendaritem.md) ou [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="c9de8-121">Defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="c9de8-122">TimeZoneDefinition</span><span class="sxs-lookup"><span data-stu-id="c9de8-122">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="c9de8-123">Define um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="c9de8-123">Defines a time zone.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c9de8-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="c9de8-124">Remarks</span></span>

<span data-ttu-id="c9de8-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9de8-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c9de8-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c9de8-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9de8-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="c9de8-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c9de8-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c9de8-128">Schema Name</span></span>  <br/> |<span data-ttu-id="c9de8-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c9de8-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="c9de8-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c9de8-130">Validation File</span></span>  <br/> |<span data-ttu-id="c9de8-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c9de8-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c9de8-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c9de8-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="c9de8-133">False</span><span class="sxs-lookup"><span data-stu-id="c9de8-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c9de8-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="c9de8-134">See also</span></span>



- [<span data-ttu-id="c9de8-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c9de8-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

