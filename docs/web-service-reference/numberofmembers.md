---
title: NumberOfMembers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberOfMembers
api_type:
- schema
ms.assetid: 845fb877-de49-4e26-8885-6f026edd9ee9
description: O elemento NumberOfMembers representa o número de usuários, recursos e salas em uma lista de distribuição.
ms.openlocfilehash: 9777660b1a54bfb5afb6e569ba1009a1654bdef3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824635"
---
# <a name="numberofmembers"></a><span data-ttu-id="a7ac8-103">NumberOfMembers</span><span class="sxs-lookup"><span data-stu-id="a7ac8-103">NumberOfMembers</span></span>

<span data-ttu-id="a7ac8-104">O elemento **NumberOfMembers** representa o número de usuários, recursos e salas em uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="a7ac8-104">The **NumberOfMembers** element represents the number of users, resources, and rooms in a distribution list.</span></span> 
  
[<span data-ttu-id="a7ac8-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a7ac8-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="a7ac8-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="a7ac8-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="a7ac8-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="a7ac8-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="a7ac8-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="a7ac8-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="a7ac8-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="a7ac8-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="a7ac8-110">Sugestão</span><span class="sxs-lookup"><span data-stu-id="a7ac8-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="a7ac8-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="a7ac8-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="a7ac8-112">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="a7ac8-112">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
[<span data-ttu-id="a7ac8-113">NumberOfMembers</span><span class="sxs-lookup"><span data-stu-id="a7ac8-113">NumberOfMembers</span></span>](numberofmembers.md)
  
```xml
<NumberOfMembers>...</NumberOfMembers>
```

 <span data-ttu-id="a7ac8-114">**int**</span><span class="sxs-lookup"><span data-stu-id="a7ac8-114">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a7ac8-115">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a7ac8-115">Attributes and elements</span></span>

<span data-ttu-id="a7ac8-116">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a7ac8-116">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a7ac8-117">Atributos</span><span class="sxs-lookup"><span data-stu-id="a7ac8-117">Attributes</span></span>

<span data-ttu-id="a7ac8-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a7ac8-118">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a7ac8-119">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a7ac8-119">Child elements</span></span>

<span data-ttu-id="a7ac8-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a7ac8-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a7ac8-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a7ac8-121">Parent elements</span></span>

|<span data-ttu-id="a7ac8-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a7ac8-122">**Element**</span></span>|<span data-ttu-id="a7ac8-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a7ac8-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a7ac8-124">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="a7ac8-124">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="a7ac8-125">Contém informações de conflito agregadas sobre o número de usuários disponíveis, o número de usuários que possuem conflitos e o número de usuários que não têm informações de disponibilidade em uma lista de distribuição para um horário de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="a7ac8-125">Contains aggregate conflict information about the number of users available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> <span data-ttu-id="a7ac8-126">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="a7ac8-126">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a7ac8-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="a7ac8-127">Remarks</span></span>

<span data-ttu-id="a7ac8-128">O valor máximo do elemento **NumberOfMembers** é 100.</span><span class="sxs-lookup"><span data-stu-id="a7ac8-128">The maximum value of the **NumberOfMembers** element is 100.</span></span> 
  
<span data-ttu-id="a7ac8-129">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="a7ac8-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a7ac8-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a7ac8-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a7ac8-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="a7ac8-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a7ac8-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a7ac8-132">Schema Name</span></span>  <br/> |<span data-ttu-id="a7ac8-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a7ac8-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="a7ac8-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a7ac8-134">Validation File</span></span>  <br/> |<span data-ttu-id="a7ac8-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a7ac8-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a7ac8-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a7ac8-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="a7ac8-137">False</span><span class="sxs-lookup"><span data-stu-id="a7ac8-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a7ac8-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="a7ac8-138">See also</span></span>



[<span data-ttu-id="a7ac8-139">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="a7ac8-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="a7ac8-140">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a7ac8-140">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="a7ac8-141">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="a7ac8-141">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

