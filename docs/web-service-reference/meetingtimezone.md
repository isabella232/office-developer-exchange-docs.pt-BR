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
ms.openlocfilehash: aef4ac4e7571ded6920cbaf90e2895d421068f55
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465468"
---
# <a name="meetingtimezone"></a><span data-ttu-id="fa308-103">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="fa308-103">MeetingTimeZone</span></span>

<span data-ttu-id="fa308-104">O elemento **MeetingTimeZone** representa o fuso horário do local onde a reunião está hospedada.</span><span class="sxs-lookup"><span data-stu-id="fa308-104">The **MeetingTimeZone** element represents the time zone of the location where the meeting is hosted.</span></span> 
  
```xml
<MeetingTimeZone>
   <BaseOffset/>
   <Standard/>
   <Daylight/>
</MeetingTimeZone>
```

 <span data-ttu-id="fa308-105">**TimeZoneType**</span><span class="sxs-lookup"><span data-stu-id="fa308-105">**TimeZoneType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fa308-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="fa308-106">Attributes and elements</span></span>

<span data-ttu-id="fa308-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fa308-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fa308-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="fa308-108">Attributes</span></span>

|<span data-ttu-id="fa308-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="fa308-109">**Attribute**</span></span>|<span data-ttu-id="fa308-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fa308-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fa308-111">**TimeZoneName**</span><span class="sxs-lookup"><span data-stu-id="fa308-111">**TimeZoneName**</span></span> <br/> |<span data-ttu-id="fa308-112">Descreve o nome do fuso horário.</span><span class="sxs-lookup"><span data-stu-id="fa308-112">Describes the name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fa308-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fa308-113">Child elements</span></span>

|<span data-ttu-id="fa308-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fa308-114">**Element**</span></span>|<span data-ttu-id="fa308-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fa308-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa308-116">BaseOffset</span><span class="sxs-lookup"><span data-stu-id="fa308-116">BaseOffset</span></span>](baseoffset.md) <br/> |<span data-ttu-id="fa308-117">Representa o deslocamento por hora do UTC para o fuso horário atual.</span><span class="sxs-lookup"><span data-stu-id="fa308-117">Represents the hourly offset from UTC for the current time zone.</span></span>  <br/> |
|[<span data-ttu-id="fa308-118">Standard</span><span class="sxs-lookup"><span data-stu-id="fa308-118">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="fa308-119">Representa a data e a hora em que o horário muda do horário de verão para o horário padrão.</span><span class="sxs-lookup"><span data-stu-id="fa308-119">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="fa308-120">Norte</span><span class="sxs-lookup"><span data-stu-id="fa308-120">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="fa308-121">Representa a data e a hora em que o horário muda do horário padrão para o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="fa308-121">Represents the date and time when the time changes from standard time to daylight saving time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fa308-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fa308-122">Parent elements</span></span>

|<span data-ttu-id="fa308-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fa308-123">**Element**</span></span>|<span data-ttu-id="fa308-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fa308-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa308-125">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="fa308-125">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="fa308-126">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fa308-126">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="fa308-127">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="fa308-127">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="fa308-128">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fa308-128">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fa308-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="fa308-129">Remarks</span></span>

<span data-ttu-id="fa308-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="fa308-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fa308-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="fa308-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fa308-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="fa308-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fa308-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fa308-133">Schema Name</span></span>  <br/> |<span data-ttu-id="fa308-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="fa308-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="fa308-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fa308-135">Validation File</span></span>  <br/> |<span data-ttu-id="fa308-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="fa308-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fa308-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="fa308-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="fa308-138">False</span><span class="sxs-lookup"><span data-stu-id="fa308-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fa308-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="fa308-139">See also</span></span>



- [<span data-ttu-id="fa308-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fa308-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

