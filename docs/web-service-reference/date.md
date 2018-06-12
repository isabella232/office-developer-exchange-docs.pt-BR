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
description: O elemento de data representa a data em que contém os horários sugeridos de reunião.
ms.openlocfilehash: 98dc9d6c599222c819b2c9ed1bacd05758ae1655
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751679"
---
# <a name="date"></a><span data-ttu-id="10edd-103">Data</span><span class="sxs-lookup"><span data-stu-id="10edd-103">Date</span></span>

<span data-ttu-id="10edd-104">O elemento de **Data** representa a data em que contém os horários sugeridos de reunião.</span><span class="sxs-lookup"><span data-stu-id="10edd-104">The **Date** element represents the date that contains the suggested meeting times.</span></span> 
  
- [<span data-ttu-id="10edd-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="10edd-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md) 
- [<span data-ttu-id="10edd-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="10edd-106">SuggestionsResponse</span></span>](suggestionsresponse.md) 
- [<span data-ttu-id="10edd-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="10edd-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)  
- [<span data-ttu-id="10edd-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="10edd-108">SuggestionDayResult</span></span>](suggestiondayresult.md)  
- [<span data-ttu-id="10edd-109">Date</span><span class="sxs-lookup"><span data-stu-id="10edd-109">Date</span></span>](date.md)
  
```xml
<Date>...</Date>
```

<span data-ttu-id="10edd-110">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="10edd-110">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="10edd-111">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="10edd-111">Attributes and elements</span></span>

<span data-ttu-id="10edd-112">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="10edd-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="10edd-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="10edd-113">Attributes</span></span>

<span data-ttu-id="10edd-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="10edd-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="10edd-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="10edd-115">Child elements</span></span>

<span data-ttu-id="10edd-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="10edd-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="10edd-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="10edd-117">Parent elements</span></span>

|<span data-ttu-id="10edd-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="10edd-118">**Element**</span></span>|<span data-ttu-id="10edd-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="10edd-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="10edd-120">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="10edd-120">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="10edd-121">Representa um único dia que contém os horários de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="10edd-121">Represents a single day that contains suggested meeting times.</span></span>  <br/><br/><span data-ttu-id="10edd-122">Este é a expressão XPath 2.0 para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="10edd-122">The following is the XPath 2.0 expression to this element:</span></span><br/><br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="10edd-123">Text value</span><span class="sxs-lookup"><span data-stu-id="10edd-123">Text value</span></span>

<span data-ttu-id="10edd-124">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="10edd-124">A text value is required.</span></span> <span data-ttu-id="10edd-125">Revise as recomendações de tipo de dados de esquema de World Wide Web Consortium (W3C) para o formato o tipo de dados primitivo dateTime.</span><span class="sxs-lookup"><span data-stu-id="10edd-125">Review the World Wide Web Consortium (W3C) schema datatype recommendations for the format of the dateTime primitive datatype.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="10edd-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="10edd-126">Remarks</span></span>

<span data-ttu-id="10edd-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="10edd-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="10edd-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="10edd-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="10edd-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="10edd-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="10edd-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="10edd-130">Schema Name</span></span>  <br/> |<span data-ttu-id="10edd-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="10edd-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="10edd-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="10edd-132">Validation File</span></span>  <br/> |<span data-ttu-id="10edd-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="10edd-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="10edd-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="10edd-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="10edd-135">False</span><span class="sxs-lookup"><span data-stu-id="10edd-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="10edd-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="10edd-136">See also</span></span>

- [<span data-ttu-id="10edd-137">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="10edd-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md) 
- [<span data-ttu-id="10edd-138">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="10edd-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="10edd-139">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="10edd-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

