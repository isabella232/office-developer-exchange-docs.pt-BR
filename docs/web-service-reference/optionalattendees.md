---
title: OptionalAttendees
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OptionalAttendees
api_type:
- schema
ms.assetid: e7c80c4d-3794-45e9-986f-6a8a687df0a4
description: O elemento OptionalAttendees representa a participantes que não são necessários para participar de uma reunião.
ms.openlocfilehash: d5d994f7e85a47b14ab47f58fb73533cf961f7e6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824658"
---
# <a name="optionalattendees"></a><span data-ttu-id="ed853-103">OptionalAttendees</span><span class="sxs-lookup"><span data-stu-id="ed853-103">OptionalAttendees</span></span>

<span data-ttu-id="ed853-104">O elemento **OptionalAttendees** representa a participantes que não são necessários para participar de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="ed853-104">The **OptionalAttendees** element represents attendees who are not required to attend a meeting.</span></span> 
  
```xml
<OptionalAttendees>
   <Attendee/>
</OptionalAttendees>
```

 <span data-ttu-id="ed853-105">**NonEmptyArrayOfAttendeesType**</span><span class="sxs-lookup"><span data-stu-id="ed853-105">**NonEmptyArrayOfAttendeesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ed853-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ed853-106">Attributes and elements</span></span>

<span data-ttu-id="ed853-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ed853-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ed853-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ed853-108">Attributes</span></span>

<span data-ttu-id="ed853-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ed853-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ed853-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ed853-110">Child elements</span></span>

|<span data-ttu-id="ed853-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ed853-111">**Element**</span></span>|<span data-ttu-id="ed853-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ed853-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed853-113">Attendee</span><span class="sxs-lookup"><span data-stu-id="ed853-113">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="ed853-114">Representa os participantes e recursos para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="ed853-114">Represents attendees and resources for a meeting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ed853-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ed853-115">Parent elements</span></span>

|<span data-ttu-id="ed853-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ed853-116">**Element**</span></span>|<span data-ttu-id="ed853-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ed853-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed853-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="ed853-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="ed853-119">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ed853-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ed853-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="ed853-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="ed853-121">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ed853-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ed853-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="ed853-122">Remarks</span></span>

<span data-ttu-id="ed853-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="ed853-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ed853-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ed853-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ed853-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="ed853-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ed853-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ed853-126">Schema name</span></span>  <br/> |<span data-ttu-id="ed853-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ed853-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="ed853-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ed853-128">Validation file</span></span>  <br/> |<span data-ttu-id="ed853-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ed853-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ed853-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="ed853-130">Can be empty</span></span>  <br/> |<span data-ttu-id="ed853-131">False</span><span class="sxs-lookup"><span data-stu-id="ed853-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ed853-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="ed853-132">See also</span></span>



- [<span data-ttu-id="ed853-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ed853-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

