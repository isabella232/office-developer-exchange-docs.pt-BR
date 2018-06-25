---
title: MaximumResultsByDay
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaximumResultsByDay
api_type:
- schema
ms.assetid: d581a12a-2b8e-4960-ae14-c8c4aa0b1849
description: O elemento MaximumResultsByDay Especifica o número de vezes que a reunião sugerido por um dia retornados na resposta.
ms.openlocfilehash: 69ab4e0b23f85e5b8786ba2dd934850cadc88f0e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824381"
---
# <a name="maximumresultsbyday"></a><span data-ttu-id="67b8f-103">MaximumResultsByDay</span><span class="sxs-lookup"><span data-stu-id="67b8f-103">MaximumResultsByDay</span></span>

<span data-ttu-id="67b8f-104">O elemento **MaximumResultsByDay** Especifica o número de vezes que a reunião sugerido por um dia retornados na resposta.</span><span class="sxs-lookup"><span data-stu-id="67b8f-104">The **MaximumResultsByDay** element specifies the number of suggested meeting times per a day returned in the response.</span></span> 
  
[<span data-ttu-id="67b8f-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="67b8f-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="67b8f-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="67b8f-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="67b8f-107">MaximumResultsByDay</span><span class="sxs-lookup"><span data-stu-id="67b8f-107">MaximumResultsByDay</span></span>](maximumresultsbyday.md)
  
```xml
<MaximumResultsByDay>...</MaximumResultsByDay>
```

<span data-ttu-id="67b8f-108">**int**</span><span class="sxs-lookup"><span data-stu-id="67b8f-108">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="67b8f-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="67b8f-109">Attributes and elements</span></span>

<span data-ttu-id="67b8f-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="67b8f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="67b8f-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="67b8f-111">Attributes</span></span>

<span data-ttu-id="67b8f-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="67b8f-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="67b8f-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="67b8f-113">Child elements</span></span>

<span data-ttu-id="67b8f-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="67b8f-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="67b8f-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="67b8f-115">Parent elements</span></span>

|<span data-ttu-id="67b8f-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="67b8f-116">**Element**</span></span>|<span data-ttu-id="67b8f-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="67b8f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="67b8f-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="67b8f-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="67b8f-119">Contém as opções para a obtenção de informações de sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="67b8f-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="67b8f-120">Este é o XPath a este elemento:</span><span class="sxs-lookup"><span data-stu-id="67b8f-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="67b8f-121">Text value</span><span class="sxs-lookup"><span data-stu-id="67b8f-121">Text value</span></span>

<span data-ttu-id="67b8f-122">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="67b8f-122">A text value is required.</span></span> <span data-ttu-id="67b8f-123">O valor de texto representa um número inteiro.</span><span class="sxs-lookup"><span data-stu-id="67b8f-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="67b8f-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="67b8f-124">Remarks</span></span>

<span data-ttu-id="67b8f-125">Esse elemento é necessário se o elemento [SuggestionsViewOptions](suggestionsviewoptions.md) é usado.</span><span class="sxs-lookup"><span data-stu-id="67b8f-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="67b8f-126">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft® Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="67b8f-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="67b8f-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="67b8f-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="67b8f-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="67b8f-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="67b8f-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="67b8f-129">Schema Name</span></span>  <br/> |<span data-ttu-id="67b8f-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="67b8f-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="67b8f-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="67b8f-131">Validation File</span></span>  <br/> |<span data-ttu-id="67b8f-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="67b8f-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="67b8f-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="67b8f-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="67b8f-134">False</span><span class="sxs-lookup"><span data-stu-id="67b8f-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="67b8f-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="67b8f-135">See also</span></span>

- [<span data-ttu-id="67b8f-136">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="67b8f-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="67b8f-137">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="67b8f-137">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

