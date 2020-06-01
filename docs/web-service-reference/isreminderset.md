---
title: ReminderSet
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsReminderSet
api_type:
- schema
ms.assetid: 6aea4cb7-ca14-4949-8e7f-660b565f6556
description: O elemento ReminderSet indica se um lembrete foi definido para o evento de calendário.
ms.openlocfilehash: e2f5fa072b549bdaf636a15313e7dfe72172f768
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460334"
---
# <a name="isreminderset"></a><span data-ttu-id="f796b-103">ReminderSet</span><span class="sxs-lookup"><span data-stu-id="f796b-103">IsReminderSet</span></span>

<span data-ttu-id="f796b-104">O elemento **ReminderSet** indica se um lembrete foi definido para o evento de calendário.</span><span class="sxs-lookup"><span data-stu-id="f796b-104">The **IsReminderSet** element indicates whether a reminder has been set for the calendar event.</span></span> 
  
[<span data-ttu-id="f796b-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="f796b-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="f796b-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="f796b-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="f796b-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="f796b-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="f796b-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="f796b-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="f796b-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="f796b-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="f796b-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="f796b-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="f796b-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="f796b-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="f796b-112">ReminderSet</span><span class="sxs-lookup"><span data-stu-id="f796b-112">IsReminderSet</span></span>](isreminderset.md)
  
```xml
<IsReminderSet>true or false</IsReminderSet>
```

 <span data-ttu-id="f796b-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="f796b-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f796b-114">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f796b-114">Attributes and elements</span></span>

<span data-ttu-id="f796b-115">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f796b-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f796b-116">Atributos</span><span class="sxs-lookup"><span data-stu-id="f796b-116">Attributes</span></span>

<span data-ttu-id="f796b-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f796b-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f796b-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f796b-118">Child elements</span></span>

<span data-ttu-id="f796b-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f796b-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f796b-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f796b-120">Parent elements</span></span>

|<span data-ttu-id="f796b-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f796b-121">**Element**</span></span>|<span data-ttu-id="f796b-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f796b-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f796b-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="f796b-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="f796b-124">Fornece informações adicionais sobre um evento de calendário.</span><span class="sxs-lookup"><span data-stu-id="f796b-124">Provides additional information about a calendar event.</span></span>  <br/> <span data-ttu-id="f796b-125">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="f796b-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f796b-126">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="f796b-126">Text value</span></span>

<span data-ttu-id="f796b-127">Um valor de texto será necessário se esse elemento for retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="f796b-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="f796b-128">Este elemento é necessário se o elemento [CalendarEventDetails](calendareventdetails.md) for usado, a menos que o elemento [IsPrivate](isprivate.md) esteja definido como **true**.</span><span class="sxs-lookup"><span data-stu-id="f796b-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used unless the [IsPrivate](isprivate.md) element is set to **true**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f796b-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="f796b-129">Remarks</span></span>

<span data-ttu-id="f796b-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="f796b-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f796b-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f796b-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f796b-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="f796b-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f796b-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f796b-133">Schema Name</span></span>  <br/> |<span data-ttu-id="f796b-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f796b-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="f796b-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f796b-135">Validation File</span></span>  <br/> |<span data-ttu-id="f796b-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f796b-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f796b-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f796b-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="f796b-138">False</span><span class="sxs-lookup"><span data-stu-id="f796b-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f796b-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="f796b-139">See also</span></span>



[<span data-ttu-id="f796b-140">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="f796b-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="f796b-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="f796b-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="f796b-142">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="f796b-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

