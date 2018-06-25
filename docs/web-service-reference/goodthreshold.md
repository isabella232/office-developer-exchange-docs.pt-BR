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
description: O elemento GoodThreshold Especifica a porcentagem de participantes que devem ter o período de tempo abrir na ordem para o período de tempo para se qualificar como um horário de reunião sugerido BOM.
ms.openlocfilehash: 8044cb2b52cb572fad8731253dffa34de9d097fa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823746"
---
# <a name="goodthreshold"></a><span data-ttu-id="fc37b-103">GoodThreshold</span><span class="sxs-lookup"><span data-stu-id="fc37b-103">GoodThreshold</span></span>

<span data-ttu-id="fc37b-104">O elemento **GoodThreshold** Especifica a porcentagem de participantes que devem ter o período de tempo abrir na ordem para o período de tempo para se qualificar como um horário de reunião sugerido BOM.</span><span class="sxs-lookup"><span data-stu-id="fc37b-104">The **GoodThreshold** element specifies the percentage of attendees that must have the time period open in order for the time period to qualify as a Good suggested meeting time.</span></span> 
  
[<span data-ttu-id="fc37b-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="fc37b-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="fc37b-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="fc37b-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="fc37b-107">GoodThreshold</span><span class="sxs-lookup"><span data-stu-id="fc37b-107">GoodThreshold</span></span>](goodthreshold.md)
  
```xml
<GoodThreshold>...</GoodThreshold>
```

 <span data-ttu-id="fc37b-108">**int**</span><span class="sxs-lookup"><span data-stu-id="fc37b-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fc37b-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="fc37b-109">Attributes and elements</span></span>

<span data-ttu-id="fc37b-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fc37b-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc37b-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="fc37b-111">Attributes</span></span>

<span data-ttu-id="fc37b-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fc37b-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fc37b-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fc37b-113">Child elements</span></span>

<span data-ttu-id="fc37b-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fc37b-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fc37b-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fc37b-115">Parent elements</span></span>

|<span data-ttu-id="fc37b-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fc37b-116">**Element**</span></span>|<span data-ttu-id="fc37b-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fc37b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc37b-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="fc37b-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="fc37b-119">Contém as opções para a obtenção de informações de sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="fc37b-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="fc37b-120">Este é o XPath a este elemento:</span><span class="sxs-lookup"><span data-stu-id="fc37b-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fc37b-121">Text value</span><span class="sxs-lookup"><span data-stu-id="fc37b-121">Text value</span></span>

<span data-ttu-id="fc37b-122">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="fc37b-122">A text value is required.</span></span> <span data-ttu-id="fc37b-123">Os valores inteiros esperada estão entre 0 e 50.</span><span class="sxs-lookup"><span data-stu-id="fc37b-123">The expected integer values are between 0 and 50.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fc37b-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="fc37b-124">Remarks</span></span>

<span data-ttu-id="fc37b-125">Esse elemento é necessário se o elemento [SuggestionsViewOptions](suggestionsviewoptions.md) é usado.</span><span class="sxs-lookup"><span data-stu-id="fc37b-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> <span data-ttu-id="fc37b-126">O elemento **GoodThreshold** também determina quais reuniões são considerados razoável.</span><span class="sxs-lookup"><span data-stu-id="fc37b-126">The **GoodThreshold** element also determines what meetings are considered Fair.</span></span> <span data-ttu-id="fc37b-127">Ele que a porcentagem de participantes com conflitos é que menor que o limite de uma boa e maior do que 50 por cento, o tempo de reunião sugerido qualifica como razoável.</span><span class="sxs-lookup"><span data-stu-id="fc37b-127">It the percentage of attendees with conflicts is less than the Good Threshold and higher than 50 percent, the suggested meeting time qualifies as Fair.</span></span> <span data-ttu-id="fc37b-128">O limite de uma boa plus 50 é igual a porcentagem que define o limite de Good/razoável.</span><span class="sxs-lookup"><span data-stu-id="fc37b-128">The Good Threshold plus 50 equals the percentage that defines the Good/Fair threshold.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="fc37b-129">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="fc37b-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="fc37b-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="fc37b-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc37b-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="fc37b-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fc37b-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fc37b-132">Schema Name</span></span>  <br/> |<span data-ttu-id="fc37b-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="fc37b-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="fc37b-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fc37b-134">Validation File</span></span>  <br/> |<span data-ttu-id="fc37b-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fc37b-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fc37b-136">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="fc37b-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="fc37b-137">False</span><span class="sxs-lookup"><span data-stu-id="fc37b-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fc37b-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="fc37b-138">See also</span></span>



[<span data-ttu-id="fc37b-139">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="fc37b-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="fc37b-140">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="fc37b-140">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

