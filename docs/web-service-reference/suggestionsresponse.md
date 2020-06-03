---
title: SuggestionsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionsResponse
api_type:
- schema
ms.assetid: d25ca143-f80c-4458-b669-346fda29a5a7
description: O elemento SuggestionsResponse contém informações de status de resposta e dados de sugestão para sugestões de reunião solicitadas.
ms.openlocfilehash: cba344f3f97777580c2cc6d296f110f20b550063
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466651"
---
# <a name="suggestionsresponse"></a><span data-ttu-id="a2994-103">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="a2994-103">SuggestionsResponse</span></span>

<span data-ttu-id="a2994-104">O elemento **SuggestionsResponse** contém informações de status de resposta e dados de sugestão para sugestões de reunião solicitadas.</span><span class="sxs-lookup"><span data-stu-id="a2994-104">The **SuggestionsResponse** element contains response status information and suggestion data for requested meeting suggestions.</span></span> 
  
[<span data-ttu-id="a2994-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a2994-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="a2994-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="a2994-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
```xml
<SuggestionsResponse>
   <ResponseMessage>...</ResponseMessage>
   <SuggestionDayResultArray>...</SuggestionDayResultArray>
</SuggestionsResponse>
```

 <span data-ttu-id="a2994-107">**SuggestionsResponseType**</span><span class="sxs-lookup"><span data-stu-id="a2994-107">**SuggestionsResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a2994-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a2994-108">Attributes and elements</span></span>

<span data-ttu-id="a2994-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a2994-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2994-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="a2994-110">Attributes</span></span>

<span data-ttu-id="a2994-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a2994-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a2994-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a2994-112">Child elements</span></span>

|<span data-ttu-id="a2994-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a2994-113">**Element**</span></span>|<span data-ttu-id="a2994-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a2994-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2994-115">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a2994-115">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="a2994-116">Fornece informações descritivas sobre o status da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2994-116">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="a2994-117">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="a2994-117">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md) <br/> |<span data-ttu-id="a2994-118">Contém uma matriz de sugestões de reunião organizadas por data.</span><span class="sxs-lookup"><span data-stu-id="a2994-118">Contains an array of meeting suggestions organized by date.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a2994-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a2994-119">Parent elements</span></span>

|<span data-ttu-id="a2994-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a2994-120">**Element**</span></span>|<span data-ttu-id="a2994-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a2994-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2994-122">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a2994-122">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md) <br/> |<span data-ttu-id="a2994-123">Contém as informações de disponibilidade dos usuários solicitados.</span><span class="sxs-lookup"><span data-stu-id="a2994-123">Contains the requested users' availability information.</span></span>  <br/> <span data-ttu-id="a2994-124">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="a2994-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a2994-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="a2994-125">Remarks</span></span>

<span data-ttu-id="a2994-126">Esse elemento não é incluído em uma resposta GetUserAvailability se [SuggestionsViewOptions](suggestionsviewoptions.md) não for definido na mensagem de solicitação GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="a2994-126">This element is not included in a GetUserAvailability response if [SuggestionsViewOptions](suggestionsviewoptions.md) is not set in the GetUserAvailability request message.</span></span> 
  
<span data-ttu-id="a2994-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="a2994-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a2994-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a2994-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2994-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="a2994-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a2994-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a2994-130">Schema Name</span></span>  <br/> |<span data-ttu-id="a2994-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="a2994-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a2994-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a2994-132">Validation File</span></span>  <br/> |<span data-ttu-id="a2994-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a2994-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a2994-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a2994-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="a2994-135">False</span><span class="sxs-lookup"><span data-stu-id="a2994-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a2994-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="a2994-136">See also</span></span>



[<span data-ttu-id="a2994-137">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="a2994-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="a2994-138">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a2994-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="a2994-139">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="a2994-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

