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
description: O elemento IsOnlineMeeting indica se a reunião online.
ms.openlocfilehash: 5a56b0b9828d6f6bec83fc0ad0f8f9579b471a72
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824061"
---
# <a name="isonlinemeeting"></a><span data-ttu-id="955c8-103">IsOnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="955c8-103">IsOnlineMeeting</span></span>

<span data-ttu-id="955c8-104">O elemento **IsOnlineMeeting** indica se a reunião online.</span><span class="sxs-lookup"><span data-stu-id="955c8-104">The **IsOnlineMeeting** element indicates whether the meeting is online.</span></span> 
  
```xml
<IsOnlineMeeting/>
```

 <span data-ttu-id="955c8-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="955c8-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="955c8-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="955c8-106">Attributes and elements</span></span>

<span data-ttu-id="955c8-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="955c8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="955c8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="955c8-108">Attributes</span></span>

<span data-ttu-id="955c8-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="955c8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="955c8-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="955c8-110">Child elements</span></span>

<span data-ttu-id="955c8-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="955c8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="955c8-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="955c8-112">Parent elements</span></span>

|<span data-ttu-id="955c8-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="955c8-113">**Element**</span></span>|<span data-ttu-id="955c8-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="955c8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="955c8-115">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="955c8-115">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="955c8-116">Representa uma reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="955c8-116">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="955c8-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="955c8-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="955c8-118">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="955c8-118">Represents an Exchange calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="955c8-119">Text value</span><span class="sxs-lookup"><span data-stu-id="955c8-119">Text value</span></span>

<span data-ttu-id="955c8-120">Se este elemento for usado, será necessário um valor de texto que representa um valor booleano.</span><span class="sxs-lookup"><span data-stu-id="955c8-120">A text value that represents a Boolean value is required if this element is used.</span></span> <span data-ttu-id="955c8-121">Um valor **true** indica que a reunião está online.</span><span class="sxs-lookup"><span data-stu-id="955c8-121">A value of **true** indicates that the meeting is online.</span></span> <span data-ttu-id="955c8-122">Um valor **false** indica que a reunião não está online.</span><span class="sxs-lookup"><span data-stu-id="955c8-122">A value of **false** indicates that the meeting is not online.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="955c8-123">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="955c8-123">Remarks</span></span>

<span data-ttu-id="955c8-124">A propriedade IsOnlineMeeting é gravável de leitura para o item de calendário do organizador.</span><span class="sxs-lookup"><span data-stu-id="955c8-124">The IsOnlineMeeting property is read-writable for the organizer's calendar item.</span></span> <span data-ttu-id="955c8-125">Ele é somente leitura para solicitações de reunião e itens de calendário dos participantes.</span><span class="sxs-lookup"><span data-stu-id="955c8-125">It is read-only for meeting requests and for attendees' calendar items.</span></span>
  
<span data-ttu-id="955c8-126">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o MicrosoftExchange 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="955c8-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="955c8-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="955c8-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="955c8-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="955c8-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="955c8-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="955c8-129">Schema name</span></span>  <br/> |<span data-ttu-id="955c8-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="955c8-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="955c8-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="955c8-131">Validation file</span></span>  <br/> |<span data-ttu-id="955c8-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="955c8-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="955c8-133">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="955c8-133">Can be empty</span></span>  <br/> |<span data-ttu-id="955c8-134">False</span><span class="sxs-lookup"><span data-stu-id="955c8-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="955c8-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="955c8-135">See also</span></span>



- [<span data-ttu-id="955c8-136">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="955c8-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

