---
title: IndividualAttendeeConflictData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndividualAttendeeConflictData
api_type:
- schema
ms.assetid: d45d3c34-abe1-40da-afd3-23bc5c3ef474
description: O elemento IndividualAttendeeConflictData contém o status de disponibilidade de um usuário ou contato para uma janela de tempo que ocorre ao mesmo tempo que o tempo de reunião sugerido identificado no elemento Suggestion.
ms.openlocfilehash: 55210230259b78e5ed9c4f0744aae003cf2e7ae5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459311"
---
# <a name="individualattendeeconflictdata"></a><span data-ttu-id="c5e3e-103">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="c5e3e-103">IndividualAttendeeConflictData</span></span>

<span data-ttu-id="c5e3e-104">O elemento **IndividualAttendeeConflictData** contém o status de disponibilidade de um usuário ou contato para uma janela de tempo que ocorre ao mesmo tempo que o tempo de reunião sugerido identificado no elemento [suggestion](suggestion.md) .</span><span class="sxs-lookup"><span data-stu-id="c5e3e-104">The **IndividualAttendeeConflictData** element contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time identified in the [Suggestion](suggestion.md) element.</span></span> 
  
[<span data-ttu-id="c5e3e-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="c5e3e-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="c5e3e-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="c5e3e-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="c5e3e-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="c5e3e-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="c5e3e-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="c5e3e-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="c5e3e-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="c5e3e-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="c5e3e-110">La</span><span class="sxs-lookup"><span data-stu-id="c5e3e-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="c5e3e-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="c5e3e-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="c5e3e-112">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="c5e3e-112">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md)
  
```xml
<IndividualAttendeeConflictData>
   <BusyType>...</BusyType>
</IndividualAttendeeConflictData>
```

 <span data-ttu-id="c5e3e-113">**IndividualAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="c5e3e-113">**IndividualAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c5e3e-114">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c5e3e-114">Attributes and elements</span></span>

<span data-ttu-id="c5e3e-115">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c5e3e-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c5e3e-116">Atributos</span><span class="sxs-lookup"><span data-stu-id="c5e3e-116">Attributes</span></span>

<span data-ttu-id="c5e3e-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c5e3e-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c5e3e-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c5e3e-118">Child elements</span></span>

|<span data-ttu-id="c5e3e-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c5e3e-119">**Element**</span></span>|<span data-ttu-id="c5e3e-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c5e3e-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5e3e-121">BusyType</span><span class="sxs-lookup"><span data-stu-id="c5e3e-121">BusyType</span></span>](busytype.md) <br/> |<span data-ttu-id="c5e3e-122">Representa o status de disponibilidade de um usuário para um tempo de reunião sugerido.</span><span class="sxs-lookup"><span data-stu-id="c5e3e-122">Represents the free/busy status of a user for a suggested meeting time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c5e3e-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c5e3e-123">Parent elements</span></span>

|<span data-ttu-id="c5e3e-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c5e3e-124">**Element**</span></span>|<span data-ttu-id="c5e3e-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c5e3e-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c5e3e-126">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="c5e3e-126">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="c5e3e-127">Contém uma matriz de dados de conflito para participantes identificados no [GetUserAvailabilityRequest](getuseravailabilityrequest.md).</span><span class="sxs-lookup"><span data-stu-id="c5e3e-127">Contains an array of conflict data for attendees identified in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md).</span></span>  <br/> <span data-ttu-id="c5e3e-128">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="c5e3e-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c5e3e-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="c5e3e-129">Remarks</span></span>

<span data-ttu-id="c5e3e-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="c5e3e-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c5e3e-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c5e3e-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c5e3e-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="c5e3e-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c5e3e-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c5e3e-133">Schema Name</span></span>  <br/> |<span data-ttu-id="c5e3e-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c5e3e-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="c5e3e-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c5e3e-135">Validation File</span></span>  <br/> |<span data-ttu-id="c5e3e-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c5e3e-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c5e3e-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c5e3e-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="c5e3e-138">False</span><span class="sxs-lookup"><span data-stu-id="c5e3e-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c5e3e-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="c5e3e-139">See also</span></span>



[<span data-ttu-id="c5e3e-140">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="c5e3e-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="c5e3e-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="c5e3e-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="c5e3e-142">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="c5e3e-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

