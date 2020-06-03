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
description: O elemento NumberOfMembersWithConflict representa o número de membros da lista de distribuição que têm um conflito com um tempo de reunião sugerido. Este elemento representa os membros que têm um status de ocupado, OOF ou provisório.
ms.openlocfilehash: 3ed81fc8adece140e8a94b08a9c2d94c2d9787c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529032"
---
# <a name="numberofmemberswithconflict"></a><span data-ttu-id="24231-104">NumberOfMembersWithConflict</span><span class="sxs-lookup"><span data-stu-id="24231-104">NumberOfMembersWithConflict</span></span>

<span data-ttu-id="24231-105">O elemento **NumberOfMembersWithConflict** representa o número de membros da lista de distribuição que têm um conflito com um tempo de reunião sugerido.</span><span class="sxs-lookup"><span data-stu-id="24231-105">The **NumberOfMembersWithConflict** element represents the number of distribution list members who have a conflict with a suggested meeting time.</span></span> <span data-ttu-id="24231-106">Este elemento representa os membros que têm um status de **ocupado**, **OOF**ou **provisório**.</span><span class="sxs-lookup"><span data-stu-id="24231-106">This element represents members who have a status of **Busy**, **OOF**, or **Tentative**.</span></span>
  
[<span data-ttu-id="24231-107">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="24231-107">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="24231-108">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="24231-108">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="24231-109">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="24231-109">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="24231-110">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="24231-110">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="24231-111">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="24231-111">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="24231-112">La</span><span class="sxs-lookup"><span data-stu-id="24231-112">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="24231-113">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="24231-113">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="24231-114">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="24231-114">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
[<span data-ttu-id="24231-115">NumberOfMembersWithConflict</span><span class="sxs-lookup"><span data-stu-id="24231-115">NumberOfMembersWithConflict</span></span>](numberofmemberswithconflict.md)
  
```xml
<NumberOfMembersWithConflict>...</NumberOfMembersWithConflict>
```

 <span data-ttu-id="24231-116">**int**</span><span class="sxs-lookup"><span data-stu-id="24231-116">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="24231-117">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="24231-117">Attributes and elements</span></span>

<span data-ttu-id="24231-118">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="24231-118">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="24231-119">Atributos</span><span class="sxs-lookup"><span data-stu-id="24231-119">Attributes</span></span>

<span data-ttu-id="24231-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="24231-120">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="24231-121">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="24231-121">Child elements</span></span>

<span data-ttu-id="24231-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="24231-122">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="24231-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="24231-123">Parent elements</span></span>

|<span data-ttu-id="24231-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="24231-124">**Element**</span></span>|<span data-ttu-id="24231-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="24231-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24231-126">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="24231-126">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="24231-127">Contém informações de conflito agregadas sobre o número de usuários que estão disponíveis, o número de usuários que têm conflitos e o número de usuários que não têm informações de disponibilidade em uma lista de distribuição para um tempo de reunião sugerido.</span><span class="sxs-lookup"><span data-stu-id="24231-127">Contains aggregate conflict information about the number of users who are available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> <span data-ttu-id="24231-128">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="24231-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="24231-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="24231-129">Remarks</span></span>

<span data-ttu-id="24231-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="24231-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="24231-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="24231-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="24231-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="24231-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="24231-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="24231-133">Schema Name</span></span>  <br/> |<span data-ttu-id="24231-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="24231-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="24231-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="24231-135">Validation File</span></span>  <br/> |<span data-ttu-id="24231-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="24231-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="24231-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="24231-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="24231-138">False</span><span class="sxs-lookup"><span data-stu-id="24231-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="24231-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="24231-139">See also</span></span>



[<span data-ttu-id="24231-140">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="24231-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="24231-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="24231-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="24231-142">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="24231-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

