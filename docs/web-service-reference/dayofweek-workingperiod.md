---
title: DayOfWeek (WorkingPeriod)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfWeek
api_type:
- schema
ms.assetid: 7a8a8cc1-392b-4db5-bb76-710477e31396
description: O elemento DayOfWeek contém a lista de dias úteis agendados para o usuário de caixa de correio.
ms.openlocfilehash: a6a68017291ba13f45b3970307669222d583fcbb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751710"
---
# <a name="dayofweek-workingperiod"></a><span data-ttu-id="a3799-103">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="a3799-103">DayOfWeek (WorkingPeriod)</span></span>

<span data-ttu-id="a3799-104">O elemento **DayOfWeek** contém a lista de dias úteis agendados para o usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="a3799-104">The **DayOfWeek** element contains the list of working days scheduled for the mailbox user.</span></span> 
  
- [<span data-ttu-id="a3799-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a3799-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)  
- [<span data-ttu-id="a3799-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="a3799-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)  
- [<span data-ttu-id="a3799-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="a3799-107">FreeBusyResponse</span></span>](freebusyresponse.md)  
- [<span data-ttu-id="a3799-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="a3799-108">FreeBusyView</span></span>](freebusyview.md)  
- [<span data-ttu-id="a3799-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="a3799-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)  
- [<span data-ttu-id="a3799-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="a3799-110">WorkingPeriodArray</span></span>](workingperiodarray.md) 
- [<span data-ttu-id="a3799-111">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="a3799-111">WorkingPeriod</span></span>](workingperiod.md)  
- [<span data-ttu-id="a3799-112">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="a3799-112">DayOfWeek (WorkingPeriod)</span></span>](dayofweek-workingperiod.md)
  
```xml
<DayOfWeek>Sunday Monday Tuesday Wednesday Thursday Friday Saturday</DayOfWeek>
```

<span data-ttu-id="a3799-113">**DaysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="a3799-113">**DaysOfWeek**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a3799-114">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a3799-114">Attributes and elements</span></span>

<span data-ttu-id="a3799-115">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a3799-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a3799-116">Atributos</span><span class="sxs-lookup"><span data-stu-id="a3799-116">Attributes</span></span>

<span data-ttu-id="a3799-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a3799-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a3799-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a3799-118">Child elements</span></span>

<span data-ttu-id="a3799-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a3799-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a3799-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a3799-120">Parent elements</span></span>

|<span data-ttu-id="a3799-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a3799-121">**Element**</span></span>|<span data-ttu-id="a3799-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a3799-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a3799-123">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="a3799-123">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="a3799-124">Contém a semana de trabalho dias e horas do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="a3799-124">Contains the work week days and hours of the mailbox user.</span></span><br/><br/><span data-ttu-id="a3799-125">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="a3799-125">The following is the XPath expression to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod[i[` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a3799-126">Text value</span><span class="sxs-lookup"><span data-stu-id="a3799-126">Text value</span></span>

<span data-ttu-id="a3799-127">Um valor de texto será retornado se o usuário de caixa de correio tem dias definidos para representar a semana de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a3799-127">A text value is returned if the mailbox user has days set to represent the work week.</span></span> <span data-ttu-id="a3799-128">Estes são os valores possíveis para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="a3799-128">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="a3799-129">Domingo</span><span class="sxs-lookup"><span data-stu-id="a3799-129">Sunday</span></span>    
- <span data-ttu-id="a3799-130">Segunda-feira</span><span class="sxs-lookup"><span data-stu-id="a3799-130">Monday</span></span>    
- <span data-ttu-id="a3799-131">Terça-feira</span><span class="sxs-lookup"><span data-stu-id="a3799-131">Tuesday</span></span>    
- <span data-ttu-id="a3799-132">Quarta-feira</span><span class="sxs-lookup"><span data-stu-id="a3799-132">Wednesday</span></span>    
- <span data-ttu-id="a3799-133">Quinta-feira</span><span class="sxs-lookup"><span data-stu-id="a3799-133">Thursday</span></span>    
- <span data-ttu-id="a3799-134">Sexta-feira</span><span class="sxs-lookup"><span data-stu-id="a3799-134">Friday</span></span>    
- <span data-ttu-id="a3799-135">Sábado</span><span class="sxs-lookup"><span data-stu-id="a3799-135">Saturday</span></span> 
    
<span data-ttu-id="a3799-136">Os valores de texto serão retornados nesta ordem.</span><span class="sxs-lookup"><span data-stu-id="a3799-136">The text values will be returned in that order.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a3799-137">Comentários</span><span class="sxs-lookup"><span data-stu-id="a3799-137">Remarks</span></span>

<span data-ttu-id="a3799-138">É importante observar que a diferença entre esse elemento e o elemento de disponibilidade [DayOfWeek (TimeZone)](dayofweek-timezone.md) é o tipo.</span><span class="sxs-lookup"><span data-stu-id="a3799-138">It is important to note that the difference between this element and the Availability [DayOfWeek (TimeZone)](dayofweek-timezone.md) element is the type.</span></span> 
  
<span data-ttu-id="a3799-139">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="a3799-139">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a3799-140">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a3799-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a3799-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="a3799-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a3799-142">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a3799-142">Schema Name</span></span>  <br/> |<span data-ttu-id="a3799-143">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a3799-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="a3799-144">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a3799-144">Validation File</span></span>  <br/> |<span data-ttu-id="a3799-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a3799-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a3799-146">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a3799-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="a3799-147">False</span><span class="sxs-lookup"><span data-stu-id="a3799-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a3799-148">Ver também</span><span class="sxs-lookup"><span data-stu-id="a3799-148">See also</span></span>

- [<span data-ttu-id="a3799-149">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="a3799-149">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="a3799-150">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a3799-150">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="a3799-151">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="a3799-151">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

