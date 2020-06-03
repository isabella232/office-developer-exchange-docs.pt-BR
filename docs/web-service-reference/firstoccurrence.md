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
ms.openlocfilehash: 22ee9018df1e89a3783c4dfb56aaf065b2c8ea6c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466294"
---
# <a name="firstoccurrence"></a><span data-ttu-id="61944-103">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="61944-103">FirstOccurrence</span></span>

<span data-ttu-id="61944-104">O elemento **FirstOccurrence** representa a primeira ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="61944-104">The **FirstOccurrence** element represents the first occurrence of a recurring calendar item.</span></span> 
  
```xml
<FirstOccurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</FirstOccurrence>
```

 <span data-ttu-id="61944-105">**OccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="61944-105">**OccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="61944-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="61944-106">Attributes and elements</span></span>

<span data-ttu-id="61944-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="61944-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="61944-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="61944-108">Attributes</span></span>

<span data-ttu-id="61944-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="61944-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="61944-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="61944-110">Child elements</span></span>

|<span data-ttu-id="61944-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="61944-111">**Element**</span></span>|<span data-ttu-id="61944-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="61944-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="61944-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="61944-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="61944-114">Contém o identificador exclusivo e a chave de alteração da primeira ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="61944-114">Contains the unique identifier and change key of the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="61944-115">Start</span><span class="sxs-lookup"><span data-stu-id="61944-115">Start</span></span>](start.md) <br/> |<span data-ttu-id="61944-116">Representa a hora de início da primeira ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="61944-116">Represents the start time of the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="61944-117">Ponto</span><span class="sxs-lookup"><span data-stu-id="61944-117">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="61944-118">Representa a hora de término da primeira ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="61944-118">Represents the end time of the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="61944-119">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="61944-119">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="61944-120">Representa a hora de início original da primeira ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="61944-120">Represents the original start time of the first occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="61944-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="61944-121">Parent elements</span></span>

|<span data-ttu-id="61944-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="61944-122">**Element**</span></span>|<span data-ttu-id="61944-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="61944-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="61944-124">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="61944-124">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="61944-125">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="61944-125">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="61944-126">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="61944-126">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="61944-127">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="61944-127">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="61944-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="61944-128">Remarks</span></span>

<span data-ttu-id="61944-129">Este elemento é válido se [CalendarItemType](calendaritemtype.md) tiver o valor RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="61944-129">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="61944-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="61944-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="61944-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="61944-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="61944-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="61944-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="61944-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="61944-133">Schema name</span></span>  <br/> |<span data-ttu-id="61944-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="61944-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="61944-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="61944-135">Validation file</span></span>  <br/> |<span data-ttu-id="61944-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="61944-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="61944-137">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="61944-137">Can be empty</span></span>  <br/> |<span data-ttu-id="61944-138">False</span><span class="sxs-lookup"><span data-stu-id="61944-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="61944-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="61944-139">See also</span></span>



- [<span data-ttu-id="61944-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="61944-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
  
[<span data-ttu-id="61944-141">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="61944-141">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

