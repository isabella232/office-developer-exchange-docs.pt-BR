---
title: Assunto (CalendarEventDetails)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Subject
api_type:
- schema
ms.assetid: 05e955b5-8e90-4043-b06b-6ce523eaed9b
description: Elemento Subject representa o assunto de um item de calendário.
ms.openlocfilehash: 5303a7568e017999f2be69c50588832748b5668a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825610"
---
# <a name="subject-calendareventdetails"></a><span data-ttu-id="3fa46-103">Assunto (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="3fa46-103">Subject (CalendarEventDetails)</span></span>

<span data-ttu-id="3fa46-104">Elemento **Subject** representa o assunto de um item de calendário.</span><span class="sxs-lookup"><span data-stu-id="3fa46-104">The **Subject** element represents the subject of a calendar item.</span></span> 
  
[<span data-ttu-id="3fa46-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="3fa46-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="3fa46-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="3fa46-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="3fa46-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="3fa46-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="3fa46-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="3fa46-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="3fa46-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="3fa46-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="3fa46-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="3fa46-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="3fa46-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="3fa46-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="3fa46-112">Assunto (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="3fa46-112">Subject (CalendarEventDetails)</span></span>](subject-calendareventdetails.md)
  
```xml
<Subject/>
```

 <span data-ttu-id="3fa46-113">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="3fa46-113">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3fa46-114">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="3fa46-114">Attributes and elements</span></span>

<span data-ttu-id="3fa46-115">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="3fa46-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3fa46-116">Atributos</span><span class="sxs-lookup"><span data-stu-id="3fa46-116">Attributes</span></span>

<span data-ttu-id="3fa46-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3fa46-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3fa46-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="3fa46-118">Child elements</span></span>

<span data-ttu-id="3fa46-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="3fa46-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3fa46-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="3fa46-120">Parent elements</span></span>

|<span data-ttu-id="3fa46-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="3fa46-121">**Element**</span></span>|<span data-ttu-id="3fa46-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3fa46-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3fa46-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="3fa46-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="3fa46-124">Fornece informações adicionais para um evento de calendário.</span><span class="sxs-lookup"><span data-stu-id="3fa46-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="3fa46-125">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="3fa46-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3fa46-126">Text value</span><span class="sxs-lookup"><span data-stu-id="3fa46-126">Text value</span></span>

<span data-ttu-id="3fa46-127">Se esse elemento é retornado em tempo de resposta, é necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="3fa46-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="3fa46-128">Este elemento não será retornado se o valor do elemento [IsPrivate](isprivate.md) for igual a **true**.</span><span class="sxs-lookup"><span data-stu-id="3fa46-128">This element will not be returned if the [IsPrivate](isprivate.md) element value is equal to **true**.</span></span> <span data-ttu-id="3fa46-129">Esse elemento pode conter uma sequência vazia.</span><span class="sxs-lookup"><span data-stu-id="3fa46-129">This element can contain an empty string.</span></span> <span data-ttu-id="3fa46-130">Esse elemento é opcional, se o elemento [CalendarEventDetails](calendareventdetails.md) é usado.</span><span class="sxs-lookup"><span data-stu-id="3fa46-130">This element is optional if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3fa46-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="3fa46-131">Remarks</span></span>

<span data-ttu-id="3fa46-132">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="3fa46-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3fa46-133">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="3fa46-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3fa46-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="3fa46-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3fa46-135">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="3fa46-135">Schema Name</span></span>  <br/> |<span data-ttu-id="3fa46-136">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="3fa46-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="3fa46-137">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="3fa46-137">Validation File</span></span>  <br/> |<span data-ttu-id="3fa46-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3fa46-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3fa46-139">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="3fa46-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="3fa46-140">False</span><span class="sxs-lookup"><span data-stu-id="3fa46-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3fa46-141">Ver também</span><span class="sxs-lookup"><span data-stu-id="3fa46-141">See also</span></span>



[<span data-ttu-id="3fa46-142">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="3fa46-142">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="3fa46-143">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="3fa46-143">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="3fa46-144">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="3fa46-144">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

