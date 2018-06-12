---
title: MeetingDurationInMinutes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingDurationInMinutes
api_type:
- schema
ms.assetid: bb86b275-9c29-4daf-8196-8d505b87a4f4
description: O elemento MeetingDurationInMinutes Especifica a duração da reunião a ser sugerido.
ms.openlocfilehash: 2ff60b69fb352c2ac7316f1ca231bb04da67ead2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824433"
---
# <a name="meetingdurationinminutes"></a><span data-ttu-id="fd7ac-103">MeetingDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="fd7ac-103">MeetingDurationInMinutes</span></span>

<span data-ttu-id="fd7ac-104">O elemento **MeetingDurationInMinutes** Especifica a duração da reunião a ser sugerido.</span><span class="sxs-lookup"><span data-stu-id="fd7ac-104">The **MeetingDurationInMinutes** element specifies the duration of the meeting to be suggested.</span></span> 
  
[<span data-ttu-id="fd7ac-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="fd7ac-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="fd7ac-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="fd7ac-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="fd7ac-107">MeetingDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="fd7ac-107">MeetingDurationInMinutes</span></span>](meetingdurationinminutes.md)
  
```xml
<MeetingDurationInMinutes>...</MeetingDurationInMinutes>
```

 <span data-ttu-id="fd7ac-108">**int**</span><span class="sxs-lookup"><span data-stu-id="fd7ac-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fd7ac-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="fd7ac-109">Attributes and elements</span></span>

<span data-ttu-id="fd7ac-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fd7ac-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd7ac-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="fd7ac-111">Attributes</span></span>

<span data-ttu-id="fd7ac-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fd7ac-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fd7ac-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fd7ac-113">Child elements</span></span>

<span data-ttu-id="fd7ac-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fd7ac-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fd7ac-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fd7ac-115">Parent elements</span></span>

|<span data-ttu-id="fd7ac-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fd7ac-116">**Element**</span></span>|<span data-ttu-id="fd7ac-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fd7ac-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fd7ac-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="fd7ac-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="fd7ac-119">Contém as opções para a obtenção de informações de sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="fd7ac-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="fd7ac-120">Este é o XPath a este elemento:</span><span class="sxs-lookup"><span data-stu-id="fd7ac-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fd7ac-121">Text value</span><span class="sxs-lookup"><span data-stu-id="fd7ac-121">Text value</span></span>

<span data-ttu-id="fd7ac-122">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="fd7ac-122">A text value is required.</span></span> <span data-ttu-id="fd7ac-123">O valor de texto representa um número inteiro.</span><span class="sxs-lookup"><span data-stu-id="fd7ac-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fd7ac-124">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="fd7ac-124">Remarks</span></span>

<span data-ttu-id="fd7ac-125">Esse elemento é necessário se o elemento [SuggestionsViewOptions](suggestionsviewoptions.md) é usado.</span><span class="sxs-lookup"><span data-stu-id="fd7ac-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="fd7ac-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="fd7ac-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="fd7ac-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="fd7ac-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd7ac-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="fd7ac-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fd7ac-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fd7ac-129">Schema Name</span></span>  <br/> |<span data-ttu-id="fd7ac-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="fd7ac-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="fd7ac-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fd7ac-131">Validation File</span></span>  <br/> |<span data-ttu-id="fd7ac-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fd7ac-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fd7ac-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="fd7ac-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="fd7ac-134">False</span><span class="sxs-lookup"><span data-stu-id="fd7ac-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fd7ac-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="fd7ac-135">See also</span></span>



[<span data-ttu-id="fd7ac-136">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="fd7ac-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="fd7ac-137">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="fd7ac-137">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

