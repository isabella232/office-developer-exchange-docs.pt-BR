---
title: AllowNewTimeProposal
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AllowNewTimeProposal
api_type:
- schema
ms.assetid: afdb4ec9-2daf-48a1-a0bb-a7f647f212f2
description: O elemento AllowNewTimeProposal indica se um novo tempo de reunião pode ser proposto para uma reunião por um participante.
ms.openlocfilehash: d5deed5044769c477ffe54cc533d5261ba2e1932
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751079"
---
# <a name="allownewtimeproposal"></a><span data-ttu-id="58d99-103">AllowNewTimeProposal</span><span class="sxs-lookup"><span data-stu-id="58d99-103">AllowNewTimeProposal</span></span>

<span data-ttu-id="58d99-104">O elemento **AllowNewTimeProposal** indica se um novo tempo de reunião pode ser proposto para uma reunião por um participante.</span><span class="sxs-lookup"><span data-stu-id="58d99-104">The **AllowNewTimeProposal** element indicates whether a new meeting time can be proposed for a meeting by an attendee.</span></span> 
  
```xml
<AllowNewTimeProposal/>
```

 <span data-ttu-id="58d99-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="58d99-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="58d99-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="58d99-106">Attributes and elements</span></span>

<span data-ttu-id="58d99-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="58d99-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="58d99-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="58d99-108">Attributes</span></span>

<span data-ttu-id="58d99-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="58d99-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="58d99-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="58d99-110">Child elements</span></span>

<span data-ttu-id="58d99-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="58d99-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="58d99-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="58d99-112">Parent elements</span></span>

|<span data-ttu-id="58d99-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="58d99-113">**Element**</span></span>|<span data-ttu-id="58d99-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="58d99-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="58d99-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="58d99-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="58d99-116">Representa uma reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="58d99-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="58d99-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="58d99-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="58d99-118">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="58d99-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="58d99-119">Text value</span><span class="sxs-lookup"><span data-stu-id="58d99-119">Text value</span></span>

<span data-ttu-id="58d99-120">É necessário um valor de texto que representa um valor booleano.</span><span class="sxs-lookup"><span data-stu-id="58d99-120">A text value that represents a Boolean value is required.</span></span> <span data-ttu-id="58d99-121">Um valor **true** indica que uma nova proposta para o tempo de reunião pode ser criada; um valor **false** indica que as novas propostas de horários não são permitidas.</span><span class="sxs-lookup"><span data-stu-id="58d99-121">A value of **true** indicates that a new proposal for the meeting time can be created; a value of **false** indicates that new time proposals are not allowed.</span></span> <span data-ttu-id="58d99-122">O organizador define esse valor na solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="58d99-122">The organizer sets this value in the meeting request.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="58d99-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="58d99-123">Remarks</span></span>

<span data-ttu-id="58d99-124">A propriedade AllowNewTimeProposal é gravável de leitura para o item de calendário do organizador.</span><span class="sxs-lookup"><span data-stu-id="58d99-124">The AllowNewTimeProposal property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="58d99-125">Ele é somente leitura para solicitações de reunião e itens de calendário dos participantes.</span><span class="sxs-lookup"><span data-stu-id="58d99-125">It is read-only for meeting requests and for attendees' calendar items.</span></span>
  
<span data-ttu-id="58d99-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="58d99-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="58d99-127">Serviços Web do Exchange não oferece suporte a novas mensagens de proposta de tempo.</span><span class="sxs-lookup"><span data-stu-id="58d99-127">Exchange Web Services does not support new time proposal messages.</span></span> <span data-ttu-id="58d99-128">Para obter as propriedades que são relacionadas às novas mensagens de proposta de tempo, use as propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="58d99-128">To get properties that are related to new time proposal messages, use extended properties.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="58d99-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="58d99-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="58d99-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="58d99-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="58d99-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="58d99-131">Schema name</span></span>  <br/> |<span data-ttu-id="58d99-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="58d99-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="58d99-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="58d99-133">Validation file</span></span>  <br/> |<span data-ttu-id="58d99-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="58d99-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="58d99-135">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="58d99-135">Can be empty</span></span>  <br/> |<span data-ttu-id="58d99-136">False</span><span class="sxs-lookup"><span data-stu-id="58d99-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="58d99-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="58d99-137">See also</span></span>

- [<span data-ttu-id="58d99-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="58d99-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

