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
description: O elemento GroupAttendeeConflictData contém informações de conflito agregadas sobre o número de usuários que estão disponíveis, o número de usuários que possuem conflitos e o número de usuários que não têm informações de disponibilidade em uma distribuição listam para um sugerida a hora da reunião.
ms.openlocfilehash: 382b4d866c95de98bd444cd6226d71813889d4f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823757"
---
# <a name="groupattendeeconflictdata"></a><span data-ttu-id="97e95-103">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="97e95-103">GroupAttendeeConflictData</span></span>

<span data-ttu-id="97e95-104">O elemento **GroupAttendeeConflictData** contém informações de conflito agregadas sobre o número de usuários que estão disponíveis, o número de usuários que possuem conflitos e o número de usuários que não têm informações de disponibilidade em uma lista de distribuição para um horário de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="97e95-104">The **GroupAttendeeConflictData** element contains aggregate conflict information about the number of users who are available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span> 
  
- [<span data-ttu-id="97e95-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="97e95-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="97e95-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="97e95-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
- [<span data-ttu-id="97e95-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="97e95-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
- [<span data-ttu-id="97e95-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="97e95-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
- [<span data-ttu-id="97e95-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="97e95-109">SuggestionArray</span></span>](suggestionarray.md)
- [<span data-ttu-id="97e95-110">Sugestão</span><span class="sxs-lookup"><span data-stu-id="97e95-110">Suggestion</span></span>](suggestion.md)
- [<span data-ttu-id="97e95-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="97e95-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
- [<span data-ttu-id="97e95-112">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="97e95-112">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
```xml
<GroupAttendeeConflictData>
   <NumberOfMembers>...</NumberOfMembers>
   <NumberOfMembersAvailable>...</NumberOfMembersAvailable>
   <NumberOfMembersWithConflict>...</NumberOfMembersWithConflict>
   <NumberOfMembersWithNoData>...</NumberOfMembersWithNoData>
</GroupAttendeeConflictData>
```

<span data-ttu-id="97e95-113">**GroupAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="97e95-113">**GroupAttendeeConflictData**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="97e95-114">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="97e95-114">Attributes and elements</span></span>

<span data-ttu-id="97e95-115">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="97e95-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97e95-116">Atributos</span><span class="sxs-lookup"><span data-stu-id="97e95-116">Attributes</span></span>

<span data-ttu-id="97e95-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="97e95-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="97e95-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="97e95-118">Child elements</span></span>

|<span data-ttu-id="97e95-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="97e95-119">**Element**</span></span>|<span data-ttu-id="97e95-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="97e95-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97e95-121">NumberOfMembers</span><span class="sxs-lookup"><span data-stu-id="97e95-121">NumberOfMembers</span></span>](numberofmembers.md) <br/> |<span data-ttu-id="97e95-122">Representa o número de usuários, recursos e salas em uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="97e95-122">Represents the number of users, resources, and rooms in a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="97e95-123">NumberOfMembersAvailable</span><span class="sxs-lookup"><span data-stu-id="97e95-123">NumberOfMembersAvailable</span></span>](numberofmembersavailable.md) <br/> |<span data-ttu-id="97e95-124">Representa o número de membros da lista de distribuição que estão disponíveis para um horário de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="97e95-124">Represents the number of distribution list members who are available for a suggested meeting time.</span></span> <span data-ttu-id="97e95-125">Esse elemento representa membros para o qual o status é **livre**.</span><span class="sxs-lookup"><span data-stu-id="97e95-125">This element represents members for whom the status is **Free**.</span></span>  <br/> |
|[<span data-ttu-id="97e95-126">NumberOfMembersWithConflict</span><span class="sxs-lookup"><span data-stu-id="97e95-126">NumberOfMembersWithConflict</span></span>](numberofmemberswithconflict.md) <br/> |<span data-ttu-id="97e95-127">Representa o número de membros da lista de distribuição que têm um conflito com um tempo de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="97e95-127">Represents the number of distribution list members who have a conflict with a suggested meeting time.</span></span> <span data-ttu-id="97e95-128">Esse elemento representa membros que possuem um status **ocupado**, **ausência temporária**ou **provisória** .</span><span class="sxs-lookup"><span data-stu-id="97e95-128">This element represents members who have a **Busy**, **OOF**, or **Tentative** status.</span></span>  <br/> |
|[<span data-ttu-id="97e95-129">NumberOfMembersWithNoData</span><span class="sxs-lookup"><span data-stu-id="97e95-129">NumberOfMembersWithNoData</span></span>](numberofmemberswithnodata.md) <br/> |<span data-ttu-id="97e95-130">Representa o número de membros de grupo que não têm dados publicados livre/ocupado para comparar com um tempo de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="97e95-130">Represents the number of group members who do not have published free/busy data to compare to a suggested meeting time.</span></span> <span data-ttu-id="97e95-131">Este elemento representa membros de uma lista de distribuição é muito grande ou membros que possuem o status de **Nenhum dado** .</span><span class="sxs-lookup"><span data-stu-id="97e95-131">This element represents members of a distribution list that is too large or members who have **No Data** status.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="97e95-132">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="97e95-132">Parent elements</span></span>

|<span data-ttu-id="97e95-133">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="97e95-133">**Element**</span></span>|<span data-ttu-id="97e95-134">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="97e95-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97e95-135">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="97e95-135">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="97e95-136">Contém uma matriz de dados de conflito para participantes consultados identificados na [operação GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="97e95-136">Contains an array of conflict data for queried attendees identified in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>  <br/> <span data-ttu-id="97e95-137">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="97e95-137">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="97e95-138">Comentários</span><span class="sxs-lookup"><span data-stu-id="97e95-138">Remarks</span></span>

<span data-ttu-id="97e95-139">O elemento **GroupAttendeeConflictData** está presente na resposta quando um participante do [GetUserAvailabilityRequest](getuseravailabilityrequest.md) é resolvido para uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="97e95-139">The **GroupAttendeeConflictData** element is present in the response when an attendee in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md) is resolved to a distribution list.</span></span> <span data-ttu-id="97e95-140">O elemento **GroupAttendeeConflictData** identifica três estados para membros de uma lista de distribuição: disponível, em conflito, ou nenhum dado.</span><span class="sxs-lookup"><span data-stu-id="97e95-140">The **GroupAttendeeConflictData** element identifies three states for members of a distribution list: available, conflicted, or no data.</span></span> <span data-ttu-id="97e95-141">Expansão de lista de distribuição dará suporte a até 100 membros.</span><span class="sxs-lookup"><span data-stu-id="97e95-141">Distribution list expansion will support up to 100 members.</span></span> <span data-ttu-id="97e95-142">Portanto, o elemento [NumberOfMembers](numberofmembers.md) pode conter um máximo de 100 membros.</span><span class="sxs-lookup"><span data-stu-id="97e95-142">Therefore, the [NumberOfMembers](numberofmembers.md) element can contain a maximum of 100 members.</span></span> <span data-ttu-id="97e95-143">Expansão de lista de distribuição é recursiva.</span><span class="sxs-lookup"><span data-stu-id="97e95-143">Distribution list expansion is recursive.</span></span> <span data-ttu-id="97e95-144">Se uma lista de distribuição contiver uma lista de distribuição de filhos que expande a associação do pai total a mais de 100 membros, na lista de distribuição de filhos não podem ser expandida e contará como uma única entrada da contagem do elemento [NumberOfMembersWithNoData](numberofmemberswithnodata.md) .</span><span class="sxs-lookup"><span data-stu-id="97e95-144">If a distribution list contains a child distribution list that expands the total parent membership to over 100 members, the child distribution list will not be expanded and will count as a single entry of the [NumberOfMembersWithNoData](numberofmemberswithnodata.md) element count.</span></span> <span data-ttu-id="97e95-145">Se uma lista de distribuição filho pode ser expandida e a associação de total pai não expande a mais de 100 membros, sua associação é expandida e as contagens do membro são adicionadas aos elementos filho do elemento **GroupAttendeeConflictData** .</span><span class="sxs-lookup"><span data-stu-id="97e95-145">If a child distribution list can be expanded and the total parent membership does not expand to over 100 members, its membership is expanded and the member counts are added to the child elements of the **GroupAttendeeConflictData** element.</span></span> 
  
<span data-ttu-id="97e95-146">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="97e95-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97e95-147">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="97e95-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97e95-148">Namespace</span><span class="sxs-lookup"><span data-stu-id="97e95-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="97e95-149">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="97e95-149">Schema Name</span></span>  <br/> |<span data-ttu-id="97e95-150">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="97e95-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="97e95-151">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="97e95-151">Validation File</span></span>  <br/> |<span data-ttu-id="97e95-152">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="97e95-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="97e95-153">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="97e95-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="97e95-154">False</span><span class="sxs-lookup"><span data-stu-id="97e95-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="97e95-155">Ver também</span><span class="sxs-lookup"><span data-stu-id="97e95-155">See also</span></span>

- [<span data-ttu-id="97e95-156">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="97e95-156">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="97e95-157">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="97e95-157">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="97e95-158">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="97e95-158">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

