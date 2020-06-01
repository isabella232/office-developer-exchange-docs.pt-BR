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
description: O elemento AllowNewTimeProposal indica se um novo horário de reunião pode ser proposto para uma reunião por um participante.
ms.openlocfilehash: b3f2c569bced08c66144680a4fddd6e8bac0cecf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464802"
---
# <a name="allownewtimeproposal"></a><span data-ttu-id="d7304-103">AllowNewTimeProposal</span><span class="sxs-lookup"><span data-stu-id="d7304-103">AllowNewTimeProposal</span></span>

<span data-ttu-id="d7304-104">O elemento **AllowNewTimeProposal** indica se um novo horário de reunião pode ser proposto para uma reunião por um participante.</span><span class="sxs-lookup"><span data-stu-id="d7304-104">The **AllowNewTimeProposal** element indicates whether a new meeting time can be proposed for a meeting by an attendee.</span></span> 
  
```xml
<AllowNewTimeProposal/>
```

 <span data-ttu-id="d7304-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="d7304-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d7304-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d7304-106">Attributes and elements</span></span>

<span data-ttu-id="d7304-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d7304-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d7304-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d7304-108">Attributes</span></span>

<span data-ttu-id="d7304-109">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="d7304-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d7304-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d7304-110">Child elements</span></span>

<span data-ttu-id="d7304-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d7304-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d7304-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d7304-112">Parent elements</span></span>

|<span data-ttu-id="d7304-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d7304-113">**Element**</span></span>|<span data-ttu-id="d7304-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d7304-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7304-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="d7304-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="d7304-116">Representa uma reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d7304-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d7304-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="d7304-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="d7304-118">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d7304-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d7304-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="d7304-119">Text value</span></span>

<span data-ttu-id="d7304-120">Um valor de texto que representa um valor booliano é necessário.</span><span class="sxs-lookup"><span data-stu-id="d7304-120">A text value that represents a Boolean value is required.</span></span> <span data-ttu-id="d7304-121">Um valor **true** indica que uma nova proposta para o tempo de reunião pode ser criada; um valor **false** indica que novas propostas de horários não são permitidas.</span><span class="sxs-lookup"><span data-stu-id="d7304-121">A value of **true** indicates that a new proposal for the meeting time can be created; a value of **false** indicates that new time proposals are not allowed.</span></span> <span data-ttu-id="d7304-122">O organizador define esse valor na solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="d7304-122">The organizer sets this value in the meeting request.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d7304-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="d7304-123">Remarks</span></span>

<span data-ttu-id="d7304-124">A propriedade AllowNewTimeProposal é leitura/gravação para o item de calendário do organizador.</span><span class="sxs-lookup"><span data-stu-id="d7304-124">The AllowNewTimeProposal property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="d7304-125">É somente leitura para solicitações de reunião e itens de calendário dos participantes.</span><span class="sxs-lookup"><span data-stu-id="d7304-125">It is read-only for meeting requests and for attendees' calendar items.</span></span>
  
<span data-ttu-id="d7304-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="d7304-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="d7304-127">Os serviços Web do Exchange não dão suporte a novas mensagens de proposta de tempo.</span><span class="sxs-lookup"><span data-stu-id="d7304-127">Exchange Web Services does not support new time proposal messages.</span></span> <span data-ttu-id="d7304-128">Para obter propriedades relacionadas a novas mensagens de proposta de tempo, use propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="d7304-128">To get properties that are related to new time proposal messages, use extended properties.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="d7304-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d7304-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d7304-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="d7304-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d7304-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d7304-131">Schema name</span></span>  <br/> |<span data-ttu-id="d7304-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d7304-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="d7304-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d7304-133">Validation file</span></span>  <br/> |<span data-ttu-id="d7304-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d7304-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d7304-135">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d7304-135">Can be empty</span></span>  <br/> |<span data-ttu-id="d7304-136">False</span><span class="sxs-lookup"><span data-stu-id="d7304-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d7304-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="d7304-137">See also</span></span>

- [<span data-ttu-id="d7304-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d7304-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

