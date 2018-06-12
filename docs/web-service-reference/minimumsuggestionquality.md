---
title: MinimumSuggestionQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MinimumSuggestionQuality
api_type:
- schema
ms.assetid: 3725cbd4-9bc1-4f7d-8929-b2c68cb46114
description: O elemento de MinimumSuggestionQuality define a qualidade das sugestões de reunião a serem retornados na resposta.
ms.openlocfilehash: ac79682bd761f678f23fc2d698a50fd7704f6fab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824468"
---
# <a name="minimumsuggestionquality"></a><span data-ttu-id="7e398-103">MinimumSuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="7e398-103">MinimumSuggestionQuality</span></span>

<span data-ttu-id="7e398-104">O elemento de **MinimumSuggestionQuality** define a qualidade das sugestões de reunião a serem retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="7e398-104">The **MinimumSuggestionQuality** element defines the quality of meeting suggestions to be returned in the response.</span></span> 
  
[<span data-ttu-id="7e398-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="7e398-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="7e398-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="7e398-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="7e398-107">MinimumSuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="7e398-107">MinimumSuggestionQuality</span></span>](minimumsuggestionquality.md)
  
```xml
<MinimumSuggestionQuality>...</MinimumSuggestionQuality>
```

 <span data-ttu-id="7e398-108">**SuggestionQuality**</span><span class="sxs-lookup"><span data-stu-id="7e398-108">**SuggestionQuality**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e398-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7e398-109">Attributes and elements</span></span>

<span data-ttu-id="7e398-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7e398-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e398-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="7e398-111">Attributes</span></span>

<span data-ttu-id="7e398-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7e398-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e398-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7e398-113">Child elements</span></span>

<span data-ttu-id="7e398-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7e398-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7e398-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7e398-115">Parent elements</span></span>

|<span data-ttu-id="7e398-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7e398-116">**Element**</span></span>|<span data-ttu-id="7e398-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7e398-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e398-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="7e398-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="7e398-119">Contém as opções para a obtenção de informações de sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="7e398-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="7e398-120">Este é o XPath a este elemento:</span><span class="sxs-lookup"><span data-stu-id="7e398-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7e398-121">Text value</span><span class="sxs-lookup"><span data-stu-id="7e398-121">Text value</span></span>

<span data-ttu-id="7e398-122">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="7e398-122">A text value is required.</span></span> <span data-ttu-id="7e398-123">A tabela a seguir lista os valores possíveis para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="7e398-123">The following table lists the possible values for this element:</span></span>
  
|<span data-ttu-id="7e398-124">**Valor**</span><span class="sxs-lookup"><span data-stu-id="7e398-124">**Value**</span></span>|<span data-ttu-id="7e398-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7e398-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7e398-126">**Excelente**</span><span class="sxs-lookup"><span data-stu-id="7e398-126">**Excellent**</span></span> <br/> |<span data-ttu-id="7e398-127">0% dos participantes têm um conflito com o tempo de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="7e398-127">0% of the attendees have a conflict with the suggested meeting time.</span></span>  <br/> |
|<span data-ttu-id="7e398-128">**BOM**</span><span class="sxs-lookup"><span data-stu-id="7e398-128">**Good**</span></span> <br/> |<span data-ttu-id="7e398-129">A porcentagem é considerada boa for definida usando o elemento [GoodThreshold](goodthreshold.md) .</span><span class="sxs-lookup"><span data-stu-id="7e398-129">The percentage that is considered good is set by using the [GoodThreshold](goodthreshold.md) element.</span></span>  <br/> |
|<span data-ttu-id="7e398-130">**Justo**</span><span class="sxs-lookup"><span data-stu-id="7e398-130">**Fair**</span></span> <br/> |<span data-ttu-id="7e398-131">A porcentagem que é considerada justa for definida usando o elemento [GoodThreshold](goodthreshold.md) .</span><span class="sxs-lookup"><span data-stu-id="7e398-131">The percentage that is considered fair is set by using the [GoodThreshold](goodthreshold.md) element.</span></span>  <br/> |
|<span data-ttu-id="7e398-132">**Baixa**</span><span class="sxs-lookup"><span data-stu-id="7e398-132">**Poor**</span></span> <br/> |<span data-ttu-id="7e398-133">50% ou mais dos participantes têm um conflito com o tempo de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="7e398-133">50% or more of the attendees have a conflict with the suggested meeting time.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7e398-134">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="7e398-134">Remarks</span></span>

<span data-ttu-id="7e398-135">Esse elemento é necessário se o elemento [SuggestionsViewOptions](suggestionsviewoptions.md) é usado.</span><span class="sxs-lookup"><span data-stu-id="7e398-135">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="7e398-136">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="7e398-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="7e398-137">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7e398-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e398-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="7e398-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7e398-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7e398-139">Schema Name</span></span>  <br/> |<span data-ttu-id="7e398-140">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7e398-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="7e398-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7e398-141">Validation File</span></span>  <br/> |<span data-ttu-id="7e398-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7e398-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7e398-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7e398-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="7e398-144">False</span><span class="sxs-lookup"><span data-stu-id="7e398-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e398-145">Ver também</span><span class="sxs-lookup"><span data-stu-id="7e398-145">See also</span></span>



[<span data-ttu-id="7e398-146">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="7e398-146">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="7e398-147">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="7e398-147">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

