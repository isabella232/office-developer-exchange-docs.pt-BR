---
title: SuggestionQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionQuality
api_type:
- schema
ms.assetid: 734f1a58-adda-4830-973e-e84bf7b870d5
description: O elemento SuggestionQuality representa a qualidade do tempo de reunião sugeridas.
ms.openlocfilehash: e67e0149226b36c22cdd00acd78f6582f826dd3e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837672"
---
# <a name="suggestionquality"></a><span data-ttu-id="729a4-103">SuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="729a4-103">SuggestionQuality</span></span>

<span data-ttu-id="729a4-104">O elemento **SuggestionQuality** representa a qualidade do tempo de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="729a4-104">The **SuggestionQuality** element represents the quality of the suggested meeting time.</span></span> 
  
[<span data-ttu-id="729a4-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="729a4-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="729a4-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="729a4-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="729a4-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="729a4-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="729a4-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="729a4-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="729a4-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="729a4-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="729a4-110">Sugestão</span><span class="sxs-lookup"><span data-stu-id="729a4-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="729a4-111">SuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="729a4-111">SuggestionQuality</span></span>](suggestionquality.md)
  
```xml
<SuggestionQuality>Excellent or Good or Fair or Poor</SuggestionQuality>
```

 <span data-ttu-id="729a4-112">**SuggestionQuality**</span><span class="sxs-lookup"><span data-stu-id="729a4-112">**SuggestionQuality**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="729a4-113">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="729a4-113">Attributes and elements</span></span>

<span data-ttu-id="729a4-114">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="729a4-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="729a4-115">Atributos</span><span class="sxs-lookup"><span data-stu-id="729a4-115">Attributes</span></span>

<span data-ttu-id="729a4-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="729a4-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="729a4-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="729a4-117">Child elements</span></span>

<span data-ttu-id="729a4-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="729a4-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="729a4-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="729a4-119">Parent elements</span></span>

|<span data-ttu-id="729a4-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="729a4-120">**Element**</span></span>|<span data-ttu-id="729a4-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="729a4-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="729a4-122">Sugestão</span><span class="sxs-lookup"><span data-stu-id="729a4-122">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="729a4-123">Representa uma única sugestão de tempo de reunião.</span><span class="sxs-lookup"><span data-stu-id="729a4-123">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="729a4-124">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="729a4-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="729a4-125">Text value</span><span class="sxs-lookup"><span data-stu-id="729a4-125">Text value</span></span>

<span data-ttu-id="729a4-126">Um valor de texto que representa um valor de **SuggestionQuality** é necessário.</span><span class="sxs-lookup"><span data-stu-id="729a4-126">A text value that represents a **SuggestionQuality** value is required.</span></span> <span data-ttu-id="729a4-127">Veja a seguir os valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="729a4-127">The following are the possible values:</span></span> 
  
- <span data-ttu-id="729a4-128">**Excelente** 100% de usuários e recursos estão disponíveis para o tempo de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="729a4-128">**Excellent** 100 percent of users and resources are available for the suggested meeting time.</span></span> 
    
- <span data-ttu-id="729a4-129">**BOM** A porcentagem mínima de usuários e os recursos disponíveis é igual ou maior que o valor do elemento de [GoodThreshold](goodthreshold.md) mais de 50.</span><span class="sxs-lookup"><span data-stu-id="729a4-129">**Good** The minimum percentage of users and resources available is equal to or greater than the [GoodThreshold](goodthreshold.md) element value plus 50.</span></span> 
    
- <span data-ttu-id="729a4-130">**Justo** A porcentagem máxima de usuários e os recursos disponíveis para um horário de reunião sugerido é igual ao valor do elemento [GoodThreshold](goodthreshold.md) mais de 50.</span><span class="sxs-lookup"><span data-stu-id="729a4-130">**Fair** The maximum percentage of users and resources available for a suggested meeting time is equal to the [GoodThreshold](goodthreshold.md) element value plus 50.</span></span> <span data-ttu-id="729a4-131">O valor mínimo para um horário de reunião de qualidade **justo** é 50 por cento.</span><span class="sxs-lookup"><span data-stu-id="729a4-131">The minimum value for a **Fair** quality meeting time is 50 percent.</span></span> 
    
- <span data-ttu-id="729a4-132">**Baixa** Menor que 50% dos usuários e recursos estão disponíveis para o tempo de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="729a4-132">**Poor** Less than 50 percent of the users and resources are available for the suggested meeting time.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="729a4-133">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="729a4-133">Remarks</span></span>

<span data-ttu-id="729a4-134">O tipo de **SuggestionQuality** também é o tipo para o [DayQuality](dayquality.md) e os elementos de [MinimumSuggestionQuality](minimumsuggestionquality.md) .</span><span class="sxs-lookup"><span data-stu-id="729a4-134">The **SuggestionQuality** type is also the type for the [DayQuality](dayquality.md) and the [MinimumSuggestionQuality](minimumsuggestionquality.md) elements.</span></span> 
  
<span data-ttu-id="729a4-135">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="729a4-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="729a4-136">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="729a4-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="729a4-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="729a4-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="729a4-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="729a4-138">Schema Name</span></span>  <br/> |<span data-ttu-id="729a4-139">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="729a4-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="729a4-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="729a4-140">Validation File</span></span>  <br/> |<span data-ttu-id="729a4-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="729a4-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="729a4-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="729a4-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="729a4-143">False</span><span class="sxs-lookup"><span data-stu-id="729a4-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="729a4-144">Ver também</span><span class="sxs-lookup"><span data-stu-id="729a4-144">See also</span></span>



[<span data-ttu-id="729a4-145">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="729a4-145">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="729a4-146">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="729a4-146">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="729a4-147">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="729a4-147">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

