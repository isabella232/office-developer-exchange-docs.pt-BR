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
description: O elemento MaximumResultsByDay especifica o número de horas de reunião sugeridas por um dia retornado na resposta.
ms.openlocfilehash: 46d5c35a83034b8b968901fbc4ee57d046b6c164
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468415"
---
# <a name="maximumresultsbyday"></a><span data-ttu-id="b26e2-103">MaximumResultsByDay</span><span class="sxs-lookup"><span data-stu-id="b26e2-103">MaximumResultsByDay</span></span>

<span data-ttu-id="b26e2-104">O elemento **MaximumResultsByDay** especifica o número de horas de reunião sugeridas por um dia retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="b26e2-104">The **MaximumResultsByDay** element specifies the number of suggested meeting times per a day returned in the response.</span></span> 
  
[<span data-ttu-id="b26e2-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="b26e2-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="b26e2-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="b26e2-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="b26e2-107">MaximumResultsByDay</span><span class="sxs-lookup"><span data-stu-id="b26e2-107">MaximumResultsByDay</span></span>](maximumresultsbyday.md)
  
```xml
<MaximumResultsByDay>...</MaximumResultsByDay>
```

<span data-ttu-id="b26e2-108">**int**</span><span class="sxs-lookup"><span data-stu-id="b26e2-108">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b26e2-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b26e2-109">Attributes and elements</span></span>

<span data-ttu-id="b26e2-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b26e2-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b26e2-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="b26e2-111">Attributes</span></span>

<span data-ttu-id="b26e2-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b26e2-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b26e2-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b26e2-113">Child elements</span></span>

<span data-ttu-id="b26e2-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b26e2-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b26e2-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b26e2-115">Parent elements</span></span>

|<span data-ttu-id="b26e2-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b26e2-116">**Element**</span></span>|<span data-ttu-id="b26e2-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b26e2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b26e2-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="b26e2-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="b26e2-119">Contém as opções para obter informações de sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="b26e2-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="b26e2-120">Este é o XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="b26e2-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b26e2-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="b26e2-121">Text value</span></span>

<span data-ttu-id="b26e2-122">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b26e2-122">A text value is required.</span></span> <span data-ttu-id="b26e2-123">O valor de texto representa um inteiro.</span><span class="sxs-lookup"><span data-stu-id="b26e2-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b26e2-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="b26e2-124">Remarks</span></span>

<span data-ttu-id="b26e2-125">Esse elemento é necessário se o elemento [SuggestionsViewOptions](suggestionsviewoptions.md) for usado.</span><span class="sxs-lookup"><span data-stu-id="b26e2-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="b26e2-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft® Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="b26e2-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="b26e2-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b26e2-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b26e2-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="b26e2-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b26e2-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b26e2-129">Schema Name</span></span>  <br/> |<span data-ttu-id="b26e2-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b26e2-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="b26e2-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b26e2-131">Validation File</span></span>  <br/> |<span data-ttu-id="b26e2-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b26e2-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b26e2-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b26e2-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="b26e2-134">False</span><span class="sxs-lookup"><span data-stu-id="b26e2-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b26e2-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="b26e2-135">See also</span></span>

- [<span data-ttu-id="b26e2-136">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="b26e2-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="b26e2-137">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="b26e2-137">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

