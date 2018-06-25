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
description: O elemento de EndTimeZone define o fuso horário para a hora de término de uma CalendarItem ou MeetingRequest.
ms.openlocfilehash: 65eeedcc7c4d0e616ae54d4e2545fd310e9ad905
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752067"
---
# <a name="endtimezone"></a><span data-ttu-id="90522-103">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="90522-103">EndTimeZone</span></span>

<span data-ttu-id="90522-104">O elemento de **EndTimeZone** define o fuso horário para a hora de término de uma [CalendarItem](calendaritem.md) ou [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="90522-104">The **EndTimeZone** element defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>
  
```xml
<EndTimeZone Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</EndTimeZone>
```

 <span data-ttu-id="90522-105">**TimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="90522-105">**TimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="90522-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="90522-106">Attributes and elements</span></span>

<span data-ttu-id="90522-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="90522-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="90522-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="90522-108">Attributes</span></span>

|<span data-ttu-id="90522-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="90522-109">**Attribute**</span></span>|<span data-ttu-id="90522-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="90522-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="90522-111">Id</span><span class="sxs-lookup"><span data-stu-id="90522-111">Id</span></span>  <br/> |<span data-ttu-id="90522-112">Representa o identificador exclusivo da definição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="90522-112">Represents the unique identifier of the time zone definition.</span></span>  <br/> |
|<span data-ttu-id="90522-113">Nome</span><span class="sxs-lookup"><span data-stu-id="90522-113">Name</span></span>  <br/> |<span data-ttu-id="90522-114">Representa o nome descritivo da definição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="90522-114">Represents the descriptive name of the time zone definition.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="90522-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="90522-115">Child elements</span></span>

|<span data-ttu-id="90522-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="90522-116">**Element**</span></span>|<span data-ttu-id="90522-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="90522-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90522-118">Períodos</span><span class="sxs-lookup"><span data-stu-id="90522-118">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="90522-119">Representa uma matriz de elementos do [período](period.md) que definem o deslocamento de tempo em fases diferentes do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="90522-119">Represents an array of [Period](period.md) elements that define the time offset at different stages of the time zone.</span></span>  <br/> |
|[<span data-ttu-id="90522-120">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="90522-120">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="90522-121">Representa uma matriz de elementos de [TransitionsGroup](transitionsgroup.md) que especificam as transições do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="90522-121">Represents an array of [TransitionsGroup](transitionsgroup.md) elements that specify time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="90522-122">Transições</span><span class="sxs-lookup"><span data-stu-id="90522-122">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="90522-123">Representa uma matriz de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="90522-123">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="90522-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="90522-124">Parent elements</span></span>

|<span data-ttu-id="90522-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="90522-125">**Element**</span></span>|<span data-ttu-id="90522-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="90522-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90522-127">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="90522-127">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="90522-128">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="90522-128">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="90522-129">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="90522-129">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="90522-130">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="90522-130">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="90522-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="90522-131">Remarks</span></span>

<span data-ttu-id="90522-132">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="90522-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="90522-133">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="90522-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="90522-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="90522-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="90522-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="90522-135">Schema Name</span></span>  <br/> |<span data-ttu-id="90522-136">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="90522-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="90522-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="90522-137">Validation File</span></span>  <br/> |<span data-ttu-id="90522-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="90522-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="90522-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="90522-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="90522-140">False</span><span class="sxs-lookup"><span data-stu-id="90522-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="90522-141">Ver também</span><span class="sxs-lookup"><span data-stu-id="90522-141">See also</span></span>



- [<span data-ttu-id="90522-142">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="90522-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

