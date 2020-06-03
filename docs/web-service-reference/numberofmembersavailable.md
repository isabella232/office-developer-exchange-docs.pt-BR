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
description: O elemento NumberOfMembersAvailable representa o número de membros da lista de distribuição que estão disponíveis para um horário de reunião sugerido. Este elemento representa Membros para os quais o status é livre.
ms.openlocfilehash: 947e1c133cc49fb7e322962e95e184fe77e09353
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462588"
---
# <a name="numberofmembersavailable"></a><span data-ttu-id="0e19e-104">NumberOfMembersAvailable</span><span class="sxs-lookup"><span data-stu-id="0e19e-104">NumberOfMembersAvailable</span></span>

<span data-ttu-id="0e19e-105">O elemento **NumberOfMembersAvailable** representa o número de membros da lista de distribuição que estão disponíveis para um horário de reunião sugerido.</span><span class="sxs-lookup"><span data-stu-id="0e19e-105">The **NumberOfMembersAvailable** element represents the number of distribution list members who are available for a suggested meeting time.</span></span> <span data-ttu-id="0e19e-106">Este elemento representa Membros para os quais o status é **livre**.</span><span class="sxs-lookup"><span data-stu-id="0e19e-106">This element represents members for whom the status is **Free**.</span></span>
  
[<span data-ttu-id="0e19e-107">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="0e19e-107">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="0e19e-108">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="0e19e-108">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="0e19e-109">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="0e19e-109">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="0e19e-110">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="0e19e-110">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="0e19e-111">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="0e19e-111">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="0e19e-112">La</span><span class="sxs-lookup"><span data-stu-id="0e19e-112">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="0e19e-113">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="0e19e-113">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="0e19e-114">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="0e19e-114">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
[<span data-ttu-id="0e19e-115">NumberOfMembersAvailable</span><span class="sxs-lookup"><span data-stu-id="0e19e-115">NumberOfMembersAvailable</span></span>](numberofmembersavailable.md)
  
```xml
<NumberOfMembersAvailable>...</NumberOfMembersAvailable>
```

 <span data-ttu-id="0e19e-116">**int**</span><span class="sxs-lookup"><span data-stu-id="0e19e-116">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0e19e-117">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0e19e-117">Attributes and elements</span></span>

<span data-ttu-id="0e19e-118">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0e19e-118">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0e19e-119">Atributos</span><span class="sxs-lookup"><span data-stu-id="0e19e-119">Attributes</span></span>

<span data-ttu-id="0e19e-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0e19e-120">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0e19e-121">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0e19e-121">Child elements</span></span>

<span data-ttu-id="0e19e-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0e19e-122">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0e19e-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0e19e-123">Parent elements</span></span>

|<span data-ttu-id="0e19e-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0e19e-124">**Element**</span></span>|<span data-ttu-id="0e19e-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0e19e-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e19e-126">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="0e19e-126">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="0e19e-127">Contém informações de conflito agregadas sobre o número de usuários que estão disponíveis, o número de usuários que têm conflitos e o número de usuários que não têm informações de disponibilidade em uma lista de distribuição para um tempo de reunião sugerido.</span><span class="sxs-lookup"><span data-stu-id="0e19e-127">Contains aggregate conflict information about the number of users who are available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> <span data-ttu-id="0e19e-128">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="0e19e-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0e19e-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="0e19e-129">Remarks</span></span>

<span data-ttu-id="0e19e-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="0e19e-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0e19e-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0e19e-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0e19e-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="0e19e-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0e19e-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0e19e-133">Schema Name</span></span>  <br/> |<span data-ttu-id="0e19e-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0e19e-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="0e19e-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0e19e-135">Validation File</span></span>  <br/> |<span data-ttu-id="0e19e-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0e19e-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0e19e-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0e19e-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="0e19e-138">False</span><span class="sxs-lookup"><span data-stu-id="0e19e-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0e19e-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="0e19e-139">See also</span></span>



[<span data-ttu-id="0e19e-140">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="0e19e-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="0e19e-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="0e19e-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="0e19e-142">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="0e19e-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

