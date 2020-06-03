---
title: Data
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Date
api_type:
- schema
ms.assetid: 2f6bc090-fff4-45b1-8d7e-8fd6e060cce2
description: O elemento Date representa a data que contém os horários de reunião sugeridos.
ms.openlocfilehash: bcc152ed6aba94907189b5579b998815be45db16
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44443785"
---
# <a name="date"></a><span data-ttu-id="d1e5e-103">Data</span><span class="sxs-lookup"><span data-stu-id="d1e5e-103">Date</span></span>

<span data-ttu-id="d1e5e-104">O elemento **Date** representa a data que contém os horários de reunião sugeridos.</span><span class="sxs-lookup"><span data-stu-id="d1e5e-104">The **Date** element represents the date that contains the suggested meeting times.</span></span> 
  
- [<span data-ttu-id="d1e5e-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d1e5e-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md) 
- [<span data-ttu-id="d1e5e-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="d1e5e-106">SuggestionsResponse</span></span>](suggestionsresponse.md) 
- [<span data-ttu-id="d1e5e-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="d1e5e-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)  
- [<span data-ttu-id="d1e5e-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="d1e5e-108">SuggestionDayResult</span></span>](suggestiondayresult.md)  
- [<span data-ttu-id="d1e5e-109">Date</span><span class="sxs-lookup"><span data-stu-id="d1e5e-109">Date</span></span>](date.md)
  
```xml
<Date>...</Date>
```

<span data-ttu-id="d1e5e-110">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="d1e5e-110">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d1e5e-111">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d1e5e-111">Attributes and elements</span></span>

<span data-ttu-id="d1e5e-112">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d1e5e-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d1e5e-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="d1e5e-113">Attributes</span></span>

<span data-ttu-id="d1e5e-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d1e5e-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d1e5e-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d1e5e-115">Child elements</span></span>

<span data-ttu-id="d1e5e-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d1e5e-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d1e5e-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d1e5e-117">Parent elements</span></span>

|<span data-ttu-id="d1e5e-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d1e5e-118">**Element**</span></span>|<span data-ttu-id="d1e5e-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d1e5e-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d1e5e-120">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="d1e5e-120">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="d1e5e-121">Representa um único dia que contém horários de reunião sugeridos.</span><span class="sxs-lookup"><span data-stu-id="d1e5e-121">Represents a single day that contains suggested meeting times.</span></span>  <br/><br/><span data-ttu-id="d1e5e-122">A seguir está a expressão XPath 2,0 para este elemento:</span><span class="sxs-lookup"><span data-stu-id="d1e5e-122">The following is the XPath 2.0 expression to this element:</span></span><br/><br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d1e5e-123">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="d1e5e-123">Text value</span></span>

<span data-ttu-id="d1e5e-124">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d1e5e-124">A text value is required.</span></span> <span data-ttu-id="d1e5e-125">Revise as recomendações de tipo de dados do esquema W3C (World Wide Web Consortium) para o formato do tipo de dados primitiva de dateTime.</span><span class="sxs-lookup"><span data-stu-id="d1e5e-125">Review the World Wide Web Consortium (W3C) schema datatype recommendations for the format of the dateTime primitive datatype.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d1e5e-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="d1e5e-126">Remarks</span></span>

<span data-ttu-id="d1e5e-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="d1e5e-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d1e5e-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d1e5e-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d1e5e-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="d1e5e-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d1e5e-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d1e5e-130">Schema Name</span></span>  <br/> |<span data-ttu-id="d1e5e-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d1e5e-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="d1e5e-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d1e5e-132">Validation File</span></span>  <br/> |<span data-ttu-id="d1e5e-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d1e5e-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d1e5e-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d1e5e-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="d1e5e-135">False</span><span class="sxs-lookup"><span data-stu-id="d1e5e-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d1e5e-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="d1e5e-136">See also</span></span>

- [<span data-ttu-id="d1e5e-137">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="d1e5e-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md) 
- [<span data-ttu-id="d1e5e-138">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d1e5e-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="d1e5e-139">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="d1e5e-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

