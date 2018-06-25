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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751345"
---
# <a name="busytype"></a><span data-ttu-id="b64b1-103">BusyType</span><span class="sxs-lookup"><span data-stu-id="b64b1-103">BusyType</span></span>

<span data-ttu-id="b64b1-104">O elemento **BusyType** representa o status livre/ocupado definido para um evento de calendário.</span><span class="sxs-lookup"><span data-stu-id="b64b1-104">The **BusyType** element represents the free/busy status set for a calendar event.</span></span> 
  
```xml
<BusyType>Free or Tentative or Busy or OOF or NoData</BusyType>
```

 <span data-ttu-id="b64b1-105">**BusyType**</span><span class="sxs-lookup"><span data-stu-id="b64b1-105">**BusyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b64b1-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b64b1-106">Attributes and elements</span></span>

<span data-ttu-id="b64b1-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b64b1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b64b1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b64b1-108">Attributes</span></span>

<span data-ttu-id="b64b1-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b64b1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b64b1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b64b1-110">Child elements</span></span>

<span data-ttu-id="b64b1-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b64b1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b64b1-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b64b1-112">Parent elements</span></span>

|<span data-ttu-id="b64b1-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b64b1-113">**Element**</span></span>|<span data-ttu-id="b64b1-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b64b1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b64b1-115">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="b64b1-115">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md) <br/> |<span data-ttu-id="b64b1-116">Contém um usuário ou contato status livre/ocupado para uma janela de tempo que ocorre ao mesmo tempo como o tempo de reunião sugeridas.</span><span class="sxs-lookup"><span data-stu-id="b64b1-116">Contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time.</span></span>  <br/> <span data-ttu-id="b64b1-117">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="b64b1-117">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/IndividualAttendeeConflictData` <br/> |
|[<span data-ttu-id="b64b1-118">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="b64b1-118">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="b64b1-119">Representa uma ocorrência de item de calendário exclusivo.</span><span class="sxs-lookup"><span data-stu-id="b64b1-119">Represents a unique calendar item occurrence.</span></span>  <br/> <span data-ttu-id="b64b1-120">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="b64b1-120">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b64b1-121">Text value</span><span class="sxs-lookup"><span data-stu-id="b64b1-121">Text value</span></span>

<span data-ttu-id="b64b1-122">Um valor de texto é necessário para esse elemento.</span><span class="sxs-lookup"><span data-stu-id="b64b1-122">A text value is required for this element.</span></span> <span data-ttu-id="b64b1-123">O valor é um tipo de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="b64b1-123">The value is a string type.</span></span> <span data-ttu-id="b64b1-124">Estes são os valores possíveis para o elemento [BusyType](busytype.md) :</span><span class="sxs-lookup"><span data-stu-id="b64b1-124">The following are the possible values for the [BusyType](busytype.md) element:</span></span> 
  
- <span data-ttu-id="b64b1-125">Disponível</span><span class="sxs-lookup"><span data-stu-id="b64b1-125">Free</span></span>
    
- <span data-ttu-id="b64b1-126">Provisório</span><span class="sxs-lookup"><span data-stu-id="b64b1-126">Tentative</span></span>
    
- <span data-ttu-id="b64b1-127">Ocupado</span><span class="sxs-lookup"><span data-stu-id="b64b1-127">Busy</span></span>
    
- <span data-ttu-id="b64b1-128">AUSÊNCIA TEMPORÁRIA</span><span class="sxs-lookup"><span data-stu-id="b64b1-128">OOF</span></span>
    
- <span data-ttu-id="b64b1-129">NoData</span><span class="sxs-lookup"><span data-stu-id="b64b1-129">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="b64b1-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="b64b1-130">Remarks</span></span>

<span data-ttu-id="b64b1-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="b64b1-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b64b1-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b64b1-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b64b1-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="b64b1-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b64b1-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b64b1-134">Schema Name</span></span>  <br/> |<span data-ttu-id="b64b1-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b64b1-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="b64b1-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b64b1-136">Validation File</span></span>  <br/> |<span data-ttu-id="b64b1-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b64b1-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b64b1-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b64b1-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="b64b1-139">False</span><span class="sxs-lookup"><span data-stu-id="b64b1-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b64b1-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="b64b1-140">See also</span></span>



[<span data-ttu-id="b64b1-141">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="b64b1-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="b64b1-142">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="b64b1-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="b64b1-143">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="b64b1-143">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

