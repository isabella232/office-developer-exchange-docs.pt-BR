---
title: Participante
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Attendee
api_type:
- schema
ms.assetid: 393c3d7e-7416-458a-b976-270b88eaaa03
description: O elemento participante representa participantes e recursos de uma reunião.
ms.openlocfilehash: f376e59b27017e0a9d27692cb1a4ae759cd1af0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457645"
---
# <a name="attendee"></a><span data-ttu-id="4f751-103">Participante</span><span class="sxs-lookup"><span data-stu-id="4f751-103">Attendee</span></span>

<span data-ttu-id="4f751-104">O elemento **participante** representa participantes e recursos de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="4f751-104">The **Attendee** element represents attendees and resources for a meeting.</span></span> 
  
```xml
<Attendee>
   <Mailbox/>
   <ResponseType/>
   <LastResponseTime/>
</Attendee>
```

 <span data-ttu-id="4f751-105">**Articipantetype**</span><span class="sxs-lookup"><span data-stu-id="4f751-105">**AttendeeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4f751-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4f751-106">Attributes and elements</span></span>

<span data-ttu-id="4f751-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4f751-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4f751-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4f751-108">Attributes</span></span>

<span data-ttu-id="4f751-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4f751-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4f751-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4f751-110">Child elements</span></span>

|<span data-ttu-id="4f751-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4f751-111">**Element**</span></span>|<span data-ttu-id="4f751-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4f751-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4f751-113">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="4f751-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="4f751-114">Identifica um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="4f751-114">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="4f751-115">ResponseType</span><span class="sxs-lookup"><span data-stu-id="4f751-115">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="4f751-116">Representa o tipo de resposta de destinatário recebido para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="4f751-116">Represents the type of recipient response that is received for a meeting.</span></span> <span data-ttu-id="4f751-117">Essa propriedade só é relevante para o item de calendário do organizador da reunião.</span><span class="sxs-lookup"><span data-stu-id="4f751-117">This property is only relevant to a meeting organizer's calendar item.</span></span>  <br/> |
|[<span data-ttu-id="4f751-118">LastResponseTime</span><span class="sxs-lookup"><span data-stu-id="4f751-118">LastResponseTime</span></span>](lastresponsetime.md) <br/> |<span data-ttu-id="4f751-119">Representa a data e a hora da última resposta recebida.</span><span class="sxs-lookup"><span data-stu-id="4f751-119">Represents the date and time of the latest response that is received.</span></span>  <br/> |
|[<span data-ttu-id="4f751-120">ProposedStart</span><span class="sxs-lookup"><span data-stu-id="4f751-120">ProposedStart</span></span>](proposedstart-attendeetype.md) <br/> |<span data-ttu-id="4f751-121">Representa a hora de início proposta de um participante para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="4f751-121">Represents an attendee's proposed start time for a meeting.</span></span> <br/> |
|[<span data-ttu-id="4f751-122">ProposedEnd</span><span class="sxs-lookup"><span data-stu-id="4f751-122">ProposedEnd</span></span>](proposedend-attendeetype.md) <br/> |<span data-ttu-id="4f751-123">Representa a hora de término proposta de um participante para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="4f751-123">Represents an attendee's proposed end time for a meeting.</span></span> <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4f751-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4f751-124">Parent elements</span></span>

|<span data-ttu-id="4f751-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4f751-125">**Element**</span></span>|<span data-ttu-id="4f751-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4f751-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4f751-127">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="4f751-127">RequiredAttendees</span></span>](requiredattendees.md) <br/> |<span data-ttu-id="4f751-128">Representa participantes que são necessários para participar de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="4f751-128">Represents attendees that are required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="4f751-129">OptionalAttendees</span><span class="sxs-lookup"><span data-stu-id="4f751-129">OptionalAttendees</span></span>](optionalattendees.md) <br/> |<span data-ttu-id="4f751-130">Representa os participantes que não precisam participar de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="4f751-130">Represents attendees that are not required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="4f751-131">Recursos</span><span class="sxs-lookup"><span data-stu-id="4f751-131">Resources</span></span>](resources.md) <br/> |<span data-ttu-id="4f751-132">Representa um recurso agendado para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="4f751-132">Represents a scheduled resource for a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4f751-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="4f751-133">Remarks</span></span>

<span data-ttu-id="4f751-134">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="4f751-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4f751-135">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="4f751-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4f751-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="4f751-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4f751-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4f751-137">Schema name</span></span>  <br/> |<span data-ttu-id="4f751-138">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="4f751-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="4f751-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4f751-139">Validation file</span></span>  <br/> |<span data-ttu-id="4f751-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4f751-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4f751-141">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="4f751-141">Can be empty</span></span>  <br/> |<span data-ttu-id="4f751-142">False</span><span class="sxs-lookup"><span data-stu-id="4f751-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4f751-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="4f751-143">See also</span></span>

- [<span data-ttu-id="4f751-144">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4f751-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

