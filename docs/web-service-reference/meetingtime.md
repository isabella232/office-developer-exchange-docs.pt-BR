---
title: MeetingTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingTime
api_type:
- schema
ms.assetid: 6e6d2d8b-e8a2-43e6-a715-0fc7d6dd44b9
description: O elemento MeetingTime representa um horário de reunião sugeridas.
ms.openlocfilehash: 1ea79be394124431aa1279ee94d5e5c6331d377b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824435"
---
# <a name="meetingtime"></a><span data-ttu-id="5c397-103">MeetingTime</span><span class="sxs-lookup"><span data-stu-id="5c397-103">MeetingTime</span></span>

<span data-ttu-id="5c397-104">O elemento **MeetingTime** representa um horário de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="5c397-104">The **MeetingTime** element represents a suggested meeting time.</span></span> 
  
[<span data-ttu-id="5c397-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="5c397-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="5c397-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="5c397-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="5c397-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="5c397-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="5c397-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="5c397-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="5c397-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="5c397-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="5c397-110">Sugestão</span><span class="sxs-lookup"><span data-stu-id="5c397-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="5c397-111">MeetingTime</span><span class="sxs-lookup"><span data-stu-id="5c397-111">MeetingTime</span></span>](meetingtime.md)
  
```xml
<MeetingTime>...</MeetingTime
```

 <span data-ttu-id="5c397-112">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="5c397-112">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c397-113">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5c397-113">Attributes and elements</span></span>

<span data-ttu-id="5c397-114">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5c397-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c397-115">Atributos</span><span class="sxs-lookup"><span data-stu-id="5c397-115">Attributes</span></span>

<span data-ttu-id="5c397-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5c397-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5c397-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5c397-117">Child elements</span></span>

<span data-ttu-id="5c397-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5c397-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5c397-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5c397-119">Parent elements</span></span>

|<span data-ttu-id="5c397-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5c397-120">**Element**</span></span>|<span data-ttu-id="5c397-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5c397-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c397-122">Sugestão</span><span class="sxs-lookup"><span data-stu-id="5c397-122">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="5c397-123">Representa uma única sugestão de tempo de reunião.</span><span class="sxs-lookup"><span data-stu-id="5c397-123">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="5c397-124">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="5c397-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5c397-125">Text value</span><span class="sxs-lookup"><span data-stu-id="5c397-125">Text value</span></span>

<span data-ttu-id="5c397-126">É necessário um valor de texto que representa um valor de **data/hora** .</span><span class="sxs-lookup"><span data-stu-id="5c397-126">A text value that represents a **dateTime** value is required.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5c397-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="5c397-127">Remarks</span></span>

<span data-ttu-id="5c397-128">O [MeetingTime](meetingtime.md) é um elemento filho obrigatório do elemento [sugestão](suggestion.md) .</span><span class="sxs-lookup"><span data-stu-id="5c397-128">The [MeetingTime](meetingtime.md) element is a required child element of the [Suggestion](suggestion.md) element.</span></span> 
  
<span data-ttu-id="5c397-129">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="5c397-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c397-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5c397-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c397-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="5c397-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5c397-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5c397-132">Schema Name</span></span>  <br/> |<span data-ttu-id="5c397-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5c397-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="5c397-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5c397-134">Validation File</span></span>  <br/> |<span data-ttu-id="5c397-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5c397-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5c397-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5c397-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="5c397-137">False</span><span class="sxs-lookup"><span data-stu-id="5c397-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5c397-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="5c397-138">See also</span></span>



[<span data-ttu-id="5c397-139">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="5c397-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="5c397-140">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="5c397-140">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="5c397-141">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="5c397-141">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

