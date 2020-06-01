---
title: Iscumprimento (CalendarEventDetails)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsMeeting
api_type:
- schema
ms.assetid: dd6900e4-e4a3-471a-909d-7240ebec501b
description: O elemento issatisfaçing indica se o evento de calendário é uma reunião ou um compromisso.
ms.openlocfilehash: b75dfba203177d6451f3847bf8d1f68014612e1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465993"
---
# <a name="ismeeting-calendareventdetails"></a><span data-ttu-id="de21f-103">Iscumprimento (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="de21f-103">IsMeeting (CalendarEventDetails)</span></span>

<span data-ttu-id="de21f-104">O elemento **Issatisfaçing** indica se o evento de calendário é uma reunião ou um compromisso.</span><span class="sxs-lookup"><span data-stu-id="de21f-104">The **IsMeeting** element indicates whether the calendar event is a meeting or an appointment.</span></span> 
  
[<span data-ttu-id="de21f-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="de21f-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="de21f-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="de21f-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="de21f-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="de21f-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="de21f-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="de21f-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="de21f-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="de21f-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="de21f-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="de21f-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="de21f-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="de21f-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="de21f-112">Iscumprimento (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="de21f-112">IsMeeting (CalendarEventDetails)</span></span>](ismeeting-calendareventdetails.md)
  
```xml
<IsMeeting>true or false</IsMeeting>
```

 <span data-ttu-id="de21f-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="de21f-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="de21f-114">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="de21f-114">Attributes and elements</span></span>

<span data-ttu-id="de21f-115">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="de21f-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="de21f-116">Atributos</span><span class="sxs-lookup"><span data-stu-id="de21f-116">Attributes</span></span>

<span data-ttu-id="de21f-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="de21f-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="de21f-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="de21f-118">Child elements</span></span>

<span data-ttu-id="de21f-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="de21f-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="de21f-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="de21f-120">Parent elements</span></span>

|<span data-ttu-id="de21f-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="de21f-121">**Element**</span></span>|<span data-ttu-id="de21f-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="de21f-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de21f-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="de21f-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="de21f-124">Fornece informações adicionais para um evento de calendário.</span><span class="sxs-lookup"><span data-stu-id="de21f-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="de21f-125">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="de21f-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="de21f-126">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="de21f-126">Text value</span></span>

<span data-ttu-id="de21f-127">Um valor de texto será necessário se esse elemento for retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="de21f-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="de21f-128">Esse elemento é necessário se o elemento [CalendarEventDetails](calendareventdetails.md) for usado.</span><span class="sxs-lookup"><span data-stu-id="de21f-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="de21f-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="de21f-129">Remarks</span></span>

<span data-ttu-id="de21f-130">A diferença entre uma reunião e um compromisso é que uma reunião é um item de calendário que inclui participantes; um compromisso é um item de calendário que não inclui participantes.</span><span class="sxs-lookup"><span data-stu-id="de21f-130">The difference between a meeting and an appointment is that a meeting is a calendar item that includes attendees; an appointment is a calendar item that does not include attendees.</span></span>
  
<span data-ttu-id="de21f-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="de21f-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="de21f-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="de21f-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="de21f-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="de21f-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="de21f-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="de21f-134">Schema Name</span></span>  <br/> |<span data-ttu-id="de21f-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="de21f-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="de21f-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="de21f-136">Validation File</span></span>  <br/> |<span data-ttu-id="de21f-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="de21f-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="de21f-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="de21f-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="de21f-139">False</span><span class="sxs-lookup"><span data-stu-id="de21f-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="de21f-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="de21f-140">See also</span></span>



[<span data-ttu-id="de21f-141">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="de21f-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="de21f-142">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="de21f-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="de21f-143">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="de21f-143">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

