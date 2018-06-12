---
title: BusyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BusyType
api_type:
- schema
ms.assetid: 26d4fae0-8c78-4705-b5e8-d6033712c41e
description: O elemento BusyType representa o status livre/ocupado definido para um evento de calendário.
ms.openlocfilehash: 6484bc70c6a05084e5d2bc1738b575fbebe4c132
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751345"
---
# <a name="busytype"></a><span data-ttu-id="76cd4-103">BusyType</span><span class="sxs-lookup"><span data-stu-id="76cd4-103">BusyType</span></span>

<span data-ttu-id="76cd4-104">O elemento **BusyType** representa o status livre/ocupado definido para um evento de calendário.</span><span class="sxs-lookup"><span data-stu-id="76cd4-104">The **BusyType** element represents the free/busy status set for a calendar event.</span></span> 
  
```xml
<BusyType>Free or Tentative or Busy or OOF or NoData</BusyType>
```

 <span data-ttu-id="76cd4-105">**BusyType**</span><span class="sxs-lookup"><span data-stu-id="76cd4-105">**BusyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="76cd4-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="76cd4-106">Attributes and elements</span></span>

<span data-ttu-id="76cd4-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="76cd4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="76cd4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="76cd4-108">Attributes</span></span>

<span data-ttu-id="76cd4-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="76cd4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="76cd4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="76cd4-110">Child elements</span></span>

<span data-ttu-id="76cd4-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="76cd4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="76cd4-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="76cd4-112">Parent elements</span></span>

|<span data-ttu-id="76cd4-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="76cd4-113">**Element**</span></span>|<span data-ttu-id="76cd4-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="76cd4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76cd4-115">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="76cd4-115">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md) <br/> |<span data-ttu-id="76cd4-116">Contém um usuário ou contato status livre/ocupado para uma janela de tempo que ocorre ao mesmo tempo como o tempo de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="76cd4-116">Contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time.</span></span>  <br/> <span data-ttu-id="76cd4-117">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="76cd4-117">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/IndividualAttendeeConflictData` <br/> |
|[<span data-ttu-id="76cd4-118">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="76cd4-118">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="76cd4-119">Representa uma ocorrência de item de calendário exclusivo.</span><span class="sxs-lookup"><span data-stu-id="76cd4-119">Represents a unique calendar item occurrence.</span></span>  <br/> <span data-ttu-id="76cd4-120">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="76cd4-120">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="76cd4-121">Text value</span><span class="sxs-lookup"><span data-stu-id="76cd4-121">Text value</span></span>

<span data-ttu-id="76cd4-122">Um valor de texto é necessário para esse elemento.</span><span class="sxs-lookup"><span data-stu-id="76cd4-122">A text value is required for this element.</span></span> <span data-ttu-id="76cd4-123">O valor é um tipo de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="76cd4-123">The value is a string type.</span></span> <span data-ttu-id="76cd4-124">Estes são os valores possíveis para o elemento [BusyType](busytype.md) :</span><span class="sxs-lookup"><span data-stu-id="76cd4-124">The following are the possible values for the [BusyType](busytype.md) element:</span></span> 
  
- <span data-ttu-id="76cd4-125">Disponível</span><span class="sxs-lookup"><span data-stu-id="76cd4-125">Free</span></span>
    
- <span data-ttu-id="76cd4-126">Provisório</span><span class="sxs-lookup"><span data-stu-id="76cd4-126">Tentative</span></span>
    
- <span data-ttu-id="76cd4-127">Ocupado</span><span class="sxs-lookup"><span data-stu-id="76cd4-127">Busy</span></span>
    
- <span data-ttu-id="76cd4-128">AUSÊNCIA TEMPORÁRIA</span><span class="sxs-lookup"><span data-stu-id="76cd4-128">OOF</span></span>
    
- <span data-ttu-id="76cd4-129">NoData</span><span class="sxs-lookup"><span data-stu-id="76cd4-129">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="76cd4-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="76cd4-130">Remarks</span></span>

<span data-ttu-id="76cd4-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="76cd4-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="76cd4-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="76cd4-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="76cd4-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="76cd4-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="76cd4-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="76cd4-134">Schema Name</span></span>  <br/> |<span data-ttu-id="76cd4-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="76cd4-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="76cd4-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="76cd4-136">Validation File</span></span>  <br/> |<span data-ttu-id="76cd4-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="76cd4-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="76cd4-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="76cd4-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="76cd4-139">False</span><span class="sxs-lookup"><span data-stu-id="76cd4-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="76cd4-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="76cd4-140">See also</span></span>



[<span data-ttu-id="76cd4-141">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="76cd4-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="76cd4-142">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="76cd4-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="76cd4-143">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="76cd4-143">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

