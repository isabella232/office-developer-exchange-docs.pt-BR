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
description: O elemento LegacyFreeBusyStatus representa o status de disponibilidade do item de calendário.
ms.openlocfilehash: ecbcae0862c9c02c0a4a61012816e4c2c6ea07b7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463227"
---
# <a name="legacyfreebusystatus"></a><span data-ttu-id="813ae-103">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="813ae-103">LegacyFreeBusyStatus</span></span>

<span data-ttu-id="813ae-104">O elemento **LegacyFreeBusyStatus** representa o status de disponibilidade do item de calendário.</span><span class="sxs-lookup"><span data-stu-id="813ae-104">The **LegacyFreeBusyStatus** element represents the free/busy status of the calendar item.</span></span> 
  
```xml
<LegacyFreeBusyStatus/>
```

<span data-ttu-id="813ae-105">**LegacyFreeBusyType**</span><span class="sxs-lookup"><span data-stu-id="813ae-105">**LegacyFreeBusyType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="813ae-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="813ae-106">Attributes and elements</span></span>

<span data-ttu-id="813ae-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="813ae-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="813ae-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="813ae-108">Attributes</span></span>

<span data-ttu-id="813ae-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="813ae-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="813ae-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="813ae-110">Child elements</span></span>

<span data-ttu-id="813ae-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="813ae-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="813ae-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="813ae-112">Parent elements</span></span>

|<span data-ttu-id="813ae-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="813ae-113">**Element**</span></span>|<span data-ttu-id="813ae-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="813ae-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="813ae-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="813ae-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="813ae-116">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="813ae-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="813ae-117">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="813ae-117">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="813ae-118">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="813ae-118">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="813ae-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="813ae-119">Text value</span></span>

<span data-ttu-id="813ae-120">Um valor de texto é necessário para este elemento.</span><span class="sxs-lookup"><span data-stu-id="813ae-120">A text value is required for this element.</span></span> <span data-ttu-id="813ae-121">Estes são os valores de texto possíveis para este elemento:</span><span class="sxs-lookup"><span data-stu-id="813ae-121">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="813ae-122">Disponível</span><span class="sxs-lookup"><span data-stu-id="813ae-122">Free</span></span> 
- <span data-ttu-id="813ae-123">Provisória</span><span class="sxs-lookup"><span data-stu-id="813ae-123">Tentative</span></span>
- <span data-ttu-id="813ae-124">Ocupado</span><span class="sxs-lookup"><span data-stu-id="813ae-124">Busy</span></span>
- <span data-ttu-id="813ae-125">TEMPORÁRIA</span><span class="sxs-lookup"><span data-stu-id="813ae-125">OOF</span></span>
- <span data-ttu-id="813ae-126">WorkingElsewhere</span><span class="sxs-lookup"><span data-stu-id="813ae-126">WorkingElsewhere</span></span>
- <span data-ttu-id="813ae-127">NoData</span><span class="sxs-lookup"><span data-stu-id="813ae-127">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="813ae-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="813ae-128">Remarks</span></span>

<span data-ttu-id="813ae-129">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="813ae-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="813ae-130">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="813ae-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="813ae-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="813ae-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="813ae-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="813ae-132">Schema name</span></span>  <br/> |<span data-ttu-id="813ae-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="813ae-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="813ae-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="813ae-134">Validation file</span></span>  <br/> |<span data-ttu-id="813ae-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="813ae-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="813ae-136">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="813ae-136">Can be empty</span></span>  <br/> |<span data-ttu-id="813ae-137">False</span><span class="sxs-lookup"><span data-stu-id="813ae-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="813ae-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="813ae-138">See also</span></span>

- [<span data-ttu-id="813ae-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="813ae-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

