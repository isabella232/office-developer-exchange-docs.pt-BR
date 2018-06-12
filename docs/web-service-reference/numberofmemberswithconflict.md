---
title: NumberOfMembersWithConflict
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberOfMembersWithConflict
api_type:
- schema
ms.assetid: e61154f7-d262-43ec-b2bf-1ba6804b28dc
description: O elemento NumberOfMembersWithConflict representa o número de membros da lista de distribuição que têm um conflito com um tempo de reunião sugeridas. Esse elemento representa membros que têm um status de ocupado, ausência temporária ou provisória.
ms.openlocfilehash: 227783b4bed32686e8e098f88498fe8ebb25e3cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824634"
---
# <a name="numberofmemberswithconflict"></a><span data-ttu-id="433db-104">NumberOfMembersWithConflict</span><span class="sxs-lookup"><span data-stu-id="433db-104">NumberOfMembersWithConflict</span></span>

<span data-ttu-id="433db-105">O elemento **NumberOfMembersWithConflict** representa o número de membros da lista de distribuição que têm um conflito com um tempo de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="433db-105">The **NumberOfMembersWithConflict** element represents the number of distribution list members who have a conflict with a suggested meeting time.</span></span> <span data-ttu-id="433db-106">Esse elemento representa membros que têm um status de **ocupado**, **ausência temporária**ou **provisória**.</span><span class="sxs-lookup"><span data-stu-id="433db-106">This element represents members who have a status of **Busy**, **OOF**, or **Tentative**.</span></span>
  
[<span data-ttu-id="433db-107">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="433db-107">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="433db-108">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="433db-108">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="433db-109">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="433db-109">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="433db-110">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="433db-110">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="433db-111">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="433db-111">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="433db-112">Sugestão</span><span class="sxs-lookup"><span data-stu-id="433db-112">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="433db-113">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="433db-113">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="433db-114">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="433db-114">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
[<span data-ttu-id="433db-115">NumberOfMembersWithConflict</span><span class="sxs-lookup"><span data-stu-id="433db-115">NumberOfMembersWithConflict</span></span>](numberofmemberswithconflict.md)
  
```xml
<NumberOfMembersWithConflict>...</NumberOfMembersWithConflict>
```

 <span data-ttu-id="433db-116">**int**</span><span class="sxs-lookup"><span data-stu-id="433db-116">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="433db-117">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="433db-117">Attributes and elements</span></span>

<span data-ttu-id="433db-118">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="433db-118">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="433db-119">Atributos</span><span class="sxs-lookup"><span data-stu-id="433db-119">Attributes</span></span>

<span data-ttu-id="433db-120">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="433db-120">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="433db-121">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="433db-121">Child elements</span></span>

<span data-ttu-id="433db-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="433db-122">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="433db-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="433db-123">Parent elements</span></span>

|<span data-ttu-id="433db-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="433db-124">**Element**</span></span>|<span data-ttu-id="433db-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="433db-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="433db-126">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="433db-126">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="433db-127">Contém informações de conflito agregadas sobre o número de usuários que estão disponíveis, o número de usuários que possuem conflitos e o número de usuários que não têm informações de disponibilidade em uma lista de distribuição para um horário de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="433db-127">Contains aggregate conflict information about the number of users who are available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> <span data-ttu-id="433db-128">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="433db-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="433db-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="433db-129">Remarks</span></span>

<span data-ttu-id="433db-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="433db-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="433db-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="433db-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="433db-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="433db-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="433db-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="433db-133">Schema Name</span></span>  <br/> |<span data-ttu-id="433db-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="433db-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="433db-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="433db-135">Validation File</span></span>  <br/> |<span data-ttu-id="433db-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="433db-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="433db-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="433db-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="433db-138">False</span><span class="sxs-lookup"><span data-stu-id="433db-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="433db-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="433db-139">See also</span></span>



[<span data-ttu-id="433db-140">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="433db-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="433db-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="433db-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="433db-142">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="433db-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
