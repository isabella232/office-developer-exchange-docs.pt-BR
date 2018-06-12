---
title: StartTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartTime
api_type:
- schema
ms.assetid: 1fac7937-7a06-4d66-9d2a-14423bcb3b37
description: O elemento StartTime representa o início de um período de tempo.
ms.openlocfilehash: 4346797d755bb6e577e1cacb8bec656a7562bf1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825560"
---
# <a name="starttime"></a><span data-ttu-id="06e88-103">StartTime</span><span class="sxs-lookup"><span data-stu-id="06e88-103">StartTime</span></span>

<span data-ttu-id="06e88-104">O elemento **StartTime** representa o início de um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="06e88-104">The **StartTime** element represents the start of a time span.</span></span> 
  
```xml
<StartTime/
```

<span data-ttu-id="06e88-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="06e88-105">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="06e88-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="06e88-106">Attributes and elements</span></span>

<span data-ttu-id="06e88-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="06e88-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="06e88-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="06e88-108">Attributes</span></span>

<span data-ttu-id="06e88-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="06e88-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="06e88-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="06e88-110">Child elements</span></span>

<span data-ttu-id="06e88-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="06e88-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="06e88-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="06e88-112">Parent elements</span></span>

|<span data-ttu-id="06e88-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="06e88-113">**Element**</span></span>|<span data-ttu-id="06e88-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="06e88-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06e88-115">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="06e88-115">TimeWindow</span></span>](timewindow.md) <br/> |<span data-ttu-id="06e88-116">Identifica o intervalo de tempo consultado para as informações de disponibilidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="06e88-116">Identifies the time span queried for the user availability information.</span></span>  <br/><br/> <span data-ttu-id="06e88-117">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="06e88-117">The following is the XPath expression to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[<span data-ttu-id="06e88-118">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="06e88-118">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="06e88-119">Identifica o intervalo de tempo que está sendo consultado para obter informações detalhadas sobre reuniões sugeridas.</span><span class="sxs-lookup"><span data-stu-id="06e88-119">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span>  <br/><br/> <span data-ttu-id="06e88-120">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="06e88-120">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow` <br/> |
|[<span data-ttu-id="06e88-121">Duração (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="06e88-121">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> | <span data-ttu-id="06e88-122">Especifica a duração para o qual o status de fora do escritório (OOF) está habilitado se o elemento [OofState](oofstate.md) for definido como **agendado**.</span><span class="sxs-lookup"><span data-stu-id="06e88-122">Specifies the duration for which the Out of Office (OOF) status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span>  <br/><br/>  <span data-ttu-id="06e88-123">A seguir estão as expressões XPath possíveis para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="06e88-123">The following are the possible XPath expressions to this element:</span></span> <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[<span data-ttu-id="06e88-124">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="06e88-124">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="06e88-125">Representa uma ocorrência de item de calendário exclusivo.</span><span class="sxs-lookup"><span data-stu-id="06e88-125">Represents a unique calendar item occurrence.</span></span> <span data-ttu-id="06e88-126">Isso é usado para fazer consultas sobre a disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="06e88-126">This is used for Availability inquiries.</span></span> <span data-ttu-id="06e88-127">O elemento **StartTime** é necessária no elemento **CalendarEvent** .</span><span class="sxs-lookup"><span data-stu-id="06e88-127">The **StartTime** element is required in the **CalendarEvent** element.</span></span> <span data-ttu-id="06e88-128">O elemento **StartTime** no elemento **CalendarEvent** é exclusivo para o tipo de **CalendarEvent** , embora ele contém os mesmos valores de faceta que contêm os elementos **StartTime** no tipo de **duração** .</span><span class="sxs-lookup"><span data-stu-id="06e88-128">The **StartTime** element in the **CalendarEvent** element is unique to the **CalendarEvent** type although it contains the same facet values that the **StartTime** elements in the **Duration** type contain.</span></span>  <br/><br/> <span data-ttu-id="06e88-129">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="06e88-129">The following is the XPath expression to this element:</span></span>  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="06e88-130">Text value</span><span class="sxs-lookup"><span data-stu-id="06e88-130">Text value</span></span>

<span data-ttu-id="06e88-131">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="06e88-131">A text value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="06e88-132">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="06e88-132">Remarks</span></span>

<span data-ttu-id="06e88-133">O elemento [EndTime](endtime.md) representa o fim do intervalo de tempo.</span><span class="sxs-lookup"><span data-stu-id="06e88-133">The [EndTime](endtime.md) element represents the end of the time span.</span></span> 
  
<span data-ttu-id="06e88-134">O esquema inclui muitos elementos [StartTime](starttime.md) .</span><span class="sxs-lookup"><span data-stu-id="06e88-134">The schema includes many [StartTime](starttime.md) elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="06e88-135">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="06e88-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="06e88-136">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="06e88-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="06e88-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="06e88-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="06e88-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="06e88-138">Schema Name</span></span>  <br/> |<span data-ttu-id="06e88-139">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="06e88-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="06e88-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="06e88-140">Validation File</span></span>  <br/> |<span data-ttu-id="06e88-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="06e88-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="06e88-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="06e88-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="06e88-143">False</span><span class="sxs-lookup"><span data-stu-id="06e88-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="06e88-144">Ver também</span><span class="sxs-lookup"><span data-stu-id="06e88-144">See also</span></span>

- [<span data-ttu-id="06e88-145">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="06e88-145">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="06e88-146">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="06e88-146">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

