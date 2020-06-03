---
title: EndTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndTime
api_type:
- schema
ms.assetid: 82e4ef4f-a557-4044-b9b7-d91622f4ac55
description: O elemento EndTime representa o final de um intervalo de tempo.
ms.openlocfilehash: 5a30b32ecfeafe582cd07dd662aacb0a960257c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462989"
---
# <a name="endtime"></a><span data-ttu-id="5c2a0-103">EndTime</span><span class="sxs-lookup"><span data-stu-id="5c2a0-103">EndTime</span></span>

<span data-ttu-id="5c2a0-104">O elemento **EndTime** representa o final de um intervalo de tempo.</span><span class="sxs-lookup"><span data-stu-id="5c2a0-104">The **EndTime** element represents the end of a time span.</span></span> 
  
```xml
<EndTime>dateTime</EndTime>
```

 <span data-ttu-id="5c2a0-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="5c2a0-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c2a0-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5c2a0-106">Attributes and elements</span></span>

<span data-ttu-id="5c2a0-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5c2a0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c2a0-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5c2a0-108">Attributes</span></span>

<span data-ttu-id="5c2a0-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5c2a0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5c2a0-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5c2a0-110">Child elements</span></span>

<span data-ttu-id="5c2a0-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5c2a0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5c2a0-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5c2a0-112">Parent elements</span></span>

|<span data-ttu-id="5c2a0-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5c2a0-113">**Element**</span></span>|<span data-ttu-id="5c2a0-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5c2a0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c2a0-115">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="5c2a0-115">TimeWindow</span></span>](timewindow.md) <br/> |<span data-ttu-id="5c2a0-116">Identifica o intervalo de tempo consultado para as informações de disponibilidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="5c2a0-116">Identifies the time span queried for the user availability information.</span></span><br/><br/> <span data-ttu-id="5c2a0-117">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="5c2a0-117">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[<span data-ttu-id="5c2a0-118">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="5c2a0-118">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="5c2a0-119">Identifica o período de tempo que é consultado para informações detalhadas sobre os horários de reunião sugeridos.</span><span class="sxs-lookup"><span data-stu-id="5c2a0-119">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span><br/><br/> <span data-ttu-id="5c2a0-120">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="5c2a0-120">The following is the XPath expression to this element:</span></span><br/><br/>  <span data-ttu-id="5c2a0-121">`/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow`.</span><span class="sxs-lookup"><span data-stu-id="5c2a0-121">`/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow`.</span></span>  <br/> |
|[<span data-ttu-id="5c2a0-122">Duração (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="5c2a0-122">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> | <span data-ttu-id="5c2a0-123">Especifica a duração para a qual o status de ausência temporária (OOF) é habilitado se o elemento [OofState](oofstate.md) estiver definido como **agendado**.</span><span class="sxs-lookup"><span data-stu-id="5c2a0-123">Specifies the duration for which the Out of Office (OOF) status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span>  <br/><br/>  <span data-ttu-id="5c2a0-124">A seguir estão as possíveis expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="5c2a0-124">The following are the possible XPath expressions to this element:</span></span><br/><br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[<span data-ttu-id="5c2a0-125">Ocorrência</span><span class="sxs-lookup"><span data-stu-id="5c2a0-125">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="5c2a0-126">Representa uma única ocorrência modificada de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="5c2a0-126">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5c2a0-127">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="5c2a0-127">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="5c2a0-128">Representa uma ocorrência de item de calendário exclusivo.</span><span class="sxs-lookup"><span data-stu-id="5c2a0-128">Represents a unique calendar item occurrence.</span></span> <span data-ttu-id="5c2a0-129">Isso é usado para consultas de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="5c2a0-129">This is used for Availability inquiries.</span></span> <span data-ttu-id="5c2a0-130">O elemento **EndTime** é necessário no elemento **CalendarEvent** .</span><span class="sxs-lookup"><span data-stu-id="5c2a0-130">The **EndTime** element is required in the **CalendarEvent** element.</span></span> <span data-ttu-id="5c2a0-131">O elemento **EndTime** no elemento **CalendarEvent** é exclusivo para o tipo **CalendarEvent** .</span><span class="sxs-lookup"><span data-stu-id="5c2a0-131">The **EndTime** element in the **CalendarEvent** element is unique to the **CalendarEvent** type.</span></span><br/><br/> <span data-ttu-id="5c2a0-132">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="5c2a0-132">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5c2a0-133">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="5c2a0-133">Text value</span></span>

<span data-ttu-id="5c2a0-134">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5c2a0-134">A text value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5c2a0-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="5c2a0-135">Remarks</span></span>

<span data-ttu-id="5c2a0-136">O elemento [StartTime](starttime.md) representa o início de um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="5c2a0-136">The [StartTime](starttime.md) element represents the beginning of a time span.</span></span> 
  
<span data-ttu-id="5c2a0-137">A hora de término representa o horário do cliente.</span><span class="sxs-lookup"><span data-stu-id="5c2a0-137">The end time represents the client's time.</span></span>
  
<span data-ttu-id="5c2a0-138">O esquema inclui muitos elementos [EndTime](endtime.md) .</span><span class="sxs-lookup"><span data-stu-id="5c2a0-138">The schema includes many [EndTime](endtime.md) elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5c2a0-139">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="5c2a0-139">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="5c2a0-140">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5c2a0-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c2a0-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="5c2a0-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5c2a0-142">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5c2a0-142">Schema Name</span></span>  <br/> |<span data-ttu-id="5c2a0-143">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5c2a0-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="5c2a0-144">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5c2a0-144">Validation File</span></span>  <br/> |<span data-ttu-id="5c2a0-145">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5c2a0-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5c2a0-146">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5c2a0-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="5c2a0-147">False</span><span class="sxs-lookup"><span data-stu-id="5c2a0-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5c2a0-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="5c2a0-148">See also</span></span>

- [<span data-ttu-id="5c2a0-149">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="5c2a0-149">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="5c2a0-150">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="5c2a0-150">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

