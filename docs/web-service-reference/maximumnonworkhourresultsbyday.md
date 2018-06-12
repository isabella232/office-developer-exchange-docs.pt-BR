---
title: MaximumNonWorkHourResultsByDay
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaximumNonWorkHourResultsByDay
api_type:
- schema
ms.assetid: 9fb7314d-779c-4b1f-9d7c-b5cb092ed134
description: O elemento MaximumNonWorkHourResultsByDay Especifica o número de resultados sugeridos para horários fora do horário normal de trabalho por dia da reunião.
ms.openlocfilehash: f931dcaabda222e1579a0a4c0e0e6e49d88c6342
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824382"
---
# <a name="maximumnonworkhourresultsbyday"></a><span data-ttu-id="8fa1a-103">MaximumNonWorkHourResultsByDay</span><span class="sxs-lookup"><span data-stu-id="8fa1a-103">MaximumNonWorkHourResultsByDay</span></span>

<span data-ttu-id="8fa1a-104">O elemento **MaximumNonWorkHourResultsByDay** Especifica o número de resultados sugeridos para horários fora do horário normal de trabalho por dia da reunião.</span><span class="sxs-lookup"><span data-stu-id="8fa1a-104">The **MaximumNonWorkHourResultsByDay** element specifies the number of suggested results for meeting times outside regular working hours per day.</span></span> 
  
[<span data-ttu-id="8fa1a-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="8fa1a-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="8fa1a-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="8fa1a-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="8fa1a-107">MaximumNonWorkHourResultsByDay</span><span class="sxs-lookup"><span data-stu-id="8fa1a-107">MaximumNonWorkHourResultsByDay</span></span>](maximumnonworkhourresultsbyday.md)
  
```xml
<MaximumNonWorkHourResultsByDay>...</MaximumNonWorkHourResultsByDay>
```

 <span data-ttu-id="8fa1a-108">**int**</span><span class="sxs-lookup"><span data-stu-id="8fa1a-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8fa1a-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8fa1a-109">Attributes and elements</span></span>

<span data-ttu-id="8fa1a-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8fa1a-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8fa1a-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="8fa1a-111">Attributes</span></span>

<span data-ttu-id="8fa1a-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8fa1a-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8fa1a-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8fa1a-113">Child elements</span></span>

<span data-ttu-id="8fa1a-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8fa1a-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8fa1a-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8fa1a-115">Parent elements</span></span>

|<span data-ttu-id="8fa1a-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8fa1a-116">**Element**</span></span>|<span data-ttu-id="8fa1a-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8fa1a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8fa1a-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="8fa1a-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="8fa1a-119">Contém as opções para a obtenção de informações de sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="8fa1a-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="8fa1a-120">Este é o XPath a este elemento:</span><span class="sxs-lookup"><span data-stu-id="8fa1a-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8fa1a-121">Text value</span><span class="sxs-lookup"><span data-stu-id="8fa1a-121">Text value</span></span>

<span data-ttu-id="8fa1a-122">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="8fa1a-122">A text value is required.</span></span> <span data-ttu-id="8fa1a-123">O valor de texto representa um número inteiro.</span><span class="sxs-lookup"><span data-stu-id="8fa1a-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8fa1a-124">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="8fa1a-124">Remarks</span></span>

<span data-ttu-id="8fa1a-125">Esse elemento é necessário se o elemento [SuggestionsViewOptions](suggestionsviewoptions.md) é usado.</span><span class="sxs-lookup"><span data-stu-id="8fa1a-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="8fa1a-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="8fa1a-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="8fa1a-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8fa1a-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8fa1a-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="8fa1a-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8fa1a-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8fa1a-129">Schema Name</span></span>  <br/> |<span data-ttu-id="8fa1a-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8fa1a-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="8fa1a-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8fa1a-131">Validation File</span></span>  <br/> |<span data-ttu-id="8fa1a-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8fa1a-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8fa1a-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8fa1a-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="8fa1a-134">False</span><span class="sxs-lookup"><span data-stu-id="8fa1a-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8fa1a-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="8fa1a-135">See also</span></span>



[<span data-ttu-id="8fa1a-136">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="8fa1a-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="8fa1a-137">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="8fa1a-137">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

