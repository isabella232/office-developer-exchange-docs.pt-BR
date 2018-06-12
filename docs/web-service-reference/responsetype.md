---
title: ResponseType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseType
api_type:
- schema
ms.assetid: cdc09dda-ce20-4504-880d-9da6025ca812
description: O elemento ResponseType representa o tipo de destinatário resposta recebida para uma reunião.
ms.openlocfilehash: fcfd47cb988ee00303b2c4205cb3d058cb6599b2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825200"
---
# <a name="responsetype"></a><span data-ttu-id="1011c-103">ResponseType</span><span class="sxs-lookup"><span data-stu-id="1011c-103">ResponseType</span></span>

<span data-ttu-id="1011c-104">O elemento **ResponseType** representa o tipo de destinatário resposta recebida para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="1011c-104">The **ResponseType** element represents the type of recipient response that is received for a meeting.</span></span> 
  
```xml
<ResponseType/>
```

 <span data-ttu-id="1011c-105">**ResponseTypeType**</span><span class="sxs-lookup"><span data-stu-id="1011c-105">**ResponseTypeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1011c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="1011c-106">Attributes and elements</span></span>

<span data-ttu-id="1011c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1011c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1011c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1011c-108">Attributes</span></span>

<span data-ttu-id="1011c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1011c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1011c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1011c-110">Child elements</span></span>

<span data-ttu-id="1011c-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1011c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1011c-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1011c-112">Parent elements</span></span>

|<span data-ttu-id="1011c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1011c-113">**Element**</span></span>|<span data-ttu-id="1011c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1011c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1011c-115">Attendee</span><span class="sxs-lookup"><span data-stu-id="1011c-115">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="1011c-116">Representa os participantes e recursos para uma reunião.</span><span class="sxs-lookup"><span data-stu-id="1011c-116">Represents attendees and resources for a meeting.</span></span>  <br/> |
|[<span data-ttu-id="1011c-117">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="1011c-117">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="1011c-118">Representa o cancelamento da reunião no armazenamento do Exchange</span><span class="sxs-lookup"><span data-stu-id="1011c-118">Represents a meeting cancellation in the Exchange store</span></span>  <br/> |
|[<span data-ttu-id="1011c-119">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="1011c-119">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="1011c-120">Representa uma mensagem de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1011c-120">Represents a meeting message in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1011c-121">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="1011c-121">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="1011c-122">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1011c-122">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1011c-123">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="1011c-123">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="1011c-124">Representa uma resposta de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1011c-124">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1011c-125">Text value</span><span class="sxs-lookup"><span data-stu-id="1011c-125">Text value</span></span>

<span data-ttu-id="1011c-126">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="1011c-126">A text value is required.</span></span> <span data-ttu-id="1011c-127">Estes são os valores de texto possíveis para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="1011c-127">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="1011c-128">Desconhecida</span><span class="sxs-lookup"><span data-stu-id="1011c-128">Unknown</span></span>
    
- <span data-ttu-id="1011c-129">Organizador</span><span class="sxs-lookup"><span data-stu-id="1011c-129">Organizer</span></span>
    
- <span data-ttu-id="1011c-130">Provisório</span><span class="sxs-lookup"><span data-stu-id="1011c-130">Tentative</span></span>
    
- <span data-ttu-id="1011c-131">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1011c-131">Accept</span></span>
    
- <span data-ttu-id="1011c-132">Recusar</span><span class="sxs-lookup"><span data-stu-id="1011c-132">Decline</span></span>
    
- <span data-ttu-id="1011c-133">NoResponseReceived</span><span class="sxs-lookup"><span data-stu-id="1011c-133">NoResponseReceived</span></span>
    
## <a name="remarks"></a><span data-ttu-id="1011c-134">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="1011c-134">Remarks</span></span>

<span data-ttu-id="1011c-135">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="1011c-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1011c-136">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="1011c-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1011c-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="1011c-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1011c-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1011c-138">Schema Name</span></span>  <br/> |<span data-ttu-id="1011c-139">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="1011c-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="1011c-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1011c-140">Validation File</span></span>  <br/> |<span data-ttu-id="1011c-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1011c-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1011c-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1011c-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="1011c-143">False</span><span class="sxs-lookup"><span data-stu-id="1011c-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1011c-144">Ver também</span><span class="sxs-lookup"><span data-stu-id="1011c-144">See also</span></span>



- [<span data-ttu-id="1011c-145">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1011c-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

