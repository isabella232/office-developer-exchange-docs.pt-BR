---
title: RequiredAttendees
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RequiredAttendees
api_type:
- schema
ms.assetid: 422f8d44-b0eb-49ca-af0f-0e22b54c78d2
description: O elemento RequiredAttendees representa participantes necessários para participar de uma reunião.
ms.openlocfilehash: 9630be828f459808b61602448a4675aac07b0106
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825149"
---
# <a name="requiredattendees"></a><span data-ttu-id="3b957-103">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="3b957-103">RequiredAttendees</span></span>

<span data-ttu-id="3b957-104">O elemento **RequiredAttendees** representa participantes necessários para participar de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="3b957-104">The **RequiredAttendees** element represents attendees that are required to attend a meeting.</span></span> 
  
```xml
<RequiredAttendees>
   <Attendee/>
</RequiredAttendees>
```

 <span data-ttu-id="3b957-105">**NonEmptyArrayOfAttendeesType**</span><span class="sxs-lookup"><span data-stu-id="3b957-105">**NonEmptyArrayOfAttendeesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3b957-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3b957-106">Attributes and elements</span></span>

<span data-ttu-id="3b957-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3b957-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3b957-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="3b957-108">Attributes</span></span>

<span data-ttu-id="3b957-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3b957-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3b957-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3b957-110">Child elements</span></span>

|<span data-ttu-id="3b957-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3b957-111">**Element**</span></span>|<span data-ttu-id="3b957-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3b957-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b957-113">Attendee</span><span class="sxs-lookup"><span data-stu-id="3b957-113">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="3b957-114">Representa os participantes e recursos para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="3b957-114">Represents attendees and resources for a meeting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3b957-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3b957-115">Parent elements</span></span>

|<span data-ttu-id="3b957-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3b957-116">**Element**</span></span>|<span data-ttu-id="3b957-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3b957-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b957-118">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="3b957-118">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="3b957-119">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3b957-119">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="3b957-120">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="3b957-120">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="3b957-121">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3b957-121">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3b957-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="3b957-122">Remarks</span></span>

<span data-ttu-id="3b957-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="3b957-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3b957-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3b957-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3b957-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="3b957-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3b957-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3b957-126">Schema name</span></span>  <br/> |<span data-ttu-id="3b957-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3b957-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="3b957-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3b957-128">Validation file</span></span>  <br/> |<span data-ttu-id="3b957-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3b957-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3b957-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="3b957-130">Can be empty</span></span>  <br/> |<span data-ttu-id="3b957-131">False</span><span class="sxs-lookup"><span data-stu-id="3b957-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3b957-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="3b957-132">See also</span></span>



- [<span data-ttu-id="3b957-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3b957-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

