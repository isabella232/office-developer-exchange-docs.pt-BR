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
description: O elemento SuggestionDayResultArray contém uma matriz de sugestões de reunião organizadas por data.
ms.openlocfilehash: 277d4cf71c31aba26cbff6f598eaa62769cae552
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457981"
---
# <a name="suggestiondayresultarray"></a><span data-ttu-id="a3d08-103">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="a3d08-103">SuggestionDayResultArray</span></span>

<span data-ttu-id="a3d08-104">O elemento **SuggestionDayResultArray** contém uma matriz de sugestões de reunião organizadas por data.</span><span class="sxs-lookup"><span data-stu-id="a3d08-104">The **SuggestionDayResultArray** element contains an array of meeting suggestions organized by date.</span></span> 
  
[<span data-ttu-id="a3d08-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a3d08-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="a3d08-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="a3d08-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="a3d08-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="a3d08-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
```xml
<SuggestionDayResultArray>
   <SuggestionDayResult>...</SuggestionDayResult>
</SuggestionDayResultArray>
```

 <span data-ttu-id="a3d08-108">**ArrayOfSuggestionDayResult**</span><span class="sxs-lookup"><span data-stu-id="a3d08-108">**ArrayOfSuggestionDayResult**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a3d08-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a3d08-109">Attributes and elements</span></span>

<span data-ttu-id="a3d08-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a3d08-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a3d08-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="a3d08-111">Attributes</span></span>

<span data-ttu-id="a3d08-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a3d08-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a3d08-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a3d08-113">Child elements</span></span>

|<span data-ttu-id="a3d08-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a3d08-114">**Element**</span></span>|<span data-ttu-id="a3d08-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a3d08-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3d08-116">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="a3d08-116">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="a3d08-117">Representa um único dia que contém horários de reunião sugeridos.</span><span class="sxs-lookup"><span data-stu-id="a3d08-117">Represents a single day that contains suggested meeting times.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a3d08-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a3d08-118">Parent elements</span></span>

|<span data-ttu-id="a3d08-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a3d08-119">**Element**</span></span>|<span data-ttu-id="a3d08-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a3d08-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3d08-121">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="a3d08-121">SuggestionsResponse</span></span>](suggestionsresponse.md) <br/> |<span data-ttu-id="a3d08-122">Contém informações de resposta e dados de sugestão para sugestões de reunião solicitadas</span><span class="sxs-lookup"><span data-stu-id="a3d08-122">Contains response information and suggestion data for requested meeting suggestions</span></span>  <br/> <span data-ttu-id="a3d08-123">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="a3d08-123">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a3d08-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="a3d08-124">Remarks</span></span>

<span data-ttu-id="a3d08-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="a3d08-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a3d08-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a3d08-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a3d08-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="a3d08-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a3d08-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a3d08-128">Schema Name</span></span>  <br/> |<span data-ttu-id="a3d08-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="a3d08-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a3d08-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a3d08-130">Validation File</span></span>  <br/> |<span data-ttu-id="a3d08-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a3d08-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a3d08-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a3d08-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="a3d08-133">False</span><span class="sxs-lookup"><span data-stu-id="a3d08-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a3d08-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="a3d08-134">See also</span></span>



[<span data-ttu-id="a3d08-135">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="a3d08-135">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="a3d08-136">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a3d08-136">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="a3d08-137">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="a3d08-137">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

