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
description: O elemento StartTimeZone define o fuso horário para a hora de início de um CalendarItem ou MeetingRequest.
ms.openlocfilehash: fa88f676c0f6a7a2e934f51274942ed3bccbc789
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458520"
---
# <a name="starttimezone"></a><span data-ttu-id="59f95-103">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="59f95-103">StartTimeZone</span></span>

<span data-ttu-id="59f95-104">O elemento **StartTimeZone** define o fuso horário para a hora de início de um [CalendarItem](calendaritem.md) ou [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="59f95-104">The **StartTimeZone** element defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>
  
```xml
<StartTimeZone Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</StartTimeZone>
```

<span data-ttu-id="59f95-105">**TimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="59f95-105">**TimeZoneDefinitionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="59f95-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="59f95-106">Attributes and elements</span></span>

<span data-ttu-id="59f95-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="59f95-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59f95-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="59f95-108">Attributes</span></span>

|<span data-ttu-id="59f95-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="59f95-109">**Attribute**</span></span>|<span data-ttu-id="59f95-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="59f95-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="59f95-111">Id</span><span class="sxs-lookup"><span data-stu-id="59f95-111">Id</span></span>  <br/> |<span data-ttu-id="59f95-112">Representa o identificador exclusivo da definição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="59f95-112">Represents the unique identifier of the time zone definition.</span></span>  <br/> |
|<span data-ttu-id="59f95-113">Nome</span><span class="sxs-lookup"><span data-stu-id="59f95-113">Name</span></span>  <br/> |<span data-ttu-id="59f95-114">Representa o nome descritivo da definição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="59f95-114">Represents the descriptive name of the time zone definition.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="59f95-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="59f95-115">Child elements</span></span>

|<span data-ttu-id="59f95-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="59f95-116">**Element**</span></span>|<span data-ttu-id="59f95-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="59f95-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59f95-118">Períodos</span><span class="sxs-lookup"><span data-stu-id="59f95-118">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="59f95-119">Representa uma matriz de elementos [period](period.md) que definem a diferença de tempo em diferentes estágios do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="59f95-119">Represents an array of [Period](period.md) elements that define the time offset at different stages of the time zone.</span></span>  <br/> |
|[<span data-ttu-id="59f95-120">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="59f95-120">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="59f95-121">Representa uma matriz de elementos [TransitionsGroup](transitionsgroup.md) que especificam transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="59f95-121">Represents an array of [TransitionsGroup](transitionsgroup.md) elements that specify time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="59f95-122">Transições</span><span class="sxs-lookup"><span data-stu-id="59f95-122">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="59f95-123">Representa uma matriz de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="59f95-123">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="59f95-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="59f95-124">Parent elements</span></span>

|<span data-ttu-id="59f95-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="59f95-125">**Element**</span></span>|<span data-ttu-id="59f95-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="59f95-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59f95-127">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="59f95-127">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="59f95-128">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="59f95-128">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="59f95-129">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="59f95-129">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="59f95-130">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="59f95-130">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="59f95-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="59f95-131">Remarks</span></span>

<span data-ttu-id="59f95-132">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="59f95-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="59f95-133">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="59f95-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59f95-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="59f95-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="59f95-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="59f95-135">Schema Name</span></span>  <br/> |<span data-ttu-id="59f95-136">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="59f95-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="59f95-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="59f95-137">Validation File</span></span>  <br/> |<span data-ttu-id="59f95-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="59f95-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="59f95-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="59f95-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="59f95-140">False</span><span class="sxs-lookup"><span data-stu-id="59f95-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="59f95-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="59f95-141">See also</span></span>

- [<span data-ttu-id="59f95-142">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="59f95-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

