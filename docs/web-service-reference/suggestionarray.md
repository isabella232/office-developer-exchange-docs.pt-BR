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
ms.openlocfilehash: ec982417c39569820beef82ae837eacbe316740c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466672"
---
# <a name="suggestionarray"></a><span data-ttu-id="fc667-103">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="fc667-103">SuggestionArray</span></span>

<span data-ttu-id="fc667-104">O elemento **SuggestionArray** contém uma matriz de sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="fc667-104">The **SuggestionArray** element contains an array of meeting suggestions.</span></span> 
  
[<span data-ttu-id="fc667-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="fc667-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="fc667-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="fc667-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="fc667-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="fc667-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="fc667-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="fc667-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="fc667-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="fc667-109">SuggestionArray</span></span>](suggestionarray.md)
  
```xml
<SuggestionArray>
   <Suggestion>...</Suggestion>
</SuggestionArray>
```

 <span data-ttu-id="fc667-110">**ArrayOfSuggestion**</span><span class="sxs-lookup"><span data-stu-id="fc667-110">**ArrayOfSuggestion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fc667-111">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="fc667-111">Attributes and elements</span></span>

<span data-ttu-id="fc667-112">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fc667-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc667-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="fc667-113">Attributes</span></span>

<span data-ttu-id="fc667-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fc667-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fc667-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fc667-115">Child elements</span></span>

|<span data-ttu-id="fc667-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fc667-116">**Element**</span></span>|<span data-ttu-id="fc667-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fc667-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc667-118">La</span><span class="sxs-lookup"><span data-stu-id="fc667-118">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="fc667-119">Representa uma única sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="fc667-119">Represents a single meeting suggestion.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fc667-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fc667-120">Parent elements</span></span>

|<span data-ttu-id="fc667-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fc667-121">**Element**</span></span>|<span data-ttu-id="fc667-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fc667-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc667-123">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="fc667-123">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="fc667-124">Representa um único dia que contém horários de reunião sugeridos.</span><span class="sxs-lookup"><span data-stu-id="fc667-124">Represents a single day that contains suggested meeting times.</span></span>  <br/> <span data-ttu-id="fc667-125">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="fc667-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fc667-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="fc667-126">Remarks</span></span>

<span data-ttu-id="fc667-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="fc667-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fc667-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="fc667-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc667-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="fc667-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fc667-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fc667-130">Schema Name</span></span>  <br/> |<span data-ttu-id="fc667-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="fc667-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="fc667-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fc667-132">Validation File</span></span>  <br/> |<span data-ttu-id="fc667-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="fc667-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fc667-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="fc667-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="fc667-135">False</span><span class="sxs-lookup"><span data-stu-id="fc667-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fc667-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="fc667-136">See also</span></span>



[<span data-ttu-id="fc667-137">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="fc667-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="fc667-138">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="fc667-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="fc667-139">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="fc667-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

