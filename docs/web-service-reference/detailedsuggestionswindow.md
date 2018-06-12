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
description: O elemento DetailedSuggestionsWindow identifica o intervalo de tempo que está sendo consultado para obter informações detalhadas sobre reuniões sugeridas.
ms.openlocfilehash: 8a3af0178d0c96b50f4dd641716a9f7a7be8f7a2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751792"
---
# <a name="detailedsuggestionswindow"></a><span data-ttu-id="7da42-103">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="7da42-103">DetailedSuggestionsWindow</span></span>

<span data-ttu-id="7da42-104">O elemento **DetailedSuggestionsWindow** identifica o intervalo de tempo que está sendo consultado para obter informações detalhadas sobre reuniões sugeridas.</span><span class="sxs-lookup"><span data-stu-id="7da42-104">The **DetailedSuggestionsWindow** element identifies the time span that is queried for detailed information about suggested meeting times.</span></span> 
  
- [<span data-ttu-id="7da42-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="7da42-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) 
- [<span data-ttu-id="7da42-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="7da42-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) 
- [<span data-ttu-id="7da42-107">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="7da42-107">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md)
  
```xml
<DetailedSuggestionsWindow>
   <StartTime>...</StartTime>
   <EndTime>...</EndTime>
</DetailedSuggestionsWindow>
```

 <span data-ttu-id="7da42-108">**Duração**</span><span class="sxs-lookup"><span data-stu-id="7da42-108">**Duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7da42-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7da42-109">Attributes and elements</span></span>

<span data-ttu-id="7da42-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7da42-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7da42-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="7da42-111">Attributes</span></span>

<span data-ttu-id="7da42-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7da42-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7da42-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7da42-113">Child elements</span></span>

|<span data-ttu-id="7da42-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7da42-114">**Element**</span></span>|<span data-ttu-id="7da42-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7da42-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7da42-116">StartTime</span><span class="sxs-lookup"><span data-stu-id="7da42-116">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="7da42-117">Representa o início do intervalo de tempo consultado para obter informações detalhadas sobre reuniões sugeridas.</span><span class="sxs-lookup"><span data-stu-id="7da42-117">Represents the start of the time span queried for detailed information about suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="7da42-118">EndTime</span><span class="sxs-lookup"><span data-stu-id="7da42-118">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="7da42-119">Representa o fim do intervalo de tempo consultado para obter informações detalhadas sobre reuniões sugeridas.</span><span class="sxs-lookup"><span data-stu-id="7da42-119">Represents the end of the time span queried for detailed information about suggested meeting times.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7da42-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7da42-120">Parent elements</span></span>

|<span data-ttu-id="7da42-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7da42-121">**Element**</span></span>|<span data-ttu-id="7da42-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7da42-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7da42-123">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="7da42-123">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="7da42-124">Contém as opções para a obtenção de informações de sugestão de reunião.</span><span class="sxs-lookup"><span data-stu-id="7da42-124">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="7da42-125">Este é o XPath a este elemento:</span><span class="sxs-lookup"><span data-stu-id="7da42-125">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7da42-126">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="7da42-126">Remarks</span></span>

<span data-ttu-id="7da42-127">Este elemento não é necessário.</span><span class="sxs-lookup"><span data-stu-id="7da42-127">This element is not required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="7da42-128">O esquema que descreve este elemento está localizado no diretório /EWS/ do computador que está executando o MicrosoftExchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="7da42-128">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="7da42-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7da42-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7da42-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="7da42-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7da42-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7da42-131">Schema Name</span></span>  <br/> |<span data-ttu-id="7da42-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7da42-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="7da42-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7da42-133">Validation File</span></span>  <br/> |<span data-ttu-id="7da42-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7da42-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7da42-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7da42-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="7da42-136">False</span><span class="sxs-lookup"><span data-stu-id="7da42-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7da42-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="7da42-137">See also</span></span>

- [<span data-ttu-id="7da42-138">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="7da42-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="7da42-139">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="7da42-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

