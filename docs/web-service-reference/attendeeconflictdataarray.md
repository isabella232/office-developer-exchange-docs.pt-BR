---
title: AttendeeConflictDataArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttendeeConflictDataArray
api_type:
- schema
ms.assetid: 1d758547-28c5-4649-8334-427480c282d6
description: O elemento AttendeeConflictDataArray contém uma matriz de dados de conflito para participantes consultados identificados na operação GetUserAvailability.
ms.openlocfilehash: 169312b8a3d37c014ba58fbfe094d786b134fc90
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751227"
---
# <a name="attendeeconflictdataarray"></a><span data-ttu-id="e476b-103">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="e476b-103">AttendeeConflictDataArray</span></span>

<span data-ttu-id="e476b-104">O elemento **AttendeeConflictDataArray** contém uma matriz de dados de conflito para participantes consultados identificados na [operação GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="e476b-104">The **AttendeeConflictDataArray** element contains an array of conflict data for queried attendees identified in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>
  
- [<span data-ttu-id="e476b-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="e476b-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
- [<span data-ttu-id="e476b-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="e476b-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
- [<span data-ttu-id="e476b-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="e476b-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
- [<span data-ttu-id="e476b-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="e476b-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
- [<span data-ttu-id="e476b-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="e476b-109">SuggestionArray</span></span>](suggestionarray.md)
  
- [<span data-ttu-id="e476b-110">Sugestão</span><span class="sxs-lookup"><span data-stu-id="e476b-110">Suggestion</span></span>](suggestion.md)
  
- [<span data-ttu-id="e476b-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="e476b-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
```xml
<ArrayOfAttendeeConflictData>
   <UnknownAttendeeConflictData>...</UnknownAttendeeConflictData>
   <IndividualAttendeeConflictData>...</IndividualAttendeeConflictData>
   <TooBigGroupAttendeeConflictData>...</TooBigGroupAttendeeConflictData>
   <GroupAttendeeConflictData>...</GroupAttendeeConflictData>
</ArrayOfAttendeeConflictData>
```

 <span data-ttu-id="e476b-112">**ArrayOfAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="e476b-112">**ArrayOfAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e476b-113">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e476b-113">Attributes and elements</span></span>

<span data-ttu-id="e476b-114">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e476b-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e476b-115">Atributos</span><span class="sxs-lookup"><span data-stu-id="e476b-115">Attributes</span></span>

<span data-ttu-id="e476b-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e476b-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e476b-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e476b-117">Child elements</span></span>

|<span data-ttu-id="e476b-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e476b-118">**Element**</span></span>|<span data-ttu-id="e476b-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e476b-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e476b-120">UnknownAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="e476b-120">UnknownAttendeeConflictData</span></span>](unknownattendeeconflictdata.md) <br/> |<span data-ttu-id="e476b-121">Representa um participante não resolvido ou um participante que não é um usuário, uma lista de distribuição ou um contato.</span><span class="sxs-lookup"><span data-stu-id="e476b-121">Represents an unresolvable attendee or an attendee that is not a user, distribution list, or contact.</span></span>  <br/> |
|[<span data-ttu-id="e476b-122">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="e476b-122">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md) <br/> |<span data-ttu-id="e476b-123">Contém um usuário ou contato status livre/ocupado para uma janela de tempo que ocorre ao mesmo tempo conforme o sugerido tempo identificado no elemento [sugestão](suggestion.md) de reunião.</span><span class="sxs-lookup"><span data-stu-id="e476b-123">Contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time identified in the [Suggestion](suggestion.md) element.</span></span>  <br/> |
|[<span data-ttu-id="e476b-124">TooBigGroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="e476b-124">TooBigGroupAttendeeConflictData</span></span>](toobiggroupattendeeconflictdata.md) <br/> |<span data-ttu-id="e476b-125">Representa um participante que resolvido como uma lista de distribuição que era muito grande para expandir.</span><span class="sxs-lookup"><span data-stu-id="e476b-125">Represents an attendee that resolved as a distribution list that was too large to expand.</span></span>  <br/> |
|[<span data-ttu-id="e476b-126">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="e476b-126">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="e476b-127">Contém informações de conflito agregadas sobre o número de usuários disponíveis, o número de usuários que possuem conflitos e o número de usuários que não têm informações de disponibilidade em uma lista de distribuição para um horário de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="e476b-127">Contains aggregate conflict information about the number of users available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e476b-128">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e476b-128">Parent elements</span></span>

|<span data-ttu-id="e476b-129">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e476b-129">**Element**</span></span>|<span data-ttu-id="e476b-130">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e476b-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e476b-131">Sugestão</span><span class="sxs-lookup"><span data-stu-id="e476b-131">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="e476b-132">Representa uma única sugestão de tempo de reunião.</span><span class="sxs-lookup"><span data-stu-id="e476b-132">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="e476b-133">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="e476b-133">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e476b-134">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="e476b-134">Remarks</span></span>

<span data-ttu-id="e476b-135">A posição de cada elemento no **AttendeeConflictDataArray** corresponde à posição dos participantes consultados no elemento [MailboxDataArray](mailboxdataarray.md) .</span><span class="sxs-lookup"><span data-stu-id="e476b-135">The position of each element in the **AttendeeConflictDataArray** corresponds to the position of the queried attendees in the [MailboxDataArray](mailboxdataarray.md) element.</span></span> <span data-ttu-id="e476b-136">Cada participante consultado deve corresponder a um dos elementos filho **AttendeeConflictDataArray** .</span><span class="sxs-lookup"><span data-stu-id="e476b-136">Each queried attendee must correspond to one of the **AttendeeConflictDataArray** child elements.</span></span> <span data-ttu-id="e476b-137">Esses elementos representam um conflito único com o tempo de reunião sugerido identificado no elemento [sugestão](suggestion.md) .</span><span class="sxs-lookup"><span data-stu-id="e476b-137">These elements represent a single conflict with the suggested meeting time identified in the [Suggestion](suggestion.md) element.</span></span> 
  
<span data-ttu-id="e476b-138">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="e476b-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e476b-139">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e476b-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e476b-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="e476b-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e476b-141">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e476b-141">Schema Name</span></span>  <br/> |<span data-ttu-id="e476b-142">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e476b-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="e476b-143">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e476b-143">Validation File</span></span>  <br/> |<span data-ttu-id="e476b-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e476b-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e476b-145">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e476b-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="e476b-146">False</span><span class="sxs-lookup"><span data-stu-id="e476b-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e476b-147">Ver também</span><span class="sxs-lookup"><span data-stu-id="e476b-147">See also</span></span>

- [<span data-ttu-id="e476b-148">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="e476b-148">GetUserAvailability operation</span></span>](getuseravailability-operation.md) 
- [<span data-ttu-id="e476b-149">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="e476b-149">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="e476b-150">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="e476b-150">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

