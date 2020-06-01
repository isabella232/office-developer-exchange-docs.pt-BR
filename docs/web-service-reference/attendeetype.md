---
title: Articipantetype
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
description: O elemento attendetype representa o tipo de participante identificado no elemento email (EmailAddresstype). Este elemento é usado em solicitações de sugestões de reunião.
ms.openlocfilehash: 104b9f38cc891310ecb47c0b47837a912ced6ab7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462294"
---
# <a name="attendeetype"></a><span data-ttu-id="3f9b7-104">Articipantetype</span><span class="sxs-lookup"><span data-stu-id="3f9b7-104">AttendeeType</span></span>

<span data-ttu-id="3f9b7-105">O elemento **Attendetype** representa o tipo de participante identificado no elemento [email (EmailAddressType)](email-emailaddresstype.md) .</span><span class="sxs-lookup"><span data-stu-id="3f9b7-105">The **AttendeeType** element represents the type of attendee that is identified in the [Email (EmailAddressType)](email-emailaddresstype.md) element.</span></span> <span data-ttu-id="3f9b7-106">Este elemento é usado em solicitações de sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="3f9b7-106">This element is used in requests for meeting suggestions.</span></span> 
  
- [<span data-ttu-id="3f9b7-107">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="3f9b7-107">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
- [<span data-ttu-id="3f9b7-108">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="3f9b7-108">MailboxDataArray</span></span>](mailboxdataarray.md)
  
- [<span data-ttu-id="3f9b7-109">MailboxData</span><span class="sxs-lookup"><span data-stu-id="3f9b7-109">MailboxData</span></span>](mailboxdata.md)
  
- [<span data-ttu-id="3f9b7-110">Articipantetype</span><span class="sxs-lookup"><span data-stu-id="3f9b7-110">AttendeeType</span></span>](attendeetype.md)
  
```xml
<AttendeeType>Organizer or Required or Optional or Room or Resource</AttendeeType>
```

 <span data-ttu-id="3f9b7-111">**MeetingAttendeeType**</span><span class="sxs-lookup"><span data-stu-id="3f9b7-111">**MeetingAttendeeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3f9b7-112">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3f9b7-112">Attributes and elements</span></span>

<span data-ttu-id="3f9b7-113">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3f9b7-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3f9b7-114">Atributos</span><span class="sxs-lookup"><span data-stu-id="3f9b7-114">Attributes</span></span>

<span data-ttu-id="3f9b7-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3f9b7-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3f9b7-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3f9b7-116">Child elements</span></span>

<span data-ttu-id="3f9b7-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3f9b7-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3f9b7-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3f9b7-118">Parent elements</span></span>

|<span data-ttu-id="3f9b7-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3f9b7-119">**Element**</span></span>|<span data-ttu-id="3f9b7-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3f9b7-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f9b7-121">MailboxData</span><span class="sxs-lookup"><span data-stu-id="3f9b7-121">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="3f9b7-122">Representa um usuário de caixa de correio individual e opções para o tipo de dados a ser retornado sobre o usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="3f9b7-122">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> <span data-ttu-id="3f9b7-123">Este é o XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="3f9b7-123">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray[i]/MailboxData` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3f9b7-124">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="3f9b7-124">Text value</span></span>

<span data-ttu-id="3f9b7-125">Um valor de texto é necessário para este elemento.</span><span class="sxs-lookup"><span data-stu-id="3f9b7-125">A text value is required for this element.</span></span> <span data-ttu-id="3f9b7-126">A tabela a seguir lista os valores possíveis para este elemento.</span><span class="sxs-lookup"><span data-stu-id="3f9b7-126">The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="3f9b7-127">**Valor**</span><span class="sxs-lookup"><span data-stu-id="3f9b7-127">**Value**</span></span>|<span data-ttu-id="3f9b7-128">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3f9b7-128">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3f9b7-129">Organizador</span><span class="sxs-lookup"><span data-stu-id="3f9b7-129">Organizer</span></span>  <br/> |<span data-ttu-id="3f9b7-130">O usuário de caixa de correio e participante que criou o item de calendário.</span><span class="sxs-lookup"><span data-stu-id="3f9b7-130">The mailbox user and attendee who created the calendar item.</span></span>  <br/> |
|<span data-ttu-id="3f9b7-131">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="3f9b7-131">Required</span></span>  <br/> |<span data-ttu-id="3f9b7-132">Um usuário de caixa de correio que é um participante necessário para a reunião.</span><span class="sxs-lookup"><span data-stu-id="3f9b7-132">A mailbox user who is a required attendee to the meeting.</span></span>  <br/> |
|<span data-ttu-id="3f9b7-133">Opcional</span><span class="sxs-lookup"><span data-stu-id="3f9b7-133">Optional</span></span>  <br/> |<span data-ttu-id="3f9b7-134">Um usuário de caixa de correio que é um participante opcional da reunião.</span><span class="sxs-lookup"><span data-stu-id="3f9b7-134">A mailbox user who is an optional attendee to the meeting.</span></span>  <br/> |
|<span data-ttu-id="3f9b7-135">Sala</span><span class="sxs-lookup"><span data-stu-id="3f9b7-135">Room</span></span>  <br/> |<span data-ttu-id="3f9b7-136">Uma entidade de caixa de correio que representa um recurso de sala usado para a reunião.</span><span class="sxs-lookup"><span data-stu-id="3f9b7-136">A mailbox entity that represents a room resource used for the meeting.</span></span>  <br/> |
|<span data-ttu-id="3f9b7-137">Resource</span><span class="sxs-lookup"><span data-stu-id="3f9b7-137">Resource</span></span>  <br/> |<span data-ttu-id="3f9b7-138">Um recurso como uma TV ou um projetor agendado para uso na reunião.</span><span class="sxs-lookup"><span data-stu-id="3f9b7-138">A resource such as a TV or projector that is scheduled for use in the meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3f9b7-139">Comentários</span><span class="sxs-lookup"><span data-stu-id="3f9b7-139">Remarks</span></span>

<span data-ttu-id="3f9b7-140">Este elemento é um elemento filho obrigatório do elemento [MailboxData](mailboxdata.md) .</span><span class="sxs-lookup"><span data-stu-id="3f9b7-140">This element is a required child element of the [MailboxData](mailboxdata.md) element.</span></span> <span data-ttu-id="3f9b7-141">Este elemento só pode ocorrer uma vez no elemento [MailboxData](mailboxdata.md) .</span><span class="sxs-lookup"><span data-stu-id="3f9b7-141">This element can only occur once in the [MailboxData](mailboxdata.md) element.</span></span> <span data-ttu-id="3f9b7-142">O esquema que descreve este elemento está localizado no diretório/EWS/do computador que está executando o MicrosoftExchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="3f9b7-142">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="3f9b7-143">O tipo de esquema attendetype é usado para representar participantes para um item de calendário.</span><span class="sxs-lookup"><span data-stu-id="3f9b7-143">The AttendeeType schema type is used to represent attendees to a calendar item.</span></span> <span data-ttu-id="3f9b7-144">Não confunda este elemento com elementos do tipo de esquema attendetype.</span><span class="sxs-lookup"><span data-stu-id="3f9b7-144">Do not confuse this element with elements of the AttendeeType schema type.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="3f9b7-145">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3f9b7-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3f9b7-146">Namespace</span><span class="sxs-lookup"><span data-stu-id="3f9b7-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3f9b7-147">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3f9b7-147">Schema Name</span></span>  <br/> |<span data-ttu-id="3f9b7-148">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3f9b7-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="3f9b7-149">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3f9b7-149">Validation File</span></span>  <br/> |<span data-ttu-id="3f9b7-150">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3f9b7-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3f9b7-151">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3f9b7-151">Can be Empty</span></span>  <br/> |<span data-ttu-id="3f9b7-152">False</span><span class="sxs-lookup"><span data-stu-id="3f9b7-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3f9b7-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="3f9b7-153">See also</span></span>

- [<span data-ttu-id="3f9b7-154">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="3f9b7-154">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="3f9b7-155">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="3f9b7-155">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="3f9b7-156">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="3f9b7-156">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

