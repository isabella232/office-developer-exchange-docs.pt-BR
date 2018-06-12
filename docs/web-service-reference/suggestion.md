---
title: Sugestão
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
description: O elemento de sugestão representa uma sugestão de reunião único.
ms.openlocfilehash: 24e2db1e0eabe35f7c971b0f1dbcbd333358f171
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837669"
---
# <a name="suggestion"></a><span data-ttu-id="e65a5-103">Sugestão</span><span class="sxs-lookup"><span data-stu-id="e65a5-103">Suggestion</span></span>

<span data-ttu-id="e65a5-104">O elemento de **sugestão** representa uma sugestão de reunião único.</span><span class="sxs-lookup"><span data-stu-id="e65a5-104">The **Suggestion** element represents a single meeting suggestion.</span></span> 
  
[<span data-ttu-id="e65a5-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="e65a5-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="e65a5-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="e65a5-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="e65a5-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="e65a5-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="e65a5-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="e65a5-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="e65a5-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="e65a5-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="e65a5-110">Sugestão</span><span class="sxs-lookup"><span data-stu-id="e65a5-110">Suggestion</span></span>](suggestion.md)
  
```xml
<Suggestion>
   <MeetingTime>...</MeetingTime>
   <IsWorkTime>...</IsWorkTime>
   <SuggestionQuality>...</SuggestionQuality>
   <AttendeeConflictDataArray>...</AttendeeConflictDataArray>
</Suggestion>
```

 <span data-ttu-id="e65a5-111">**Sugestão**</span><span class="sxs-lookup"><span data-stu-id="e65a5-111">**Suggestion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e65a5-112">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e65a5-112">Attributes and elements</span></span>

<span data-ttu-id="e65a5-113">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e65a5-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e65a5-114">Atributos</span><span class="sxs-lookup"><span data-stu-id="e65a5-114">Attributes</span></span>

<span data-ttu-id="e65a5-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e65a5-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e65a5-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e65a5-116">Child elements</span></span>

|<span data-ttu-id="e65a5-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e65a5-117">**Element**</span></span>|<span data-ttu-id="e65a5-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e65a5-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e65a5-119">MeetingTime</span><span class="sxs-lookup"><span data-stu-id="e65a5-119">MeetingTime</span></span>](meetingtime.md) <br/> |<span data-ttu-id="e65a5-120">Representa um horário de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="e65a5-120">Represents a suggested meeting time.</span></span>  <br/> |
|[<span data-ttu-id="e65a5-121">IsWorkTime</span><span class="sxs-lookup"><span data-stu-id="e65a5-121">IsWorkTime</span></span>](isworktime.md) <br/> |<span data-ttu-id="e65a5-122">Indica se o horário da reunião sugerido ocorre durante o horário de trabalho agendado.</span><span class="sxs-lookup"><span data-stu-id="e65a5-122">Represents whether the suggested meeting time occurs during scheduled work hours.</span></span>  <br/> |
|[<span data-ttu-id="e65a5-123">SuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="e65a5-123">SuggestionQuality</span></span>](suggestionquality.md) <br/> |<span data-ttu-id="e65a5-124">Representa a qualidade do tempo de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="e65a5-124">Represents the quality of the suggested meeting time.</span></span>  <br/> |
|[<span data-ttu-id="e65a5-125">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="e65a5-125">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="e65a5-126">Contém uma matriz de informações que descrevem os conflitos entre usuários, recursos e o tempo de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="e65a5-126">Contains an array of information that describes conflicts between users and resources and the suggested meeting time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e65a5-127">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e65a5-127">Parent elements</span></span>

|<span data-ttu-id="e65a5-128">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e65a5-128">**Element**</span></span>|<span data-ttu-id="e65a5-129">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e65a5-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e65a5-130">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="e65a5-130">SuggestionArray</span></span>](suggestionarray.md) <br/> |<span data-ttu-id="e65a5-131">Contém uma matriz de reuniões sugeridas.</span><span class="sxs-lookup"><span data-stu-id="e65a5-131">Contains an array of suggested meeting times.</span></span>  <br/> <span data-ttu-id="e65a5-132">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="e65a5-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e65a5-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="e65a5-133">Remarks</span></span>

<span data-ttu-id="e65a5-134">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="e65a5-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e65a5-135">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e65a5-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e65a5-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="e65a5-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e65a5-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e65a5-137">Schema Name</span></span>  <br/> |<span data-ttu-id="e65a5-138">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e65a5-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="e65a5-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e65a5-139">Validation File</span></span>  <br/> |<span data-ttu-id="e65a5-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e65a5-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e65a5-141">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e65a5-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="e65a5-142">False</span><span class="sxs-lookup"><span data-stu-id="e65a5-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e65a5-143">Ver também</span><span class="sxs-lookup"><span data-stu-id="e65a5-143">See also</span></span>



[<span data-ttu-id="e65a5-144">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="e65a5-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="e65a5-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="e65a5-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="e65a5-146">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="e65a5-146">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

