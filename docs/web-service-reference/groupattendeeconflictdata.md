---
title: GroupAttendeeConflictData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupAttendeeConflictData
api_type:
- schema
ms.assetid: fd8bf19a-298b-4135-93e8-ead3db7e1142
description: O elemento GroupAttendeeConflictData contém informações de conflito de agregação sobre o número de usuários que estão disponíveis, o número de usuários que têm conflitos e o número de usuários que não têm informações de disponibilidade em uma lista de distribuição para um tempo de reunião sugerido.
ms.openlocfilehash: c75a4e6f8fdff7fb2514f448350fee9f1acb9775
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462926"
---
# <a name="groupattendeeconflictdata"></a><span data-ttu-id="e854a-103">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="e854a-103">GroupAttendeeConflictData</span></span>

<span data-ttu-id="e854a-104">O elemento **GroupAttendeeConflictData** contém informações de conflito de agregação sobre o número de usuários que estão disponíveis, o número de usuários que têm conflitos e o número de usuários que não têm informações de disponibilidade em uma lista de distribuição para um tempo de reunião sugerido.</span><span class="sxs-lookup"><span data-stu-id="e854a-104">The **GroupAttendeeConflictData** element contains aggregate conflict information about the number of users who are available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span> 
  
- [<span data-ttu-id="e854a-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="e854a-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="e854a-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="e854a-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
- [<span data-ttu-id="e854a-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="e854a-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
- [<span data-ttu-id="e854a-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="e854a-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
- [<span data-ttu-id="e854a-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="e854a-109">SuggestionArray</span></span>](suggestionarray.md)
- [<span data-ttu-id="e854a-110">La</span><span class="sxs-lookup"><span data-stu-id="e854a-110">Suggestion</span></span>](suggestion.md)
- [<span data-ttu-id="e854a-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="e854a-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
- [<span data-ttu-id="e854a-112">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="e854a-112">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
```xml
<GroupAttendeeConflictData>
   <NumberOfMembers>...</NumberOfMembers>
   <NumberOfMembersAvailable>...</NumberOfMembersAvailable>
   <NumberOfMembersWithConflict>...</NumberOfMembersWithConflict>
   <NumberOfMembersWithNoData>...</NumberOfMembersWithNoData>
</GroupAttendeeConflictData>
```

<span data-ttu-id="e854a-113">**GroupAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="e854a-113">**GroupAttendeeConflictData**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e854a-114">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e854a-114">Attributes and elements</span></span>

<span data-ttu-id="e854a-115">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e854a-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e854a-116">Atributos</span><span class="sxs-lookup"><span data-stu-id="e854a-116">Attributes</span></span>

<span data-ttu-id="e854a-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e854a-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e854a-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e854a-118">Child elements</span></span>

|<span data-ttu-id="e854a-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e854a-119">**Element**</span></span>|<span data-ttu-id="e854a-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e854a-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e854a-121">NumberOfMembers</span><span class="sxs-lookup"><span data-stu-id="e854a-121">NumberOfMembers</span></span>](numberofmembers.md) <br/> |<span data-ttu-id="e854a-122">Representa o número de usuários, recursos e salas em uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="e854a-122">Represents the number of users, resources, and rooms in a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="e854a-123">NumberOfMembersAvailable</span><span class="sxs-lookup"><span data-stu-id="e854a-123">NumberOfMembersAvailable</span></span>](numberofmembersavailable.md) <br/> |<span data-ttu-id="e854a-124">Representa o número de membros da lista de distribuição que estão disponíveis para um tempo de reunião sugerido.</span><span class="sxs-lookup"><span data-stu-id="e854a-124">Represents the number of distribution list members who are available for a suggested meeting time.</span></span> <span data-ttu-id="e854a-125">Este elemento representa Membros para os quais o status é **livre**.</span><span class="sxs-lookup"><span data-stu-id="e854a-125">This element represents members for whom the status is **Free**.</span></span>  <br/> |
|[<span data-ttu-id="e854a-126">NumberOfMembersWithConflict</span><span class="sxs-lookup"><span data-stu-id="e854a-126">NumberOfMembersWithConflict</span></span>](numberofmemberswithconflict.md) <br/> |<span data-ttu-id="e854a-127">Representa o número de membros da lista de distribuição que têm um conflito com um tempo de reunião sugerido.</span><span class="sxs-lookup"><span data-stu-id="e854a-127">Represents the number of distribution list members who have a conflict with a suggested meeting time.</span></span> <span data-ttu-id="e854a-128">Este elemento representa os membros que têm um status **ocupado**, **OOF**ou **provisório** .</span><span class="sxs-lookup"><span data-stu-id="e854a-128">This element represents members who have a **Busy**, **OOF**, or **Tentative** status.</span></span>  <br/> |
|[<span data-ttu-id="e854a-129">NumberOfMembersWithNoData</span><span class="sxs-lookup"><span data-stu-id="e854a-129">NumberOfMembersWithNoData</span></span>](numberofmemberswithnodata.md) <br/> |<span data-ttu-id="e854a-130">Representa o número de membros do grupo que não publicaram dados de disponibilidade para comparar com um horário de reunião sugerido.</span><span class="sxs-lookup"><span data-stu-id="e854a-130">Represents the number of group members who do not have published free/busy data to compare to a suggested meeting time.</span></span> <span data-ttu-id="e854a-131">Este elemento representa os membros de uma lista de distribuição muito grande ou membros que não têm status de **dados** .</span><span class="sxs-lookup"><span data-stu-id="e854a-131">This element represents members of a distribution list that is too large or members who have **No Data** status.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e854a-132">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e854a-132">Parent elements</span></span>

|<span data-ttu-id="e854a-133">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e854a-133">**Element**</span></span>|<span data-ttu-id="e854a-134">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e854a-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e854a-135">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="e854a-135">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="e854a-136">Contém uma matriz de dados de conflito para participantes consultados identificados na [operação GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="e854a-136">Contains an array of conflict data for queried attendees identified in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>  <br/> <span data-ttu-id="e854a-137">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="e854a-137">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e854a-138">Comentários</span><span class="sxs-lookup"><span data-stu-id="e854a-138">Remarks</span></span>

<span data-ttu-id="e854a-139">O elemento **GroupAttendeeConflictData** está presente na resposta quando um participante do [GetUserAvailabilityRequest](getuseravailabilityrequest.md) é resolvido para uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="e854a-139">The **GroupAttendeeConflictData** element is present in the response when an attendee in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md) is resolved to a distribution list.</span></span> <span data-ttu-id="e854a-140">O elemento **GroupAttendeeConflictData** identifica três Estados de membros de uma lista de distribuição: disponível, conflitante ou nenhum dado.</span><span class="sxs-lookup"><span data-stu-id="e854a-140">The **GroupAttendeeConflictData** element identifies three states for members of a distribution list: available, conflicted, or no data.</span></span> <span data-ttu-id="e854a-141">A expansão da lista de distribuição suportará até 100 membros.</span><span class="sxs-lookup"><span data-stu-id="e854a-141">Distribution list expansion will support up to 100 members.</span></span> <span data-ttu-id="e854a-142">Portanto, o elemento [NumberOfMembers](numberofmembers.md) pode conter um máximo de 100 membros.</span><span class="sxs-lookup"><span data-stu-id="e854a-142">Therefore, the [NumberOfMembers](numberofmembers.md) element can contain a maximum of 100 members.</span></span> <span data-ttu-id="e854a-143">A expansão da lista de distribuição é recursiva.</span><span class="sxs-lookup"><span data-stu-id="e854a-143">Distribution list expansion is recursive.</span></span> <span data-ttu-id="e854a-144">Se uma lista de distribuição contiver uma lista de distribuição de filhos que expanda a associação pai total para mais de 100 membros, a lista de distribuição secundária não será expandida e será contará como uma única entrada da contagem de elementos [NumberOfMembersWithNoData](numberofmemberswithnodata.md) .</span><span class="sxs-lookup"><span data-stu-id="e854a-144">If a distribution list contains a child distribution list that expands the total parent membership to over 100 members, the child distribution list will not be expanded and will count as a single entry of the [NumberOfMembersWithNoData](numberofmemberswithnodata.md) element count.</span></span> <span data-ttu-id="e854a-145">Se uma lista de distribuição filha puder ser expandida e a associação pai total não for expandida para mais de 100 membros, sua associação será expandida e as contagens de membro serão adicionadas aos elementos filho do elemento **GroupAttendeeConflictData** .</span><span class="sxs-lookup"><span data-stu-id="e854a-145">If a child distribution list can be expanded and the total parent membership does not expand to over 100 members, its membership is expanded and the member counts are added to the child elements of the **GroupAttendeeConflictData** element.</span></span> 
  
<span data-ttu-id="e854a-146">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="e854a-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e854a-147">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e854a-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e854a-148">Namespace</span><span class="sxs-lookup"><span data-stu-id="e854a-148">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e854a-149">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e854a-149">Schema Name</span></span>  <br/> |<span data-ttu-id="e854a-150">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e854a-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="e854a-151">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e854a-151">Validation File</span></span>  <br/> |<span data-ttu-id="e854a-152">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e854a-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e854a-153">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e854a-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="e854a-154">False</span><span class="sxs-lookup"><span data-stu-id="e854a-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e854a-155">Confira também</span><span class="sxs-lookup"><span data-stu-id="e854a-155">See also</span></span>

- [<span data-ttu-id="e854a-156">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="e854a-156">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="e854a-157">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="e854a-157">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="e854a-158">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="e854a-158">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

