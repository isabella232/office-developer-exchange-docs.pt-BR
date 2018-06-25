---
title: CalendarEventDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarEventDetails
api_type:
- schema
ms.assetid: 2dca0192-b91b-4154-aa09-84da74e875e9
description: O elemento CalendarEventDetails fornece informações adicionais sobre um evento de calendário.
ms.openlocfilehash: 8df4f3ed4f66c7dcba00e1f0c5b0c383075da0a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751349"
---
# <a name="calendareventdetails"></a><span data-ttu-id="950d3-103">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="950d3-103">CalendarEventDetails</span></span>

<span data-ttu-id="950d3-104">O elemento **CalendarEventDetails** fornece informações adicionais sobre um evento de calendário.</span><span class="sxs-lookup"><span data-stu-id="950d3-104">The **CalendarEventDetails** element provides additional information about a calendar event.</span></span> 
  
[<span data-ttu-id="950d3-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="950d3-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="950d3-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="950d3-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="950d3-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="950d3-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="950d3-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="950d3-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="950d3-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="950d3-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="950d3-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="950d3-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="950d3-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="950d3-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
```xml
<CalendarEventDetails>
   <ID/>
   <Subject/>
   <Location/>
   <IsMeeting/>
   <IsRecurring/>
   <IsException/>
   <IsReminderSet/>
   <IsPrivate/>
</CalendarEventDetails>
```

 <span data-ttu-id="950d3-112">**CalendarEventDetails**</span><span class="sxs-lookup"><span data-stu-id="950d3-112">**CalendarEventDetails**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="950d3-113">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="950d3-113">Attributes and elements</span></span>

<span data-ttu-id="950d3-114">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="950d3-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="950d3-115">Atributos</span><span class="sxs-lookup"><span data-stu-id="950d3-115">Attributes</span></span>

<span data-ttu-id="950d3-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="950d3-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="950d3-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="950d3-117">Child elements</span></span>

|<span data-ttu-id="950d3-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="950d3-118">**Element**</span></span>|<span data-ttu-id="950d3-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="950d3-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="950d3-120">ID DO</span><span class="sxs-lookup"><span data-stu-id="950d3-120">ID</span></span>](id.md) <br/> |<span data-ttu-id="950d3-121">Representa a identificação de entrada do item do calendário.</span><span class="sxs-lookup"><span data-stu-id="950d3-121">Represents the entry ID of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="950d3-122">Assunto (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="950d3-122">Subject (CalendarEventDetails)</span></span>](subject-calendareventdetails.md) <br/> |<span data-ttu-id="950d3-123">Representa o assunto do item de calendário.</span><span class="sxs-lookup"><span data-stu-id="950d3-123">Represents the subject of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="950d3-124">Local (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="950d3-124">Location (CalendarEventDetails)</span></span>](location-calendareventdetails.md) <br/> |<span data-ttu-id="950d3-125">Representa o campo de localização do item de calendário.</span><span class="sxs-lookup"><span data-stu-id="950d3-125">Represents the location field of the calendar item.</span></span>  <br/> |
|[<span data-ttu-id="950d3-126">IsMeeting (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="950d3-126">IsMeeting (CalendarEventDetails)</span></span>](ismeeting-calendareventdetails.md) <br/> |<span data-ttu-id="950d3-127">Indica se o evento de calendário é uma reunião ou um compromisso.</span><span class="sxs-lookup"><span data-stu-id="950d3-127">Indicates whether the calendar event is a meeting or an appointment.</span></span>  <br/> |
|[<span data-ttu-id="950d3-128">IsRecurring (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="950d3-128">IsRecurring (CalendarEventDetails)</span></span>](isrecurring-calendareventdetails.md) <br/> |<span data-ttu-id="950d3-129">Indica se o evento de calendário é uma instância de um item de calendário recorrente ou um item de calendário único.</span><span class="sxs-lookup"><span data-stu-id="950d3-129">Indicates whether the calendar event is an instance of a recurring calendar item or a single calendar item.</span></span>  <br/> |
|[<span data-ttu-id="950d3-130">IsException</span><span class="sxs-lookup"><span data-stu-id="950d3-130">IsException</span></span>](isexception.md) <br/> |<span data-ttu-id="950d3-131">Indica se uma instância de um item de calendário recorrente é alterada do mestre.</span><span class="sxs-lookup"><span data-stu-id="950d3-131">Indicates whether an instance of a recurring calendar item is changed from the master.</span></span>  <br/> |
|[<span data-ttu-id="950d3-132">IsReminderSet</span><span class="sxs-lookup"><span data-stu-id="950d3-132">IsReminderSet</span></span>](isreminderset.md) <br/> |<span data-ttu-id="950d3-133">Indica se um lembrete tiver sido definido para o evento de calendário.</span><span class="sxs-lookup"><span data-stu-id="950d3-133">Indicates whether a reminder has been set for the calendar event.</span></span>  <br/> |
|[<span data-ttu-id="950d3-134">IsPrivate</span><span class="sxs-lookup"><span data-stu-id="950d3-134">IsPrivate</span></span>](isprivate.md) <br/> |<span data-ttu-id="950d3-135">Indica se o item do calendário é privado.</span><span class="sxs-lookup"><span data-stu-id="950d3-135">Indicates whether the calendar item is private.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="950d3-136">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="950d3-136">Parent elements</span></span>

|<span data-ttu-id="950d3-137">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="950d3-137">**Element**</span></span>|<span data-ttu-id="950d3-138">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="950d3-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="950d3-139">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="950d3-139">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="950d3-140">Representa uma ocorrência de item de calendário exclusivo.</span><span class="sxs-lookup"><span data-stu-id="950d3-140">Represents a unique calendar item occurrence.</span></span>  <br/> <span data-ttu-id="950d3-141">Este é a expressão XPath 2.0 para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="950d3-141">The following is the XPath 2.0 expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="950d3-142">Comentários</span><span class="sxs-lookup"><span data-stu-id="950d3-142">Remarks</span></span>

<span data-ttu-id="950d3-143">Todos os elementos filhos são listados na sequência em que ocorrem.</span><span class="sxs-lookup"><span data-stu-id="950d3-143">All the child elements are listed in the sequence in which they occur.</span></span> 
  
<span data-ttu-id="950d3-144">Se o elemento [IsPrivate](isprivate.md) for **true**, todos os outros elementos no elemento [CalendarEventDetails](calendareventdetails.md) não são retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="950d3-144">If the [IsPrivate](isprivate.md) element is **true**, all the other elements in the [CalendarEventDetails](calendareventdetails.md) element are not returned in the response.</span></span> 
  
<span data-ttu-id="950d3-145">A operação GetUserAvailability não retorna informações detalhadas do chamador, a menos que o chamador tem acesso de leitura no calendário do usuário de destino.</span><span class="sxs-lookup"><span data-stu-id="950d3-145">The GetUserAvailability operation does not return detailed caller information unless the caller has read access on the target user's calendar.</span></span> <span data-ttu-id="950d3-146">Você pode definir permissões de acesso usando o Shell de gerenciamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="950d3-146">You can set access permissions by using the Exchange Management Shell.</span></span>
  
<span data-ttu-id="950d3-147">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="950d3-147">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="950d3-148">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="950d3-148">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="950d3-149">Namespace</span><span class="sxs-lookup"><span data-stu-id="950d3-149">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="950d3-150">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="950d3-150">Schema Name</span></span>  <br/> |<span data-ttu-id="950d3-151">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="950d3-151">Types schema</span></span>  <br/> |
|<span data-ttu-id="950d3-152">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="950d3-152">Validation File</span></span>  <br/> |<span data-ttu-id="950d3-153">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="950d3-153">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="950d3-154">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="950d3-154">Can be Empty</span></span>  <br/> |<span data-ttu-id="950d3-155">False</span><span class="sxs-lookup"><span data-stu-id="950d3-155">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="950d3-156">Ver também</span><span class="sxs-lookup"><span data-stu-id="950d3-156">See also</span></span>



[<span data-ttu-id="950d3-157">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="950d3-157">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="950d3-158">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="950d3-158">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="950d3-159">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="950d3-159">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

