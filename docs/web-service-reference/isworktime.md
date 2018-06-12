---
title: IsWorkTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsWorkTime
api_type:
- schema
ms.assetid: 5243dd19-3593-4a81-bb2d-90496e04cb98
description: O elemento IsWorkTime indica se o horário da reunião sugerido ocorre durante o horário de trabalho agendado.
ms.openlocfilehash: c687b29df226ebb28cdf01d3a2da62590f790924
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824135"
---
# <a name="isworktime"></a><span data-ttu-id="ea9b8-103">IsWorkTime</span><span class="sxs-lookup"><span data-stu-id="ea9b8-103">IsWorkTime</span></span>

<span data-ttu-id="ea9b8-104">O elemento **IsWorkTime** indica se o horário da reunião sugerido ocorre durante o horário de trabalho agendado.</span><span class="sxs-lookup"><span data-stu-id="ea9b8-104">The **IsWorkTime** element represents whether the suggested meeting time occurs during scheduled work hours.</span></span> 
  
[<span data-ttu-id="ea9b8-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="ea9b8-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="ea9b8-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="ea9b8-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="ea9b8-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="ea9b8-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="ea9b8-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="ea9b8-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="ea9b8-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="ea9b8-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="ea9b8-110">Sugestão</span><span class="sxs-lookup"><span data-stu-id="ea9b8-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="ea9b8-111">IsWorkTime</span><span class="sxs-lookup"><span data-stu-id="ea9b8-111">IsWorkTime</span></span>](isworktime.md)
  
```xml
<IsWorkTime>true or false</IsWorkTime>
```

 <span data-ttu-id="ea9b8-112">**boolean**</span><span class="sxs-lookup"><span data-stu-id="ea9b8-112">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ea9b8-113">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ea9b8-113">Attributes and elements</span></span>

<span data-ttu-id="ea9b8-114">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ea9b8-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ea9b8-115">Atributos</span><span class="sxs-lookup"><span data-stu-id="ea9b8-115">Attributes</span></span>

<span data-ttu-id="ea9b8-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ea9b8-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ea9b8-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ea9b8-117">Child elements</span></span>

<span data-ttu-id="ea9b8-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ea9b8-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ea9b8-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ea9b8-119">Parent elements</span></span>

|<span data-ttu-id="ea9b8-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ea9b8-120">**Element**</span></span>|<span data-ttu-id="ea9b8-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ea9b8-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea9b8-122">Sugestão</span><span class="sxs-lookup"><span data-stu-id="ea9b8-122">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="ea9b8-123">Representa uma única sugestão de tempo de reunião.</span><span class="sxs-lookup"><span data-stu-id="ea9b8-123">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="ea9b8-124">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="ea9b8-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ea9b8-125">Text value</span><span class="sxs-lookup"><span data-stu-id="ea9b8-125">Text value</span></span>

<span data-ttu-id="ea9b8-126">É necessário um valor de texto que representa um valor booleano.</span><span class="sxs-lookup"><span data-stu-id="ea9b8-126">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ea9b8-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="ea9b8-127">Remarks</span></span>

<span data-ttu-id="ea9b8-128">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="ea9b8-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ea9b8-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ea9b8-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ea9b8-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="ea9b8-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ea9b8-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ea9b8-131">Schema Name</span></span>  <br/> |<span data-ttu-id="ea9b8-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ea9b8-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="ea9b8-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ea9b8-133">Validation File</span></span>  <br/> |<span data-ttu-id="ea9b8-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ea9b8-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ea9b8-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ea9b8-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="ea9b8-136">False</span><span class="sxs-lookup"><span data-stu-id="ea9b8-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ea9b8-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="ea9b8-137">See also</span></span>



[<span data-ttu-id="ea9b8-138">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="ea9b8-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="ea9b8-139">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="ea9b8-139">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="ea9b8-140">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="ea9b8-140">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

