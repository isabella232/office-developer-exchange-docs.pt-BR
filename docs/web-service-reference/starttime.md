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
ms.openlocfilehash: 16bee698b65dc512a709e2af9ddfe8629347fee3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458562"
---
# <a name="starttime"></a><span data-ttu-id="10e71-103">StartTime</span><span class="sxs-lookup"><span data-stu-id="10e71-103">StartTime</span></span>

<span data-ttu-id="10e71-104">O elemento **StartTime** representa o início de um período de tempo.</span><span class="sxs-lookup"><span data-stu-id="10e71-104">The **StartTime** element represents the start of a time span.</span></span> 
  
```xml
<StartTime/
```

<span data-ttu-id="10e71-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="10e71-105">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="10e71-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="10e71-106">Attributes and elements</span></span>

<span data-ttu-id="10e71-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="10e71-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="10e71-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="10e71-108">Attributes</span></span>

<span data-ttu-id="10e71-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="10e71-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="10e71-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="10e71-110">Child elements</span></span>

<span data-ttu-id="10e71-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="10e71-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="10e71-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="10e71-112">Parent elements</span></span>

|<span data-ttu-id="10e71-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="10e71-113">**Element**</span></span>|<span data-ttu-id="10e71-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="10e71-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="10e71-115">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="10e71-115">TimeWindow</span></span>](timewindow.md) <br/> |<span data-ttu-id="10e71-116">Identifica o intervalo de tempo consultado para as informações de disponibilidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="10e71-116">Identifies the time span queried for the user availability information.</span></span>  <br/><br/> <span data-ttu-id="10e71-117">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="10e71-117">The following is the XPath expression to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[<span data-ttu-id="10e71-118">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="10e71-118">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="10e71-119">Identifica o período de tempo que é consultado para informações detalhadas sobre os horários de reunião sugeridos.</span><span class="sxs-lookup"><span data-stu-id="10e71-119">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span>  <br/><br/> <span data-ttu-id="10e71-120">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="10e71-120">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow` <br/> |
|[<span data-ttu-id="10e71-121">Duração (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="10e71-121">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> | <span data-ttu-id="10e71-122">Especifica a duração para a qual o status de ausência temporária (OOF) é habilitado se o elemento [OofState](oofstate.md) estiver definido como **agendado**.</span><span class="sxs-lookup"><span data-stu-id="10e71-122">Specifies the duration for which the Out of Office (OOF) status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span>  <br/><br/>  <span data-ttu-id="10e71-123">A seguir estão as possíveis expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="10e71-123">The following are the possible XPath expressions to this element:</span></span> <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[<span data-ttu-id="10e71-124">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="10e71-124">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="10e71-125">Representa uma ocorrência de item de calendário exclusivo.</span><span class="sxs-lookup"><span data-stu-id="10e71-125">Represents a unique calendar item occurrence.</span></span> <span data-ttu-id="10e71-126">Isso é usado para consultas de disponibilidade.</span><span class="sxs-lookup"><span data-stu-id="10e71-126">This is used for Availability inquiries.</span></span> <span data-ttu-id="10e71-127">O elemento **StartTime** é necessário no elemento **CalendarEvent** .</span><span class="sxs-lookup"><span data-stu-id="10e71-127">The **StartTime** element is required in the **CalendarEvent** element.</span></span> <span data-ttu-id="10e71-128">O elemento **StartTime** no elemento **CalendarEvent** é exclusivo para o tipo **CalendarEvent** , embora contenha os mesmos valores de faceta que os elementos **StartTime** no tipo de **duração** contêm.</span><span class="sxs-lookup"><span data-stu-id="10e71-128">The **StartTime** element in the **CalendarEvent** element is unique to the **CalendarEvent** type although it contains the same facet values that the **StartTime** elements in the **Duration** type contain.</span></span>  <br/><br/> <span data-ttu-id="10e71-129">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="10e71-129">The following is the XPath expression to this element:</span></span>  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="10e71-130">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="10e71-130">Text value</span></span>

<span data-ttu-id="10e71-131">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="10e71-131">A text value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="10e71-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="10e71-132">Remarks</span></span>

<span data-ttu-id="10e71-133">O elemento [EndTime](endtime.md) representa o final do intervalo de tempo.</span><span class="sxs-lookup"><span data-stu-id="10e71-133">The [EndTime](endtime.md) element represents the end of the time span.</span></span> 
  
<span data-ttu-id="10e71-134">O esquema inclui muitos elementos [StartTime](starttime.md) .</span><span class="sxs-lookup"><span data-stu-id="10e71-134">The schema includes many [StartTime](starttime.md) elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="10e71-135">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="10e71-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="10e71-136">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="10e71-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="10e71-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="10e71-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="10e71-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="10e71-138">Schema Name</span></span>  <br/> |<span data-ttu-id="10e71-139">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="10e71-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="10e71-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="10e71-140">Validation File</span></span>  <br/> |<span data-ttu-id="10e71-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="10e71-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="10e71-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="10e71-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="10e71-143">False</span><span class="sxs-lookup"><span data-stu-id="10e71-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="10e71-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="10e71-144">See also</span></span>

- [<span data-ttu-id="10e71-145">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="10e71-145">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="10e71-146">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="10e71-146">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

