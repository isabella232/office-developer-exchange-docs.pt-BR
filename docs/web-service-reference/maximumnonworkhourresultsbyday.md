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
description: O elemento MaximumNonWorkHourResultsByDay especifica o número de resultados sugeridos para horários de reuniões fora de horas de trabalho normais por dia.
ms.openlocfilehash: 410d6bd84838d979af6bc53ca47f445ae55a09e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465496"
---
# <a name="maximumnonworkhourresultsbyday"></a><span data-ttu-id="3282f-103">MaximumNonWorkHourResultsByDay</span><span class="sxs-lookup"><span data-stu-id="3282f-103">MaximumNonWorkHourResultsByDay</span></span>

<span data-ttu-id="3282f-104">O elemento **MaximumNonWorkHourResultsByDay** especifica o número de resultados sugeridos para horários de reuniões fora de horas de trabalho normais por dia.</span><span class="sxs-lookup"><span data-stu-id="3282f-104">The **MaximumNonWorkHourResultsByDay** element specifies the number of suggested results for meeting times outside regular working hours per day.</span></span> 
  
[<span data-ttu-id="3282f-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="3282f-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="3282f-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="3282f-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="3282f-107">MaximumNonWorkHourResultsByDay</span><span class="sxs-lookup"><span data-stu-id="3282f-107">MaximumNonWorkHourResultsByDay</span></span>](maximumnonworkhourresultsbyday.md)
  
```xml
<MaximumNonWorkHourResultsByDay>...</MaximumNonWorkHourResultsByDay>
```

 <span data-ttu-id="3282f-108">**int**</span><span class="sxs-lookup"><span data-stu-id="3282f-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3282f-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="3282f-109">Attributes and elements</span></span>

<span data-ttu-id="3282f-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3282f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3282f-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="3282f-111">Attributes</span></span>

<span data-ttu-id="3282f-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3282f-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3282f-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3282f-113">Child elements</span></span>

<span data-ttu-id="3282f-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3282f-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3282f-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3282f-115">Parent elements</span></span>

|<span data-ttu-id="3282f-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3282f-116">**Element**</span></span>|<span data-ttu-id="3282f-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3282f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3282f-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="3282f-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="3282f-119">Contém as opções para obter informações de sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="3282f-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="3282f-120">Este é o XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="3282f-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3282f-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="3282f-121">Text value</span></span>

<span data-ttu-id="3282f-122">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3282f-122">A text value is required.</span></span> <span data-ttu-id="3282f-123">O valor de texto representa um inteiro.</span><span class="sxs-lookup"><span data-stu-id="3282f-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3282f-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="3282f-124">Remarks</span></span>

<span data-ttu-id="3282f-125">Esse elemento é necessário se o elemento [SuggestionsViewOptions](suggestionsviewoptions.md) for usado.</span><span class="sxs-lookup"><span data-stu-id="3282f-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="3282f-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="3282f-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="3282f-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="3282f-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3282f-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="3282f-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3282f-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3282f-129">Schema Name</span></span>  <br/> |<span data-ttu-id="3282f-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3282f-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="3282f-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3282f-131">Validation File</span></span>  <br/> |<span data-ttu-id="3282f-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3282f-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3282f-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3282f-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="3282f-134">False</span><span class="sxs-lookup"><span data-stu-id="3282f-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3282f-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="3282f-135">See also</span></span>



[<span data-ttu-id="3282f-136">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="3282f-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="3282f-137">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="3282f-137">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

