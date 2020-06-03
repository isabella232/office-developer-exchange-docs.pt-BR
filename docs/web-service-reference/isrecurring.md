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
description: O elemento IsRecurring indica se um item de calendário, uma solicitação de reunião ou uma tarefa é parte de um item recorrente. Este elemento é somente leitura.
ms.openlocfilehash: 72c71c1955b69f1c0df855ce4bd0ed02d4c89122
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526484"
---
# <a name="isrecurring"></a><span data-ttu-id="3b76e-104">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="3b76e-104">IsRecurring</span></span>

<span data-ttu-id="3b76e-105">O elemento **IsRecurring** indica se um item de calendário, uma solicitação de reunião ou uma tarefa é parte de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="3b76e-105">The **IsRecurring** element indicates whether a calendar item, meeting request, or task is part of a recurring item.</span></span> <span data-ttu-id="3b76e-106">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="3b76e-106">This element is read-only.</span></span> 
  
```xml
<IsRecurring/>
```

 <span data-ttu-id="3b76e-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="3b76e-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3b76e-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3b76e-108">Attributes and elements</span></span>

<span data-ttu-id="3b76e-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3b76e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3b76e-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="3b76e-110">Attributes</span></span>

<span data-ttu-id="3b76e-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3b76e-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3b76e-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3b76e-112">Child elements</span></span>

<span data-ttu-id="3b76e-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3b76e-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3b76e-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3b76e-114">Parent elements</span></span>

|<span data-ttu-id="3b76e-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3b76e-115">**Element**</span></span>|<span data-ttu-id="3b76e-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3b76e-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b76e-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="3b76e-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="3b76e-118">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3b76e-118">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="3b76e-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="3b76e-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="3b76e-120">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3b76e-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3b76e-121">Tarefa</span><span class="sxs-lookup"><span data-stu-id="3b76e-121">Task</span></span>](task.md) <br/> |<span data-ttu-id="3b76e-122">Representa uma tarefa no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="3b76e-122">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3b76e-123">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="3b76e-123">Text value</span></span>

<span data-ttu-id="3b76e-124">Um valor de texto que representa um valor booliano é necessário.</span><span class="sxs-lookup"><span data-stu-id="3b76e-124">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3b76e-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="3b76e-125">Remarks</span></span>

<span data-ttu-id="3b76e-126">A tabela a seguir mostra como a propriedade **IsRecurring** é definida para diferentes tipos de item de calendário para os organizadores e participantes e para solicitações de reunião e atualizações.</span><span class="sxs-lookup"><span data-stu-id="3b76e-126">The following table shows how the **IsRecurring** property is set for different calendar item types for organizers and attendees and for meeting requests and updates.</span></span> 
  
|<span data-ttu-id="3b76e-127">**Tipo CalendarItem**</span><span class="sxs-lookup"><span data-stu-id="3b76e-127">**CalendarItem Type**</span></span>|<span data-ttu-id="3b76e-128">**Organizador <br/> (IsRecurring)**</span><span class="sxs-lookup"><span data-stu-id="3b76e-128">**Organizer  <br/> (IsRecurring)**</span></span>|<span data-ttu-id="3b76e-129">**Participante <br/> (IsRecurring)**</span><span class="sxs-lookup"><span data-stu-id="3b76e-129">**Attendee  <br/> (IsRecurring)**</span></span>|<span data-ttu-id="3b76e-130">**Solicitação de reunião/atualização <br/> (IsRecurring)**</span><span class="sxs-lookup"><span data-stu-id="3b76e-130">**Meeting request/update  <br/> (IsRecurring)**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="3b76e-131">Ocorrência única</span><span class="sxs-lookup"><span data-stu-id="3b76e-131">Single Occurrence</span></span>  <br/> |<span data-ttu-id="3b76e-132">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="3b76e-132">**FALSE**</span></span> <br/> |<span data-ttu-id="3b76e-133">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="3b76e-133">**FALSE**</span></span> <br/> |<span data-ttu-id="3b76e-134">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="3b76e-134">**FALSE**</span></span> <br/> |
|<span data-ttu-id="3b76e-135">Mestre recorrente</span><span class="sxs-lookup"><span data-stu-id="3b76e-135">Recurring Master</span></span>  <br/> |<span data-ttu-id="3b76e-136">**FALSE**</span><span class="sxs-lookup"><span data-stu-id="3b76e-136">**FALSE**</span></span> <br/> |<span data-ttu-id="3b76e-137">**VERDADEIRO**</span><span class="sxs-lookup"><span data-stu-id="3b76e-137">**TRUE**</span></span> <br/> |<span data-ttu-id="3b76e-138">**VERDADEIRO**</span><span class="sxs-lookup"><span data-stu-id="3b76e-138">**TRUE**</span></span> <br/> |
|<span data-ttu-id="3b76e-139">Exceção recorrente</span><span class="sxs-lookup"><span data-stu-id="3b76e-139">Recurring Exception</span></span>  <br/> |<span data-ttu-id="3b76e-140">**VERDADEIRO**</span><span class="sxs-lookup"><span data-stu-id="3b76e-140">**TRUE**</span></span> <br/> |<span data-ttu-id="3b76e-141">**VERDADEIRO**</span><span class="sxs-lookup"><span data-stu-id="3b76e-141">**TRUE**</span></span> <br/> |<span data-ttu-id="3b76e-142">**VERDADEIRO**</span><span class="sxs-lookup"><span data-stu-id="3b76e-142">**TRUE**</span></span> <br/> |
   
<span data-ttu-id="3b76e-143">O valor da propriedade **IsRecurring** que é definido para itens de calendário mestre recorrentes para o organizador está incorreto; Esse valor deve ser definido como **true**.</span><span class="sxs-lookup"><span data-stu-id="3b76e-143">The **IsRecurring** property value that is set for recurring master calendar items for the organizer is incorrect; this value should be set to **TRUE**.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="3b76e-144">A operação GetUserAvailability também tem um elemento [IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="3b76e-144">The GetUserAvailability operation also has an [IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md) element.</span></span> 
  
<span data-ttu-id="3b76e-145">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="3b76e-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3b76e-146">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3b76e-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3b76e-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="3b76e-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3b76e-148">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3b76e-148">Schema name</span></span>  <br/> |<span data-ttu-id="3b76e-149">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3b76e-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="3b76e-150">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3b76e-150">Validation file</span></span>  <br/> |<span data-ttu-id="3b76e-151">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3b76e-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3b76e-152">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="3b76e-152">Can be empty</span></span>  <br/> |<span data-ttu-id="3b76e-153">False</span><span class="sxs-lookup"><span data-stu-id="3b76e-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3b76e-154">Confira também</span><span class="sxs-lookup"><span data-stu-id="3b76e-154">See also</span></span>



[<span data-ttu-id="3b76e-155">TaskType. IsRecurring</span><span class="sxs-lookup"><span data-stu-id="3b76e-155">TaskType.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurring.aspx)
  
[<span data-ttu-id="3b76e-156">CalendarEventDetails. IsRecurring</span><span class="sxs-lookup"><span data-stu-id="3b76e-156">CalendarEventDetails.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarEventDetails.IsRecurring.aspx)
  
[<span data-ttu-id="3b76e-157">CalendarItemType. IsRecurring</span><span class="sxs-lookup"><span data-stu-id="3b76e-157">CalendarItemType.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurring.aspx)
  
[<span data-ttu-id="3b76e-158">MeetingRequestMessageType. IsRecurring</span><span class="sxs-lookup"><span data-stu-id="3b76e-158">MeetingRequestMessageType.IsRecurring</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurring.aspx)
  
[<span data-ttu-id="3b76e-159">CalendarItemType.IsRecurringSpecified</span><span class="sxs-lookup"><span data-stu-id="3b76e-159">CalendarItemType.IsRecurringSpecified</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurringSpecified.aspx)
  
[<span data-ttu-id="3b76e-160">MeetingRequestMessageType.IsRecurringSpecified</span><span class="sxs-lookup"><span data-stu-id="3b76e-160">MeetingRequestMessageType.IsRecurringSpecified</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurringSpecified.aspx)
  
[<span data-ttu-id="3b76e-161">TaskType. IsRecurringSpecified</span><span class="sxs-lookup"><span data-stu-id="3b76e-161">TaskType.IsRecurringSpecified</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurringSpecified.aspx)


- [<span data-ttu-id="3b76e-162">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="3b76e-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

