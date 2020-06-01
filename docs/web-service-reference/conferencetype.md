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
description: O elemento ConferenceType descreve o tipo de conferência que é executado com um item de calendário.
ms.openlocfilehash: 482fc09d709e2b151b255107af59cb98de236aec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463927"
---
# <a name="conferencetype"></a><span data-ttu-id="2e3d0-103">ConferenceType</span><span class="sxs-lookup"><span data-stu-id="2e3d0-103">ConferenceType</span></span>

<span data-ttu-id="2e3d0-104">O elemento **ConferenceType** descreve o tipo de conferência que é executado com um item de calendário.</span><span class="sxs-lookup"><span data-stu-id="2e3d0-104">The **ConferenceType** element describes the type of conferencing that is performed with a calendar item.</span></span> 
  
```xml
<ConferenceType/>
```

 <span data-ttu-id="2e3d0-105">**int**</span><span class="sxs-lookup"><span data-stu-id="2e3d0-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2e3d0-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="2e3d0-106">Attributes and elements</span></span>

<span data-ttu-id="2e3d0-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2e3d0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2e3d0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="2e3d0-108">Attributes</span></span>

<span data-ttu-id="2e3d0-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2e3d0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2e3d0-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2e3d0-110">Child elements</span></span>

<span data-ttu-id="2e3d0-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="2e3d0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2e3d0-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2e3d0-112">Parent elements</span></span>

|<span data-ttu-id="2e3d0-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2e3d0-113">**Element**</span></span>|<span data-ttu-id="2e3d0-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2e3d0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2e3d0-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="2e3d0-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="2e3d0-116">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2e3d0-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="2e3d0-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="2e3d0-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="2e3d0-118">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2e3d0-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2e3d0-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="2e3d0-119">Text value</span></span>

<span data-ttu-id="2e3d0-120">Um valor de texto que representa um valor inteiro será necessário se esse elemento for usado.</span><span class="sxs-lookup"><span data-stu-id="2e3d0-120">A text value that represents an integer value is required if this element is used.</span></span> <span data-ttu-id="2e3d0-121">Estes são os valores possíveis para este elemento:</span><span class="sxs-lookup"><span data-stu-id="2e3d0-121">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="2e3d0-122">0 = NetMeeting</span><span class="sxs-lookup"><span data-stu-id="2e3d0-122">0 = NetMeeting</span></span>
    
- <span data-ttu-id="2e3d0-123">1 = NetShow</span><span class="sxs-lookup"><span data-stu-id="2e3d0-123">1 = NetShow</span></span>
    
- <span data-ttu-id="2e3d0-124">2 = chat</span><span class="sxs-lookup"><span data-stu-id="2e3d0-124">2 = Chat</span></span>
    
## <a name="remarks"></a><span data-ttu-id="2e3d0-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="2e3d0-125">Remarks</span></span>

<span data-ttu-id="2e3d0-126">A propriedade **MeetingWorkspaceUrl** é leitura/gravação para o item de calendário do organizador.</span><span class="sxs-lookup"><span data-stu-id="2e3d0-126">The **MeetingWorkspaceUrl** property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="2e3d0-127">É somente leitura para solicitações de reunião e itens de calendário do participante.</span><span class="sxs-lookup"><span data-stu-id="2e3d0-127">It is read-only for meeting requests and for attendee's calendar items.</span></span> 
  
<span data-ttu-id="2e3d0-128">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="2e3d0-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="2e3d0-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="2e3d0-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2e3d0-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="2e3d0-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2e3d0-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2e3d0-131">Schema Name</span></span>  <br/> |<span data-ttu-id="2e3d0-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="2e3d0-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="2e3d0-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2e3d0-133">Validation File</span></span>  <br/> |<span data-ttu-id="2e3d0-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2e3d0-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2e3d0-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2e3d0-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="2e3d0-136">False</span><span class="sxs-lookup"><span data-stu-id="2e3d0-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2e3d0-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="2e3d0-137">See also</span></span>



- [<span data-ttu-id="2e3d0-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="2e3d0-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

