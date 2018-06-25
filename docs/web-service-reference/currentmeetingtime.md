---
title: CurrentMeetingTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CurrentMeetingTime
api_type:
- schema
ms.assetid: 1ff68154-24b5-465a-a31c-3d3bab0d491e
description: O elemento CurrentMeetingTime representa a hora de início de uma reunião que você deseja atualizar com o horário de uma reunião proposto pelo participante de uma reunião.
ms.openlocfilehash: 88adbe566270d759986e9b55afd4827c0513ca43
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751650"
---
# <a name="currentmeetingtime"></a><span data-ttu-id="0e98b-103">CurrentMeetingTime</span><span class="sxs-lookup"><span data-stu-id="0e98b-103">CurrentMeetingTime</span></span>

<span data-ttu-id="0e98b-104">O elemento **CurrentMeetingTime** representa a hora de início de uma reunião que você deseja atualizar com o horário de uma reunião proposto pelo participante de uma reunião.</span><span class="sxs-lookup"><span data-stu-id="0e98b-104">The **CurrentMeetingTime** element represents the start time of a meeting that you want to update with a meeting time proposed by a meeting attendee.</span></span> 
  
[<span data-ttu-id="0e98b-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="0e98b-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="0e98b-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="0e98b-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="0e98b-107">CurrentMeetingTime</span><span class="sxs-lookup"><span data-stu-id="0e98b-107">CurrentMeetingTime</span></span>](currentmeetingtime.md)
  
```xml
<CurrentMeetingTime>...</CurrentMeetingTime>
```

 <span data-ttu-id="0e98b-108">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="0e98b-108">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0e98b-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0e98b-109">Attributes and elements</span></span>

<span data-ttu-id="0e98b-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0e98b-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0e98b-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="0e98b-111">Attributes</span></span>

<span data-ttu-id="0e98b-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0e98b-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0e98b-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0e98b-113">Child elements</span></span>

<span data-ttu-id="0e98b-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0e98b-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0e98b-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0e98b-115">Parent elements</span></span>

|<span data-ttu-id="0e98b-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0e98b-116">**Element**</span></span>|<span data-ttu-id="0e98b-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0e98b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e98b-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="0e98b-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="0e98b-119">Contém as opções para a obtenção de informações de sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="0e98b-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="0e98b-120">Este é o XPath a este elemento:</span><span class="sxs-lookup"><span data-stu-id="0e98b-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0e98b-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="0e98b-121">Remarks</span></span>

<span data-ttu-id="0e98b-122">Este elemento não é necessário.</span><span class="sxs-lookup"><span data-stu-id="0e98b-122">This element is not required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="0e98b-123">O esquema que descreve este elemento está localizado no diretório /EWS/ do computador que está executando o MicrosoftExchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="0e98b-123">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="0e98b-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0e98b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0e98b-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="0e98b-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0e98b-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0e98b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="0e98b-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0e98b-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="0e98b-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0e98b-128">Validation File</span></span>  <br/> |<span data-ttu-id="0e98b-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0e98b-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0e98b-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0e98b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="0e98b-131">False</span><span class="sxs-lookup"><span data-stu-id="0e98b-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0e98b-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="0e98b-132">See also</span></span>



[<span data-ttu-id="0e98b-133">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="0e98b-133">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="0e98b-134">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="0e98b-134">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

