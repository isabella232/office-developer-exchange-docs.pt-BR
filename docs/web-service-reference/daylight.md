---
title: Norte
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
description: O elemento Daylight representa a data e hora em que o horário se altera do horário padrão para o horário de verão.
ms.openlocfilehash: bf2041cb4677f837ddb5b399041f1c19a7b5f577
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457456"
---
# <a name="daylight"></a><span data-ttu-id="e6335-103">Norte</span><span class="sxs-lookup"><span data-stu-id="e6335-103">Daylight</span></span>

<span data-ttu-id="e6335-104">O elemento **Daylight** representa a data e hora em que o horário se altera do horário padrão para o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="e6335-104">The **Daylight** element represents the date and time when the time changes from standard time to daylight saving time.</span></span> 
  
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

<span data-ttu-id="e6335-105">**Timechangtype**</span><span class="sxs-lookup"><span data-stu-id="e6335-105">**TimeChangeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e6335-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e6335-106">Attributes and elements</span></span>

<span data-ttu-id="e6335-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e6335-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e6335-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e6335-108">Attributes</span></span>

|<span data-ttu-id="e6335-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="e6335-109">**Attribute**</span></span>|<span data-ttu-id="e6335-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e6335-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e6335-111">**TimeZoneName**</span><span class="sxs-lookup"><span data-stu-id="e6335-111">**TimeZoneName**</span></span> <br/> |<span data-ttu-id="e6335-112">Descreve o nome do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="e6335-112">Describes the name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e6335-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e6335-113">Child elements</span></span>

|<span data-ttu-id="e6335-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e6335-114">**Element**</span></span>|<span data-ttu-id="e6335-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e6335-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e6335-116">Offset</span><span class="sxs-lookup"><span data-stu-id="e6335-116">Offset</span></span>](offset.md) <br/> |<span data-ttu-id="e6335-117">Descreve o deslocamento do [BaseOffset](baseoffset.md).</span><span class="sxs-lookup"><span data-stu-id="e6335-117">Describes the offset from the [BaseOffset](baseoffset.md).</span></span> <span data-ttu-id="e6335-118">O deslocamento base além desse deslocamento identifica o tempo de acordo com o horário padrão ou de verão.</span><span class="sxs-lookup"><span data-stu-id="e6335-118">The base offset in addition to this offset identifies the time according to whether it is standard or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="e6335-119">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="e6335-119">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="e6335-120">Descreve um padrão relativo de recorrência anual para um padrão de data de transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="e6335-120">Describes a relative yearly recurrence pattern for a time zone transition date pattern.</span></span>  <br/> |
|[<span data-ttu-id="e6335-121">AbsoluteDate</span><span class="sxs-lookup"><span data-stu-id="e6335-121">AbsoluteDate</span></span>](absolutedate.md) <br/> |<span data-ttu-id="e6335-122">Representa a data em que o horário muda de horário padrão ou de horário de verão.</span><span class="sxs-lookup"><span data-stu-id="e6335-122">Represents the date when the time changes from standard or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="e6335-123">Tempo (timechangtype)</span><span class="sxs-lookup"><span data-stu-id="e6335-123">Time (TimeChangeType)</span></span>](time-timechangetype.md) <br/> |<span data-ttu-id="e6335-124">Descreve o momento em que a hora é alterada entre o horário padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="e6335-124">Describes the time when the time changes between standard time and daylight saving time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e6335-125">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e6335-125">Parent elements</span></span>

|<span data-ttu-id="e6335-126">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e6335-126">**Element**</span></span>|<span data-ttu-id="e6335-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e6335-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e6335-128">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="e6335-128">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="e6335-129">Representa o fuso horário do local onde a reunião está hospedada.</span><span class="sxs-lookup"><span data-stu-id="e6335-129">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e6335-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="e6335-130">Remarks</span></span>

<span data-ttu-id="e6335-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="e6335-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e6335-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e6335-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e6335-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="e6335-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e6335-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e6335-134">Schema Name</span></span>  <br/> |<span data-ttu-id="e6335-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e6335-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="e6335-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e6335-136">Validation File</span></span>  <br/> |<span data-ttu-id="e6335-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e6335-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e6335-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e6335-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="e6335-139">False</span><span class="sxs-lookup"><span data-stu-id="e6335-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e6335-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="e6335-140">See also</span></span>

- [<span data-ttu-id="e6335-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e6335-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

