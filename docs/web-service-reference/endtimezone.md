---
title: EndTimeZone
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndTimeZone
api_type:
- schema
ms.assetid: 6c53c337-be60-4d22-9e9e-a0c140c5e913
description: O elemento endtimezone define o fuso horário para a hora de término de um CalendarItem ou MeetingRequest.
ms.openlocfilehash: 83ab2ab90e2bed7658fe83ed33a72b60d5f10135
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462982"
---
# <a name="endtimezone"></a><span data-ttu-id="ee8b5-103">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="ee8b5-103">EndTimeZone</span></span>

<span data-ttu-id="ee8b5-104">O elemento **endtimezone** define o fuso horário para a hora de término de um [CalendarItem](calendaritem.md) ou [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="ee8b5-104">The **EndTimeZone** element defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>
  
```xml
<EndTimeZone Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</EndTimeZone>
```

 <span data-ttu-id="ee8b5-105">**TimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="ee8b5-105">**TimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ee8b5-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ee8b5-106">Attributes and elements</span></span>

<span data-ttu-id="ee8b5-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ee8b5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ee8b5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ee8b5-108">Attributes</span></span>

|<span data-ttu-id="ee8b5-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="ee8b5-109">**Attribute**</span></span>|<span data-ttu-id="ee8b5-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ee8b5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ee8b5-111">Id</span><span class="sxs-lookup"><span data-stu-id="ee8b5-111">Id</span></span>  <br/> |<span data-ttu-id="ee8b5-112">Representa o identificador exclusivo da definição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="ee8b5-112">Represents the unique identifier of the time zone definition.</span></span>  <br/> |
|<span data-ttu-id="ee8b5-113">Nome</span><span class="sxs-lookup"><span data-stu-id="ee8b5-113">Name</span></span>  <br/> |<span data-ttu-id="ee8b5-114">Representa o nome descritivo da definição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="ee8b5-114">Represents the descriptive name of the time zone definition.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ee8b5-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ee8b5-115">Child elements</span></span>

|<span data-ttu-id="ee8b5-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ee8b5-116">**Element**</span></span>|<span data-ttu-id="ee8b5-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ee8b5-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ee8b5-118">Períodos</span><span class="sxs-lookup"><span data-stu-id="ee8b5-118">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="ee8b5-119">Representa uma matriz de elementos [period](period.md) que definem a diferença de tempo em diferentes estágios do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="ee8b5-119">Represents an array of [Period](period.md) elements that define the time offset at different stages of the time zone.</span></span>  <br/> |
|[<span data-ttu-id="ee8b5-120">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="ee8b5-120">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="ee8b5-121">Representa uma matriz de elementos [TransitionsGroup](transitionsgroup.md) que especificam transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="ee8b5-121">Represents an array of [TransitionsGroup](transitionsgroup.md) elements that specify time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="ee8b5-122">Transições</span><span class="sxs-lookup"><span data-stu-id="ee8b5-122">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="ee8b5-123">Representa uma matriz de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="ee8b5-123">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ee8b5-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ee8b5-124">Parent elements</span></span>

|<span data-ttu-id="ee8b5-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ee8b5-125">**Element**</span></span>|<span data-ttu-id="ee8b5-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ee8b5-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ee8b5-127">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="ee8b5-127">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="ee8b5-128">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ee8b5-128">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ee8b5-129">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="ee8b5-129">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="ee8b5-130">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ee8b5-130">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ee8b5-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="ee8b5-131">Remarks</span></span>

<span data-ttu-id="ee8b5-132">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="ee8b5-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ee8b5-133">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ee8b5-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ee8b5-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="ee8b5-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ee8b5-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ee8b5-135">Schema Name</span></span>  <br/> |<span data-ttu-id="ee8b5-136">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ee8b5-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="ee8b5-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ee8b5-137">Validation File</span></span>  <br/> |<span data-ttu-id="ee8b5-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ee8b5-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ee8b5-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ee8b5-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="ee8b5-140">False</span><span class="sxs-lookup"><span data-stu-id="ee8b5-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ee8b5-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="ee8b5-141">See also</span></span>



- [<span data-ttu-id="ee8b5-142">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ee8b5-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

