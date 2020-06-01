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
description: O elemento IsWorkTime indica se o tempo de reunião sugerido ocorre durante o horário de trabalho agendado.
ms.openlocfilehash: a3f3c73d585bee6f73863e2be64eea245be674f4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467575"
---
# <a name="isworktime"></a><span data-ttu-id="c4e49-103">IsWorkTime</span><span class="sxs-lookup"><span data-stu-id="c4e49-103">IsWorkTime</span></span>

<span data-ttu-id="c4e49-104">O elemento **IsWorkTime** indica se o tempo de reunião sugerido ocorre durante o horário de trabalho agendado.</span><span class="sxs-lookup"><span data-stu-id="c4e49-104">The **IsWorkTime** element represents whether the suggested meeting time occurs during scheduled work hours.</span></span> 
  
[<span data-ttu-id="c4e49-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="c4e49-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="c4e49-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="c4e49-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="c4e49-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="c4e49-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="c4e49-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="c4e49-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="c4e49-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="c4e49-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="c4e49-110">La</span><span class="sxs-lookup"><span data-stu-id="c4e49-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="c4e49-111">IsWorkTime</span><span class="sxs-lookup"><span data-stu-id="c4e49-111">IsWorkTime</span></span>](isworktime.md)
  
```xml
<IsWorkTime>true or false</IsWorkTime>
```

 <span data-ttu-id="c4e49-112">**boolean**</span><span class="sxs-lookup"><span data-stu-id="c4e49-112">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c4e49-113">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c4e49-113">Attributes and elements</span></span>

<span data-ttu-id="c4e49-114">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c4e49-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c4e49-115">Atributos</span><span class="sxs-lookup"><span data-stu-id="c4e49-115">Attributes</span></span>

<span data-ttu-id="c4e49-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c4e49-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c4e49-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c4e49-117">Child elements</span></span>

<span data-ttu-id="c4e49-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c4e49-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c4e49-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c4e49-119">Parent elements</span></span>

|<span data-ttu-id="c4e49-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c4e49-120">**Element**</span></span>|<span data-ttu-id="c4e49-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c4e49-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c4e49-122">La</span><span class="sxs-lookup"><span data-stu-id="c4e49-122">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="c4e49-123">Representa uma única sugestão de horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="c4e49-123">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="c4e49-124">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="c4e49-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c4e49-125">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c4e49-125">Text value</span></span>

<span data-ttu-id="c4e49-126">Um valor de texto que representa um valor booliano é necessário.</span><span class="sxs-lookup"><span data-stu-id="c4e49-126">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c4e49-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="c4e49-127">Remarks</span></span>

<span data-ttu-id="c4e49-128">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="c4e49-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c4e49-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c4e49-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c4e49-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="c4e49-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c4e49-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c4e49-131">Schema Name</span></span>  <br/> |<span data-ttu-id="c4e49-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c4e49-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="c4e49-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c4e49-133">Validation File</span></span>  <br/> |<span data-ttu-id="c4e49-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c4e49-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c4e49-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c4e49-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="c4e49-136">False</span><span class="sxs-lookup"><span data-stu-id="c4e49-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c4e49-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="c4e49-137">See also</span></span>



[<span data-ttu-id="c4e49-138">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="c4e49-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="c4e49-139">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="c4e49-139">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="c4e49-140">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="c4e49-140">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

