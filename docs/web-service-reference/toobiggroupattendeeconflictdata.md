---
title: TooBigGroupAttendeeConflictData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TooBigGroupAttendeeConflictData
api_type:
- schema
ms.assetid: 1512428d-ce22-4da9-b1c1-446b4bcd0a21
description: O elemento TooBigGroupAttendeeConflictData representa um participante que foi resolvido como uma lista de distribuição, mas a lista de distribuição era muito grande para expandir.
ms.openlocfilehash: 1137368d13cb5b88fd2a7866cadc6d69b783c75b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837788"
---
# <a name="toobiggroupattendeeconflictdata"></a><span data-ttu-id="c8888-103">TooBigGroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="c8888-103">TooBigGroupAttendeeConflictData</span></span>

<span data-ttu-id="c8888-104">O elemento **TooBigGroupAttendeeConflictData** representa um participante que foi resolvido como uma lista de distribuição, mas a lista de distribuição era muito grande para expandir.</span><span class="sxs-lookup"><span data-stu-id="c8888-104">The **TooBigGroupAttendeeConflictData** element represents an attendee that was resolved as a distribution list but the distribution list was too large to expand.</span></span> 
  
[<span data-ttu-id="c8888-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="c8888-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="c8888-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="c8888-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="c8888-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="c8888-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="c8888-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="c8888-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="c8888-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="c8888-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="c8888-110">Sugestão</span><span class="sxs-lookup"><span data-stu-id="c8888-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="c8888-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="c8888-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="c8888-112">TooBigGroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="c8888-112">TooBigGroupAttendeeConflictData</span></span>](toobiggroupattendeeconflictdata.md)
  
```xml
<TooBigGroupAttendeeConflictData/>
```

 <span data-ttu-id="c8888-113">**TooBigGroupAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="c8888-113">**TooBigGroupAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c8888-114">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c8888-114">Attributes and elements</span></span>

<span data-ttu-id="c8888-115">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c8888-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c8888-116">Atributos</span><span class="sxs-lookup"><span data-stu-id="c8888-116">Attributes</span></span>

<span data-ttu-id="c8888-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c8888-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c8888-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c8888-118">Child elements</span></span>

<span data-ttu-id="c8888-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c8888-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c8888-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c8888-120">Parent elements</span></span>

|<span data-ttu-id="c8888-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c8888-121">**Element**</span></span>|<span data-ttu-id="c8888-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c8888-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c8888-123">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="c8888-123">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="c8888-124">Contém uma matriz de dados de conflito para participantes identificados no [GetUserAvailabilityRequest](getuseravailabilityrequest.md).</span><span class="sxs-lookup"><span data-stu-id="c8888-124">Contains an array of conflict data for attendees identified in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md).</span></span>  <br/> <span data-ttu-id="c8888-125">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="c8888-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c8888-126">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="c8888-126">Remarks</span></span>

<span data-ttu-id="c8888-127">Listas de distribuição que contenham mais de 100 membros não podem ser expandidas.</span><span class="sxs-lookup"><span data-stu-id="c8888-127">Distribution lists that contain more than 100 members cannot be expanded.</span></span>
  
<span data-ttu-id="c8888-128">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="c8888-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c8888-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c8888-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c8888-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="c8888-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c8888-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c8888-131">Schema Name</span></span>  <br/> |<span data-ttu-id="c8888-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c8888-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="c8888-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c8888-133">Validation File</span></span>  <br/> |<span data-ttu-id="c8888-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c8888-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c8888-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c8888-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="c8888-136">False</span><span class="sxs-lookup"><span data-stu-id="c8888-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c8888-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="c8888-137">See also</span></span>



[<span data-ttu-id="c8888-138">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="c8888-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="c8888-139">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="c8888-139">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="c8888-140">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="c8888-140">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

