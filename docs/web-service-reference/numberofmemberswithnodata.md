---
title: NumberOfMembersWithNoData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberOfMembersWithNoData
api_type:
- schema
ms.assetid: 7ca9c57c-9519-442c-a9f4-dca2b0309716
description: O elemento NumberOfMembersWithNoData representa o número de membros da lista de distribuição que não publicaram dados de disponibilidade para comparar com um horário de reunião sugerido. Este elemento representa os membros de uma lista de distribuição muito grande ou membros que não têm status de dados.
ms.openlocfilehash: df41adc14f4c35c0e24d0f3c54f74a63527859d6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462546"
---
# <a name="numberofmemberswithnodata"></a><span data-ttu-id="b2115-104">NumberOfMembersWithNoData</span><span class="sxs-lookup"><span data-stu-id="b2115-104">NumberOfMembersWithNoData</span></span>

<span data-ttu-id="b2115-105">O elemento **NumberOfMembersWithNoData** representa o número de membros da lista de distribuição que não publicaram dados de disponibilidade para comparar com um horário de reunião sugerido.</span><span class="sxs-lookup"><span data-stu-id="b2115-105">The **NumberOfMembersWithNoData** element represents the number of distribution list members who do not have published free/busy data to compare to a suggested meeting time.</span></span> <span data-ttu-id="b2115-106">Este elemento representa os membros de uma lista de distribuição muito grande ou membros que não têm status de **dados** .</span><span class="sxs-lookup"><span data-stu-id="b2115-106">This element represents members of a distribution list that is too large or members who have **No Data** status.</span></span> 
  
[<span data-ttu-id="b2115-107">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="b2115-107">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="b2115-108">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="b2115-108">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="b2115-109">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="b2115-109">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="b2115-110">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="b2115-110">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="b2115-111">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="b2115-111">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="b2115-112">La</span><span class="sxs-lookup"><span data-stu-id="b2115-112">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="b2115-113">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="b2115-113">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="b2115-114">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="b2115-114">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
[<span data-ttu-id="b2115-115">NumberOfMembersWithNoData</span><span class="sxs-lookup"><span data-stu-id="b2115-115">NumberOfMembersWithNoData</span></span>](numberofmemberswithnodata.md)
  
```xml
<NumberOfMembersWithNoData>...</NumberOfMembersWithNoData>
```

 <span data-ttu-id="b2115-116">**int**</span><span class="sxs-lookup"><span data-stu-id="b2115-116">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b2115-117">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b2115-117">Attributes and elements</span></span>

<span data-ttu-id="b2115-118">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b2115-118">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b2115-119">Atributos</span><span class="sxs-lookup"><span data-stu-id="b2115-119">Attributes</span></span>

<span data-ttu-id="b2115-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2115-120">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b2115-121">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b2115-121">Child elements</span></span>

<span data-ttu-id="b2115-122">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b2115-122">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b2115-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b2115-123">Parent elements</span></span>

|<span data-ttu-id="b2115-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b2115-124">**Element**</span></span>|<span data-ttu-id="b2115-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b2115-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b2115-126">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="b2115-126">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="b2115-127">Contém informações de conflito agregadas sobre o número de usuários que estão disponíveis, o número de usuários que têm conflitos e o número de usuários que não têm informações de disponibilidade em uma lista de distribuição para um tempo de reunião sugerido.</span><span class="sxs-lookup"><span data-stu-id="b2115-127">Contains aggregate conflict information about the number of users who are available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> <span data-ttu-id="b2115-128">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="b2115-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b2115-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="b2115-129">Remarks</span></span>

<span data-ttu-id="b2115-130">Um contato em um grupo que não tem uma caixa de correio é um exemplo de um membro da lista de distribuição que não tem dados de calendário.</span><span class="sxs-lookup"><span data-stu-id="b2115-130">A contact in a group who does not have a mailbox is an example of a distribution list member who does not have calendar data.</span></span> <span data-ttu-id="b2115-131">Um contato também pode não ter status de **dados** pelos seguintes motivos:</span><span class="sxs-lookup"><span data-stu-id="b2115-131">A contact may also have **No Data** status for the following reasons:</span></span> 
  
- <span data-ttu-id="b2115-132">As permissões são insuficientes.</span><span class="sxs-lookup"><span data-stu-id="b2115-132">Permissions are insufficient.</span></span>
    
- <span data-ttu-id="b2115-133">A lista de distribuição é muito grande para ser expandida.</span><span class="sxs-lookup"><span data-stu-id="b2115-133">The distribution list is too large to expand.</span></span>
    
- <span data-ttu-id="b2115-134">O serviço de diretório do Active Directory não está disponível.</span><span class="sxs-lookup"><span data-stu-id="b2115-134">The Active Directory directory service is unavailable.</span></span>
    
<span data-ttu-id="b2115-135">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="b2115-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b2115-136">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b2115-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b2115-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="b2115-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b2115-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b2115-138">Schema Name</span></span>  <br/> |<span data-ttu-id="b2115-139">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b2115-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="b2115-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b2115-140">Validation File</span></span>  <br/> |<span data-ttu-id="b2115-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b2115-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b2115-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b2115-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="b2115-143">False</span><span class="sxs-lookup"><span data-stu-id="b2115-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b2115-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="b2115-144">See also</span></span>



[<span data-ttu-id="b2115-145">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="b2115-145">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="b2115-146">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="b2115-146">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="b2115-147">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="b2115-147">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

