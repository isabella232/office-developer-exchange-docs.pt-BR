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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459311"
---
# <a name="individualattendeeconflictdata"></a><span data-ttu-id="2600c-103">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="2600c-103">IndividualAttendeeConflictData</span></span>

<span data-ttu-id="2600c-104">O elemento **IndividualAttendeeConflictData** contém o status de disponibilidade de um usuário ou contato para uma janela de tempo que ocorre ao mesmo tempo que o tempo de reunião sugerido identificado no elemento [suggestion](suggestion.md) .</span><span class="sxs-lookup"><span data-stu-id="2600c-104">The **IndividualAttendeeConflictData** element contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time identified in the [Suggestion](suggestion.md) element.</span></span> 
  
[<span data-ttu-id="2600c-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="2600c-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="2600c-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="2600c-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="2600c-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="2600c-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="2600c-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="2600c-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="2600c-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="2600c-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="2600c-110">La</span><span class="sxs-lookup"><span data-stu-id="2600c-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="2600c-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="2600c-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="2600c-112">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="2600c-112">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md)
  
```xml
<IndividualAttendeeConflictData>
   <BusyType>...</BusyType>
</IndividualAttendeeConflictData>
```

 <span data-ttu-id="2600c-113">**IndividualAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="2600c-113">**IndividualAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2600c-114">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="2600c-114">Attributes and elements</span></span>

<span data-ttu-id="2600c-115">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2600c-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2600c-116">Atributos</span><span class="sxs-lookup"><span data-stu-id="2600c-116">Attributes</span></span>

<span data-ttu-id="2600c-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2600c-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2600c-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2600c-118">Child elements</span></span>

|<span data-ttu-id="2600c-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2600c-119">**Element**</span></span>|<span data-ttu-id="2600c-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2600c-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2600c-121">BusyType</span><span class="sxs-lookup"><span data-stu-id="2600c-121">BusyType</span></span>](busytype.md) <br/> |<span data-ttu-id="2600c-122">Representa o status de disponibilidade de um usuário para um tempo de reunião sugerido.</span><span class="sxs-lookup"><span data-stu-id="2600c-122">Represents the free/busy status of a user for a suggested meeting time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2600c-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2600c-123">Parent elements</span></span>

|<span data-ttu-id="2600c-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2600c-124">**Element**</span></span>|<span data-ttu-id="2600c-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2600c-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2600c-126">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="2600c-126">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="2600c-127">Contém uma matriz de dados de conflito para participantes identificados no [GetUserAvailabilityRequest](getuseravailabilityrequest.md).</span><span class="sxs-lookup"><span data-stu-id="2600c-127">Contains an array of conflict data for attendees identified in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md).</span></span>  <br/> <span data-ttu-id="2600c-128">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="2600c-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2600c-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="2600c-129">Remarks</span></span>

<span data-ttu-id="2600c-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="2600c-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2600c-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="2600c-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2600c-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="2600c-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2600c-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2600c-133">Schema Name</span></span>  <br/> |<span data-ttu-id="2600c-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="2600c-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="2600c-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2600c-135">Validation File</span></span>  <br/> |<span data-ttu-id="2600c-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2600c-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2600c-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2600c-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="2600c-138">False</span><span class="sxs-lookup"><span data-stu-id="2600c-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2600c-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="2600c-139">See also</span></span>



[<span data-ttu-id="2600c-140">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="2600c-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="2600c-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="2600c-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="2600c-142">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="2600c-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

