---
title: AttendeeType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttendeeType
api_type:
- schema
ms.assetid: 048043a8-dbad-45a0-97c8-4cad63d8898b
description: O elemento AttendeeType representa o tipo de participante que é identificado no elemento de Email (EmailAddressType). Este elemento é usado nas solicitações para sugestões de reunião.
ms.openlocfilehash: a08532ed78296102ee252c1e0c40beee7ca8ea5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751230"
---
# <a name="attendeetype"></a><span data-ttu-id="aefec-104">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="aefec-104">AttendeeType</span></span>

<span data-ttu-id="aefec-105">O elemento **AttendeeType** representa o tipo de participante que é identificado no elemento de [Email (EmailAddressType)](email-emailaddresstype.md) .</span><span class="sxs-lookup"><span data-stu-id="aefec-105">The **AttendeeType** element represents the type of attendee that is identified in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="aefec-106">Este elemento é usado nas solicitações para sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="aefec-106">This element is used in requests for meeting suggestions.</span></span> 
  
- [<span data-ttu-id="aefec-107">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="aefec-107">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
- [<span data-ttu-id="aefec-108">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="aefec-108">MailboxDataArray</span></span>](mailboxdataarray.md)
  
- [<span data-ttu-id="aefec-109">MailboxData</span><span class="sxs-lookup"><span data-stu-id="aefec-109">MailboxData</span></span>](mailboxdata.md)
  
- [<span data-ttu-id="aefec-110">AttendeeType</span><span class="sxs-lookup"><span data-stu-id="aefec-110">AttendeeType</span></span>](attendeetype.md)
  
```xml
<AttendeeType>Organizer or Required or Optional or Room or Resource</AttendeeType>
```

 <span data-ttu-id="aefec-111">**MeetingAttendeeType**</span><span class="sxs-lookup"><span data-stu-id="aefec-111">**MeetingAttendeeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aefec-112">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="aefec-112">Attributes and elements</span></span>

<span data-ttu-id="aefec-113">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="aefec-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aefec-114">Atributos</span><span class="sxs-lookup"><span data-stu-id="aefec-114">Attributes</span></span>

<span data-ttu-id="aefec-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="aefec-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aefec-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="aefec-116">Child elements</span></span>

<span data-ttu-id="aefec-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="aefec-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="aefec-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="aefec-118">Parent elements</span></span>

|<span data-ttu-id="aefec-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="aefec-119">**Element**</span></span>|<span data-ttu-id="aefec-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aefec-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aefec-121">MailboxData</span><span class="sxs-lookup"><span data-stu-id="aefec-121">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="aefec-122">Representa um usuário de caixa de correio individual e opções para o tipo de dados a serem retornadas sobre o usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="aefec-122">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="aefec-123">Este é o XPath a este elemento:</span><span class="sxs-lookup"><span data-stu-id="aefec-123">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="aefec-124">Text value</span><span class="sxs-lookup"><span data-stu-id="aefec-124">Text value</span></span>

<span data-ttu-id="aefec-125">Um valor de texto é necessário para esse elemento.</span><span class="sxs-lookup"><span data-stu-id="aefec-125">A text value is required for this element.</span></span> <span data-ttu-id="aefec-126">A tabela a seguir lista os valores possíveis para esse elemento.</span><span class="sxs-lookup"><span data-stu-id="aefec-126">The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="aefec-127">**Valor**</span><span class="sxs-lookup"><span data-stu-id="aefec-127">**Value**</span></span>|<span data-ttu-id="aefec-128">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aefec-128">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="aefec-129">Organizador</span><span class="sxs-lookup"><span data-stu-id="aefec-129">Organizer</span></span>  <br/> |<span data-ttu-id="aefec-130">O usuário de caixa de correio e o participante que criou o item de calendário.</span><span class="sxs-lookup"><span data-stu-id="aefec-130">The mailbox user and attendee who created the calendar item.</span></span>  <br/> |
|<span data-ttu-id="aefec-131">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="aefec-131">Required</span></span>  <br/> |<span data-ttu-id="aefec-132">Um usuário de caixa de correio que seja um participante necessário para a reunião.</span><span class="sxs-lookup"><span data-stu-id="aefec-132">A mailbox user who is a required attendee to the meeting.</span></span>  <br/> |
|<span data-ttu-id="aefec-133">Opcional</span><span class="sxs-lookup"><span data-stu-id="aefec-133">Optional</span></span>  <br/> |<span data-ttu-id="aefec-134">Um usuário de caixa de correio que um participante opcional para a reunião.</span><span class="sxs-lookup"><span data-stu-id="aefec-134">A mailbox user who is an optional attendee to the meeting.</span></span>  <br/> |
|<span data-ttu-id="aefec-135">Sala</span><span class="sxs-lookup"><span data-stu-id="aefec-135">Room</span></span>  <br/> |<span data-ttu-id="aefec-136">Uma entidade de caixa de correio que representa um recurso de sala usado para a reunião.</span><span class="sxs-lookup"><span data-stu-id="aefec-136">A mailbox entity that represents a room resource used for the meeting.</span></span>  <br/> |
|<span data-ttu-id="aefec-137">Recurso</span><span class="sxs-lookup"><span data-stu-id="aefec-137">Resource</span></span>  <br/> |<span data-ttu-id="aefec-138">Um recurso, como uma TV ou projetor que esteja agendado para ser usado na reunião.</span><span class="sxs-lookup"><span data-stu-id="aefec-138">A resource such as a TV or projector that is scheduled for use in the meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aefec-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="aefec-139">Remarks</span></span>

<span data-ttu-id="aefec-140">Este é um elemento necessário filho do elemento [MailboxData](mailboxdata.md) .</span><span class="sxs-lookup"><span data-stu-id="aefec-140">This element is a required child element of the [MailboxData](mailboxdata.md) element.</span></span> <span data-ttu-id="aefec-141">Esse elemento pode ocorrer apenas uma vez no elemento [MailboxData](mailboxdata.md) .</span><span class="sxs-lookup"><span data-stu-id="aefec-141">This element can only occur once in the [MailboxData](mailboxdata.md) element.</span></span> <span data-ttu-id="aefec-142">O esquema que descreve este elemento está localizado no diretório /EWS/ do computador que está executando o MicrosoftExchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="aefec-142">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="aefec-143">O tipo de esquema AttendeeType é usado para representar um item de calendário de participantes.</span><span class="sxs-lookup"><span data-stu-id="aefec-143">The AttendeeType schema type is used to represent attendees to a calendar item.</span></span> <span data-ttu-id="aefec-144">Não confunda esse elemento com elementos do tipo AttendeeType esquema.</span><span class="sxs-lookup"><span data-stu-id="aefec-144">Do not confuse this element with elements of the AttendeeType schema type.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="aefec-145">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="aefec-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aefec-146">Namespace</span><span class="sxs-lookup"><span data-stu-id="aefec-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aefec-147">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="aefec-147">Schema Name</span></span>  <br/> |<span data-ttu-id="aefec-148">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="aefec-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="aefec-149">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="aefec-149">Validation File</span></span>  <br/> |<span data-ttu-id="aefec-150">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="aefec-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aefec-151">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="aefec-151">Can be Empty</span></span>  <br/> |<span data-ttu-id="aefec-152">False</span><span class="sxs-lookup"><span data-stu-id="aefec-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aefec-153">Ver também</span><span class="sxs-lookup"><span data-stu-id="aefec-153">See also</span></span>

- [<span data-ttu-id="aefec-154">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="aefec-154">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="aefec-155">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="aefec-155">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="aefec-156">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="aefec-156">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

