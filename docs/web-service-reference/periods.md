---
title: Períodos
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Periods
api_type:
- schema
ms.assetid: 7920d81d-abba-4232-8bfe-49267b6c9a36
description: O elemento periods representa uma matriz de períodos que definem a diferença de tempo em estágios diferentes do fuso horário.
ms.openlocfilehash: 773457a6e4c0237eaeaf23109a7022427cc7dd0d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467771"
---
# <a name="periods"></a><span data-ttu-id="00c59-103">Períodos</span><span class="sxs-lookup"><span data-stu-id="00c59-103">Periods</span></span>

<span data-ttu-id="00c59-104">O elemento **periods** representa uma matriz de períodos que definem a diferença de tempo em estágios diferentes do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="00c59-104">The **Periods** element represents an array of periods that define the time offset at different stages of the time zone.</span></span> 
  
```xml
<Periods>
   <Period/>
</Periods>
```

 <span data-ttu-id="00c59-105">**NonEmptyArrayOfPeriodsType**</span><span class="sxs-lookup"><span data-stu-id="00c59-105">**NonEmptyArrayOfPeriodsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="00c59-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="00c59-106">Attributes and elements</span></span>

<span data-ttu-id="00c59-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="00c59-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00c59-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="00c59-108">Attributes</span></span>

<span data-ttu-id="00c59-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="00c59-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="00c59-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="00c59-110">Child elements</span></span>

|<span data-ttu-id="00c59-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="00c59-111">**Element**</span></span>|<span data-ttu-id="00c59-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="00c59-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00c59-113">Period</span><span class="sxs-lookup"><span data-stu-id="00c59-113">Period</span></span>](period.md) <br/> |<span data-ttu-id="00c59-114">Define o nome, a diferença de tempo e o identificador exclusivo de um estágio específico do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="00c59-114">Defines the name, time offset, and unique identifier for a specific stage of the time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="00c59-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="00c59-115">Parent elements</span></span>

|<span data-ttu-id="00c59-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="00c59-116">**Element**</span></span>|<span data-ttu-id="00c59-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="00c59-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00c59-118">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="00c59-118">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="00c59-119">Define o fuso horário para a hora de início de um [CalendarItem](calendaritem.md) ou [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="00c59-119">Defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="00c59-120">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="00c59-120">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="00c59-121">Define o fuso horário para a hora de término de um [CalendarItem](calendaritem.md) ou [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="00c59-121">Defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="00c59-122">TimeZoneDefinition</span><span class="sxs-lookup"><span data-stu-id="00c59-122">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="00c59-123">Define um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="00c59-123">Defines a time zone.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="00c59-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="00c59-124">Remarks</span></span>

<span data-ttu-id="00c59-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="00c59-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="00c59-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="00c59-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00c59-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="00c59-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="00c59-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="00c59-128">Schema Name</span></span>  <br/> |<span data-ttu-id="00c59-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="00c59-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="00c59-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="00c59-130">Validation File</span></span>  <br/> |<span data-ttu-id="00c59-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="00c59-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="00c59-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="00c59-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="00c59-133">False</span><span class="sxs-lookup"><span data-stu-id="00c59-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="00c59-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="00c59-134">See also</span></span>



- [<span data-ttu-id="00c59-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="00c59-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

