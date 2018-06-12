---
title: SuggestionDayResultArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionDayResultArray
api_type:
- schema
ms.assetid: eeba9eff-5eca-4002-b5a5-8fb794feaba1
description: O elemento SuggestionDayResultArray contém uma matriz de reunião sugestões organizados por data.
ms.openlocfilehash: c208104356606a5d9961461ad8743a772d2410d8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837673"
---
# <a name="suggestiondayresultarray"></a><span data-ttu-id="5e905-103">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="5e905-103">SuggestionDayResultArray</span></span>

<span data-ttu-id="5e905-104">O elemento **SuggestionDayResultArray** contém uma matriz de reunião sugestões organizados por data.</span><span class="sxs-lookup"><span data-stu-id="5e905-104">The **SuggestionDayResultArray** element contains an array of meeting suggestions organized by date.</span></span> 
  
[<span data-ttu-id="5e905-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="5e905-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="5e905-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="5e905-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="5e905-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="5e905-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
```xml
<SuggestionDayResultArray>
   <SuggestionDayResult>...</SuggestionDayResult>
</SuggestionDayResultArray>
```

 <span data-ttu-id="5e905-108">**ArrayOfSuggestionDayResult**</span><span class="sxs-lookup"><span data-stu-id="5e905-108">**ArrayOfSuggestionDayResult**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5e905-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5e905-109">Attributes and elements</span></span>

<span data-ttu-id="5e905-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5e905-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5e905-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="5e905-111">Attributes</span></span>

<span data-ttu-id="5e905-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5e905-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5e905-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5e905-113">Child elements</span></span>

|<span data-ttu-id="5e905-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5e905-114">**Element**</span></span>|<span data-ttu-id="5e905-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5e905-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5e905-116">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="5e905-116">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="5e905-117">Representa um único dia que contém os horários de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="5e905-117">Represents a single day that contains suggested meeting times.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5e905-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5e905-118">Parent elements</span></span>

|<span data-ttu-id="5e905-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5e905-119">**Element**</span></span>|<span data-ttu-id="5e905-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5e905-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5e905-121">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="5e905-121">SuggestionsResponse</span></span>](suggestionsresponse.md) <br/> |<span data-ttu-id="5e905-122">Contém dados de informações e sugestão de resposta for solicitado sugestões de reunião</span><span class="sxs-lookup"><span data-stu-id="5e905-122">Contains response information and suggestion data for requested meeting suggestions</span></span>  <br/> <span data-ttu-id="5e905-123">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="5e905-123">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5e905-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="5e905-124">Remarks</span></span>

<span data-ttu-id="5e905-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="5e905-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5e905-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5e905-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5e905-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="5e905-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5e905-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5e905-128">Schema Name</span></span>  <br/> |<span data-ttu-id="5e905-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="5e905-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5e905-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5e905-130">Validation File</span></span>  <br/> |<span data-ttu-id="5e905-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5e905-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5e905-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5e905-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="5e905-133">False</span><span class="sxs-lookup"><span data-stu-id="5e905-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5e905-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="5e905-134">See also</span></span>



[<span data-ttu-id="5e905-135">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="5e905-135">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="5e905-136">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="5e905-136">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="5e905-137">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="5e905-137">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

