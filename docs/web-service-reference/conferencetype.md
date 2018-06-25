---
title: ConferenceType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConferenceType
api_type:
- schema
ms.assetid: 6bcf6c18-2695-44b1-aabe-dadc52b2633a
description: O elemento ConferenceType descreve o tipo de conferência que for executado com um item de calendário.
ms.openlocfilehash: d312420606c5e1914fe321ae7c7c512f0833199c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751416"
---
# <a name="conferencetype"></a><span data-ttu-id="a2f8d-103">ConferenceType</span><span class="sxs-lookup"><span data-stu-id="a2f8d-103">ConferenceType</span></span>

<span data-ttu-id="a2f8d-104">O elemento **ConferenceType** descreve o tipo de conferência que for executado com um item de calendário.</span><span class="sxs-lookup"><span data-stu-id="a2f8d-104">The **ConferenceType** element describes the type of conferencing that is performed with a calendar item.</span></span> 
  
```xml
<ConferenceType/>
```

 <span data-ttu-id="a2f8d-105">**int**</span><span class="sxs-lookup"><span data-stu-id="a2f8d-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a2f8d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a2f8d-106">Attributes and elements</span></span>

<span data-ttu-id="a2f8d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a2f8d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2f8d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a2f8d-108">Attributes</span></span>

<span data-ttu-id="a2f8d-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a2f8d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a2f8d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a2f8d-110">Child elements</span></span>

<span data-ttu-id="a2f8d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a2f8d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a2f8d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a2f8d-112">Parent elements</span></span>

|<span data-ttu-id="a2f8d-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a2f8d-113">**Element**</span></span>|<span data-ttu-id="a2f8d-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a2f8d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2f8d-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="a2f8d-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="a2f8d-116">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a2f8d-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="a2f8d-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="a2f8d-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="a2f8d-118">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a2f8d-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a2f8d-119">Text value</span><span class="sxs-lookup"><span data-stu-id="a2f8d-119">Text value</span></span>

<span data-ttu-id="a2f8d-120">Se este elemento for usado, será necessário um valor de texto que representa um valor inteiro.</span><span class="sxs-lookup"><span data-stu-id="a2f8d-120">A text value that represents an integer value is required if this element is used.</span></span> <span data-ttu-id="a2f8d-121">Estes são os valores possíveis para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="a2f8d-121">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="a2f8d-122">0 = o NetMeeting</span><span class="sxs-lookup"><span data-stu-id="a2f8d-122">0 = NetMeeting</span></span>
    
- <span data-ttu-id="a2f8d-123">1 = a NetShow</span><span class="sxs-lookup"><span data-stu-id="a2f8d-123">1 = NetShow</span></span>
    
- <span data-ttu-id="a2f8d-124">2 = bate-papo</span><span class="sxs-lookup"><span data-stu-id="a2f8d-124">2 = Chat</span></span>
    
## <a name="remarks"></a><span data-ttu-id="a2f8d-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="a2f8d-125">Remarks</span></span>

<span data-ttu-id="a2f8d-126">A propriedade **MeetingWorkspaceUrl** é gravável de leitura para o item de calendário do organizador.</span><span class="sxs-lookup"><span data-stu-id="a2f8d-126">The **MeetingWorkspaceUrl** property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="a2f8d-127">Ele é somente leitura para solicitações de reunião e itens de calendário do participante.</span><span class="sxs-lookup"><span data-stu-id="a2f8d-127">It is read-only for meeting requests and for attendee's calendar items.</span></span> 
  
<span data-ttu-id="a2f8d-128">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="a2f8d-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="a2f8d-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a2f8d-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2f8d-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="a2f8d-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a2f8d-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a2f8d-131">Schema Name</span></span>  <br/> |<span data-ttu-id="a2f8d-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a2f8d-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="a2f8d-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a2f8d-133">Validation File</span></span>  <br/> |<span data-ttu-id="a2f8d-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a2f8d-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a2f8d-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a2f8d-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="a2f8d-136">False</span><span class="sxs-lookup"><span data-stu-id="a2f8d-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a2f8d-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="a2f8d-137">See also</span></span>



- [<span data-ttu-id="a2f8d-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a2f8d-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

