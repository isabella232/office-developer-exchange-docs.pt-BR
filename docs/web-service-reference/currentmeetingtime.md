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
description: O elemento CurrentMeetingTime representa a hora de início de uma reunião que você deseja atualizar com um horário de reunião proposto por um participante da reunião.
ms.openlocfilehash: e79616fd735cbf6410e85450bd75c1276923f171
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458772"
---
# <a name="currentmeetingtime"></a><span data-ttu-id="1a576-103">CurrentMeetingTime</span><span class="sxs-lookup"><span data-stu-id="1a576-103">CurrentMeetingTime</span></span>

<span data-ttu-id="1a576-104">O elemento **CurrentMeetingTime** representa a hora de início de uma reunião que você deseja atualizar com um horário de reunião proposto por um participante da reunião.</span><span class="sxs-lookup"><span data-stu-id="1a576-104">The **CurrentMeetingTime** element represents the start time of a meeting that you want to update with a meeting time proposed by a meeting attendee.</span></span> 
  
[<span data-ttu-id="1a576-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="1a576-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="1a576-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="1a576-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="1a576-107">CurrentMeetingTime</span><span class="sxs-lookup"><span data-stu-id="1a576-107">CurrentMeetingTime</span></span>](currentmeetingtime.md)
  
```xml
<CurrentMeetingTime>...</CurrentMeetingTime>
```

 <span data-ttu-id="1a576-108">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="1a576-108">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1a576-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="1a576-109">Attributes and elements</span></span>

<span data-ttu-id="1a576-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1a576-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a576-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="1a576-111">Attributes</span></span>

<span data-ttu-id="1a576-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1a576-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1a576-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1a576-113">Child elements</span></span>

<span data-ttu-id="1a576-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1a576-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1a576-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1a576-115">Parent elements</span></span>

|<span data-ttu-id="1a576-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1a576-116">**Element**</span></span>|<span data-ttu-id="1a576-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1a576-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a576-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="1a576-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="1a576-119">Contém as opções para obter informações de sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="1a576-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="1a576-120">Este é o XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="1a576-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1a576-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="1a576-121">Remarks</span></span>

<span data-ttu-id="1a576-122">Esse elemento não é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a576-122">This element is not required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="1a576-123">O esquema que descreve este elemento está localizado no diretório/EWS/do computador que está executando o MicrosoftExchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="1a576-123">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="1a576-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="1a576-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1a576-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="1a576-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1a576-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1a576-126">Schema Name</span></span>  <br/> |<span data-ttu-id="1a576-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="1a576-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="1a576-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1a576-128">Validation File</span></span>  <br/> |<span data-ttu-id="1a576-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1a576-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1a576-130">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1a576-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="1a576-131">False</span><span class="sxs-lookup"><span data-stu-id="1a576-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1a576-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="1a576-132">See also</span></span>



[<span data-ttu-id="1a576-133">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="1a576-133">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="1a576-134">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="1a576-134">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

