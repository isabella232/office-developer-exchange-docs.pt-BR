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
description: O elemento IsRecurring indica se o evento de calendário é uma instância de um item de calendário recorrente ou um item de calendário único.
ms.openlocfilehash: 87a168dc48bdd5ba2ea9398dd84f696e7729db44
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824103"
---
# <a name="isrecurring-calendareventdetails"></a><span data-ttu-id="95d89-103">IsRecurring (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="95d89-103">IsRecurring (CalendarEventDetails)</span></span>

<span data-ttu-id="95d89-104">O elemento **IsRecurring** indica se o evento de calendário é uma instância de um item de calendário recorrente ou um item de calendário único.</span><span class="sxs-lookup"><span data-stu-id="95d89-104">The **IsRecurring** element indicates whether the calendar event is an instance of a recurring calendar item or a single calendar item.</span></span> 
  
[<span data-ttu-id="95d89-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="95d89-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="95d89-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="95d89-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="95d89-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="95d89-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="95d89-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="95d89-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="95d89-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="95d89-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="95d89-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="95d89-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="95d89-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="95d89-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="95d89-112">IsRecurring (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="95d89-112">IsRecurring (CalendarEventDetails)</span></span>](isrecurring-calendareventdetails.md)
  
```xml
<IsRecurring>true or false</IsRecurring>
```

 <span data-ttu-id="95d89-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="95d89-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="95d89-114">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="95d89-114">Attributes and elements</span></span>

<span data-ttu-id="95d89-115">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="95d89-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="95d89-116">Atributos</span><span class="sxs-lookup"><span data-stu-id="95d89-116">Attributes</span></span>

<span data-ttu-id="95d89-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="95d89-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="95d89-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="95d89-118">Child elements</span></span>

<span data-ttu-id="95d89-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="95d89-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="95d89-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="95d89-120">Parent elements</span></span>

|<span data-ttu-id="95d89-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="95d89-121">**Element**</span></span>|<span data-ttu-id="95d89-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="95d89-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="95d89-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="95d89-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="95d89-124">Fornece informações adicionais sobre um evento de calendário.</span><span class="sxs-lookup"><span data-stu-id="95d89-124">Provides additional information about a calendar event.</span></span>  <br/> <span data-ttu-id="95d89-125">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="95d89-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="95d89-126">Text value</span><span class="sxs-lookup"><span data-stu-id="95d89-126">Text value</span></span>

<span data-ttu-id="95d89-127">Se esse elemento é retornado em tempo de resposta, é necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="95d89-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="95d89-128">Esse elemento é necessário se o elemento [CalendarEventDetails](calendareventdetails.md) é usado.</span><span class="sxs-lookup"><span data-stu-id="95d89-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="95d89-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="95d89-129">Remarks</span></span>

<span data-ttu-id="95d89-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="95d89-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="95d89-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="95d89-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="95d89-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="95d89-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="95d89-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="95d89-133">Schema Name</span></span>  <br/> |<span data-ttu-id="95d89-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="95d89-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="95d89-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="95d89-135">Validation File</span></span>  <br/> |<span data-ttu-id="95d89-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="95d89-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="95d89-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="95d89-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="95d89-138">False</span><span class="sxs-lookup"><span data-stu-id="95d89-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="95d89-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="95d89-139">See also</span></span>



[<span data-ttu-id="95d89-140">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="95d89-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="95d89-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="95d89-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="95d89-142">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="95d89-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

