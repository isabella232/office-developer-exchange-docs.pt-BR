---
title: Standard
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Standard
api_type:
- schema
ms.assetid: d598f0a6-e296-423f-8ce5-3da57cfd8189
description: O elemento padrão representa a data e hora em que o horário muda do horário de verão para o horário padrão.
ms.openlocfilehash: 1214a1debb53c9a31ca7c92a0c9e5c0722960d75
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467561"
---
# <a name="standard"></a><span data-ttu-id="803df-103">Standard</span><span class="sxs-lookup"><span data-stu-id="803df-103">Standard</span></span>

<span data-ttu-id="803df-104">O elemento **padrão** representa a data e hora em que o horário muda do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="803df-104">The **Standard** element represents the date and time when the time changes from daylight saving time to standard time.</span></span> 
  
```xml
<Standard TimeZoneName="">
   <Offset/>
   <RelativeYearlyRecurrence/>
   <Time/>
</Standard>
```

```xml
<Standard TimeZoneName="">
   <Offset/>
   <AbsoluteDate/>
   <Time/>
</Standard>
```

<span data-ttu-id="803df-105">**Timechangtype**</span><span class="sxs-lookup"><span data-stu-id="803df-105">**TimeChangeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="803df-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="803df-106">Attributes and elements</span></span>

<span data-ttu-id="803df-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="803df-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="803df-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="803df-108">Attributes</span></span>

|<span data-ttu-id="803df-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="803df-109">**Attribute**</span></span>|<span data-ttu-id="803df-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="803df-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="803df-111">**TimeZoneName**</span><span class="sxs-lookup"><span data-stu-id="803df-111">**TimeZoneName**</span></span> <br/> |<span data-ttu-id="803df-112">Descreve o nome do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="803df-112">Describes the name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="803df-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="803df-113">Child elements</span></span>

|<span data-ttu-id="803df-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="803df-114">**Element**</span></span>|<span data-ttu-id="803df-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="803df-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="803df-116">Offset</span><span class="sxs-lookup"><span data-stu-id="803df-116">Offset</span></span>](offset.md) <br/> |<span data-ttu-id="803df-117">Descreve o deslocamento do [BaseOffset](baseoffset.md).</span><span class="sxs-lookup"><span data-stu-id="803df-117">Describes the offset from the [BaseOffset](baseoffset.md).</span></span> <span data-ttu-id="803df-118">Junto com o elemento **BaseOffset** , o elemento **offset** identifica se o horário é horário padrão ou horário de verão.</span><span class="sxs-lookup"><span data-stu-id="803df-118">Together with the **BaseOffset** element, the **Offset** element identifies whether the time is standard time or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="803df-119">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="803df-119">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="803df-120">Descreve um padrão relativo de recorrência anual para uma data de transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="803df-120">Describes a relative yearly recurrence pattern for a time zone transition date.</span></span>  <br/> |
|[<span data-ttu-id="803df-121">AbsoluteDate</span><span class="sxs-lookup"><span data-stu-id="803df-121">AbsoluteDate</span></span>](absolutedate.md) <br/> |<span data-ttu-id="803df-122">Representa a data em que o horário muda do horário padrão ou horário de verão.</span><span class="sxs-lookup"><span data-stu-id="803df-122">Represents the date when the time changes from standard time or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="803df-123">Tempo (timechangtype)</span><span class="sxs-lookup"><span data-stu-id="803df-123">Time (TimeChangeType)</span></span>](time-timechangetype.md) <br/> |<span data-ttu-id="803df-124">Descreve o momento em que a hora é alterada entre o horário padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="803df-124">Describes the time when the time changes between standard time and daylight saving time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="803df-125">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="803df-125">Parent elements</span></span>

|<span data-ttu-id="803df-126">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="803df-126">**Element**</span></span>|<span data-ttu-id="803df-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="803df-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="803df-128">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="803df-128">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="803df-129">Representa o fuso horário do local onde a reunião está hospedada.</span><span class="sxs-lookup"><span data-stu-id="803df-129">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="803df-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="803df-130">Remarks</span></span>

<span data-ttu-id="803df-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="803df-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="803df-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="803df-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="803df-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="803df-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="803df-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="803df-134">Schema Name</span></span>  <br/> |<span data-ttu-id="803df-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="803df-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="803df-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="803df-136">Validation File</span></span>  <br/> |<span data-ttu-id="803df-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="803df-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="803df-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="803df-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="803df-139">False</span><span class="sxs-lookup"><span data-stu-id="803df-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="803df-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="803df-140">See also</span></span>

- [<span data-ttu-id="803df-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="803df-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

