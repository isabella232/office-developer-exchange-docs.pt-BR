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
description: O elemento MeetingTime representa um horário de reunião sugerido.
ms.openlocfilehash: 3a7031e70eb8b22adc8030c1cec09d33399332ee
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530447"
---
# <a name="meetingtime"></a><span data-ttu-id="3f965-103">MeetingTime</span><span class="sxs-lookup"><span data-stu-id="3f965-103">MeetingTime</span></span>

<span data-ttu-id="3f965-104">O elemento **MeetingTime** representa um horário de reunião sugerido.</span><span class="sxs-lookup"><span data-stu-id="3f965-104">The **MeetingTime** element represents a suggested meeting time.</span></span> 
  
[<span data-ttu-id="3f965-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="3f965-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="3f965-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="3f965-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="3f965-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="3f965-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="3f965-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="3f965-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="3f965-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="3f965-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="3f965-110">La</span><span class="sxs-lookup"><span data-stu-id="3f965-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="3f965-111">MeetingTime</span><span class="sxs-lookup"><span data-stu-id="3f965-111">MeetingTime</span></span>](meetingtime.md)
  
```xml
<MeetingTime>...</MeetingTime
```

 <span data-ttu-id="3f965-112">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="3f965-112">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3f965-113">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3f965-113">Attributes and elements</span></span>

<span data-ttu-id="3f965-114">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3f965-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3f965-115">Atributos</span><span class="sxs-lookup"><span data-stu-id="3f965-115">Attributes</span></span>

<span data-ttu-id="3f965-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3f965-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3f965-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3f965-117">Child elements</span></span>

<span data-ttu-id="3f965-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3f965-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3f965-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3f965-119">Parent elements</span></span>

|<span data-ttu-id="3f965-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3f965-120">**Element**</span></span>|<span data-ttu-id="3f965-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3f965-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f965-122">La</span><span class="sxs-lookup"><span data-stu-id="3f965-122">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="3f965-123">Representa uma única sugestão de horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="3f965-123">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="3f965-124">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="3f965-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3f965-125">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="3f965-125">Text value</span></span>

<span data-ttu-id="3f965-126">Um valor de texto que representa um valor de **DateTime** é necessário.</span><span class="sxs-lookup"><span data-stu-id="3f965-126">A text value that represents a **dateTime** value is required.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3f965-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="3f965-127">Remarks</span></span>

<span data-ttu-id="3f965-128">O elemento [MeetingTime](meetingtime.md) é um elemento filho obrigatório do elemento [suggestion](suggestion.md) .</span><span class="sxs-lookup"><span data-stu-id="3f965-128">The [MeetingTime](meetingtime.md) element is a required child element of the [Suggestion](suggestion.md) element.</span></span> 
  
<span data-ttu-id="3f965-129">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="3f965-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3f965-130">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3f965-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3f965-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="3f965-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3f965-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3f965-132">Schema Name</span></span>  <br/> |<span data-ttu-id="3f965-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3f965-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="3f965-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3f965-134">Validation File</span></span>  <br/> |<span data-ttu-id="3f965-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3f965-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3f965-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3f965-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="3f965-137">False</span><span class="sxs-lookup"><span data-stu-id="3f965-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3f965-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="3f965-138">See also</span></span>



[<span data-ttu-id="3f965-139">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="3f965-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="3f965-140">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="3f965-140">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="3f965-141">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="3f965-141">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

