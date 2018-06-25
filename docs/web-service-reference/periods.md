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
description: O elemento de períodos representa uma matriz de períodos que definem o deslocamento de tempo em fases diferentes do fuso horário.
ms.openlocfilehash: f2f9cf7c724b453d2b1975fcf72c55bc02caa54b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824729"
---
# <a name="periods"></a><span data-ttu-id="15dfa-103">Períodos</span><span class="sxs-lookup"><span data-stu-id="15dfa-103">Periods</span></span>

<span data-ttu-id="15dfa-104">O elemento de **períodos** representa uma matriz de períodos que definem o deslocamento de tempo em fases diferentes do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="15dfa-104">The **Periods** element represents an array of periods that define the time offset at different stages of the time zone.</span></span> 
  
```xml
<Periods>
   <Period/>
</Periods>
```

 <span data-ttu-id="15dfa-105">**NonEmptyArrayOfPeriodsType**</span><span class="sxs-lookup"><span data-stu-id="15dfa-105">**NonEmptyArrayOfPeriodsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="15dfa-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="15dfa-106">Attributes and elements</span></span>

<span data-ttu-id="15dfa-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="15dfa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="15dfa-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="15dfa-108">Attributes</span></span>

<span data-ttu-id="15dfa-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="15dfa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="15dfa-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="15dfa-110">Child elements</span></span>

|<span data-ttu-id="15dfa-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="15dfa-111">**Element**</span></span>|<span data-ttu-id="15dfa-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="15dfa-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15dfa-113">Period</span><span class="sxs-lookup"><span data-stu-id="15dfa-113">Period</span></span>](period.md) <br/> |<span data-ttu-id="15dfa-114">Define o nome, a diferença de horário e o identificador exclusivo de um estágio específico do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="15dfa-114">Defines the name, time offset, and unique identifier for a specific stage of the time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="15dfa-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="15dfa-115">Parent elements</span></span>

|<span data-ttu-id="15dfa-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="15dfa-116">**Element**</span></span>|<span data-ttu-id="15dfa-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="15dfa-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15dfa-118">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="15dfa-118">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="15dfa-119">Define o fuso horário para a hora de início de uma [CalendarItem](calendaritem.md) ou [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="15dfa-119">Defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="15dfa-120">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="15dfa-120">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="15dfa-121">Define o fuso horário para a hora de término de uma [CalendarItem](calendaritem.md) ou [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="15dfa-121">Defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="15dfa-122">Timezonedefinition pela última vez</span><span class="sxs-lookup"><span data-stu-id="15dfa-122">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="15dfa-123">Define um fuso horário.</span><span class="sxs-lookup"><span data-stu-id="15dfa-123">Defines a time zone.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="15dfa-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="15dfa-124">Remarks</span></span>

<span data-ttu-id="15dfa-125">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="15dfa-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="15dfa-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="15dfa-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="15dfa-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="15dfa-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="15dfa-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="15dfa-128">Schema Name</span></span>  <br/> |<span data-ttu-id="15dfa-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="15dfa-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="15dfa-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="15dfa-130">Validation File</span></span>  <br/> |<span data-ttu-id="15dfa-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="15dfa-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="15dfa-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="15dfa-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="15dfa-133">False</span><span class="sxs-lookup"><span data-stu-id="15dfa-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="15dfa-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="15dfa-134">See also</span></span>



- [<span data-ttu-id="15dfa-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="15dfa-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

