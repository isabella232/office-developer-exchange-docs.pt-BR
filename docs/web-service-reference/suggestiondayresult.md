---
title: SuggestionDayResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionDayResult
api_type:
- schema
ms.assetid: 916b1cbb-f2e3-471d-84b0-e33467616652
description: O elemento SuggestionDayResult representa um único dia que contém horários de reunião sugeridos.
ms.openlocfilehash: af907b62acefb4913814907722b98d326bd0535b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457988"
---
# <a name="suggestiondayresult"></a><span data-ttu-id="4c331-103">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="4c331-103">SuggestionDayResult</span></span>

<span data-ttu-id="4c331-104">O elemento **SuggestionDayResult** representa um único dia que contém horários de reunião sugeridos.</span><span class="sxs-lookup"><span data-stu-id="4c331-104">The **SuggestionDayResult** element represents a single day that contains suggested meeting times.</span></span> 
  
[<span data-ttu-id="4c331-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="4c331-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="4c331-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="4c331-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="4c331-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="4c331-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="4c331-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="4c331-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
```xml
<SuggestionDayResult>
   <Date>...</Date>
   <DayQuality>...</DayQuality>
   <SuggestionArray>...</SuggestionArray>
</SuggestionDayResult>
```

 <span data-ttu-id="4c331-109">**SuggestionDayResult**</span><span class="sxs-lookup"><span data-stu-id="4c331-109">**SuggestionDayResult**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4c331-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4c331-110">Attributes and elements</span></span>

<span data-ttu-id="4c331-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4c331-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4c331-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="4c331-112">Attributes</span></span>

<span data-ttu-id="4c331-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4c331-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4c331-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4c331-114">Child elements</span></span>

|<span data-ttu-id="4c331-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4c331-115">**Element**</span></span>|<span data-ttu-id="4c331-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4c331-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4c331-117">Date</span><span class="sxs-lookup"><span data-stu-id="4c331-117">Date</span></span>](date.md) <br/> |<span data-ttu-id="4c331-118">Representa a data que contém os horários de reunião sugeridos.</span><span class="sxs-lookup"><span data-stu-id="4c331-118">Represents the date that contains the suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="4c331-119">DayQuality</span><span class="sxs-lookup"><span data-stu-id="4c331-119">DayQuality</span></span>](dayquality.md) <br/> |<span data-ttu-id="4c331-120">Representa a qualidade do dia para conter os horários de reunião sugeridos de qualidade.</span><span class="sxs-lookup"><span data-stu-id="4c331-120">Represents the quality of the day for containing quality suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="4c331-121">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="4c331-121">SuggestionArray</span></span>](suggestionarray.md) <br/> |<span data-ttu-id="4c331-122">Contém uma matriz de sugestões de reunião.</span><span class="sxs-lookup"><span data-stu-id="4c331-122">Contains an array of meeting suggestions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4c331-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4c331-123">Parent elements</span></span>

|<span data-ttu-id="4c331-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4c331-124">**Element**</span></span>|<span data-ttu-id="4c331-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4c331-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4c331-126">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="4c331-126">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md) <br/> |<span data-ttu-id="4c331-127">Contém uma matriz de sugestões de reunião organizadas por data.</span><span class="sxs-lookup"><span data-stu-id="4c331-127">Contains an array of meeting suggestions organized by date.</span></span>  <br/> <span data-ttu-id="4c331-128">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="4c331-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4c331-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="4c331-129">Remarks</span></span>

<span data-ttu-id="4c331-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="4c331-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4c331-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="4c331-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4c331-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="4c331-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4c331-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4c331-133">Schema Name</span></span>  <br/> |<span data-ttu-id="4c331-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="4c331-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="4c331-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4c331-135">Validation File</span></span>  <br/> |<span data-ttu-id="4c331-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4c331-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4c331-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4c331-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="4c331-138">False</span><span class="sxs-lookup"><span data-stu-id="4c331-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4c331-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="4c331-139">See also</span></span>



[<span data-ttu-id="4c331-140">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="4c331-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="4c331-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="4c331-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="4c331-142">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="4c331-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

