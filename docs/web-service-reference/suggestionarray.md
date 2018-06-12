---
title: SuggestionArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionArray
api_type:
- schema
ms.assetid: c1c26008-7b14-4563-8db5-bceb0f475b1b
description: O elemento SuggestionArray contém uma matriz de sugestões de reunião.
ms.openlocfilehash: d595ae77de293a1975e15102f3f2c3395e6da633
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837670"
---
# <a name="suggestionarray"></a><span data-ttu-id="d86d5-103">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="d86d5-103">SuggestionArray</span></span>

<span data-ttu-id="d86d5-104">O elemento **SuggestionArray** contém uma matriz de sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="d86d5-104">The **SuggestionArray** element contains an array of meeting suggestions.</span></span> 
  
[<span data-ttu-id="d86d5-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d86d5-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="d86d5-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="d86d5-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="d86d5-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="d86d5-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="d86d5-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="d86d5-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="d86d5-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="d86d5-109">SuggestionArray</span></span>](suggestionarray.md)
  
```xml
<SuggestionArray>
   <Suggestion>...</Suggestion>
</SuggestionArray>
```

 <span data-ttu-id="d86d5-110">**ArrayOfSuggestion**</span><span class="sxs-lookup"><span data-stu-id="d86d5-110">**ArrayOfSuggestion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d86d5-111">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d86d5-111">Attributes and elements</span></span>

<span data-ttu-id="d86d5-112">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d86d5-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d86d5-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="d86d5-113">Attributes</span></span>

<span data-ttu-id="d86d5-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d86d5-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d86d5-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d86d5-115">Child elements</span></span>

|<span data-ttu-id="d86d5-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d86d5-116">**Element**</span></span>|<span data-ttu-id="d86d5-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d86d5-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d86d5-118">Sugestão</span><span class="sxs-lookup"><span data-stu-id="d86d5-118">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="d86d5-119">Representa uma sugestão de reunião único.</span><span class="sxs-lookup"><span data-stu-id="d86d5-119">Represents a single meeting suggestion.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d86d5-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d86d5-120">Parent elements</span></span>

|<span data-ttu-id="d86d5-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d86d5-121">**Element**</span></span>|<span data-ttu-id="d86d5-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d86d5-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d86d5-123">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="d86d5-123">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="d86d5-124">Representa um único dia que contém os horários de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="d86d5-124">Represents a single day that contains suggested meeting times.</span></span>  <br/> <span data-ttu-id="d86d5-125">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="d86d5-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d86d5-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="d86d5-126">Remarks</span></span>

<span data-ttu-id="d86d5-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="d86d5-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d86d5-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d86d5-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d86d5-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="d86d5-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d86d5-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d86d5-130">Schema Name</span></span>  <br/> |<span data-ttu-id="d86d5-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d86d5-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="d86d5-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d86d5-132">Validation File</span></span>  <br/> |<span data-ttu-id="d86d5-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d86d5-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d86d5-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d86d5-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="d86d5-135">False</span><span class="sxs-lookup"><span data-stu-id="d86d5-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d86d5-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="d86d5-136">See also</span></span>



[<span data-ttu-id="d86d5-137">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="d86d5-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="d86d5-138">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d86d5-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="d86d5-139">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="d86d5-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

