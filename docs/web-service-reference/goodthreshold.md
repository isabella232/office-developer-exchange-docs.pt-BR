---
title: GoodThreshold
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GoodThreshold
api_type:
- schema
ms.assetid: 68f607f5-7271-46a6-8ffc-91878185a683
description: O elemento GoodThreshold especifica a porcentagem de participantes que devem ter o período de tempo aberto para que o período de tempo se qualifique como um bom horário de reunião.
ms.openlocfilehash: 34ea433ad7315d61df8cf8e22bae1166d3210af3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457309"
---
# <a name="goodthreshold"></a><span data-ttu-id="a5872-103">GoodThreshold</span><span class="sxs-lookup"><span data-stu-id="a5872-103">GoodThreshold</span></span>

<span data-ttu-id="a5872-104">O elemento **GoodThreshold** especifica a porcentagem de participantes que devem ter o período de tempo aberto para que o período de tempo se qualifique como um bom horário de reunião.</span><span class="sxs-lookup"><span data-stu-id="a5872-104">The **GoodThreshold** element specifies the percentage of attendees that must have the time period open in order for the time period to qualify as a Good suggested meeting time.</span></span> 
  
[<span data-ttu-id="a5872-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="a5872-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="a5872-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="a5872-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="a5872-107">GoodThreshold</span><span class="sxs-lookup"><span data-stu-id="a5872-107">GoodThreshold</span></span>](goodthreshold.md)
  
```xml
<GoodThreshold>...</GoodThreshold>
```

 <span data-ttu-id="a5872-108">**int**</span><span class="sxs-lookup"><span data-stu-id="a5872-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a5872-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a5872-109">Attributes and elements</span></span>

<span data-ttu-id="a5872-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a5872-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a5872-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="a5872-111">Attributes</span></span>

<span data-ttu-id="a5872-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a5872-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a5872-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a5872-113">Child elements</span></span>

<span data-ttu-id="a5872-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a5872-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a5872-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a5872-115">Parent elements</span></span>

|<span data-ttu-id="a5872-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a5872-116">**Element**</span></span>|<span data-ttu-id="a5872-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a5872-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5872-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="a5872-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="a5872-119">Contém as opções para obter informações de sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="a5872-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="a5872-120">Este é o XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="a5872-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a5872-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="a5872-121">Text value</span></span>

<span data-ttu-id="a5872-122">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5872-122">A text value is required.</span></span> <span data-ttu-id="a5872-123">Os valores inteiros esperados estão entre 0 e 50.</span><span class="sxs-lookup"><span data-stu-id="a5872-123">The expected integer values are between 0 and 50.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a5872-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="a5872-124">Remarks</span></span>

<span data-ttu-id="a5872-125">Esse elemento é necessário se o elemento [SuggestionsViewOptions](suggestionsviewoptions.md) for usado.</span><span class="sxs-lookup"><span data-stu-id="a5872-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> <span data-ttu-id="a5872-126">O elemento **GoodThreshold** também determina quais reuniões são consideradas justas.</span><span class="sxs-lookup"><span data-stu-id="a5872-126">The **GoodThreshold** element also determines what meetings are considered Fair.</span></span> <span data-ttu-id="a5872-127">A porcentagem de participantes com conflitos é menor do que o limite bom e maior que 50%, o tempo de reunião sugerido é qualificado como justo.</span><span class="sxs-lookup"><span data-stu-id="a5872-127">It the percentage of attendees with conflicts is less than the Good Threshold and higher than 50 percent, the suggested meeting time qualifies as Fair.</span></span> <span data-ttu-id="a5872-128">O bom limite mais 50 equivale à porcentagem que define o limite bom/justo.</span><span class="sxs-lookup"><span data-stu-id="a5872-128">The Good Threshold plus 50 equals the percentage that defines the Good/Fair threshold.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="a5872-129">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="a5872-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="a5872-130">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a5872-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a5872-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="a5872-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a5872-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a5872-132">Schema Name</span></span>  <br/> |<span data-ttu-id="a5872-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a5872-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="a5872-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a5872-134">Validation File</span></span>  <br/> |<span data-ttu-id="a5872-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a5872-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a5872-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a5872-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="a5872-137">False</span><span class="sxs-lookup"><span data-stu-id="a5872-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a5872-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="a5872-138">See also</span></span>



[<span data-ttu-id="a5872-139">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="a5872-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="a5872-140">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="a5872-140">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

