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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824433"
---
# <a name="meetingdurationinminutes"></a><span data-ttu-id="ed1e3-103">MeetingDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="ed1e3-103">MeetingDurationInMinutes</span></span>

<span data-ttu-id="ed1e3-104">O elemento **MeetingDurationInMinutes** Especifica a duração da reunião a ser sugerido.</span><span class="sxs-lookup"><span data-stu-id="ed1e3-104">The **MeetingDurationInMinutes** element specifies the duration of the meeting to be suggested.</span></span> 
  
[<span data-ttu-id="ed1e3-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="ed1e3-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="ed1e3-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="ed1e3-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="ed1e3-107">MeetingDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="ed1e3-107">MeetingDurationInMinutes</span></span>](meetingdurationinminutes.md)
  
```xml
<MeetingDurationInMinutes>...</MeetingDurationInMinutes>
```

 <span data-ttu-id="ed1e3-108">**int**</span><span class="sxs-lookup"><span data-stu-id="ed1e3-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ed1e3-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ed1e3-109">Attributes and elements</span></span>

<span data-ttu-id="ed1e3-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ed1e3-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ed1e3-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="ed1e3-111">Attributes</span></span>

<span data-ttu-id="ed1e3-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ed1e3-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ed1e3-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ed1e3-113">Child elements</span></span>

<span data-ttu-id="ed1e3-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ed1e3-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ed1e3-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ed1e3-115">Parent elements</span></span>

|<span data-ttu-id="ed1e3-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ed1e3-116">**Element**</span></span>|<span data-ttu-id="ed1e3-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ed1e3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed1e3-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="ed1e3-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="ed1e3-119">Contém as opções para a obtenção de informações de sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="ed1e3-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="ed1e3-120">Este é o XPath a este elemento:</span><span class="sxs-lookup"><span data-stu-id="ed1e3-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ed1e3-121">Text value</span><span class="sxs-lookup"><span data-stu-id="ed1e3-121">Text value</span></span>

<span data-ttu-id="ed1e3-122">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="ed1e3-122">A text value is required.</span></span> <span data-ttu-id="ed1e3-123">O valor de texto representa um número inteiro.</span><span class="sxs-lookup"><span data-stu-id="ed1e3-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ed1e3-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="ed1e3-124">Remarks</span></span>

<span data-ttu-id="ed1e3-125">Esse elemento é necessário se o elemento [SuggestionsViewOptions](suggestionsviewoptions.md) é usado.</span><span class="sxs-lookup"><span data-stu-id="ed1e3-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="ed1e3-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="ed1e3-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="ed1e3-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ed1e3-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ed1e3-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="ed1e3-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ed1e3-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ed1e3-129">Schema Name</span></span>  <br/> |<span data-ttu-id="ed1e3-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ed1e3-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="ed1e3-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ed1e3-131">Validation File</span></span>  <br/> |<span data-ttu-id="ed1e3-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ed1e3-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ed1e3-133">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ed1e3-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="ed1e3-134">False</span><span class="sxs-lookup"><span data-stu-id="ed1e3-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ed1e3-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="ed1e3-135">See also</span></span>



[<span data-ttu-id="ed1e3-136">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="ed1e3-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="ed1e3-137">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="ed1e3-137">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

