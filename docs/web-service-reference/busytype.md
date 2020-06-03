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
description: O elemento BusyType representa o status de disponibilidade definido para um evento de calendário.
ms.openlocfilehash: 7c2d18c21156a8603d3caeeb796a56c5d8afcba5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459080"
---
# <a name="busytype"></a><span data-ttu-id="0e17c-103">BusyType</span><span class="sxs-lookup"><span data-stu-id="0e17c-103">BusyType</span></span>

<span data-ttu-id="0e17c-104">O elemento **BusyType** representa o status de disponibilidade definido para um evento de calendário.</span><span class="sxs-lookup"><span data-stu-id="0e17c-104">The **BusyType** element represents the free/busy status set for a calendar event.</span></span> 
  
```xml
<BusyType>Free or Tentative or Busy or OOF or NoData</BusyType>
```

 <span data-ttu-id="0e17c-105">**BusyType**</span><span class="sxs-lookup"><span data-stu-id="0e17c-105">**BusyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0e17c-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="0e17c-106">Attributes and elements</span></span>

<span data-ttu-id="0e17c-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0e17c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0e17c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0e17c-108">Attributes</span></span>

<span data-ttu-id="0e17c-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0e17c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0e17c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0e17c-110">Child elements</span></span>

<span data-ttu-id="0e17c-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0e17c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0e17c-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0e17c-112">Parent elements</span></span>

|<span data-ttu-id="0e17c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0e17c-113">**Element**</span></span>|<span data-ttu-id="0e17c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0e17c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e17c-115">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="0e17c-115">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md) <br/> |<span data-ttu-id="0e17c-116">Contém o status de disponibilidade de um usuário ou contato para uma janela de tempo que ocorre ao mesmo tempo que o tempo de reunião sugerido.</span><span class="sxs-lookup"><span data-stu-id="0e17c-116">Contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time.</span></span>  <br/> <span data-ttu-id="0e17c-117">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="0e17c-117">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/IndividualAttendeeConflictData` <br/> |
|[<span data-ttu-id="0e17c-118">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="0e17c-118">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="0e17c-119">Representa uma ocorrência de item de calendário exclusivo.</span><span class="sxs-lookup"><span data-stu-id="0e17c-119">Represents a unique calendar item occurrence.</span></span>  <br/> <span data-ttu-id="0e17c-120">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="0e17c-120">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0e17c-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="0e17c-121">Text value</span></span>

<span data-ttu-id="0e17c-122">Um valor de texto é necessário para este elemento.</span><span class="sxs-lookup"><span data-stu-id="0e17c-122">A text value is required for this element.</span></span> <span data-ttu-id="0e17c-123">O valor é um tipo de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="0e17c-123">The value is a string type.</span></span> <span data-ttu-id="0e17c-124">Estes são os valores possíveis para o elemento [BusyType](busytype.md) :</span><span class="sxs-lookup"><span data-stu-id="0e17c-124">The following are the possible values for the [BusyType](busytype.md) element:</span></span> 
  
- <span data-ttu-id="0e17c-125">Disponível</span><span class="sxs-lookup"><span data-stu-id="0e17c-125">Free</span></span>
    
- <span data-ttu-id="0e17c-126">Provisória</span><span class="sxs-lookup"><span data-stu-id="0e17c-126">Tentative</span></span>
    
- <span data-ttu-id="0e17c-127">Ocupado</span><span class="sxs-lookup"><span data-stu-id="0e17c-127">Busy</span></span>
    
- <span data-ttu-id="0e17c-128">TEMPORÁRIA</span><span class="sxs-lookup"><span data-stu-id="0e17c-128">OOF</span></span>
    
- <span data-ttu-id="0e17c-129">NoData</span><span class="sxs-lookup"><span data-stu-id="0e17c-129">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="0e17c-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="0e17c-130">Remarks</span></span>

<span data-ttu-id="0e17c-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="0e17c-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0e17c-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="0e17c-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0e17c-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="0e17c-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0e17c-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0e17c-134">Schema Name</span></span>  <br/> |<span data-ttu-id="0e17c-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0e17c-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="0e17c-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0e17c-136">Validation File</span></span>  <br/> |<span data-ttu-id="0e17c-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0e17c-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0e17c-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0e17c-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="0e17c-139">False</span><span class="sxs-lookup"><span data-stu-id="0e17c-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0e17c-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="0e17c-140">See also</span></span>



[<span data-ttu-id="0e17c-141">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="0e17c-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="0e17c-142">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="0e17c-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="0e17c-143">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="0e17c-143">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

