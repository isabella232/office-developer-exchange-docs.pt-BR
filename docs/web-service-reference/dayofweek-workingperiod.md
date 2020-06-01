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
description: O elemento DayOfWeek contém a lista de dias úteis agendados para o usuário da caixa de correio.
ms.openlocfilehash: 06d4a7d5541b3b71fcbf9be9beb7512d06853283
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457442"
---
# <a name="dayofweek-workingperiod"></a><span data-ttu-id="36efd-103">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="36efd-103">DayOfWeek (WorkingPeriod)</span></span>

<span data-ttu-id="36efd-104">O elemento **DayOfWeek** contém a lista de dias úteis agendados para o usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="36efd-104">The **DayOfWeek** element contains the list of working days scheduled for the mailbox user.</span></span> 
  
- [<span data-ttu-id="36efd-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="36efd-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)  
- [<span data-ttu-id="36efd-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="36efd-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)  
- [<span data-ttu-id="36efd-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="36efd-107">FreeBusyResponse</span></span>](freebusyresponse.md)  
- [<span data-ttu-id="36efd-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="36efd-108">FreeBusyView</span></span>](freebusyview.md)  
- [<span data-ttu-id="36efd-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="36efd-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)  
- [<span data-ttu-id="36efd-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="36efd-110">WorkingPeriodArray</span></span>](workingperiodarray.md) 
- [<span data-ttu-id="36efd-111">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="36efd-111">WorkingPeriod</span></span>](workingperiod.md)  
- [<span data-ttu-id="36efd-112">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="36efd-112">DayOfWeek (WorkingPeriod)</span></span>](dayofweek-workingperiod.md)
  
```xml
<DayOfWeek>Sunday Monday Tuesday Wednesday Thursday Friday Saturday</DayOfWeek>
```

<span data-ttu-id="36efd-113">**DaysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="36efd-113">**DaysOfWeek**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="36efd-114">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="36efd-114">Attributes and elements</span></span>

<span data-ttu-id="36efd-115">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="36efd-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36efd-116">Atributos</span><span class="sxs-lookup"><span data-stu-id="36efd-116">Attributes</span></span>

<span data-ttu-id="36efd-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="36efd-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="36efd-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="36efd-118">Child elements</span></span>

<span data-ttu-id="36efd-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="36efd-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="36efd-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="36efd-120">Parent elements</span></span>

|<span data-ttu-id="36efd-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="36efd-121">**Element**</span></span>|<span data-ttu-id="36efd-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="36efd-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36efd-123">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="36efd-123">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="36efd-124">Contém os dias e as horas da semana de trabalho do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="36efd-124">Contains the work week days and hours of the mailbox user.</span></span><br/><br/><span data-ttu-id="36efd-125">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="36efd-125">The following is the XPath expression to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod[i[` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="36efd-126">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="36efd-126">Text value</span></span>

<span data-ttu-id="36efd-127">Um valor de texto será retornado se o usuário da caixa de correio tiver dias definidos para representar a semana de trabalho.</span><span class="sxs-lookup"><span data-stu-id="36efd-127">A text value is returned if the mailbox user has days set to represent the work week.</span></span> <span data-ttu-id="36efd-128">Estes são os valores possíveis para este elemento:</span><span class="sxs-lookup"><span data-stu-id="36efd-128">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="36efd-129">Domingo</span><span class="sxs-lookup"><span data-stu-id="36efd-129">Sunday</span></span>    
- <span data-ttu-id="36efd-130">Segunda-feira</span><span class="sxs-lookup"><span data-stu-id="36efd-130">Monday</span></span>    
- <span data-ttu-id="36efd-131">Terça-feira</span><span class="sxs-lookup"><span data-stu-id="36efd-131">Tuesday</span></span>    
- <span data-ttu-id="36efd-132">Quarta-feira</span><span class="sxs-lookup"><span data-stu-id="36efd-132">Wednesday</span></span>    
- <span data-ttu-id="36efd-133">Quinta-feira</span><span class="sxs-lookup"><span data-stu-id="36efd-133">Thursday</span></span>    
- <span data-ttu-id="36efd-134">Sexta-feira</span><span class="sxs-lookup"><span data-stu-id="36efd-134">Friday</span></span>    
- <span data-ttu-id="36efd-135">Sábado</span><span class="sxs-lookup"><span data-stu-id="36efd-135">Saturday</span></span> 
    
<span data-ttu-id="36efd-136">Os valores de texto serão retornados nessa ordem.</span><span class="sxs-lookup"><span data-stu-id="36efd-136">The text values will be returned in that order.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="36efd-137">Comentários</span><span class="sxs-lookup"><span data-stu-id="36efd-137">Remarks</span></span>

<span data-ttu-id="36efd-138">É importante observar que a diferença entre este elemento e o elemento de disponibilidade de [DayOfWeek (TimeZone)](dayofweek-timezone.md) é o tipo.</span><span class="sxs-lookup"><span data-stu-id="36efd-138">It is important to note that the difference between this element and the Availability [DayOfWeek (TimeZone)](dayofweek-timezone.md) element is the type.</span></span> 
  
<span data-ttu-id="36efd-139">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="36efd-139">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="36efd-140">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="36efd-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36efd-141">Namespace</span><span class="sxs-lookup"><span data-stu-id="36efd-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="36efd-142">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="36efd-142">Schema Name</span></span>  <br/> |<span data-ttu-id="36efd-143">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="36efd-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="36efd-144">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="36efd-144">Validation File</span></span>  <br/> |<span data-ttu-id="36efd-145">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="36efd-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="36efd-146">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="36efd-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="36efd-147">False</span><span class="sxs-lookup"><span data-stu-id="36efd-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="36efd-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="36efd-148">See also</span></span>

- [<span data-ttu-id="36efd-149">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="36efd-149">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="36efd-150">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="36efd-150">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="36efd-151">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="36efd-151">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

