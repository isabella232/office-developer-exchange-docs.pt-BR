---
title: IsOnlineMeeting
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsOnlineMeeting
api_type:
- schema
ms.assetid: c29df676-0f3a-4694-a42f-522c6d16872f
description: O elemento IsOnlineMeeting indica se a reunião está online.
ms.openlocfilehash: d2d60c8a51ad7e03c33b57709d9173e79d162268
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460397"
---
# <a name="isonlinemeeting"></a><span data-ttu-id="217dc-103">IsOnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="217dc-103">IsOnlineMeeting</span></span>

<span data-ttu-id="217dc-104">O elemento **IsOnlineMeeting** indica se a reunião está online.</span><span class="sxs-lookup"><span data-stu-id="217dc-104">The **IsOnlineMeeting** element indicates whether the meeting is online.</span></span> 
  
```xml
<IsOnlineMeeting/>
```

 <span data-ttu-id="217dc-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="217dc-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="217dc-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="217dc-106">Attributes and elements</span></span>

<span data-ttu-id="217dc-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="217dc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="217dc-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="217dc-108">Attributes</span></span>

<span data-ttu-id="217dc-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="217dc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="217dc-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="217dc-110">Child elements</span></span>

<span data-ttu-id="217dc-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="217dc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="217dc-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="217dc-112">Parent elements</span></span>

|<span data-ttu-id="217dc-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="217dc-113">**Element**</span></span>|<span data-ttu-id="217dc-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="217dc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="217dc-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="217dc-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="217dc-116">Representa uma reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="217dc-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="217dc-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="217dc-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="217dc-118">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="217dc-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="217dc-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="217dc-119">Text value</span></span>

<span data-ttu-id="217dc-120">Um valor de texto que representa um valor booliano é necessário se esse elemento for usado.</span><span class="sxs-lookup"><span data-stu-id="217dc-120">A text value that represents a Boolean value is required if this element is used.</span></span> <span data-ttu-id="217dc-121">Um valor **true** indica que a reunião está online.</span><span class="sxs-lookup"><span data-stu-id="217dc-121">A value of **true** indicates that the meeting is online.</span></span> <span data-ttu-id="217dc-122">Um valor **false** indica que a reunião não está online.</span><span class="sxs-lookup"><span data-stu-id="217dc-122">A value of **false** indicates that the meeting is not online.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="217dc-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="217dc-123">Remarks</span></span>

<span data-ttu-id="217dc-124">A Propriedade IsOnlineMeeting é leitura/gravação para o item de calendário do organizador.</span><span class="sxs-lookup"><span data-stu-id="217dc-124">The IsOnlineMeeting property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="217dc-125">É somente leitura para solicitações de reunião e itens de calendário dos participantes.</span><span class="sxs-lookup"><span data-stu-id="217dc-125">It is read-only for meeting requests and for attendees' calendar items.</span></span>
  
<span data-ttu-id="217dc-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="217dc-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="217dc-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="217dc-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="217dc-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="217dc-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="217dc-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="217dc-129">Schema name</span></span>  <br/> |<span data-ttu-id="217dc-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="217dc-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="217dc-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="217dc-131">Validation file</span></span>  <br/> |<span data-ttu-id="217dc-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="217dc-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="217dc-133">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="217dc-133">Can be empty</span></span>  <br/> |<span data-ttu-id="217dc-134">False</span><span class="sxs-lookup"><span data-stu-id="217dc-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="217dc-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="217dc-135">See also</span></span>



- [<span data-ttu-id="217dc-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="217dc-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

