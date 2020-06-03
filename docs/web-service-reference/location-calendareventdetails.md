---
title: Local (CalendarEventDetails)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Location
api_type:
- schema
ms.assetid: 883cce6e-66b8-4dbc-935c-83ef5100a953
description: O elemento Location representa o campo local do item do calendário.
ms.openlocfilehash: 4a590c315d2211ce9128305a514e68f1c785596c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467995"
---
# <a name="location-calendareventdetails"></a><span data-ttu-id="11917-103">Local (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="11917-103">Location (CalendarEventDetails)</span></span>

<span data-ttu-id="11917-104">O elemento **Location** representa o campo local do item do calendário.</span><span class="sxs-lookup"><span data-stu-id="11917-104">The **Location** element represents the location field of the calendar item.</span></span> 
  
[<span data-ttu-id="11917-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="11917-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="11917-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="11917-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="11917-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="11917-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="11917-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="11917-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="11917-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="11917-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="11917-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="11917-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="11917-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="11917-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="11917-112">Local (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="11917-112">Location (CalendarEventDetails)</span></span>](location-calendareventdetails.md)
  
```xml
<Location/>
```

 <span data-ttu-id="11917-113">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="11917-113">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="11917-114">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="11917-114">Attributes and elements</span></span>

<span data-ttu-id="11917-115">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="11917-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="11917-116">Atributos</span><span class="sxs-lookup"><span data-stu-id="11917-116">Attributes</span></span>

<span data-ttu-id="11917-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="11917-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="11917-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="11917-118">Child elements</span></span>

<span data-ttu-id="11917-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="11917-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="11917-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="11917-120">Parent elements</span></span>

|<span data-ttu-id="11917-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="11917-121">**Element**</span></span>|<span data-ttu-id="11917-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="11917-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11917-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="11917-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="11917-124">Fornece informações adicionais para um evento de calendário.</span><span class="sxs-lookup"><span data-stu-id="11917-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="11917-125">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="11917-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="11917-126">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="11917-126">Text value</span></span>

<span data-ttu-id="11917-127">Um valor de texto será necessário se esse elemento for retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="11917-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="11917-128">Este elemento pode conter uma cadeia de caracteres vazia.</span><span class="sxs-lookup"><span data-stu-id="11917-128">This element can contain an empty string.</span></span> <span data-ttu-id="11917-129">Este elemento é opcional se o elemento [CalendarEventDetails](calendareventdetails.md) for usado.</span><span class="sxs-lookup"><span data-stu-id="11917-129">This element is optional if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="11917-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="11917-130">Remarks</span></span>

<span data-ttu-id="11917-131">Este elemento mapeia para uma propriedade nomeada PR_Location MAPI.</span><span class="sxs-lookup"><span data-stu-id="11917-131">This element maps to a PR_Location MAPI named property.</span></span>
  
<span data-ttu-id="11917-132">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="11917-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="11917-133">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="11917-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="11917-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="11917-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="11917-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="11917-135">Schema Name</span></span>  <br/> |<span data-ttu-id="11917-136">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="11917-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="11917-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="11917-137">Validation File</span></span>  <br/> |<span data-ttu-id="11917-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="11917-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="11917-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="11917-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="11917-140">False</span><span class="sxs-lookup"><span data-stu-id="11917-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="11917-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="11917-141">See also</span></span>



[<span data-ttu-id="11917-142">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="11917-142">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="11917-143">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="11917-143">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="11917-144">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="11917-144">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

