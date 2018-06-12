---
title: Horário de verão
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Daylight
api_type:
- schema
ms.assetid: ea400839-fba8-4a5e-a5d1-9b677afc0ff9
description: O elemento de verão representa a data e hora de quando o tempo é alterado do período padrão para o horário de verão.
ms.openlocfilehash: cdb6ed305f1d77a73b952f8c659991f3b2a8df7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751699"
---
# <a name="daylight"></a><span data-ttu-id="7e729-103">Horário de verão</span><span class="sxs-lookup"><span data-stu-id="7e729-103">Daylight</span></span>

<span data-ttu-id="7e729-104">O elemento de **verão** representa a data e hora de quando o tempo é alterado do período padrão para o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="7e729-104">The **Daylight** element represents the date and time when the time changes from standard time to daylight saving time.</span></span> 
  
```xml
<Daylight TimeZoneName="">
   <Offset/>
   <RelativeYearlyRecurrence/>
   <Time/>
</Daylight>
```

```xml
<Daylight TimeZoneName="">
   <Offset/>
   <AbsoluteDate/>
   <Time/>
</Daylight>
```

<span data-ttu-id="7e729-105">**TimeChangeType**</span><span class="sxs-lookup"><span data-stu-id="7e729-105">**TimeChangeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7e729-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7e729-106">Attributes and elements</span></span>

<span data-ttu-id="7e729-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7e729-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e729-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7e729-108">Attributes</span></span>

|<span data-ttu-id="7e729-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="7e729-109">**Attribute**</span></span>|<span data-ttu-id="7e729-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7e729-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7e729-111">**TimeZoneName**</span><span class="sxs-lookup"><span data-stu-id="7e729-111">**TimeZoneName**</span></span> <br/> |<span data-ttu-id="7e729-112">Descreve o nome do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="7e729-112">Describes the name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7e729-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7e729-113">Child elements</span></span>

|<span data-ttu-id="7e729-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7e729-114">**Element**</span></span>|<span data-ttu-id="7e729-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7e729-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e729-116">Offset</span><span class="sxs-lookup"><span data-stu-id="7e729-116">Offset</span></span>](offset.md) <br/> |<span data-ttu-id="7e729-117">Descreve o deslocamento, desde o [BaseOffset](baseoffset.md).</span><span class="sxs-lookup"><span data-stu-id="7e729-117">Describes the offset from the [BaseOffset](baseoffset.md).</span></span> <span data-ttu-id="7e729-118">Base de deslocamento além este deslocamento identifica a hora de acordo com se ele está standard ou o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="7e729-118">The base offset in addition to this offset identifies the time according to whether it is standard or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="7e729-119">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="7e729-119">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="7e729-120">Descreve um padrão de recorrência anual relativa para um padrão de data de transição do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="7e729-120">Describes a relative yearly recurrence pattern for a time zone transition date pattern.</span></span>  <br/> |
|[<span data-ttu-id="7e729-121">AbsoluteDate</span><span class="sxs-lookup"><span data-stu-id="7e729-121">AbsoluteDate</span></span>](absolutedate.md) <br/> |<span data-ttu-id="7e729-122">Representa a data quando o tempo é alterado de standard ou o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="7e729-122">Represents the date when the time changes from standard or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="7e729-123">Tempo (TimeChangeType)</span><span class="sxs-lookup"><span data-stu-id="7e729-123">Time (TimeChangeType)</span></span>](time-timechangetype.md) <br/> |<span data-ttu-id="7e729-124">Descreve o tempo quando o tempo é alterado entre o período padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="7e729-124">Describes the time when the time changes between standard time and daylight saving time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7e729-125">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7e729-125">Parent elements</span></span>

|<span data-ttu-id="7e729-126">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7e729-126">**Element**</span></span>|<span data-ttu-id="7e729-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7e729-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e729-128">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="7e729-128">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="7e729-129">Representa o fuso horário do local onde a reunião está hospedada.</span><span class="sxs-lookup"><span data-stu-id="7e729-129">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7e729-130">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="7e729-130">Remarks</span></span>

<span data-ttu-id="7e729-131">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="7e729-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e729-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7e729-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e729-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="7e729-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7e729-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7e729-134">Schema Name</span></span>  <br/> |<span data-ttu-id="7e729-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7e729-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="7e729-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7e729-136">Validation File</span></span>  <br/> |<span data-ttu-id="7e729-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7e729-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7e729-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7e729-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="7e729-139">False</span><span class="sxs-lookup"><span data-stu-id="7e729-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e729-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="7e729-140">See also</span></span>

- [<span data-ttu-id="7e729-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7e729-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

