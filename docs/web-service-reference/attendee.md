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
description: O elemento Attendee representa participantes e recursos para uma reunião.
ms.openlocfilehash: 60cb0839c2f6de69b833c11f4594d40c14cd8887
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751225"
---
# <a name="attendee"></a><span data-ttu-id="e64c0-103">Participante</span><span class="sxs-lookup"><span data-stu-id="e64c0-103">Attendee</span></span>

<span data-ttu-id="e64c0-104">O elemento **Attendee** representa participantes e recursos para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="e64c0-104">The **Attendee** element represents attendees and resources for a meeting.</span></span> 
  
```xml
<Attendee>
   <Mailbox/>
   <ResponseType/>
   <LastResponseTime/>
</Attendee>
```

 <span data-ttu-id="e64c0-105">**AttendeeType**</span><span class="sxs-lookup"><span data-stu-id="e64c0-105">**AttendeeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e64c0-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e64c0-106">Attributes and elements</span></span>

<span data-ttu-id="e64c0-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e64c0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e64c0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e64c0-108">Attributes</span></span>

<span data-ttu-id="e64c0-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e64c0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e64c0-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e64c0-110">Child elements</span></span>

|<span data-ttu-id="e64c0-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e64c0-111">**Element**</span></span>|<span data-ttu-id="e64c0-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e64c0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e64c0-113">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="e64c0-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="e64c0-114">Identifica um endereço de email totalmente resolvido.</span><span class="sxs-lookup"><span data-stu-id="e64c0-114">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="e64c0-115">ResponseType</span><span class="sxs-lookup"><span data-stu-id="e64c0-115">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="e64c0-116">Representa o tipo de destinatário resposta recebida para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="e64c0-116">Represents the type of recipient response that is received for a meeting.</span></span> <span data-ttu-id="e64c0-117">Essa propriedade só é relevante para o item de calendário do organizador da reunião.</span><span class="sxs-lookup"><span data-stu-id="e64c0-117">This property is only relevant to a meeting organizer's calendar item.</span></span>  <br/> |
|[<span data-ttu-id="e64c0-118">LastResponseTime</span><span class="sxs-lookup"><span data-stu-id="e64c0-118">LastResponseTime</span></span>](lastresponsetime.md) <br/> |<span data-ttu-id="e64c0-119">Representa a data e hora da resposta mais recente que é recebida.</span><span class="sxs-lookup"><span data-stu-id="e64c0-119">Represents the date and time of the latest response that is received.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e64c0-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e64c0-120">Parent elements</span></span>

|<span data-ttu-id="e64c0-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e64c0-121">**Element**</span></span>|<span data-ttu-id="e64c0-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e64c0-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e64c0-123">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="e64c0-123">RequiredAttendees</span></span>](requiredattendees.md) <br/> |<span data-ttu-id="e64c0-124">Representa os participantes necessários para participar de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="e64c0-124">Represents attendees that are required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="e64c0-125">OptionalAttendees</span><span class="sxs-lookup"><span data-stu-id="e64c0-125">OptionalAttendees</span></span>](optionalattendees.md) <br/> |<span data-ttu-id="e64c0-126">Representa a participantes que não são necessárias para participar de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="e64c0-126">Represents attendees that are not required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="e64c0-127">Recursos</span><span class="sxs-lookup"><span data-stu-id="e64c0-127">Resources</span></span>](resources.md) <br/> |<span data-ttu-id="e64c0-128">Representa um recurso agendado para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="e64c0-128">Represents a scheduled resource for a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e64c0-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="e64c0-129">Remarks</span></span>

<span data-ttu-id="e64c0-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="e64c0-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e64c0-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e64c0-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e64c0-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="e64c0-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e64c0-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e64c0-133">Schema name</span></span>  <br/> |<span data-ttu-id="e64c0-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e64c0-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="e64c0-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e64c0-135">Validation file</span></span>  <br/> |<span data-ttu-id="e64c0-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e64c0-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e64c0-137">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="e64c0-137">Can be empty</span></span>  <br/> |<span data-ttu-id="e64c0-138">False</span><span class="sxs-lookup"><span data-stu-id="e64c0-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e64c0-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="e64c0-139">See also</span></span>

- [<span data-ttu-id="e64c0-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e64c0-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

