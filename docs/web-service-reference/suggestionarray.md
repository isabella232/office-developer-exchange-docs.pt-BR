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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837670"
---
# <a name="suggestionarray"></a><span data-ttu-id="7cdea-103">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="7cdea-103">SuggestionArray</span></span>

<span data-ttu-id="7cdea-104">O elemento **SuggestionArray** contém uma matriz de sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="7cdea-104">The **SuggestionArray** element contains an array of meeting suggestions.</span></span> 
  
[<span data-ttu-id="7cdea-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="7cdea-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="7cdea-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="7cdea-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="7cdea-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="7cdea-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="7cdea-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="7cdea-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="7cdea-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="7cdea-109">SuggestionArray</span></span>](suggestionarray.md)
  
```xml
<SuggestionArray>
   <Suggestion>...</Suggestion>
</SuggestionArray>
```

 <span data-ttu-id="7cdea-110">**ArrayOfSuggestion**</span><span class="sxs-lookup"><span data-stu-id="7cdea-110">**ArrayOfSuggestion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7cdea-111">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7cdea-111">Attributes and elements</span></span>

<span data-ttu-id="7cdea-112">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7cdea-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7cdea-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="7cdea-113">Attributes</span></span>

<span data-ttu-id="7cdea-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7cdea-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7cdea-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7cdea-115">Child elements</span></span>

|<span data-ttu-id="7cdea-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7cdea-116">**Element**</span></span>|<span data-ttu-id="7cdea-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7cdea-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7cdea-118">Sugestão</span><span class="sxs-lookup"><span data-stu-id="7cdea-118">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="7cdea-119">Representa uma sugestão de reunião único.</span><span class="sxs-lookup"><span data-stu-id="7cdea-119">Represents a single meeting suggestion.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7cdea-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7cdea-120">Parent elements</span></span>

|<span data-ttu-id="7cdea-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7cdea-121">**Element**</span></span>|<span data-ttu-id="7cdea-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7cdea-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7cdea-123">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="7cdea-123">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="7cdea-124">Representa um único dia que contém os horários de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="7cdea-124">Represents a single day that contains suggested meeting times.</span></span>  <br/> <span data-ttu-id="7cdea-125">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="7cdea-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7cdea-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="7cdea-126">Remarks</span></span>

<span data-ttu-id="7cdea-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="7cdea-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7cdea-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7cdea-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7cdea-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="7cdea-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7cdea-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7cdea-130">Schema Name</span></span>  <br/> |<span data-ttu-id="7cdea-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7cdea-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="7cdea-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7cdea-132">Validation File</span></span>  <br/> |<span data-ttu-id="7cdea-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7cdea-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7cdea-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7cdea-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="7cdea-135">False</span><span class="sxs-lookup"><span data-stu-id="7cdea-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7cdea-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="7cdea-136">See also</span></span>



[<span data-ttu-id="7cdea-137">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="7cdea-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="7cdea-138">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="7cdea-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="7cdea-139">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="7cdea-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

