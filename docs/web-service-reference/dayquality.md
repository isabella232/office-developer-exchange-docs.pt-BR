---
title: DayQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayQuality
api_type:
- schema
ms.assetid: cd0eb239-6e7f-4a5a-b245-659f170550b7
description: O elemento DayQuality representa a qualidade do dia para conter os horários de reunião sugerido de qualidade.
ms.openlocfilehash: 156d5bc58d481c9c812793da4722272ac76adaad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751711"
---
# <a name="dayquality"></a><span data-ttu-id="6209d-103">DayQuality</span><span class="sxs-lookup"><span data-stu-id="6209d-103">DayQuality</span></span>

<span data-ttu-id="6209d-104">O elemento **DayQuality** representa a qualidade do dia para contendo qualidade sugerida horários de reuniões.</span><span class="sxs-lookup"><span data-stu-id="6209d-104">The **DayQuality** element represents the quality of the day for containing quality suggested meeting times.</span></span> 
  
- [<span data-ttu-id="6209d-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="6209d-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)  
- [<span data-ttu-id="6209d-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="6209d-106">SuggestionsResponse</span></span>](suggestionsresponse.md) 
- [<span data-ttu-id="6209d-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="6209d-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)  
- [<span data-ttu-id="6209d-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="6209d-108">SuggestionDayResult</span></span>](suggestiondayresult.md) 
- [<span data-ttu-id="6209d-109">DayQuality</span><span class="sxs-lookup"><span data-stu-id="6209d-109">DayQuality</span></span>](dayquality.md)
  
```xml
<DayQuality>Excellent or Good or Fair or Poor</DayQuality>
```

<span data-ttu-id="6209d-110">**SuggestionQuality**</span><span class="sxs-lookup"><span data-stu-id="6209d-110">**SuggestionQuality**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6209d-111">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6209d-111">Attributes and elements</span></span>

<span data-ttu-id="6209d-112">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6209d-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6209d-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="6209d-113">Attributes</span></span>

<span data-ttu-id="6209d-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6209d-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6209d-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6209d-115">Child elements</span></span>

<span data-ttu-id="6209d-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6209d-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6209d-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6209d-117">Parent elements</span></span>

|<span data-ttu-id="6209d-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6209d-118">**Element**</span></span>|<span data-ttu-id="6209d-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6209d-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6209d-120">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="6209d-120">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="6209d-121">Representa um único dia que contém os horários de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="6209d-121">Represents a single day that contains suggested meeting times.</span></span>  <br/><br/><span data-ttu-id="6209d-122">Este é a expressão XPath 2.0 para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="6209d-122">The following is the XPath 2.0 expression to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6209d-123">Text value</span><span class="sxs-lookup"><span data-stu-id="6209d-123">Text value</span></span>

<span data-ttu-id="6209d-124">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="6209d-124">A text value is required.</span></span> <span data-ttu-id="6209d-125">Estes são os valores possíveis para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="6209d-125">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="6209d-126">**Excelente**</span><span class="sxs-lookup"><span data-stu-id="6209d-126">**Excellent**</span></span>   
- <span data-ttu-id="6209d-127">**BOM**</span><span class="sxs-lookup"><span data-stu-id="6209d-127">**Good**</span></span>    
- <span data-ttu-id="6209d-128">**Justo**</span><span class="sxs-lookup"><span data-stu-id="6209d-128">**Fair**</span></span>    
- <span data-ttu-id="6209d-129">**Baixa**</span><span class="sxs-lookup"><span data-stu-id="6209d-129">**Poor**</span></span>
    
## <a name="remarks"></a><span data-ttu-id="6209d-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="6209d-130">Remarks</span></span>

<span data-ttu-id="6209d-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="6209d-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6209d-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6209d-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6209d-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="6209d-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6209d-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6209d-134">Schema Name</span></span>  <br/> |<span data-ttu-id="6209d-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="6209d-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="6209d-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6209d-136">Validation File</span></span>  <br/> |<span data-ttu-id="6209d-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6209d-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6209d-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6209d-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="6209d-139">False</span><span class="sxs-lookup"><span data-stu-id="6209d-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6209d-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="6209d-140">See also</span></span>

- [<span data-ttu-id="6209d-141">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="6209d-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="6209d-142">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="6209d-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="6209d-143">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="6209d-143">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

