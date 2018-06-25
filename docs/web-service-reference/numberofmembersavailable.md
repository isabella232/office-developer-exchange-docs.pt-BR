---
title: NumberOfMembersAvailable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberOfMembersAvailable
api_type:
- schema
ms.assetid: e367a278-1622-4b65-955f-2d4b2fc6e4d7
description: O elemento NumberOfMembersAvailable representa o número de membros da lista de distribuição que estão disponíveis para um horário de reunião sugeridas. Esse elemento representa membros para o qual o status é livre.
ms.openlocfilehash: 8669f61fbd640c160ad54739c5a15407b3dd470a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824641"
---
# <a name="numberofmembersavailable"></a><span data-ttu-id="63375-104">NumberOfMembersAvailable</span><span class="sxs-lookup"><span data-stu-id="63375-104">NumberOfMembersAvailable</span></span>

<span data-ttu-id="63375-105">O elemento **NumberOfMembersAvailable** representa o número de membros da lista de distribuição que estão disponíveis para um horário de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="63375-105">The **NumberOfMembersAvailable** element represents the number of distribution list members who are available for a suggested meeting time.</span></span> <span data-ttu-id="63375-106">Esse elemento representa membros para o qual o status é **livre**.</span><span class="sxs-lookup"><span data-stu-id="63375-106">This element represents members for whom the status is **Free**.</span></span>
  
[<span data-ttu-id="63375-107">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="63375-107">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="63375-108">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="63375-108">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="63375-109">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="63375-109">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="63375-110">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="63375-110">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="63375-111">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="63375-111">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="63375-112">Sugestão</span><span class="sxs-lookup"><span data-stu-id="63375-112">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="63375-113">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="63375-113">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="63375-114">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="63375-114">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
[<span data-ttu-id="63375-115">NumberOfMembersAvailable</span><span class="sxs-lookup"><span data-stu-id="63375-115">NumberOfMembersAvailable</span></span>](numberofmembersavailable.md)
  
```xml
<NumberOfMembersAvailable>...</NumberOfMembersAvailable>
```

 <span data-ttu-id="63375-116">**int**</span><span class="sxs-lookup"><span data-stu-id="63375-116">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="63375-117">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="63375-117">Attributes and elements</span></span>

<span data-ttu-id="63375-118">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="63375-118">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63375-119">Atributos</span><span class="sxs-lookup"><span data-stu-id="63375-119">Attributes</span></span>

<span data-ttu-id="63375-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="63375-120">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="63375-121">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="63375-121">Child elements</span></span>

<span data-ttu-id="63375-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="63375-122">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="63375-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="63375-123">Parent elements</span></span>

|<span data-ttu-id="63375-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="63375-124">**Element**</span></span>|<span data-ttu-id="63375-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="63375-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63375-126">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="63375-126">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="63375-127">Contém informações de conflito agregadas sobre o número de usuários que estão disponíveis, o número de usuários que possuem conflitos e o número de usuários que não têm informações de disponibilidade em uma lista de distribuição para um horário de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="63375-127">Contains aggregate conflict information about the number of users who are available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> <span data-ttu-id="63375-128">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="63375-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="63375-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="63375-129">Remarks</span></span>

<span data-ttu-id="63375-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="63375-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="63375-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="63375-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="63375-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="63375-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="63375-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="63375-133">Schema Name</span></span>  <br/> |<span data-ttu-id="63375-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="63375-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="63375-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="63375-135">Validation File</span></span>  <br/> |<span data-ttu-id="63375-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="63375-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="63375-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="63375-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="63375-138">False</span><span class="sxs-lookup"><span data-stu-id="63375-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="63375-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="63375-139">See also</span></span>



[<span data-ttu-id="63375-140">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="63375-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="63375-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="63375-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="63375-142">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="63375-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

