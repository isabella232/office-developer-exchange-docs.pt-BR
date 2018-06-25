---
title: FirstOccurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FirstOccurrence
api_type:
- schema
ms.assetid: d6748860-ce0d-4d2e-b7e4-9ed834f1e45a
description: O elemento FirstOccurrence representa a primeira ocorrência de um item de calendário recorrente.
ms.openlocfilehash: e5244e74bdd5a4b8e22c6e63811db53b46fa353a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752316"
---
# <a name="firstoccurrence"></a><span data-ttu-id="554bf-103">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="554bf-103">FirstOccurrence</span></span>

<span data-ttu-id="554bf-104">O elemento **FirstOccurrence** representa a primeira ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="554bf-104">The **FirstOccurrence** element represents the first occurrence of a recurring calendar item.</span></span> 
  
```xml
<FirstOccurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</FirstOccurrence>
```

 <span data-ttu-id="554bf-105">**OccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="554bf-105">**OccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="554bf-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="554bf-106">Attributes and elements</span></span>

<span data-ttu-id="554bf-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="554bf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="554bf-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="554bf-108">Attributes</span></span>

<span data-ttu-id="554bf-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="554bf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="554bf-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="554bf-110">Child elements</span></span>

|<span data-ttu-id="554bf-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="554bf-111">**Element**</span></span>|<span data-ttu-id="554bf-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="554bf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="554bf-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="554bf-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="554bf-114">Contém o identificador e alterar a chave exclusiva da primeira ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="554bf-114">Contains the unique identifier and change key of the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="554bf-115">Start</span><span class="sxs-lookup"><span data-stu-id="554bf-115">Start</span></span>](start.md) <br/> |<span data-ttu-id="554bf-116">Representa a hora de início da primeira ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="554bf-116">Represents the start time of the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="554bf-117">End</span><span class="sxs-lookup"><span data-stu-id="554bf-117">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="554bf-118">Representa a hora de término da primeira ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="554bf-118">Represents the end time of the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="554bf-119">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="554bf-119">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="554bf-120">Representa a hora de início original da primeira ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="554bf-120">Represents the original start time of the first occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="554bf-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="554bf-121">Parent elements</span></span>

|<span data-ttu-id="554bf-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="554bf-122">**Element**</span></span>|<span data-ttu-id="554bf-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="554bf-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="554bf-124">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="554bf-124">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="554bf-125">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="554bf-125">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="554bf-126">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="554bf-126">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="554bf-127">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="554bf-127">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="554bf-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="554bf-128">Remarks</span></span>

<span data-ttu-id="554bf-129">Esse elemento é válido se [CalendarItemType](calendaritemtype.md) tem o valor de RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="554bf-129">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="554bf-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="554bf-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="554bf-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="554bf-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="554bf-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="554bf-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="554bf-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="554bf-133">Schema name</span></span>  <br/> |<span data-ttu-id="554bf-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="554bf-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="554bf-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="554bf-135">Validation file</span></span>  <br/> |<span data-ttu-id="554bf-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="554bf-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="554bf-137">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="554bf-137">Can be empty</span></span>  <br/> |<span data-ttu-id="554bf-138">False</span><span class="sxs-lookup"><span data-stu-id="554bf-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="554bf-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="554bf-139">See also</span></span>



- [<span data-ttu-id="554bf-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="554bf-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
[<span data-ttu-id="554bf-141">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="554bf-141">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

