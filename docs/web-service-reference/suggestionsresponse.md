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
description: O elemento SuggestionsResponse contém dados de informações e sugestão de status de resposta para sugestões de reunião solicitada.
ms.openlocfilehash: 614b58a1df8e340c6be468ccddd3b37537d32591
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837674"
---
# <a name="suggestionsresponse"></a><span data-ttu-id="98d19-103">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="98d19-103">SuggestionsResponse</span></span>

<span data-ttu-id="98d19-104">O elemento **SuggestionsResponse** contém dados de informações e sugestão de status de resposta para sugestões de reunião solicitada.</span><span class="sxs-lookup"><span data-stu-id="98d19-104">The **SuggestionsResponse** element contains response status information and suggestion data for requested meeting suggestions.</span></span> 
  
[<span data-ttu-id="98d19-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="98d19-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="98d19-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="98d19-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
```xml
<SuggestionsResponse>
   <ResponseMessage>...</ResponseMessage>
   <SuggestionDayResultArray>...</SuggestionDayResultArray>
</SuggestionsResponse>
```

 <span data-ttu-id="98d19-107">**SuggestionsResponseType**</span><span class="sxs-lookup"><span data-stu-id="98d19-107">**SuggestionsResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="98d19-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="98d19-108">Attributes and elements</span></span>

<span data-ttu-id="98d19-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="98d19-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="98d19-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="98d19-110">Attributes</span></span>

<span data-ttu-id="98d19-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="98d19-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="98d19-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="98d19-112">Child elements</span></span>

|<span data-ttu-id="98d19-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="98d19-113">**Element**</span></span>|<span data-ttu-id="98d19-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="98d19-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="98d19-115">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="98d19-115">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="98d19-116">Fornece informações descritivas sobre o status de resposta.</span><span class="sxs-lookup"><span data-stu-id="98d19-116">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="98d19-117">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="98d19-117">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md) <br/> |<span data-ttu-id="98d19-118">Contém uma matriz de reunião sugestões organizados por data.</span><span class="sxs-lookup"><span data-stu-id="98d19-118">Contains an array of meeting suggestions organized by date.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="98d19-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="98d19-119">Parent elements</span></span>

|<span data-ttu-id="98d19-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="98d19-120">**Element**</span></span>|<span data-ttu-id="98d19-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="98d19-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="98d19-122">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="98d19-122">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md) <br/> |<span data-ttu-id="98d19-123">Contém informações de disponibilidade dos usuários solicitada.</span><span class="sxs-lookup"><span data-stu-id="98d19-123">Contains the requested users' availability information.</span></span>  <br/> <span data-ttu-id="98d19-124">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="98d19-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="98d19-125">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="98d19-125">Remarks</span></span>

<span data-ttu-id="98d19-126">Esse elemento não está incluído em uma resposta GetUserAvailability se [SuggestionsViewOptions](suggestionsviewoptions.md) não estiver definida na mensagem de solicitação GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="98d19-126">This element is not included in a GetUserAvailability response if [SuggestionsViewOptions](suggestionsviewoptions.md) is not set in the GetUserAvailability request message.</span></span> 
  
<span data-ttu-id="98d19-127">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="98d19-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="98d19-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="98d19-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="98d19-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="98d19-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="98d19-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="98d19-130">Schema Name</span></span>  <br/> |<span data-ttu-id="98d19-131">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="98d19-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="98d19-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="98d19-132">Validation File</span></span>  <br/> |<span data-ttu-id="98d19-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="98d19-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="98d19-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="98d19-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="98d19-135">False</span><span class="sxs-lookup"><span data-stu-id="98d19-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="98d19-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="98d19-136">See also</span></span>



[<span data-ttu-id="98d19-137">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="98d19-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="98d19-138">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="98d19-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="98d19-139">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="98d19-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

