---
title: ID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ID
api_type:
- schema
ms.assetid: 8caf922f-56bd-466a-a68f-d6cb236f2eec
description: O elemento ID representa a identificação de entrada do item do calendário.
ms.openlocfilehash: 429413bbfb0206effc3ea97eb11527449c67211c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456483"
---
# <a name="id"></a><span data-ttu-id="70f26-103">ID</span><span class="sxs-lookup"><span data-stu-id="70f26-103">ID</span></span>

<span data-ttu-id="70f26-104">O elemento **ID** representa a identificação de entrada do item do calendário.</span><span class="sxs-lookup"><span data-stu-id="70f26-104">The **ID** element represents the entry ID of the calendar item.</span></span> 
  
[<span data-ttu-id="70f26-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="70f26-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="70f26-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="70f26-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="70f26-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="70f26-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="70f26-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="70f26-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="70f26-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="70f26-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="70f26-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="70f26-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="70f26-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="70f26-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="70f26-112">ID</span><span class="sxs-lookup"><span data-stu-id="70f26-112">ID</span></span>](id.md)
  
```xml
<ID>...</ID>
```

 <span data-ttu-id="70f26-113">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="70f26-113">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="70f26-114">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="70f26-114">Attributes and elements</span></span>

<span data-ttu-id="70f26-115">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="70f26-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70f26-116">Atributos</span><span class="sxs-lookup"><span data-stu-id="70f26-116">Attributes</span></span>

<span data-ttu-id="70f26-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="70f26-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="70f26-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="70f26-118">Child elements</span></span>

<span data-ttu-id="70f26-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="70f26-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="70f26-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="70f26-120">Parent elements</span></span>

|<span data-ttu-id="70f26-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="70f26-121">**Element**</span></span>|<span data-ttu-id="70f26-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="70f26-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70f26-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="70f26-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="70f26-124">Fornece informações adicionais para um evento de calendário.</span><span class="sxs-lookup"><span data-stu-id="70f26-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="70f26-125">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="70f26-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="70f26-126">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="70f26-126">Text value</span></span>

<span data-ttu-id="70f26-127">Um valor de texto será necessário se esse elemento for retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="70f26-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="70f26-128">Esse elemento é necessário se o elemento [CalendarEventDetails](calendareventdetails.md) for usado.</span><span class="sxs-lookup"><span data-stu-id="70f26-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="70f26-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="70f26-129">Remarks</span></span>

<span data-ttu-id="70f26-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="70f26-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="70f26-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="70f26-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="70f26-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="70f26-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="70f26-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="70f26-133">Schema Name</span></span>  <br/> |<span data-ttu-id="70f26-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="70f26-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="70f26-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="70f26-135">Validation File</span></span>  <br/> |<span data-ttu-id="70f26-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="70f26-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="70f26-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="70f26-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="70f26-138">False</span><span class="sxs-lookup"><span data-stu-id="70f26-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="70f26-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="70f26-139">See also</span></span>



[<span data-ttu-id="70f26-140">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="70f26-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="70f26-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="70f26-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="70f26-142">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="70f26-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

