---
title: Fuso horário (disponibilidade)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZone
api_type:
- schema
ms.assetid: d662ffae-1f93-4c08-85a4-c69de2f7c681
description: O elemento TimeZone contém elementos que identificam as informações de fuso horário. Esse elemento também contém informações sobre a transição entre o período padrão e o horário de verão.
ms.openlocfilehash: dc2466e8039819edc82294ff05f1746ada64cb43
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837765"
---
# <a name="timezone-availability"></a><span data-ttu-id="11f19-104">Fuso horário (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="11f19-104">TimeZone (Availability)</span></span>

<span data-ttu-id="11f19-105">O elemento **TimeZone** contém elementos que identificam as informações de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="11f19-105">The **TimeZone** element contains elements that identify time zone information.</span></span> <span data-ttu-id="11f19-106">Esse elemento também contém informações sobre a transição entre o período padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="11f19-106">This element also contains information about the transition between standard time and daylight saving time.</span></span> 
  
```xml
<TimeZone>
   <Bias/>
   <StandardTime/>
   <DaylightTime/>
</TimeZone>
```

 <span data-ttu-id="11f19-107">**SerializableTimeZone**</span><span class="sxs-lookup"><span data-stu-id="11f19-107">**SerializableTimeZone**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="11f19-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="11f19-108">Attributes and elements</span></span>

<span data-ttu-id="11f19-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="11f19-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="11f19-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="11f19-110">Attributes</span></span>

<span data-ttu-id="11f19-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="11f19-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="11f19-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="11f19-112">Child elements</span></span>

|<span data-ttu-id="11f19-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="11f19-113">**Element**</span></span>|<span data-ttu-id="11f19-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="11f19-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11f19-115">Bias (UTC)</span><span class="sxs-lookup"><span data-stu-id="11f19-115">Bias (UTC)</span></span>](bias-utc.md) <br/> |<span data-ttu-id="11f19-116">Representa o deslocamento geral do tempo Universal Coordenado (UTC).</span><span class="sxs-lookup"><span data-stu-id="11f19-116">Represents the general offset from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="11f19-117">Este valor está em minutos.</span><span class="sxs-lookup"><span data-stu-id="11f19-117">This value is in minutes.</span></span>  <br/> |
|[<span data-ttu-id="11f19-118">StandardTime</span><span class="sxs-lookup"><span data-stu-id="11f19-118">StandardTime</span></span>](standardtime.md) <br/> |<span data-ttu-id="11f19-119">Representa um deslocamento, desde o momento em relação ao UTC representado pelo elemento [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="11f19-119">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="11f19-120">Horário de verão em regiões onde o horário de verão é observado, esse elemento também contém informações sobre a transição para a hora padrão.</span><span class="sxs-lookup"><span data-stu-id="11f19-120">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span>  <br/> |
|[<span data-ttu-id="11f19-121">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="11f19-121">DaylightTime</span></span>](daylighttime.md) <br/> |<span data-ttu-id="11f19-122">Representa um deslocamento, desde o momento em relação ao UTC representado pelo [Bias (UTC)](bias-utc.md) elemento em regiões onde o horário de verão é observado.</span><span class="sxs-lookup"><span data-stu-id="11f19-122">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="11f19-123">Esse elemento também contém informações sobre como ocorre a transição do horário de verão do período padrão.</span><span class="sxs-lookup"><span data-stu-id="11f19-123">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="11f19-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="11f19-124">Parent elements</span></span>

|<span data-ttu-id="11f19-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="11f19-125">**Element**</span></span>|<span data-ttu-id="11f19-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="11f19-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11f19-127">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="11f19-127">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="11f19-128">Contém os argumentos usados para obter informações de disponibilidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="11f19-128">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="11f19-129">Este é um elemento raiz.</span><span class="sxs-lookup"><span data-stu-id="11f19-129">This is a root element.</span></span>  <br/> <span data-ttu-id="11f19-130">O elemento de **fuso horário** na mensagem GetUserAvailabilityRequest representa o fuso horário em que os valores de data/hora na solicitação são especificados.</span><span class="sxs-lookup"><span data-stu-id="11f19-130">The **TimeZone** element in the GetUserAvailabilityRequest message represents the time zone in which the DateTime values in the request are specified.</span></span> <span data-ttu-id="11f19-131">Os valores de data/hora retornados pelo serviço de disponibilidade também estão neste fuso horário.</span><span class="sxs-lookup"><span data-stu-id="11f19-131">The DateTime values returned by the Availability service are also in this time zone.</span></span>  <br/> <span data-ttu-id="11f19-132">Este é o XPath a este elemento:</span><span class="sxs-lookup"><span data-stu-id="11f19-132">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
|[<span data-ttu-id="11f19-133">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="11f19-133">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md) <br/> |<span data-ttu-id="11f19-134">Representa as configurações de fuso horário e o horário de trabalho para o usuário de caixa de correio solicitada.</span><span class="sxs-lookup"><span data-stu-id="11f19-134">Represents the time zone settings and working hours for the requested mailbox user.</span></span>  <br/> <span data-ttu-id="11f19-135">O elemento de **fuso horário** na mensagem GetUserAvailabilityResponse representa as configurações de fuso horário do usuário da caixa de correio solicitada.</span><span class="sxs-lookup"><span data-stu-id="11f19-135">The **TimeZone** element in the GetUserAvailabilityResponse message represents the time zone settings of the requested mailbox user.</span></span>  <br/> <span data-ttu-id="11f19-136">Este é o XPath a este elemento:</span><span class="sxs-lookup"><span data-stu-id="11f19-136">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="11f19-137">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="11f19-137">Remarks</span></span>

<span data-ttu-id="11f19-138">Esse elemento é necessário no elemento [GetUserAvailabilityRequest](getuseravailabilityrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="11f19-138">This element is required in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md) element.</span></span> <span data-ttu-id="11f19-139">Esse elemento ocorre no máximo uma vez ou menos zero vezes quando o elemento pai é o elemento [WorkingHours](workinghours-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="11f19-139">This element occurs at most once or at least zero times when the parent element is the [WorkingHours](workinghours-ex15websvcsotherref.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="11f19-140">Example</span><span class="sxs-lookup"><span data-stu-id="11f19-140">Example</span></span>

<span data-ttu-id="11f19-141">O exemplo a seguir mostra a parte de uma solicitação XML que identifica um deslocamento do UTC de 8 horas no aplicativo cliente.</span><span class="sxs-lookup"><span data-stu-id="11f19-141">The following example shows part of an XML request that identifies an offset from UTC of 8 hours in the client application.</span></span>
  
```XML
<TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
  <Bias>480</Bias>
  <StandardTime>
    <Bias>0</Bias>
    <Time>02:00:00</Time>
    <DayOrder>1</DayOrder>
    <Month>11</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </StandardTime>
  <DaylightTime>
    <Bias>-60</Bias>
    <Time>02:00:00</Time>
    <DayOrder>2</DayOrder>
    <Month>3</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </DaylightTime>
</TimeZone>
```

## <a name="element-information"></a><span data-ttu-id="11f19-142">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="11f19-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="11f19-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="11f19-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="11f19-144">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="11f19-144">Schema Name</span></span>  <br/> |<span data-ttu-id="11f19-145">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="11f19-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="11f19-146">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="11f19-146">Validation File</span></span>  <br/> |<span data-ttu-id="11f19-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="11f19-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="11f19-148">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="11f19-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="11f19-149">False</span><span class="sxs-lookup"><span data-stu-id="11f19-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="11f19-150">Ver também</span><span class="sxs-lookup"><span data-stu-id="11f19-150">See also</span></span>



[<span data-ttu-id="11f19-151">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="11f19-151">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="11f19-152">Bias</span><span class="sxs-lookup"><span data-stu-id="11f19-152">Bias</span></span>](bias.md)


[<span data-ttu-id="11f19-153">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="11f19-153">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

