---
title: LegacyFreeBusyStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- LegacyFreeBusyStatus
api_type:
- schema
ms.assetid: ee5f3046-b79f-4f68-9455-1a688cee2745
description: O elemento LegacyFreeBusyStatus representa o status livre/ocupado do item de calendário.
ms.openlocfilehash: 681d7256dbef09c6c43d33ea1fc92b5d05e73a41
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824247"
---
# <a name="legacyfreebusystatus"></a><span data-ttu-id="ad1d0-103">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="ad1d0-103">LegacyFreeBusyStatus</span></span>

<span data-ttu-id="ad1d0-104">O elemento **LegacyFreeBusyStatus** representa o status livre/ocupado do item de calendário.</span><span class="sxs-lookup"><span data-stu-id="ad1d0-104">The **LegacyFreeBusyStatus** element represents the free/busy status of the calendar item.</span></span> 
  
```xml
<LegacyFreeBusyStatus/>
```

<span data-ttu-id="ad1d0-105">**LegacyFreeBusyType**</span><span class="sxs-lookup"><span data-stu-id="ad1d0-105">**LegacyFreeBusyType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ad1d0-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ad1d0-106">Attributes and elements</span></span>

<span data-ttu-id="ad1d0-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ad1d0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad1d0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ad1d0-108">Attributes</span></span>

<span data-ttu-id="ad1d0-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ad1d0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad1d0-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ad1d0-110">Child elements</span></span>

<span data-ttu-id="ad1d0-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ad1d0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ad1d0-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ad1d0-112">Parent elements</span></span>

|<span data-ttu-id="ad1d0-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ad1d0-113">**Element**</span></span>|<span data-ttu-id="ad1d0-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ad1d0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad1d0-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="ad1d0-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="ad1d0-116">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad1d0-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="ad1d0-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="ad1d0-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="ad1d0-118">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad1d0-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ad1d0-119">Text value</span><span class="sxs-lookup"><span data-stu-id="ad1d0-119">Text value</span></span>

<span data-ttu-id="ad1d0-120">Um valor de texto é necessário para esse elemento.</span><span class="sxs-lookup"><span data-stu-id="ad1d0-120">A text value is required for this element.</span></span> <span data-ttu-id="ad1d0-121">Estes são os valores de texto possíveis para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="ad1d0-121">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="ad1d0-122">Disponível</span><span class="sxs-lookup"><span data-stu-id="ad1d0-122">Free</span></span> 
- <span data-ttu-id="ad1d0-123">Provisório</span><span class="sxs-lookup"><span data-stu-id="ad1d0-123">Tentative</span></span>
- <span data-ttu-id="ad1d0-124">Ocupado</span><span class="sxs-lookup"><span data-stu-id="ad1d0-124">Busy</span></span>
- <span data-ttu-id="ad1d0-125">AUSÊNCIA TEMPORÁRIA</span><span class="sxs-lookup"><span data-stu-id="ad1d0-125">OOF</span></span>
- <span data-ttu-id="ad1d0-126">WorkingElsewhere</span><span class="sxs-lookup"><span data-stu-id="ad1d0-126">WorkingElsewhere</span></span>
- <span data-ttu-id="ad1d0-127">NoData</span><span class="sxs-lookup"><span data-stu-id="ad1d0-127">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="ad1d0-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="ad1d0-128">Remarks</span></span>

<span data-ttu-id="ad1d0-129">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="ad1d0-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ad1d0-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ad1d0-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad1d0-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="ad1d0-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ad1d0-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ad1d0-132">Schema name</span></span>  <br/> |<span data-ttu-id="ad1d0-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ad1d0-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="ad1d0-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ad1d0-134">Validation file</span></span>  <br/> |<span data-ttu-id="ad1d0-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ad1d0-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ad1d0-136">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="ad1d0-136">Can be empty</span></span>  <br/> |<span data-ttu-id="ad1d0-137">False</span><span class="sxs-lookup"><span data-stu-id="ad1d0-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ad1d0-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="ad1d0-138">See also</span></span>

- [<span data-ttu-id="ad1d0-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ad1d0-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

