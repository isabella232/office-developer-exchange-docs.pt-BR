---
title: RecurrenceId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurrenceId
api_type:
- schema
ms.assetid: 9ef3569d-ee56-4b22-b008-609fb3337da7
description: O elemento RecurrenceId é usado para identificar uma instância específica de um item de calendário recorrente.
ms.openlocfilehash: 078bec85e1ca1530137f9935365d7dd3e530ea34
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825005"
---
# <a name="recurrenceid"></a><span data-ttu-id="df5fb-103">RecurrenceId</span><span class="sxs-lookup"><span data-stu-id="df5fb-103">RecurrenceId</span></span>

<span data-ttu-id="df5fb-104">O elemento **RecurrenceId** é usado para identificar uma instância específica de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="df5fb-104">The **RecurrenceId** element is used to identify a specific instance of a recurring calendar item.</span></span> 
  
```xml
<RecurrenceId/>
```

 <span data-ttu-id="df5fb-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="df5fb-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="df5fb-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="df5fb-106">Attributes and elements</span></span>

<span data-ttu-id="df5fb-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="df5fb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="df5fb-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="df5fb-108">Attributes</span></span>

<span data-ttu-id="df5fb-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="df5fb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="df5fb-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="df5fb-110">Child elements</span></span>

<span data-ttu-id="df5fb-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="df5fb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="df5fb-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="df5fb-112">Parent elements</span></span>

|<span data-ttu-id="df5fb-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="df5fb-113">**Element**</span></span>|<span data-ttu-id="df5fb-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="df5fb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="df5fb-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="df5fb-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="df5fb-116">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="df5fb-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="df5fb-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="df5fb-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="df5fb-118">Representa uma mensagem de reunião.</span><span class="sxs-lookup"><span data-stu-id="df5fb-118">Represents a meeting message.</span></span>  <br/> |
|[<span data-ttu-id="df5fb-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="df5fb-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="df5fb-120">Representa uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="df5fb-120">Represents a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="df5fb-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="df5fb-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="df5fb-122">Representa uma resposta de reunião.</span><span class="sxs-lookup"><span data-stu-id="df5fb-122">Represents a meeting response.</span></span>  <br/> |
|[<span data-ttu-id="df5fb-123">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="df5fb-123">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="df5fb-124">Representa o cancelamento da reunião.</span><span class="sxs-lookup"><span data-stu-id="df5fb-124">Represents a meeting cancellation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="df5fb-125">Text value</span><span class="sxs-lookup"><span data-stu-id="df5fb-125">Text value</span></span>

<span data-ttu-id="df5fb-126">O valor de texto representa um valor de data/hora que identifica uma ocorrência de calendário.</span><span class="sxs-lookup"><span data-stu-id="df5fb-126">The text value represents a date/time value that identifies a calendar occurrence.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="df5fb-127">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="df5fb-127">Remarks</span></span>

<span data-ttu-id="df5fb-128">Essa propriedade é usada com a propriedade [UID](uid.md) para identificar uma instância específica de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="df5fb-128">This property is used with the [UID](uid.md) property to identify a specific instance of a recurring calendar item.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="df5fb-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="df5fb-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="df5fb-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="df5fb-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="df5fb-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="df5fb-131">Schema Name</span></span>  <br/> |<span data-ttu-id="df5fb-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="df5fb-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="df5fb-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="df5fb-133">Validation File</span></span>  <br/> |<span data-ttu-id="df5fb-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="df5fb-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="df5fb-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="df5fb-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="df5fb-136">False</span><span class="sxs-lookup"><span data-stu-id="df5fb-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="df5fb-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="df5fb-137">See also</span></span>



- [<span data-ttu-id="df5fb-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="df5fb-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

