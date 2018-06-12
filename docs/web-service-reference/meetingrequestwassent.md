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
description: O elemento MeetingRequestWasSent indica se foi enviada uma solicitação de reunião a participantes solicitados.
ms.openlocfilehash: 0a87b1d773997e08ab96726375e4c8ce010faaf7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824438"
---
# <a name="meetingrequestwassent"></a><span data-ttu-id="20947-103">MeetingRequestWasSent</span><span class="sxs-lookup"><span data-stu-id="20947-103">MeetingRequestWasSent</span></span>

<span data-ttu-id="20947-104">O elemento **MeetingRequestWasSent** indica se foi enviada uma solicitação de reunião a participantes solicitados.</span><span class="sxs-lookup"><span data-stu-id="20947-104">The **MeetingRequestWasSent** element indicates whether a meeting request has been sent to requested attendees.</span></span> 
  
```xml
<MeetingRequestWasSent/>
```

 <span data-ttu-id="20947-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="20947-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="20947-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="20947-106">Attributes and elements</span></span>

<span data-ttu-id="20947-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="20947-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="20947-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="20947-108">Attributes</span></span>

<span data-ttu-id="20947-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="20947-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="20947-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="20947-110">Child elements</span></span>

<span data-ttu-id="20947-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="20947-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="20947-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="20947-112">Parent elements</span></span>

|<span data-ttu-id="20947-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="20947-113">**Element**</span></span>|<span data-ttu-id="20947-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="20947-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20947-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="20947-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="20947-116">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="20947-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="20947-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="20947-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="20947-118">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="20947-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="20947-119">Text value</span><span class="sxs-lookup"><span data-stu-id="20947-119">Text value</span></span>

<span data-ttu-id="20947-120">Um valor de texto que representa um valor booleano é necessário se este elemento é incluído.</span><span class="sxs-lookup"><span data-stu-id="20947-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="20947-121">Um valor **true** indica que uma solicitação de reunião foi enviada.</span><span class="sxs-lookup"><span data-stu-id="20947-121">A value of **true** indicates that a meeting request was sent.</span></span> <span data-ttu-id="20947-122">Um valor **false** indica que uma solicitação de reunião não foi enviada.</span><span class="sxs-lookup"><span data-stu-id="20947-122">A value of **false** indicates that a meeting request has not been sent.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="20947-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="20947-123">Remarks</span></span>

<span data-ttu-id="20947-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="20947-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="20947-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="20947-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="20947-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="20947-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="20947-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="20947-127">Schema name</span></span>  <br/> |<span data-ttu-id="20947-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="20947-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="20947-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="20947-129">Validation file</span></span>  <br/> |<span data-ttu-id="20947-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="20947-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="20947-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="20947-131">Can be empty</span></span>  <br/> |<span data-ttu-id="20947-132">False</span><span class="sxs-lookup"><span data-stu-id="20947-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="20947-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="20947-133">See also</span></span>



- [<span data-ttu-id="20947-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="20947-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

