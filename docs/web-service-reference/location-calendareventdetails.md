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
description: O elemento Location representa o campo de localização do item de calendário.
ms.openlocfilehash: 3678bd94851633fcca9817c020106670b57d110c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824245"
---
# <a name="location-calendareventdetails"></a><span data-ttu-id="a085b-103">Local (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="a085b-103">Location (CalendarEventDetails)</span></span>

<span data-ttu-id="a085b-104">O elemento **Location** representa o campo de localização do item de calendário.</span><span class="sxs-lookup"><span data-stu-id="a085b-104">The **Location** element represents the location field of the calendar item.</span></span> 
  
[<span data-ttu-id="a085b-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a085b-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="a085b-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="a085b-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="a085b-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="a085b-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="a085b-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="a085b-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="a085b-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="a085b-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="a085b-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="a085b-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="a085b-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="a085b-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="a085b-112">Local (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="a085b-112">Location (CalendarEventDetails)</span></span>](location-calendareventdetails.md)
  
```xml
<Location/>
```

 <span data-ttu-id="a085b-113">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="a085b-113">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a085b-114">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a085b-114">Attributes and elements</span></span>

<span data-ttu-id="a085b-115">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a085b-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a085b-116">Atributos</span><span class="sxs-lookup"><span data-stu-id="a085b-116">Attributes</span></span>

<span data-ttu-id="a085b-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a085b-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a085b-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a085b-118">Child elements</span></span>

<span data-ttu-id="a085b-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a085b-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a085b-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a085b-120">Parent elements</span></span>

|<span data-ttu-id="a085b-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a085b-121">**Element**</span></span>|<span data-ttu-id="a085b-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a085b-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a085b-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="a085b-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="a085b-124">Fornece informações adicionais para um evento de calendário.</span><span class="sxs-lookup"><span data-stu-id="a085b-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="a085b-125">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="a085b-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a085b-126">Text value</span><span class="sxs-lookup"><span data-stu-id="a085b-126">Text value</span></span>

<span data-ttu-id="a085b-127">Se esse elemento é retornado em tempo de resposta, é necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="a085b-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="a085b-128">Esse elemento pode conter uma sequência vazia.</span><span class="sxs-lookup"><span data-stu-id="a085b-128">This element can contain an empty string.</span></span> <span data-ttu-id="a085b-129">Esse elemento é opcional, se o elemento [CalendarEventDetails](calendareventdetails.md) é usado.</span><span class="sxs-lookup"><span data-stu-id="a085b-129">This element is optional if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a085b-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="a085b-130">Remarks</span></span>

<span data-ttu-id="a085b-131">Esse elemento mapeia para uma MAPI PR_Location propriedade nomeada.</span><span class="sxs-lookup"><span data-stu-id="a085b-131">This element maps to a PR_Location MAPI named property.</span></span>
  
<span data-ttu-id="a085b-132">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="a085b-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a085b-133">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a085b-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a085b-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="a085b-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a085b-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a085b-135">Schema Name</span></span>  <br/> |<span data-ttu-id="a085b-136">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a085b-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="a085b-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a085b-137">Validation File</span></span>  <br/> |<span data-ttu-id="a085b-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a085b-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a085b-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a085b-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="a085b-140">False</span><span class="sxs-lookup"><span data-stu-id="a085b-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a085b-141">Ver também</span><span class="sxs-lookup"><span data-stu-id="a085b-141">See also</span></span>



[<span data-ttu-id="a085b-142">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="a085b-142">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="a085b-143">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a085b-143">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="a085b-144">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="a085b-144">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

