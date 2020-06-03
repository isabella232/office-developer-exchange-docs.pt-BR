---
title: DetailedSuggestionsWindow
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DetailedSuggestionsWindow
api_type:
- schema
ms.assetid: 7b348d63-6a7d-45f4-9562-5c42243d63a5
description: O elemento DetailedSuggestionsWindow identifica o intervalo de tempo que é consultado para obter informações detalhadas sobre horários de reunião sugeridos.
ms.openlocfilehash: 45d582f2642c0e3d8f6330b09946230c8842618d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467841"
---
# <a name="detailedsuggestionswindow"></a><span data-ttu-id="ca265-103">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="ca265-103">DetailedSuggestionsWindow</span></span>

<span data-ttu-id="ca265-104">O elemento **DetailedSuggestionsWindow** identifica o intervalo de tempo que é consultado para obter informações detalhadas sobre horários de reunião sugeridos.</span><span class="sxs-lookup"><span data-stu-id="ca265-104">The **DetailedSuggestionsWindow** element identifies the time span that is queried for detailed information about suggested meeting times.</span></span> 
  
- [<span data-ttu-id="ca265-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="ca265-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) 
- [<span data-ttu-id="ca265-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="ca265-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) 
- [<span data-ttu-id="ca265-107">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="ca265-107">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md)
  
```xml
<DetailedSuggestionsWindow>
   <StartTime>...</StartTime>
   <EndTime>...</EndTime>
</DetailedSuggestionsWindow>
```

 <span data-ttu-id="ca265-108">**Duration**</span><span class="sxs-lookup"><span data-stu-id="ca265-108">**Duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ca265-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ca265-109">Attributes and elements</span></span>

<span data-ttu-id="ca265-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ca265-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ca265-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="ca265-111">Attributes</span></span>

<span data-ttu-id="ca265-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ca265-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ca265-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ca265-113">Child elements</span></span>

|<span data-ttu-id="ca265-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ca265-114">**Element**</span></span>|<span data-ttu-id="ca265-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ca265-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ca265-116">StartTime</span><span class="sxs-lookup"><span data-stu-id="ca265-116">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="ca265-117">Representa o início do período de tempo consultado para obter informações detalhadas sobre os horários de reunião sugeridos.</span><span class="sxs-lookup"><span data-stu-id="ca265-117">Represents the start of the time span queried for detailed information about suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="ca265-118">EndTime</span><span class="sxs-lookup"><span data-stu-id="ca265-118">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="ca265-119">Representa o fim do período de tempo consultado para obter informações detalhadas sobre os horários de reunião sugeridos.</span><span class="sxs-lookup"><span data-stu-id="ca265-119">Represents the end of the time span queried for detailed information about suggested meeting times.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ca265-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ca265-120">Parent elements</span></span>

|<span data-ttu-id="ca265-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ca265-121">**Element**</span></span>|<span data-ttu-id="ca265-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ca265-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ca265-123">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="ca265-123">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="ca265-124">Contém as opções para obter informações de sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="ca265-124">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="ca265-125">Este é o XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="ca265-125">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ca265-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="ca265-126">Remarks</span></span>

<span data-ttu-id="ca265-127">Esse elemento não é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca265-127">This element is not required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="ca265-128">O esquema que descreve este elemento está localizado no diretório/EWS/do computador que está executando o MicrosoftExchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="ca265-128">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="ca265-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ca265-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ca265-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="ca265-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ca265-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ca265-131">Schema Name</span></span>  <br/> |<span data-ttu-id="ca265-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ca265-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="ca265-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ca265-133">Validation File</span></span>  <br/> |<span data-ttu-id="ca265-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ca265-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ca265-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ca265-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="ca265-136">False</span><span class="sxs-lookup"><span data-stu-id="ca265-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ca265-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="ca265-137">See also</span></span>

- [<span data-ttu-id="ca265-138">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="ca265-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="ca265-139">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="ca265-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

