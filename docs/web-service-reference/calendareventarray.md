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
ms.openlocfilehash: 2e56b7b2b94e12401ba708dfca94101064d625e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751348"
---
# <a name="calendareventarray"></a><span data-ttu-id="25d51-103">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="25d51-103">CalendarEventArray</span></span>

<span data-ttu-id="25d51-104">O elemento **CalendarEventArray** contém um conjunto de ocorrências de item de calendário exclusivo que representam a disponibilidade do usuário solicitado.</span><span class="sxs-lookup"><span data-stu-id="25d51-104">The **CalendarEventArray** element contains a set of unique calendar item occurrences that represent the requested user's availability.</span></span> 
  
[<span data-ttu-id="25d51-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="25d51-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="25d51-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="25d51-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="25d51-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="25d51-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="25d51-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="25d51-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="25d51-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="25d51-109">CalendarEventArray</span></span>](calendareventarray.md)
  
```xml
<CalendarEventArray>
   <CalendarEvent>...</CalendarEvent>
</CalendarEventArray>
```

 <span data-ttu-id="25d51-110">**ArrayOfCalendarEvent**</span><span class="sxs-lookup"><span data-stu-id="25d51-110">**ArrayOfCalendarEvent**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="25d51-111">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="25d51-111">Attributes and elements</span></span>

<span data-ttu-id="25d51-112">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="25d51-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="25d51-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="25d51-113">Attributes</span></span>

<span data-ttu-id="25d51-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="25d51-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="25d51-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="25d51-115">Child elements</span></span>

|<span data-ttu-id="25d51-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="25d51-116">**Element**</span></span>|<span data-ttu-id="25d51-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="25d51-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25d51-118">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="25d51-118">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="25d51-119">Representa uma ocorrência de item de calendário exclusivo.</span><span class="sxs-lookup"><span data-stu-id="25d51-119">Represents a unique calendar item occurrence.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="25d51-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="25d51-120">Parent elements</span></span>

|<span data-ttu-id="25d51-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="25d51-121">**Element**</span></span>|<span data-ttu-id="25d51-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="25d51-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25d51-123">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="25d51-123">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="25d51-124">Contém informações de disponibilidade para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="25d51-124">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="25d51-125">Este é a expressão XPath 2.0 para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="25d51-125">The following is the XPath 2.0 expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="25d51-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="25d51-126">Remarks</span></span>

<span data-ttu-id="25d51-127">O nível de detalhes fornecidos por esse elemento depende as permissões concedidas para o solicitante.</span><span class="sxs-lookup"><span data-stu-id="25d51-127">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span> <span data-ttu-id="25d51-128">Esse elemento é incluído quando o elemento [FreeBusyViewType](freebusyviewtype.md) estiver definido como **FreeBusy**, **FreeBusyMerged**, **Detailed**ou **DetailedMerged**.</span><span class="sxs-lookup"><span data-stu-id="25d51-128">This element is included when the [FreeBusyViewType](freebusyviewtype.md) element is set to **FreeBusy**, **FreeBusyMerged**, **Detailed**, or **DetailedMerged**.</span></span> <span data-ttu-id="25d51-129">Este elemento não inclui todos os elementos filho se não há itens de calendário estiverem presentes na janela de tempo solicitada.</span><span class="sxs-lookup"><span data-stu-id="25d51-129">This element does not include any child elements if no calendar items are present in the requested time window.</span></span> 
  
<span data-ttu-id="25d51-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="25d51-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="25d51-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="25d51-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="25d51-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="25d51-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="25d51-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="25d51-133">Schema Name</span></span>  <br/> |<span data-ttu-id="25d51-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="25d51-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="25d51-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="25d51-135">Validation File</span></span>  <br/> |<span data-ttu-id="25d51-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="25d51-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="25d51-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="25d51-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="25d51-138">False</span><span class="sxs-lookup"><span data-stu-id="25d51-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="25d51-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="25d51-139">See also</span></span>



[<span data-ttu-id="25d51-140">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="25d51-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="25d51-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="25d51-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="25d51-142">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="25d51-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

