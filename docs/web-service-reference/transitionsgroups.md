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
description: O elemento TransitionsGroups representa uma matriz dos grupos de transição do fuso horário.
ms.openlocfilehash: 546dd3c96187bf9f1ebf574b37b689e26e3af997
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837800"
---
# <a name="transitionsgroups"></a><span data-ttu-id="af6e6-103">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="af6e6-103">TransitionsGroups</span></span>

<span data-ttu-id="af6e6-104">O elemento **TransitionsGroups** representa uma matriz dos grupos de transição do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="af6e6-104">The **TransitionsGroups** element represents an array of time zone transition groups.</span></span> 
  
```XML
<TransitionsGroups>
   <TransitionsGroup/>
</TransitionsGroups>
```

 <span data-ttu-id="af6e6-105">**ArrayOfTransitionsGroupsType**</span><span class="sxs-lookup"><span data-stu-id="af6e6-105">**ArrayOfTransitionsGroupsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="af6e6-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="af6e6-106">Attributes and elements</span></span>

<span data-ttu-id="af6e6-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="af6e6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="af6e6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="af6e6-108">Attributes</span></span>

<span data-ttu-id="af6e6-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="af6e6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="af6e6-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="af6e6-110">Child elements</span></span>

|<span data-ttu-id="af6e6-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="af6e6-111">**Element**</span></span>|<span data-ttu-id="af6e6-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="af6e6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af6e6-113">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="af6e6-113">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="af6e6-114">Representa uma matriz de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="af6e6-114">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="af6e6-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="af6e6-115">Parent elements</span></span>

|<span data-ttu-id="af6e6-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="af6e6-116">**Element**</span></span>|<span data-ttu-id="af6e6-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="af6e6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af6e6-118">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="af6e6-118">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="af6e6-119">Define o fuso horário para a hora de início de uma [CalendarItem](calendaritem.md) ou [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="af6e6-119">Defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="af6e6-120">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="af6e6-120">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="af6e6-121">Define o fuso horário para a hora de término de uma [CalendarItem](calendaritem.md) ou [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="af6e6-121">Defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="af6e6-122">Timezonedefinition pela última vez</span><span class="sxs-lookup"><span data-stu-id="af6e6-122">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="af6e6-123">Define um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="af6e6-123">Defines a time zone.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="af6e6-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="af6e6-124">Remarks</span></span>

<span data-ttu-id="af6e6-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="af6e6-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="af6e6-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="af6e6-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="af6e6-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="af6e6-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="af6e6-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="af6e6-128">Schema Name</span></span>  <br/> |<span data-ttu-id="af6e6-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="af6e6-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="af6e6-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="af6e6-130">Validation File</span></span>  <br/> |<span data-ttu-id="af6e6-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="af6e6-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="af6e6-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="af6e6-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="af6e6-133">False</span><span class="sxs-lookup"><span data-stu-id="af6e6-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="af6e6-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="af6e6-134">See also</span></span>



- [<span data-ttu-id="af6e6-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="af6e6-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

