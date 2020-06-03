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
ms.openlocfilehash: c91087f42d806afb0a0d3d607cc84f14a1a6c1b0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462595"
---
# <a name="numberofmembers"></a><span data-ttu-id="696dc-103">NumberOfMembers</span><span class="sxs-lookup"><span data-stu-id="696dc-103">NumberOfMembers</span></span>

<span data-ttu-id="696dc-104">O elemento **NumberOfMembers** representa o número de usuários, recursos e salas em uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="696dc-104">The **NumberOfMembers** element represents the number of users, resources, and rooms in a distribution list.</span></span> 
  
[<span data-ttu-id="696dc-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="696dc-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="696dc-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="696dc-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="696dc-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="696dc-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="696dc-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="696dc-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="696dc-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="696dc-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="696dc-110">La</span><span class="sxs-lookup"><span data-stu-id="696dc-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="696dc-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="696dc-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="696dc-112">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="696dc-112">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
[<span data-ttu-id="696dc-113">NumberOfMembers</span><span class="sxs-lookup"><span data-stu-id="696dc-113">NumberOfMembers</span></span>](numberofmembers.md)
  
```xml
<NumberOfMembers>...</NumberOfMembers>
```

 <span data-ttu-id="696dc-114">**int**</span><span class="sxs-lookup"><span data-stu-id="696dc-114">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="696dc-115">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="696dc-115">Attributes and elements</span></span>

<span data-ttu-id="696dc-116">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="696dc-116">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="696dc-117">Atributos</span><span class="sxs-lookup"><span data-stu-id="696dc-117">Attributes</span></span>

<span data-ttu-id="696dc-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="696dc-118">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="696dc-119">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="696dc-119">Child elements</span></span>

<span data-ttu-id="696dc-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="696dc-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="696dc-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="696dc-121">Parent elements</span></span>

|<span data-ttu-id="696dc-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="696dc-122">**Element**</span></span>|<span data-ttu-id="696dc-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="696dc-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="696dc-124">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="696dc-124">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="696dc-125">Contém informações de conflito agregadas sobre o número de usuários disponíveis, o número de usuários que têm conflitos e o número de usuários que não têm informações de disponibilidade em uma lista de distribuição para um tempo de reunião sugerido.</span><span class="sxs-lookup"><span data-stu-id="696dc-125">Contains aggregate conflict information about the number of users available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> <span data-ttu-id="696dc-126">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="696dc-126">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="696dc-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="696dc-127">Remarks</span></span>

<span data-ttu-id="696dc-128">O valor máximo do elemento **NumberOfMembers** é 100.</span><span class="sxs-lookup"><span data-stu-id="696dc-128">The maximum value of the **NumberOfMembers** element is 100.</span></span> 
  
<span data-ttu-id="696dc-129">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="696dc-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="696dc-130">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="696dc-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="696dc-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="696dc-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="696dc-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="696dc-132">Schema Name</span></span>  <br/> |<span data-ttu-id="696dc-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="696dc-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="696dc-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="696dc-134">Validation File</span></span>  <br/> |<span data-ttu-id="696dc-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="696dc-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="696dc-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="696dc-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="696dc-137">False</span><span class="sxs-lookup"><span data-stu-id="696dc-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="696dc-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="696dc-138">See also</span></span>



[<span data-ttu-id="696dc-139">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="696dc-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="696dc-140">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="696dc-140">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="696dc-141">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="696dc-141">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

