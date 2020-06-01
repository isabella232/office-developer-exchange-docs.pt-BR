---
title: CalendarEventArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarEventArray
api_type:
- schema
ms.assetid: a00f7f56-d7f1-429d-ae02-97043718c864
description: O elemento CalendarEventArray contém um conjunto de ocorrências de item de calendário exclusivo que representam a disponibilidade do usuário solicitado.
ms.openlocfilehash: 6badba2477a9d48c6d109740de454e2815d3c211
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463367"
---
# <a name="calendareventarray"></a><span data-ttu-id="93799-103">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="93799-103">CalendarEventArray</span></span>

<span data-ttu-id="93799-104">O elemento **CalendarEventArray** contém um conjunto de ocorrências de item de calendário exclusivo que representam a disponibilidade do usuário solicitado.</span><span class="sxs-lookup"><span data-stu-id="93799-104">The **CalendarEventArray** element contains a set of unique calendar item occurrences that represent the requested user's availability.</span></span> 
  
[<span data-ttu-id="93799-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="93799-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="93799-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="93799-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="93799-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="93799-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="93799-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="93799-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="93799-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="93799-109">CalendarEventArray</span></span>](calendareventarray.md)
  
```xml
<CalendarEventArray>
   <CalendarEvent>...</CalendarEvent>
</CalendarEventArray>
```

 <span data-ttu-id="93799-110">**ArrayOfCalendarEvent**</span><span class="sxs-lookup"><span data-stu-id="93799-110">**ArrayOfCalendarEvent**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93799-111">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="93799-111">Attributes and elements</span></span>

<span data-ttu-id="93799-112">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="93799-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93799-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="93799-113">Attributes</span></span>

<span data-ttu-id="93799-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="93799-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93799-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="93799-115">Child elements</span></span>

|<span data-ttu-id="93799-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="93799-116">**Element**</span></span>|<span data-ttu-id="93799-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="93799-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93799-118">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="93799-118">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="93799-119">Representa uma ocorrência de item de calendário exclusivo.</span><span class="sxs-lookup"><span data-stu-id="93799-119">Represents a unique calendar item occurrence.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="93799-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="93799-120">Parent elements</span></span>

|<span data-ttu-id="93799-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="93799-121">**Element**</span></span>|<span data-ttu-id="93799-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="93799-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93799-123">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="93799-123">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="93799-124">Contém informações de disponibilidade para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="93799-124">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="93799-125">A seguir está a expressão XPath 2,0 para este elemento:</span><span class="sxs-lookup"><span data-stu-id="93799-125">The following is the XPath 2.0 expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="93799-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="93799-126">Remarks</span></span>

<span data-ttu-id="93799-127">O nível de detalhes fornecido por esse elemento depende das permissões concedidas ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="93799-127">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span> <span data-ttu-id="93799-128">Este elemento é incluído quando o elemento [FreeBusyViewType](freebusyviewtype.md) é definido como **FreeBusy**, **FreeBusyMerged**, **detailed**ou **DetailedMerged**.</span><span class="sxs-lookup"><span data-stu-id="93799-128">This element is included when the [FreeBusyViewType](freebusyviewtype.md) element is set to **FreeBusy**, **FreeBusyMerged**, **Detailed**, or **DetailedMerged**.</span></span> <span data-ttu-id="93799-129">Esse elemento não inclui nenhum elemento filho se nenhum item de calendário estiver presente na janela de tempo solicitada.</span><span class="sxs-lookup"><span data-stu-id="93799-129">This element does not include any child elements if no calendar items are present in the requested time window.</span></span> 
  
<span data-ttu-id="93799-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="93799-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93799-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="93799-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93799-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="93799-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="93799-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="93799-133">Schema Name</span></span>  <br/> |<span data-ttu-id="93799-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="93799-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="93799-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="93799-135">Validation File</span></span>  <br/> |<span data-ttu-id="93799-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="93799-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="93799-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="93799-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="93799-138">False</span><span class="sxs-lookup"><span data-stu-id="93799-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="93799-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="93799-139">See also</span></span>



[<span data-ttu-id="93799-140">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="93799-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="93799-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="93799-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="93799-142">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="93799-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

