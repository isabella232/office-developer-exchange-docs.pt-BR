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
description: O elemento DayQuality representa a qualidade do dia para conter os horários de reunião sugeridos de qualidade.
ms.openlocfilehash: 41cc8313dccb1a5172fefc167e6ed90a21109ec5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455111"
---
# <a name="dayquality"></a><span data-ttu-id="07702-103">DayQuality</span><span class="sxs-lookup"><span data-stu-id="07702-103">DayQuality</span></span>

<span data-ttu-id="07702-104">O elemento **DayQuality** representa a qualidade do dia para conter os horários de reunião sugeridos de qualidade.</span><span class="sxs-lookup"><span data-stu-id="07702-104">The **DayQuality** element represents the quality of the day for containing quality suggested meeting times.</span></span> 
  
- [<span data-ttu-id="07702-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="07702-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)  
- [<span data-ttu-id="07702-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="07702-106">SuggestionsResponse</span></span>](suggestionsresponse.md) 
- [<span data-ttu-id="07702-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="07702-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)  
- [<span data-ttu-id="07702-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="07702-108">SuggestionDayResult</span></span>](suggestiondayresult.md) 
- [<span data-ttu-id="07702-109">DayQuality</span><span class="sxs-lookup"><span data-stu-id="07702-109">DayQuality</span></span>](dayquality.md)
  
```xml
<DayQuality>Excellent or Good or Fair or Poor</DayQuality>
```

<span data-ttu-id="07702-110">**SuggestionQuality**</span><span class="sxs-lookup"><span data-stu-id="07702-110">**SuggestionQuality**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="07702-111">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="07702-111">Attributes and elements</span></span>

<span data-ttu-id="07702-112">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="07702-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="07702-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="07702-113">Attributes</span></span>

<span data-ttu-id="07702-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="07702-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="07702-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="07702-115">Child elements</span></span>

<span data-ttu-id="07702-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="07702-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="07702-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="07702-117">Parent elements</span></span>

|<span data-ttu-id="07702-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="07702-118">**Element**</span></span>|<span data-ttu-id="07702-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="07702-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07702-120">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="07702-120">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="07702-121">Representa um único dia que contém horários de reunião sugeridos.</span><span class="sxs-lookup"><span data-stu-id="07702-121">Represents a single day that contains suggested meeting times.</span></span>  <br/><br/><span data-ttu-id="07702-122">A seguir está a expressão XPath 2,0 para este elemento:</span><span class="sxs-lookup"><span data-stu-id="07702-122">The following is the XPath 2.0 expression to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="07702-123">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="07702-123">Text value</span></span>

<span data-ttu-id="07702-124">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="07702-124">A text value is required.</span></span> <span data-ttu-id="07702-125">Estes são os valores possíveis para este elemento:</span><span class="sxs-lookup"><span data-stu-id="07702-125">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="07702-126">**Excelente**</span><span class="sxs-lookup"><span data-stu-id="07702-126">**Excellent**</span></span>   
- <span data-ttu-id="07702-127">**Good**</span><span class="sxs-lookup"><span data-stu-id="07702-127">**Good**</span></span>    
- <span data-ttu-id="07702-128">**Grande**</span><span class="sxs-lookup"><span data-stu-id="07702-128">**Fair**</span></span>    
- <span data-ttu-id="07702-129">**Ruim**</span><span class="sxs-lookup"><span data-stu-id="07702-129">**Poor**</span></span>
    
## <a name="remarks"></a><span data-ttu-id="07702-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="07702-130">Remarks</span></span>

<span data-ttu-id="07702-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="07702-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="07702-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="07702-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07702-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="07702-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="07702-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="07702-134">Schema Name</span></span>  <br/> |<span data-ttu-id="07702-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="07702-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="07702-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="07702-136">Validation File</span></span>  <br/> |<span data-ttu-id="07702-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="07702-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="07702-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="07702-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="07702-139">False</span><span class="sxs-lookup"><span data-stu-id="07702-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="07702-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="07702-140">See also</span></span>

- [<span data-ttu-id="07702-141">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="07702-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="07702-142">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="07702-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="07702-143">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="07702-143">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

