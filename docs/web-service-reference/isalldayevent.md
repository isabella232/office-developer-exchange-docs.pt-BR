---
title: IsAllDayEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAllDayEvent
api_type:
- schema
ms.assetid: 29140a64-9d7a-4a14-a10d-c98197c9831b
description: O elemento IsAllDayEvent indica se uma solicitação de reunião ou item de calendário representa um evento de dia inteiro.
ms.openlocfilehash: 81cf1e7d8338275540f264de7cbf194005e7770c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823983"
---
# <a name="isalldayevent"></a><span data-ttu-id="251b2-103">IsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="251b2-103">IsAllDayEvent</span></span>

<span data-ttu-id="251b2-104">O elemento **IsAllDayEvent** indica se uma solicitação de reunião ou item de calendário representa um evento de dia inteiro.</span><span class="sxs-lookup"><span data-stu-id="251b2-104">The **IsAllDayEvent** element indicates whether a calendar item or meeting request represents an all-day event.</span></span> 
  
```xml
<IsAllDayEvent/>
```

 <span data-ttu-id="251b2-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="251b2-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="251b2-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="251b2-106">Attributes and elements</span></span>

<span data-ttu-id="251b2-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="251b2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="251b2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="251b2-108">Attributes</span></span>

<span data-ttu-id="251b2-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="251b2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="251b2-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="251b2-110">Child elements</span></span>

<span data-ttu-id="251b2-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="251b2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="251b2-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="251b2-112">Parent elements</span></span>

|<span data-ttu-id="251b2-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="251b2-113">**Element**</span></span>|<span data-ttu-id="251b2-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="251b2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="251b2-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="251b2-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="251b2-116">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="251b2-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="251b2-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="251b2-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="251b2-118">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="251b2-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="251b2-119">Text value</span><span class="sxs-lookup"><span data-stu-id="251b2-119">Text value</span></span>

<span data-ttu-id="251b2-120">Um valor de texto que representa um valor booleano é necessário se este elemento é incluído.</span><span class="sxs-lookup"><span data-stu-id="251b2-120">A text value that represents a Boolean value is required if this element is included.</span></span> <span data-ttu-id="251b2-121">Um valor **true** indica que o item representa um evento de dia inteiro.</span><span class="sxs-lookup"><span data-stu-id="251b2-121">A value of **true** indicates that the item represents an all-day event.</span></span> <span data-ttu-id="251b2-122">Um valor **false** indica que o item abrange menos que o horário de trabalho do usuário.</span><span class="sxs-lookup"><span data-stu-id="251b2-122">A value of **false** indicates that the item spans less than a user's working hours.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="251b2-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="251b2-123">Remarks</span></span>

<span data-ttu-id="251b2-124">Um evento de dia inteiro abrange a duração de horário de trabalho que está definida para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="251b2-124">An all-day event spans the duration of working hours that is defined for a mailbox.</span></span>
  
<span data-ttu-id="251b2-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="251b2-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="251b2-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="251b2-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="251b2-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="251b2-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="251b2-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="251b2-128">Schema name</span></span>  <br/> |<span data-ttu-id="251b2-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="251b2-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="251b2-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="251b2-130">Validation file</span></span>  <br/> |<span data-ttu-id="251b2-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="251b2-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="251b2-132">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="251b2-132">Can be empty</span></span>  <br/> |<span data-ttu-id="251b2-133">False</span><span class="sxs-lookup"><span data-stu-id="251b2-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="251b2-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="251b2-134">See also</span></span>



- [<span data-ttu-id="251b2-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="251b2-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

