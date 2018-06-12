---
title: IsPrivate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsPrivate
api_type:
- schema
ms.assetid: 1712bc94-9789-4507-8521-bde1be51e331
description: O elemento IsPrivate indica se o item do calendário é privado.
ms.openlocfilehash: 37c0357b3eab2314ee74e1c98287b3dc05a3bf26
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824095"
---
# <a name="isprivate"></a><span data-ttu-id="1b576-103">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="1b576-103">IsPrivate</span></span>

<span data-ttu-id="1b576-104">O elemento **IsPrivate** indica se o item do calendário é privado.</span><span class="sxs-lookup"><span data-stu-id="1b576-104">The **IsPrivate** element indicates whether the calendar item is private.</span></span> 
  
[<span data-ttu-id="1b576-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1b576-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="1b576-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="1b576-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="1b576-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="1b576-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="1b576-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="1b576-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="1b576-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="1b576-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="1b576-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="1b576-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="1b576-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="1b576-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="1b576-112">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="1b576-112">IsPrivate</span></span>](isprivate.md)
  
```xml
<IsPrivate>true or false</IsPrivate>
```

 <span data-ttu-id="1b576-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="1b576-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1b576-114">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="1b576-114">Attributes and elements</span></span>

<span data-ttu-id="1b576-115">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1b576-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1b576-116">Atributos</span><span class="sxs-lookup"><span data-stu-id="1b576-116">Attributes</span></span>

<span data-ttu-id="1b576-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1b576-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1b576-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1b576-118">Child elements</span></span>

<span data-ttu-id="1b576-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1b576-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1b576-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1b576-120">Parent elements</span></span>

|<span data-ttu-id="1b576-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1b576-121">**Element**</span></span>|<span data-ttu-id="1b576-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1b576-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b576-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="1b576-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="1b576-124">Fornece informações adicionais sobre um evento de calendário.</span><span class="sxs-lookup"><span data-stu-id="1b576-124">Provides additional information about a calendar event.</span></span>  <br/> <span data-ttu-id="1b576-125">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="1b576-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1b576-126">Text value</span><span class="sxs-lookup"><span data-stu-id="1b576-126">Text value</span></span>

<span data-ttu-id="1b576-127">É necessário um valor de texto que representa um valor booleano.</span><span class="sxs-lookup"><span data-stu-id="1b576-127">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1b576-128">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="1b576-128">Remarks</span></span>

<span data-ttu-id="1b576-129">Se este elemento for usado, os outros elementos no elemento [CalendarEventDetails](calendareventdetails.md) não serão incluídos na resposta.</span><span class="sxs-lookup"><span data-stu-id="1b576-129">If this element is used, the other elements in the [CalendarEventDetails](calendareventdetails.md) element will not be included in the response.</span></span> 
  
<span data-ttu-id="1b576-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="1b576-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1b576-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="1b576-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1b576-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="1b576-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1b576-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1b576-133">Schema Name</span></span>  <br/> |<span data-ttu-id="1b576-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="1b576-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="1b576-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1b576-135">Validation File</span></span>  <br/> |<span data-ttu-id="1b576-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1b576-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1b576-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1b576-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="1b576-138">False</span><span class="sxs-lookup"><span data-stu-id="1b576-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1b576-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="1b576-139">See also</span></span>



[<span data-ttu-id="1b576-140">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="1b576-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="1b576-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1b576-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="1b576-142">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="1b576-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

