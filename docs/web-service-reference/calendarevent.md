---
title: CalendarEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarEvent
api_type:
- schema
ms.assetid: 91958c01-1fcb-4ac0-8601-5e5b434c988a
description: O elemento CalendarEvent representa uma ocorrência de item de calendário exclusiva.
ms.openlocfilehash: 8bf37c907ed726e33dd2b1eff9add5d6235704da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459073"
---
# <a name="calendarevent"></a><span data-ttu-id="388a7-103">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="388a7-103">CalendarEvent</span></span>

<span data-ttu-id="388a7-104">O elemento **CalendarEvent** representa uma ocorrência de item de calendário exclusiva.</span><span class="sxs-lookup"><span data-stu-id="388a7-104">The **CalendarEvent** element represents a unique calendar item occurrence.</span></span> 
  
[<span data-ttu-id="388a7-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="388a7-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="388a7-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="388a7-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="388a7-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="388a7-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="388a7-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="388a7-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="388a7-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="388a7-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="388a7-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="388a7-110">CalendarEvent</span></span>](calendarevent.md)
  
```xml
<CalendarEvent>
   <StartTime>...</StartTime>
   <EndTime>...</EndTime>
   <BusyType>...</BusyType>
   <CalendarEventDetails>...</CalendarEventDetails>
</CalendarEvent>
```

 <span data-ttu-id="388a7-111">**CalendarEvent**</span><span class="sxs-lookup"><span data-stu-id="388a7-111">**CalendarEvent**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="388a7-112">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="388a7-112">Attributes and elements</span></span>

<span data-ttu-id="388a7-113">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="388a7-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="388a7-114">Atributos</span><span class="sxs-lookup"><span data-stu-id="388a7-114">Attributes</span></span>

<span data-ttu-id="388a7-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="388a7-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="388a7-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="388a7-116">Child elements</span></span>

|<span data-ttu-id="388a7-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="388a7-117">**Element**</span></span>|<span data-ttu-id="388a7-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="388a7-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="388a7-119">StartTime</span><span class="sxs-lookup"><span data-stu-id="388a7-119">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="388a7-120">Representa o início de um evento de calendário.</span><span class="sxs-lookup"><span data-stu-id="388a7-120">Represents the start of a calendar event.</span></span> <span data-ttu-id="388a7-121">Este é um elemento filho obrigatório.</span><span class="sxs-lookup"><span data-stu-id="388a7-121">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="388a7-122">EndTime</span><span class="sxs-lookup"><span data-stu-id="388a7-122">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="388a7-123">Representa o final de um evento de calendário.</span><span class="sxs-lookup"><span data-stu-id="388a7-123">Represents the end of a calendar event.</span></span> <span data-ttu-id="388a7-124">Este é um elemento filho obrigatório.</span><span class="sxs-lookup"><span data-stu-id="388a7-124">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="388a7-125">BusyType</span><span class="sxs-lookup"><span data-stu-id="388a7-125">BusyType</span></span>](busytype.md) <br/> |<span data-ttu-id="388a7-126">Representa o status de disponibilidade definido para um evento de calendário.</span><span class="sxs-lookup"><span data-stu-id="388a7-126">Represents the free/busy status set for a calendar event.</span></span> <span data-ttu-id="388a7-127">Este é um elemento filho obrigatório.</span><span class="sxs-lookup"><span data-stu-id="388a7-127">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="388a7-128">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="388a7-128">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="388a7-129">Fornece informações adicionais para um evento de calendário.</span><span class="sxs-lookup"><span data-stu-id="388a7-129">Provides additional information for a calendar event.</span></span> <span data-ttu-id="388a7-130">Este é um elemento filho opcional.</span><span class="sxs-lookup"><span data-stu-id="388a7-130">This is an optional child element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="388a7-131">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="388a7-131">Parent elements</span></span>

|<span data-ttu-id="388a7-132">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="388a7-132">**Element**</span></span>|<span data-ttu-id="388a7-133">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="388a7-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="388a7-134">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="388a7-134">CalendarEventArray</span></span>](calendareventarray.md) <br/> |<span data-ttu-id="388a7-135">Contém um conjunto de ocorrências de item de calendário exclusivo que representam a disponibilidade do usuário solicitado.</span><span class="sxs-lookup"><span data-stu-id="388a7-135">Contains a set of unique calendar item occurrences that represent the requested user's availability.</span></span>  <br/> <span data-ttu-id="388a7-136">A seguir está a expressão XPath 2,0 para este elemento:</span><span class="sxs-lookup"><span data-stu-id="388a7-136">The following is the XPath 2.0 expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="388a7-137">Comentários</span><span class="sxs-lookup"><span data-stu-id="388a7-137">Remarks</span></span>

<span data-ttu-id="388a7-138">O compromisso e os horários de reunião são retornados no fuso horário do cliente.</span><span class="sxs-lookup"><span data-stu-id="388a7-138">The appointment and meeting times are returned in the time zone of the client.</span></span> <span data-ttu-id="388a7-139">Todos os elementos filho são listados na sequência em que ocorrem.</span><span class="sxs-lookup"><span data-stu-id="388a7-139">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="388a7-140">O nível de detalhes fornecido por esse elemento depende das permissões concedidas ao solicitante.</span><span class="sxs-lookup"><span data-stu-id="388a7-140">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="388a7-141">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="388a7-141">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="388a7-142">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="388a7-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="388a7-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="388a7-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="388a7-144">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="388a7-144">Schema Name</span></span>  <br/> |<span data-ttu-id="388a7-145">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="388a7-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="388a7-146">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="388a7-146">Validation File</span></span>  <br/> |<span data-ttu-id="388a7-147">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="388a7-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="388a7-148">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="388a7-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="388a7-149">False</span><span class="sxs-lookup"><span data-stu-id="388a7-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="388a7-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="388a7-150">See also</span></span>



[<span data-ttu-id="388a7-151">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="388a7-151">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="388a7-152">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="388a7-152">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="388a7-153">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="388a7-153">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

