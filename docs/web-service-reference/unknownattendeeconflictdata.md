---
title: UnknownAttendeeConflictData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnknownAttendeeConflictData
api_type:
- schema
ms.assetid: 70e41268-c231-4587-9d23-e46927fe5272
description: O elemento UnknownAttendeeConflictData representa um participante não resolvido ou um participante que não é um usuário, uma lista de distribuição ou um contato.
ms.openlocfilehash: b4362e0117e3939c21342a1ab8079d95512aec79
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459865"
---
# <a name="unknownattendeeconflictdata"></a><span data-ttu-id="bf55a-103">UnknownAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="bf55a-103">UnknownAttendeeConflictData</span></span>

<span data-ttu-id="bf55a-104">O elemento **UnknownAttendeeConflictData** representa um participante não resolvido ou um participante que não é um usuário, uma lista de distribuição ou um contato.</span><span class="sxs-lookup"><span data-stu-id="bf55a-104">The **UnknownAttendeeConflictData** element represents an unresolvable attendee or an attendee that is not a user, distribution list, or contact.</span></span> 
  
[<span data-ttu-id="bf55a-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="bf55a-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="bf55a-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="bf55a-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="bf55a-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="bf55a-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="bf55a-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="bf55a-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="bf55a-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="bf55a-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="bf55a-110">La</span><span class="sxs-lookup"><span data-stu-id="bf55a-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="bf55a-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="bf55a-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="bf55a-112">UnknownAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="bf55a-112">UnknownAttendeeConflictData</span></span>](unknownattendeeconflictdata.md)
  
```xml
<UnknownAttendeeConflictData/>
```

 <span data-ttu-id="bf55a-113">**UnknownAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="bf55a-113">**UnknownAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bf55a-114">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="bf55a-114">Attributes and elements</span></span>

<span data-ttu-id="bf55a-115">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="bf55a-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bf55a-116">Atributos</span><span class="sxs-lookup"><span data-stu-id="bf55a-116">Attributes</span></span>

<span data-ttu-id="bf55a-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bf55a-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bf55a-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="bf55a-118">Child elements</span></span>

<span data-ttu-id="bf55a-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bf55a-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bf55a-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="bf55a-120">Parent elements</span></span>

|<span data-ttu-id="bf55a-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bf55a-121">**Element**</span></span>|<span data-ttu-id="bf55a-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bf55a-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bf55a-123">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="bf55a-123">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="bf55a-124">Contém uma matriz de dados de conflito para participantes consultados identificados na [operação GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="bf55a-124">Contains an array of conflict data for queried attendees identified in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>  <br/> <span data-ttu-id="bf55a-125">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="bf55a-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bf55a-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="bf55a-126">Remarks</span></span>

<span data-ttu-id="bf55a-127">Um participante é desconhecido se não puder ser resolvido em relação a um objeto de serviço de diretório do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bf55a-127">An attendee is unknown if it cannot be resolved against an Active Directory directory service object.</span></span> <span data-ttu-id="bf55a-128">Um participante não será resolvido se não puder ser determinado como um usuário, um grupo ou um contato.</span><span class="sxs-lookup"><span data-stu-id="bf55a-128">An attendee is unresolved if it cannot be determined to be a user, group, or contact.</span></span> <span data-ttu-id="bf55a-129">Por exemplo, um participante não será resolvido se for uma pasta pública habilitada para email.</span><span class="sxs-lookup"><span data-stu-id="bf55a-129">For example, an attendee will not be resolved if it is a mail-enabled public folder.</span></span>
  
<span data-ttu-id="bf55a-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="bf55a-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bf55a-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="bf55a-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bf55a-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="bf55a-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bf55a-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="bf55a-133">Schema Name</span></span>  <br/> |<span data-ttu-id="bf55a-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="bf55a-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="bf55a-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="bf55a-135">Validation File</span></span>  <br/> |<span data-ttu-id="bf55a-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="bf55a-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bf55a-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="bf55a-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="bf55a-138">False</span><span class="sxs-lookup"><span data-stu-id="bf55a-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bf55a-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="bf55a-139">See also</span></span>



[<span data-ttu-id="bf55a-140">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="bf55a-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="bf55a-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="bf55a-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="bf55a-142">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="bf55a-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

