---
title: MeetingTimeZone
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingTimeZone
api_type:
- schema
ms.assetid: 413b47d9-8126-462c-9a4f-4e771a5e8889
description: O elemento MeetingTimeZone representa o fuso horário do local onde a reunião está hospedada.
ms.openlocfilehash: ce014ac6d8841e451927a94049cb4e8860886fdf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824440"
---
# <a name="meetingtimezone"></a><span data-ttu-id="f3b83-103">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="f3b83-103">MeetingTimeZone</span></span>

<span data-ttu-id="f3b83-104">O elemento **MeetingTimeZone** representa o fuso horário do local onde a reunião está hospedada.</span><span class="sxs-lookup"><span data-stu-id="f3b83-104">The **MeetingTimeZone** element represents the time zone of the location where the meeting is hosted.</span></span> 
  
```xml
<MeetingTimeZone>
   <BaseOffset/>
   <Standard/>
   <Daylight/>
</MeetingTimeZone>
```

 <span data-ttu-id="f3b83-105">**TimeZoneType**</span><span class="sxs-lookup"><span data-stu-id="f3b83-105">**TimeZoneType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f3b83-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f3b83-106">Attributes and elements</span></span>

<span data-ttu-id="f3b83-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f3b83-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3b83-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f3b83-108">Attributes</span></span>

|<span data-ttu-id="f3b83-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="f3b83-109">**Attribute**</span></span>|<span data-ttu-id="f3b83-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f3b83-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f3b83-111">**TimeZoneName**</span><span class="sxs-lookup"><span data-stu-id="f3b83-111">**TimeZoneName**</span></span> <br/> |<span data-ttu-id="f3b83-112">Descreve o nome do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="f3b83-112">Describes the name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f3b83-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f3b83-113">Child elements</span></span>

|<span data-ttu-id="f3b83-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f3b83-114">**Element**</span></span>|<span data-ttu-id="f3b83-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f3b83-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f3b83-116">BaseOffset</span><span class="sxs-lookup"><span data-stu-id="f3b83-116">BaseOffset</span></span>](baseoffset.md) <br/> |<span data-ttu-id="f3b83-117">Representa a por hora deslocamento a partir do UTC para o fuso horário atual.</span><span class="sxs-lookup"><span data-stu-id="f3b83-117">Represents the hourly offset from UTC for the current time zone.</span></span>  <br/> |
|[<span data-ttu-id="f3b83-118">Standard</span><span class="sxs-lookup"><span data-stu-id="f3b83-118">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="f3b83-119">Representa a data e hora de quando o tempo é alterado de horário de verão para a hora padrão.</span><span class="sxs-lookup"><span data-stu-id="f3b83-119">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="f3b83-120">Horário de verão</span><span class="sxs-lookup"><span data-stu-id="f3b83-120">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="f3b83-121">Representa a data e hora de quando o tempo é alterado do período padrão para o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="f3b83-121">Represents the date and time when the time changes from standard time to daylight saving time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f3b83-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f3b83-122">Parent elements</span></span>

|<span data-ttu-id="f3b83-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f3b83-123">**Element**</span></span>|<span data-ttu-id="f3b83-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f3b83-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f3b83-125">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="f3b83-125">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="f3b83-126">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f3b83-126">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="f3b83-127">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="f3b83-127">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="f3b83-128">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f3b83-128">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f3b83-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="f3b83-129">Remarks</span></span>

<span data-ttu-id="f3b83-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="f3b83-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f3b83-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f3b83-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f3b83-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="f3b83-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f3b83-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f3b83-133">Schema Name</span></span>  <br/> |<span data-ttu-id="f3b83-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f3b83-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="f3b83-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f3b83-135">Validation File</span></span>  <br/> |<span data-ttu-id="f3b83-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f3b83-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f3b83-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f3b83-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="f3b83-138">False</span><span class="sxs-lookup"><span data-stu-id="f3b83-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f3b83-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="f3b83-139">See also</span></span>



- [<span data-ttu-id="f3b83-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f3b83-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

