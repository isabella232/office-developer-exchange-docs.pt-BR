---
title: IsRecurring (CalendarEventDetails)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsRecurring
api_type:
- schema
ms.assetid: 42323940-0ccb-4a05-86e4-262bde5e41b0
description: O elemento IsRecurring indica se o evento de calendário é uma instância de um item de calendário recorrente ou de um único item de calendário.
ms.openlocfilehash: f9a9c8b4d2a20d42dbec7cd6fd36935eb0b941f4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530250"
---
# <a name="isrecurring-calendareventdetails"></a><span data-ttu-id="d7d04-103">IsRecurring (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="d7d04-103">IsRecurring (CalendarEventDetails)</span></span>

<span data-ttu-id="d7d04-104">O elemento **IsRecurring** indica se o evento de calendário é uma instância de um item de calendário recorrente ou de um único item de calendário.</span><span class="sxs-lookup"><span data-stu-id="d7d04-104">The **IsRecurring** element indicates whether the calendar event is an instance of a recurring calendar item or a single calendar item.</span></span> 
  
[<span data-ttu-id="d7d04-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d7d04-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="d7d04-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="d7d04-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="d7d04-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="d7d04-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="d7d04-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="d7d04-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="d7d04-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="d7d04-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="d7d04-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="d7d04-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="d7d04-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="d7d04-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="d7d04-112">IsRecurring (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="d7d04-112">IsRecurring (CalendarEventDetails)</span></span>](isrecurring-calendareventdetails.md)
  
```xml
<IsRecurring>true or false</IsRecurring>
```

 <span data-ttu-id="d7d04-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="d7d04-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d7d04-114">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d7d04-114">Attributes and elements</span></span>

<span data-ttu-id="d7d04-115">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d7d04-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d7d04-116">Atributos</span><span class="sxs-lookup"><span data-stu-id="d7d04-116">Attributes</span></span>

<span data-ttu-id="d7d04-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d7d04-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d7d04-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d7d04-118">Child elements</span></span>

<span data-ttu-id="d7d04-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d7d04-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d7d04-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d7d04-120">Parent elements</span></span>

|<span data-ttu-id="d7d04-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d7d04-121">**Element**</span></span>|<span data-ttu-id="d7d04-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d7d04-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7d04-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="d7d04-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="d7d04-124">Fornece informações adicionais sobre um evento de calendário.</span><span class="sxs-lookup"><span data-stu-id="d7d04-124">Provides additional information about a calendar event.</span></span>  <br/> <span data-ttu-id="d7d04-125">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="d7d04-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d7d04-126">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="d7d04-126">Text value</span></span>

<span data-ttu-id="d7d04-127">Um valor de texto será necessário se esse elemento for retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="d7d04-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="d7d04-128">Esse elemento é necessário se o elemento [CalendarEventDetails](calendareventdetails.md) for usado.</span><span class="sxs-lookup"><span data-stu-id="d7d04-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d7d04-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="d7d04-129">Remarks</span></span>

<span data-ttu-id="d7d04-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="d7d04-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d7d04-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d7d04-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d7d04-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="d7d04-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d7d04-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d7d04-133">Schema Name</span></span>  <br/> |<span data-ttu-id="d7d04-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d7d04-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="d7d04-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d7d04-135">Validation File</span></span>  <br/> |<span data-ttu-id="d7d04-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d7d04-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d7d04-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d7d04-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="d7d04-138">False</span><span class="sxs-lookup"><span data-stu-id="d7d04-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d7d04-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="d7d04-139">See also</span></span>



[<span data-ttu-id="d7d04-140">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="d7d04-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="d7d04-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d7d04-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="d7d04-142">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="d7d04-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

