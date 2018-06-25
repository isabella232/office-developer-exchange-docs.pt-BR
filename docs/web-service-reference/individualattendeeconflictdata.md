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
description: O elemento IndividualAttendeeConflictData contém um usuário ou o status livre/ocupado para uma janela de tempo que ocorre ao mesmo tempo como o tempo de reunião sugerido do contato identificado no elemento sugestão.
ms.openlocfilehash: 0bd164e08a6f3685415452b7c82a4220cf69d792
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823930"
---
# <a name="individualattendeeconflictdata"></a><span data-ttu-id="271f1-103">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="271f1-103">IndividualAttendeeConflictData</span></span>

<span data-ttu-id="271f1-104">O elemento **IndividualAttendeeConflictData** contém um usuário ou o status livre/ocupado para uma janela de tempo que ocorre ao mesmo tempo como o tempo de reunião sugerido do contato identificado no elemento [sugestão](suggestion.md) .</span><span class="sxs-lookup"><span data-stu-id="271f1-104">The **IndividualAttendeeConflictData** element contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time identified in the [Suggestion](suggestion.md) element.</span></span> 
  
[<span data-ttu-id="271f1-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="271f1-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="271f1-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="271f1-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="271f1-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="271f1-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="271f1-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="271f1-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="271f1-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="271f1-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="271f1-110">Sugestão</span><span class="sxs-lookup"><span data-stu-id="271f1-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="271f1-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="271f1-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="271f1-112">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="271f1-112">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md)
  
```xml
<IndividualAttendeeConflictData>
   <BusyType>...</BusyType>
</IndividualAttendeeConflictData>
```

 <span data-ttu-id="271f1-113">**IndividualAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="271f1-113">**IndividualAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="271f1-114">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="271f1-114">Attributes and elements</span></span>

<span data-ttu-id="271f1-115">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="271f1-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="271f1-116">Atributos</span><span class="sxs-lookup"><span data-stu-id="271f1-116">Attributes</span></span>

<span data-ttu-id="271f1-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="271f1-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="271f1-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="271f1-118">Child elements</span></span>

|<span data-ttu-id="271f1-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="271f1-119">**Element**</span></span>|<span data-ttu-id="271f1-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="271f1-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="271f1-121">BusyType</span><span class="sxs-lookup"><span data-stu-id="271f1-121">BusyType</span></span>](busytype.md) <br/> |<span data-ttu-id="271f1-122">Representa o status livre/ocupado de um usuário por um tempo de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="271f1-122">Represents the free/busy status of a user for a suggested meeting time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="271f1-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="271f1-123">Parent elements</span></span>

|<span data-ttu-id="271f1-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="271f1-124">**Element**</span></span>|<span data-ttu-id="271f1-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="271f1-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="271f1-126">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="271f1-126">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="271f1-127">Contém uma matriz de dados de conflito para participantes identificados no [GetUserAvailabilityRequest](getuseravailabilityrequest.md).</span><span class="sxs-lookup"><span data-stu-id="271f1-127">Contains an array of conflict data for attendees identified in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md).</span></span>  <br/> <span data-ttu-id="271f1-128">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="271f1-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="271f1-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="271f1-129">Remarks</span></span>

<span data-ttu-id="271f1-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="271f1-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="271f1-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="271f1-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="271f1-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="271f1-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="271f1-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="271f1-133">Schema Name</span></span>  <br/> |<span data-ttu-id="271f1-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="271f1-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="271f1-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="271f1-135">Validation File</span></span>  <br/> |<span data-ttu-id="271f1-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="271f1-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="271f1-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="271f1-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="271f1-138">False</span><span class="sxs-lookup"><span data-stu-id="271f1-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="271f1-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="271f1-139">See also</span></span>



[<span data-ttu-id="271f1-140">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="271f1-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="271f1-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="271f1-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="271f1-142">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="271f1-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

