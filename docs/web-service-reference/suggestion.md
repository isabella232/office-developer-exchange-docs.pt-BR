---
title: La
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Suggestion
api_type:
- schema
ms.assetid: 040a5c8f-b62f-4d1d-9d2c-dc3c5e01481f
description: O elemento suggestion representa uma única sugestão de reunião.
ms.openlocfilehash: 25821abd5463ddba86a487709c8d2f8d928a94cc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530377"
---
# <a name="suggestion"></a><span data-ttu-id="dab69-103">La</span><span class="sxs-lookup"><span data-stu-id="dab69-103">Suggestion</span></span>

<span data-ttu-id="dab69-104">O elemento **suggestion** representa uma única sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="dab69-104">The **Suggestion** element represents a single meeting suggestion.</span></span> 
  
[<span data-ttu-id="dab69-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="dab69-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="dab69-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="dab69-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="dab69-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="dab69-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="dab69-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="dab69-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="dab69-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="dab69-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="dab69-110">La</span><span class="sxs-lookup"><span data-stu-id="dab69-110">Suggestion</span></span>](suggestion.md)
  
```xml
<Suggestion>
   <MeetingTime>...</MeetingTime>
   <IsWorkTime>...</IsWorkTime>
   <SuggestionQuality>...</SuggestionQuality>
   <AttendeeConflictDataArray>...</AttendeeConflictDataArray>
</Suggestion>
```

 <span data-ttu-id="dab69-111">**La**</span><span class="sxs-lookup"><span data-stu-id="dab69-111">**Suggestion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dab69-112">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="dab69-112">Attributes and elements</span></span>

<span data-ttu-id="dab69-113">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="dab69-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dab69-114">Atributos</span><span class="sxs-lookup"><span data-stu-id="dab69-114">Attributes</span></span>

<span data-ttu-id="dab69-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dab69-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dab69-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="dab69-116">Child elements</span></span>

|<span data-ttu-id="dab69-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dab69-117">**Element**</span></span>|<span data-ttu-id="dab69-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dab69-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dab69-119">MeetingTime</span><span class="sxs-lookup"><span data-stu-id="dab69-119">MeetingTime</span></span>](meetingtime.md) <br/> |<span data-ttu-id="dab69-120">Representa um horário de reunião sugerido.</span><span class="sxs-lookup"><span data-stu-id="dab69-120">Represents a suggested meeting time.</span></span>  <br/> |
|[<span data-ttu-id="dab69-121">IsWorkTime</span><span class="sxs-lookup"><span data-stu-id="dab69-121">IsWorkTime</span></span>](isworktime.md) <br/> |<span data-ttu-id="dab69-122">Indica se o tempo de reunião sugerido ocorre durante o horário de trabalho agendado.</span><span class="sxs-lookup"><span data-stu-id="dab69-122">Represents whether the suggested meeting time occurs during scheduled work hours.</span></span>  <br/> |
|[<span data-ttu-id="dab69-123">SuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="dab69-123">SuggestionQuality</span></span>](suggestionquality.md) <br/> |<span data-ttu-id="dab69-124">Representa a qualidade do tempo de reunião sugerido.</span><span class="sxs-lookup"><span data-stu-id="dab69-124">Represents the quality of the suggested meeting time.</span></span>  <br/> |
|[<span data-ttu-id="dab69-125">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="dab69-125">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="dab69-126">Contém uma matriz de informações que descreve conflitos entre usuários e recursos e o tempo de reunião sugerido.</span><span class="sxs-lookup"><span data-stu-id="dab69-126">Contains an array of information that describes conflicts between users and resources and the suggested meeting time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dab69-127">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="dab69-127">Parent elements</span></span>

|<span data-ttu-id="dab69-128">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dab69-128">**Element**</span></span>|<span data-ttu-id="dab69-129">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dab69-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dab69-130">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="dab69-130">SuggestionArray</span></span>](suggestionarray.md) <br/> |<span data-ttu-id="dab69-131">Contém uma matriz de horários de reunião sugeridos.</span><span class="sxs-lookup"><span data-stu-id="dab69-131">Contains an array of suggested meeting times.</span></span>  <br/> <span data-ttu-id="dab69-132">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="dab69-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dab69-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="dab69-133">Remarks</span></span>

<span data-ttu-id="dab69-134">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="dab69-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dab69-135">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="dab69-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dab69-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="dab69-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dab69-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="dab69-137">Schema Name</span></span>  <br/> |<span data-ttu-id="dab69-138">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="dab69-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="dab69-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="dab69-139">Validation File</span></span>  <br/> |<span data-ttu-id="dab69-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="dab69-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dab69-141">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="dab69-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="dab69-142">False</span><span class="sxs-lookup"><span data-stu-id="dab69-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dab69-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="dab69-143">See also</span></span>



[<span data-ttu-id="dab69-144">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="dab69-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="dab69-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="dab69-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="dab69-146">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="dab69-146">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

