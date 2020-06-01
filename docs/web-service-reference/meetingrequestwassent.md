---
title: MeetingRequestWasSent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingRequestWasSent
api_type:
- schema
ms.assetid: 9192400a-8eef-4147-9f94-aa8ea91b41d8
description: O elemento MeetingRequestWasSent indica se uma solicitação de reunião foi enviada aos participantes solicitados.
ms.openlocfilehash: d5005eb86d5f8d2f438a69e634f0617c2311d720
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44465762"
---
# <a name="meetingrequestwassent"></a><span data-ttu-id="26f6b-103">MeetingRequestWasSent</span><span class="sxs-lookup"><span data-stu-id="26f6b-103">MeetingRequestWasSent</span></span>

<span data-ttu-id="26f6b-104">O elemento **MeetingRequestWasSent** indica se uma solicitação de reunião foi enviada aos participantes solicitados.</span><span class="sxs-lookup"><span data-stu-id="26f6b-104">The **MeetingRequestWasSent** element indicates whether a meeting request has been sent to requested attendees.</span></span> 
  
```xml
<MeetingRequestWasSent/>
```

 <span data-ttu-id="26f6b-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="26f6b-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="26f6b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="26f6b-106">Attributes and elements</span></span>

<span data-ttu-id="26f6b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="26f6b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26f6b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="26f6b-108">Attributes</span></span>

<span data-ttu-id="26f6b-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="26f6b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="26f6b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="26f6b-110">Child elements</span></span>

<span data-ttu-id="26f6b-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="26f6b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="26f6b-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="26f6b-112">Parent elements</span></span>

|<span data-ttu-id="26f6b-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="26f6b-113">**Element**</span></span>|<span data-ttu-id="26f6b-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="26f6b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26f6b-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="26f6b-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="26f6b-116">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="26f6b-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="26f6b-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="26f6b-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="26f6b-118">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="26f6b-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="26f6b-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="26f6b-119">Text value</span></span>

<span data-ttu-id="26f6b-120">Um valor de texto que representa um valor booliano é necessário se esse elemento for incluído.</span><span class="sxs-lookup"><span data-stu-id="26f6b-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="26f6b-121">Um valor **true** indica que uma solicitação de reunião foi enviada.</span><span class="sxs-lookup"><span data-stu-id="26f6b-121">A value of **true** indicates that a meeting request was sent.</span></span> <span data-ttu-id="26f6b-122">Um valor **false** indica que uma solicitação de reunião não foi enviada.</span><span class="sxs-lookup"><span data-stu-id="26f6b-122">A value of **false** indicates that a meeting request has not been sent.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="26f6b-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="26f6b-123">Remarks</span></span>

<span data-ttu-id="26f6b-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="26f6b-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26f6b-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="26f6b-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26f6b-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="26f6b-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="26f6b-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="26f6b-127">Schema name</span></span>  <br/> |<span data-ttu-id="26f6b-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="26f6b-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="26f6b-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="26f6b-129">Validation file</span></span>  <br/> |<span data-ttu-id="26f6b-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="26f6b-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="26f6b-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="26f6b-131">Can be empty</span></span>  <br/> |<span data-ttu-id="26f6b-132">False</span><span class="sxs-lookup"><span data-stu-id="26f6b-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="26f6b-133">Confira também</span><span class="sxs-lookup"><span data-stu-id="26f6b-133">See also</span></span>



- [<span data-ttu-id="26f6b-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="26f6b-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

