---
title: StartTimeZone
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartTimeZone
api_type:
- schema
ms.assetid: d38c4dc1-4ecb-42a1-8d57-a451b16a2de2
description: O elemento de StartTimeZone define o fuso horário para a hora de início de uma CalendarItem ou MeetingRequest.
ms.openlocfilehash: 6d21869c4b3be048db27dcc9f128fff868aebcb5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825559"
---
# <a name="starttimezone"></a><span data-ttu-id="2e0d3-103">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="2e0d3-103">StartTimeZone</span></span>

<span data-ttu-id="2e0d3-104">O elemento de **StartTimeZone** define o fuso horário para a hora de início de uma [CalendarItem](calendaritem.md) ou [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="2e0d3-104">The **StartTimeZone** element defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>
  
```xml
<StartTimeZone Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</StartTimeZone>
```

<span data-ttu-id="2e0d3-105">**TimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="2e0d3-105">**TimeZoneDefinitionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2e0d3-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="2e0d3-106">Attributes and elements</span></span>

<span data-ttu-id="2e0d3-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2e0d3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2e0d3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2e0d3-108">Attributes</span></span>

|<span data-ttu-id="2e0d3-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="2e0d3-109">**Attribute**</span></span>|<span data-ttu-id="2e0d3-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2e0d3-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2e0d3-111">Id</span><span class="sxs-lookup"><span data-stu-id="2e0d3-111">Id</span></span>  <br/> |<span data-ttu-id="2e0d3-112">Representa o identificador exclusivo da definição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="2e0d3-112">Represents the unique identifier of the time zone definition.</span></span>  <br/> |
|<span data-ttu-id="2e0d3-113">Nome</span><span class="sxs-lookup"><span data-stu-id="2e0d3-113">Name</span></span>  <br/> |<span data-ttu-id="2e0d3-114">Representa o nome descritivo da definição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="2e0d3-114">Represents the descriptive name of the time zone definition.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2e0d3-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2e0d3-115">Child elements</span></span>

|<span data-ttu-id="2e0d3-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2e0d3-116">**Element**</span></span>|<span data-ttu-id="2e0d3-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2e0d3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2e0d3-118">Períodos</span><span class="sxs-lookup"><span data-stu-id="2e0d3-118">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="2e0d3-119">Representa uma matriz de elementos do [período](period.md) que definem o deslocamento de tempo em fases diferentes do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="2e0d3-119">Represents an array of [Period](period.md) elements that define the time offset at different stages of the time zone.</span></span>  <br/> |
|[<span data-ttu-id="2e0d3-120">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="2e0d3-120">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="2e0d3-121">Representa uma matriz de elementos de [TransitionsGroup](transitionsgroup.md) que especificam as transições do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="2e0d3-121">Represents an array of [TransitionsGroup](transitionsgroup.md) elements that specify time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="2e0d3-122">Transições</span><span class="sxs-lookup"><span data-stu-id="2e0d3-122">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="2e0d3-123">Representa uma matriz de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="2e0d3-123">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2e0d3-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2e0d3-124">Parent elements</span></span>

|<span data-ttu-id="2e0d3-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2e0d3-125">**Element**</span></span>|<span data-ttu-id="2e0d3-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2e0d3-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2e0d3-127">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="2e0d3-127">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="2e0d3-128">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2e0d3-128">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="2e0d3-129">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="2e0d3-129">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="2e0d3-130">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2e0d3-130">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2e0d3-131">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="2e0d3-131">Remarks</span></span>

<span data-ttu-id="2e0d3-132">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="2e0d3-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2e0d3-133">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="2e0d3-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2e0d3-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="2e0d3-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2e0d3-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2e0d3-135">Schema Name</span></span>  <br/> |<span data-ttu-id="2e0d3-136">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="2e0d3-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="2e0d3-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2e0d3-137">Validation File</span></span>  <br/> |<span data-ttu-id="2e0d3-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2e0d3-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2e0d3-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2e0d3-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="2e0d3-140">False</span><span class="sxs-lookup"><span data-stu-id="2e0d3-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2e0d3-141">Ver também</span><span class="sxs-lookup"><span data-stu-id="2e0d3-141">See also</span></span>

- [<span data-ttu-id="2e0d3-142">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2e0d3-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

