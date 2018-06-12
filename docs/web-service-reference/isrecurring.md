---
title: IsRecurring
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
ms.assetid: f4df6997-8d5b-4893-a4a5-fc7047e0a9c3
description: O elemento IsRecurring indica se um item de calendário, solicitação de reunião ou tarefa é parte de um item recorrente. Este elemento é somente leitura.
ms.openlocfilehash: dfb0c28fe225792c7128409a8cf010627c624fe0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824104"
---
# <a name="isrecurring"></a><span data-ttu-id="7cefe-104">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="7cefe-104">IsRecurring</span></span>

<span data-ttu-id="7cefe-105">O elemento **IsRecurring** indica se um item de calendário, solicitação de reunião ou tarefa é parte de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="7cefe-105">The **IsRecurring** element indicates whether a calendar item, meeting request, or task is part of a recurring item.</span></span> <span data-ttu-id="7cefe-106">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="7cefe-106">This element is read-only.</span></span> 
  
```xml
<IsRecurring/>
```

 <span data-ttu-id="7cefe-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="7cefe-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7cefe-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7cefe-108">Attributes and elements</span></span>

<span data-ttu-id="7cefe-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7cefe-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7cefe-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="7cefe-110">Attributes</span></span>

<span data-ttu-id="7cefe-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7cefe-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7cefe-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7cefe-112">Child elements</span></span>

<span data-ttu-id="7cefe-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7cefe-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7cefe-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7cefe-114">Parent elements</span></span>

|<span data-ttu-id="7cefe-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7cefe-115">**Element**</span></span>|<span data-ttu-id="7cefe-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7cefe-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7cefe-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="7cefe-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="7cefe-118">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7cefe-118">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="7cefe-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="7cefe-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="7cefe-120">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7cefe-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7cefe-121">Task</span><span class="sxs-lookup"><span data-stu-id="7cefe-121">Task</span></span>](task.md) <br/> |<span data-ttu-id="7cefe-122">Representa uma tarefa no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7cefe-122">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7cefe-123">Text value</span><span class="sxs-lookup"><span data-stu-id="7cefe-123">Text value</span></span>

<span data-ttu-id="7cefe-124">É necessário um valor de texto que representa um valor booleano.</span><span class="sxs-lookup"><span data-stu-id="7cefe-124">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7cefe-125">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="7cefe-125">Remarks</span></span>

<span data-ttu-id="7cefe-126">A tabela a seguir mostra como a propriedade **IsRecurring** é definida para tipos de item de calendário diferente para organizadores e participantes e para solicitações de reunião e atualizações.</span><span class="sxs-lookup"><span data-stu-id="7cefe-126">The following table shows how the **IsRecurring** property is set for different calendar item types for organizers and attendees and for meeting requests and updates.</span></span> 
  
|<span data-ttu-id="7cefe-127">**Tipo de CalendarItem**</span><span class="sxs-lookup"><span data-stu-id="7cefe-127">**CalendarItem Type**</span></span>|<span data-ttu-id="7cefe-128">**Organizador <br/> (IsRecurring)**</span><span class="sxs-lookup"><span data-stu-id="7cefe-128">**Organizer  <br/> (IsRecurring)**</span></span>|<span data-ttu-id="7cefe-129">**Participante <br/> (IsRecurring)**</span><span class="sxs-lookup"><span data-stu-id="7cefe-129">**Attendee  <br/> (IsRecurring)**</span></span>|<span data-ttu-id="7cefe-130">**Atualizar/solicitação de reunião <br/> (IsRecurring)**</span><span class="sxs-lookup"><span data-stu-id="7cefe-130">**Meeting request/update  <br/> (IsRecurring)**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="7cefe-131">Ocorrência única</span><span class="sxs-lookup"><span data-stu-id="7cefe-131">Single Occurrence</span></span>  <br/> |<span data-ttu-id="7cefe-132">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="7cefe-132">**FALSE**</span></span> <br/> |<span data-ttu-id="7cefe-133">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="7cefe-133">**FALSE**</span></span> <br/> |<span data-ttu-id="7cefe-134">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="7cefe-134">**FALSE**</span></span> <br/> |
|<span data-ttu-id="7cefe-135">Mestre recorrente</span><span class="sxs-lookup"><span data-stu-id="7cefe-135">Recurring Master</span></span>  <br/> |<span data-ttu-id="7cefe-136">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="7cefe-136">**FALSE**</span></span> <br/> |<span data-ttu-id="7cefe-137">**TRUE**</span><span class="sxs-lookup"><span data-stu-id="7cefe-137">**TRUE**</span></span> <br/> |<span data-ttu-id="7cefe-138">**TRUE**</span><span class="sxs-lookup"><span data-stu-id="7cefe-138">**TRUE**</span></span> <br/> |
|<span data-ttu-id="7cefe-139">Exceção recorrente</span><span class="sxs-lookup"><span data-stu-id="7cefe-139">Recurring Exception</span></span>  <br/> |<span data-ttu-id="7cefe-140">**TRUE**</span><span class="sxs-lookup"><span data-stu-id="7cefe-140">**TRUE**</span></span> <br/> |<span data-ttu-id="7cefe-141">**TRUE**</span><span class="sxs-lookup"><span data-stu-id="7cefe-141">**TRUE**</span></span> <br/> |<span data-ttu-id="7cefe-142">**TRUE**</span><span class="sxs-lookup"><span data-stu-id="7cefe-142">**TRUE**</span></span> <br/> |
   
<span data-ttu-id="7cefe-143">O valor da propriedade **IsRecurring** que está definido para itens de calendário mestre recorrentes para o organizador está incorreto; Este valor deve ser definido como **TRUE**.</span><span class="sxs-lookup"><span data-stu-id="7cefe-143">The **IsRecurring** property value that is set for recurring master calendar items for the organizer is incorrect; this value should be set to **TRUE**.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="7cefe-144">A operação GetUserAvailability também tem um elemento [IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="7cefe-144">The GetUserAvailability operation also has an [IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md) element.</span></span> 
  
<span data-ttu-id="7cefe-145">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="7cefe-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7cefe-146">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7cefe-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7cefe-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="7cefe-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7cefe-148">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7cefe-148">Schema name</span></span>  <br/> |<span data-ttu-id="7cefe-149">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7cefe-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="7cefe-150">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7cefe-150">Validation file</span></span>  <br/> |<span data-ttu-id="7cefe-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7cefe-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7cefe-152">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="7cefe-152">Can be empty</span></span>  <br/> |<span data-ttu-id="7cefe-153">False</span><span class="sxs-lookup"><span data-stu-id="7cefe-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7cefe-154">Ver também</span><span class="sxs-lookup"><span data-stu-id="7cefe-154">See also</span></span>



[<span data-ttu-id="7cefe-155">TaskType.IsRecurring</span><span class="sxs-lookup"><span data-stu-id="7cefe-155">TaskType.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurring.aspx)
  
[<span data-ttu-id="7cefe-156">CalendarEventDetails.IsRecurring</span><span class="sxs-lookup"><span data-stu-id="7cefe-156">CalendarEventDetails.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarEventDetails.IsRecurring.aspx)
  
[<span data-ttu-id="7cefe-157">CalendarItemType.IsRecurring</span><span class="sxs-lookup"><span data-stu-id="7cefe-157">CalendarItemType.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurring.aspx)
  
[<span data-ttu-id="7cefe-158">MeetingRequestMessageType.IsRecurring</span><span class="sxs-lookup"><span data-stu-id="7cefe-158">MeetingRequestMessageType.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurring.aspx)
  
[<span data-ttu-id="7cefe-159">CalendarItemType.IsRecurringSpecified</span><span class="sxs-lookup"><span data-stu-id="7cefe-159">CalendarItemType.IsRecurringSpecified</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurringSpecified.aspx)
  
[<span data-ttu-id="7cefe-160">MeetingRequestMessageType.IsRecurringSpecified</span><span class="sxs-lookup"><span data-stu-id="7cefe-160">MeetingRequestMessageType.IsRecurringSpecified</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurringSpecified.aspx)
  
[<span data-ttu-id="7cefe-161">TaskType.IsRecurringSpecified</span><span class="sxs-lookup"><span data-stu-id="7cefe-161">TaskType.IsRecurringSpecified</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurringSpecified.aspx)


- [<span data-ttu-id="7cefe-162">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7cefe-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

