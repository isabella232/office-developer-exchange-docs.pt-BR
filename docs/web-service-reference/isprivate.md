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
description: O elemento IsPrivate indica se o item de calendário é privado.
ms.openlocfilehash: c36c659414700439436cd2ca903e443164c1473b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457799"
---
# <a name="isprivate"></a><span data-ttu-id="8fd18-103">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="8fd18-103">IsPrivate</span></span>

<span data-ttu-id="8fd18-104">O elemento **IsPrivate** indica se o item de calendário é privado.</span><span class="sxs-lookup"><span data-stu-id="8fd18-104">The **IsPrivate** element indicates whether the calendar item is private.</span></span> 
  
[<span data-ttu-id="8fd18-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="8fd18-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="8fd18-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="8fd18-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="8fd18-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="8fd18-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="8fd18-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="8fd18-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="8fd18-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="8fd18-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="8fd18-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="8fd18-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="8fd18-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="8fd18-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="8fd18-112">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="8fd18-112">IsPrivate</span></span>](isprivate.md)
  
```xml
<IsPrivate>true or false</IsPrivate>
```

 <span data-ttu-id="8fd18-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="8fd18-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8fd18-114">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8fd18-114">Attributes and elements</span></span>

<span data-ttu-id="8fd18-115">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8fd18-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8fd18-116">Atributos</span><span class="sxs-lookup"><span data-stu-id="8fd18-116">Attributes</span></span>

<span data-ttu-id="8fd18-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8fd18-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8fd18-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8fd18-118">Child elements</span></span>

<span data-ttu-id="8fd18-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8fd18-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8fd18-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8fd18-120">Parent elements</span></span>

|<span data-ttu-id="8fd18-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8fd18-121">**Element**</span></span>|<span data-ttu-id="8fd18-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8fd18-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8fd18-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="8fd18-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="8fd18-124">Fornece informações adicionais sobre um evento de calendário.</span><span class="sxs-lookup"><span data-stu-id="8fd18-124">Provides additional information about a calendar event.</span></span>  <br/> <span data-ttu-id="8fd18-125">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="8fd18-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8fd18-126">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="8fd18-126">Text value</span></span>

<span data-ttu-id="8fd18-127">Um valor de texto que representa um valor booliano é necessário.</span><span class="sxs-lookup"><span data-stu-id="8fd18-127">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8fd18-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="8fd18-128">Remarks</span></span>

<span data-ttu-id="8fd18-129">Se esse elemento for usado, os outros elementos no elemento [CalendarEventDetails](calendareventdetails.md) não serão incluídos na resposta.</span><span class="sxs-lookup"><span data-stu-id="8fd18-129">If this element is used, the other elements in the [CalendarEventDetails](calendareventdetails.md) element will not be included in the response.</span></span> 
  
<span data-ttu-id="8fd18-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="8fd18-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8fd18-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="8fd18-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8fd18-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="8fd18-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8fd18-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8fd18-133">Schema Name</span></span>  <br/> |<span data-ttu-id="8fd18-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8fd18-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="8fd18-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8fd18-135">Validation File</span></span>  <br/> |<span data-ttu-id="8fd18-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8fd18-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8fd18-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8fd18-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="8fd18-138">False</span><span class="sxs-lookup"><span data-stu-id="8fd18-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8fd18-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="8fd18-139">See also</span></span>



[<span data-ttu-id="8fd18-140">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="8fd18-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="8fd18-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="8fd18-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="8fd18-142">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="8fd18-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

