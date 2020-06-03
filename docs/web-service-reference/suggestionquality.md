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
description: O elemento SuggestionQuality representa a qualidade do tempo de reunião sugerido.
ms.openlocfilehash: 3f8c15ccabd03687dc386a0328020cbc0bc802c4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457974"
---
# <a name="suggestionquality"></a><span data-ttu-id="eb2f7-103">SuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="eb2f7-103">SuggestionQuality</span></span>

<span data-ttu-id="eb2f7-104">O elemento **SuggestionQuality** representa a qualidade do tempo de reunião sugerido.</span><span class="sxs-lookup"><span data-stu-id="eb2f7-104">The **SuggestionQuality** element represents the quality of the suggested meeting time.</span></span> 
  
[<span data-ttu-id="eb2f7-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="eb2f7-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="eb2f7-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="eb2f7-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="eb2f7-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="eb2f7-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="eb2f7-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="eb2f7-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="eb2f7-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="eb2f7-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="eb2f7-110">La</span><span class="sxs-lookup"><span data-stu-id="eb2f7-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="eb2f7-111">SuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="eb2f7-111">SuggestionQuality</span></span>](suggestionquality.md)
  
```xml
<SuggestionQuality>Excellent or Good or Fair or Poor</SuggestionQuality>
```

 <span data-ttu-id="eb2f7-112">**SuggestionQuality**</span><span class="sxs-lookup"><span data-stu-id="eb2f7-112">**SuggestionQuality**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eb2f7-113">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="eb2f7-113">Attributes and elements</span></span>

<span data-ttu-id="eb2f7-114">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="eb2f7-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eb2f7-115">Atributos</span><span class="sxs-lookup"><span data-stu-id="eb2f7-115">Attributes</span></span>

<span data-ttu-id="eb2f7-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb2f7-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eb2f7-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="eb2f7-117">Child elements</span></span>

<span data-ttu-id="eb2f7-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="eb2f7-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="eb2f7-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="eb2f7-119">Parent elements</span></span>

|<span data-ttu-id="eb2f7-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="eb2f7-120">**Element**</span></span>|<span data-ttu-id="eb2f7-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="eb2f7-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb2f7-122">La</span><span class="sxs-lookup"><span data-stu-id="eb2f7-122">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="eb2f7-123">Representa uma única sugestão de horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="eb2f7-123">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="eb2f7-124">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="eb2f7-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="eb2f7-125">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="eb2f7-125">Text value</span></span>

<span data-ttu-id="eb2f7-126">Um valor de texto que representa um valor de **SuggestionQuality** é necessário.</span><span class="sxs-lookup"><span data-stu-id="eb2f7-126">A text value that represents a **SuggestionQuality** value is required.</span></span> <span data-ttu-id="eb2f7-127">Veja a seguir os valores possíveis:</span><span class="sxs-lookup"><span data-stu-id="eb2f7-127">The following are the possible values:</span></span> 
  
- <span data-ttu-id="eb2f7-128">**Excelente** 100% dos usuários e recursos estão disponíveis para o tempo de reunião sugerido.</span><span class="sxs-lookup"><span data-stu-id="eb2f7-128">**Excellent** 100 percent of users and resources are available for the suggested meeting time.</span></span> 
    
- <span data-ttu-id="eb2f7-129">**Bom** A porcentagem mínima de usuários e recursos disponíveis é igual ou maior do que o valor do elemento [GoodThreshold](goodthreshold.md) mais 50.</span><span class="sxs-lookup"><span data-stu-id="eb2f7-129">**Good** The minimum percentage of users and resources available is equal to or greater than the [GoodThreshold](goodthreshold.md) element value plus 50.</span></span> 
    
- <span data-ttu-id="eb2f7-130">**Justa** A porcentagem máxima de usuários e recursos disponíveis para um horário de reunião sugerido é igual ao valor do elemento [GoodThreshold](goodthreshold.md) mais 50.</span><span class="sxs-lookup"><span data-stu-id="eb2f7-130">**Fair** The maximum percentage of users and resources available for a suggested meeting time is equal to the [GoodThreshold](goodthreshold.md) element value plus 50.</span></span> <span data-ttu-id="eb2f7-131">O valor mínimo para um tempo de reunião de qualidade **justa** é de 50 por cento.</span><span class="sxs-lookup"><span data-stu-id="eb2f7-131">The minimum value for a **Fair** quality meeting time is 50 percent.</span></span> 
    
- <span data-ttu-id="eb2f7-132">**Ruim** Menos de 50% dos usuários e recursos estão disponíveis para o tempo de reunião sugerido.</span><span class="sxs-lookup"><span data-stu-id="eb2f7-132">**Poor** Less than 50 percent of the users and resources are available for the suggested meeting time.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="eb2f7-133">Comentários</span><span class="sxs-lookup"><span data-stu-id="eb2f7-133">Remarks</span></span>

<span data-ttu-id="eb2f7-134">O tipo **SuggestionQuality** também é o tipo dos elementos [DayQuality](dayquality.md) e [MinimumSuggestionQuality](minimumsuggestionquality.md) .</span><span class="sxs-lookup"><span data-stu-id="eb2f7-134">The **SuggestionQuality** type is also the type for the [DayQuality](dayquality.md) and the [MinimumSuggestionQuality](minimumsuggestionquality.md) elements.</span></span> 
  
<span data-ttu-id="eb2f7-135">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="eb2f7-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eb2f7-136">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="eb2f7-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eb2f7-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="eb2f7-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eb2f7-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="eb2f7-138">Schema Name</span></span>  <br/> |<span data-ttu-id="eb2f7-139">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="eb2f7-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="eb2f7-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="eb2f7-140">Validation File</span></span>  <br/> |<span data-ttu-id="eb2f7-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="eb2f7-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="eb2f7-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="eb2f7-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="eb2f7-143">False</span><span class="sxs-lookup"><span data-stu-id="eb2f7-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eb2f7-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="eb2f7-144">See also</span></span>



[<span data-ttu-id="eb2f7-145">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="eb2f7-145">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="eb2f7-146">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="eb2f7-146">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="eb2f7-147">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="eb2f7-147">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

