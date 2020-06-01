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
description: O elemento TimeZone contém elementos que identificam informações de fuso horário. Esse elemento também contém informações sobre a transição entre o horário padrão e o horário de verão.
ms.openlocfilehash: ba4b0a4805dba54450e01e89c5e9ef746404b716
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460271"
---
# <a name="timezone-availability"></a><span data-ttu-id="835e0-104">Fuso horário (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="835e0-104">TimeZone (Availability)</span></span>

<span data-ttu-id="835e0-105">O elemento **timezone** contém elementos que identificam informações de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="835e0-105">The **TimeZone** element contains elements that identify time zone information.</span></span> <span data-ttu-id="835e0-106">Esse elemento também contém informações sobre a transição entre o horário padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="835e0-106">This element also contains information about the transition between standard time and daylight saving time.</span></span> 
  
```xml
<TimeZone>
   <Bias/>
   <StandardTime/>
   <DaylightTime/>
</TimeZone>
```

 <span data-ttu-id="835e0-107">**SerializableTimeZone**</span><span class="sxs-lookup"><span data-stu-id="835e0-107">**SerializableTimeZone**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="835e0-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="835e0-108">Attributes and elements</span></span>

<span data-ttu-id="835e0-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="835e0-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="835e0-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="835e0-110">Attributes</span></span>

<span data-ttu-id="835e0-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="835e0-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="835e0-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="835e0-112">Child elements</span></span>

|<span data-ttu-id="835e0-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="835e0-113">**Element**</span></span>|<span data-ttu-id="835e0-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="835e0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="835e0-115">Bias (UTC)</span><span class="sxs-lookup"><span data-stu-id="835e0-115">Bias (UTC)</span></span>](bias-utc.md) <br/> |<span data-ttu-id="835e0-116">Representa o deslocamento geral do tempo universal coordenado (UTC).</span><span class="sxs-lookup"><span data-stu-id="835e0-116">Represents the general offset from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="835e0-117">Este valor está em minutos.</span><span class="sxs-lookup"><span data-stu-id="835e0-117">This value is in minutes.</span></span>  <br/> |
|[<span data-ttu-id="835e0-118">StandardTime</span><span class="sxs-lookup"><span data-stu-id="835e0-118">StandardTime</span></span>](standardtime.md) <br/> |<span data-ttu-id="835e0-119">Representa um deslocamento do tempo relativo ao UTC representado pelo elemento [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="835e0-119">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="835e0-120">Esse elemento também contém informações sobre a transição para o horário padrão do horário de verão nas regiões nas quais o horário de verão é observado.</span><span class="sxs-lookup"><span data-stu-id="835e0-120">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span>  <br/> |
|[<span data-ttu-id="835e0-121">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="835e0-121">DaylightTime</span></span>](daylighttime.md) <br/> |<span data-ttu-id="835e0-122">Representa um deslocamento do tempo relativo ao UTC representado pelo elemento [Bias (UTC)](bias-utc.md) nas regiões em que o horário de verão é observado.</span><span class="sxs-lookup"><span data-stu-id="835e0-122">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="835e0-123">Esse elemento também contém informações sobre quando ocorre a transição para o horário de Verão do horário padrão.</span><span class="sxs-lookup"><span data-stu-id="835e0-123">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="835e0-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="835e0-124">Parent elements</span></span>

|<span data-ttu-id="835e0-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="835e0-125">**Element**</span></span>|<span data-ttu-id="835e0-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="835e0-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="835e0-127">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="835e0-127">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="835e0-128">Contém os argumentos usados para obter informações de disponibilidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="835e0-128">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="835e0-129">Este é um elemento raiz.</span><span class="sxs-lookup"><span data-stu-id="835e0-129">This is a root element.</span></span>  <br/> <span data-ttu-id="835e0-130">O elemento **timezone** na mensagem GetUserAvailabilityRequest representa o fuso horário em que os valores DateTime da solicitação são especificados.</span><span class="sxs-lookup"><span data-stu-id="835e0-130">The **TimeZone** element in the GetUserAvailabilityRequest message represents the time zone in which the DateTime values in the request are specified.</span></span> <span data-ttu-id="835e0-131">Os valores DateTime retornados pelo serviço de disponibilidade também estão neste fuso horário.</span><span class="sxs-lookup"><span data-stu-id="835e0-131">The DateTime values returned by the Availability service are also in this time zone.</span></span>  <br/> <span data-ttu-id="835e0-132">Este é o XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="835e0-132">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
|[<span data-ttu-id="835e0-133">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="835e0-133">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md) <br/> |<span data-ttu-id="835e0-134">Representa as configurações de fuso horário e as horas de trabalho do usuário de caixa de correio solicitado.</span><span class="sxs-lookup"><span data-stu-id="835e0-134">Represents the time zone settings and working hours for the requested mailbox user.</span></span>  <br/> <span data-ttu-id="835e0-135">O elemento **timezone** na mensagem GetUserAvailabilityResponse representa as configurações de fuso horário do usuário de caixa de correio solicitado.</span><span class="sxs-lookup"><span data-stu-id="835e0-135">The **TimeZone** element in the GetUserAvailabilityResponse message represents the time zone settings of the requested mailbox user.</span></span>  <br/> <span data-ttu-id="835e0-136">Este é o XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="835e0-136">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="835e0-137">Comentários</span><span class="sxs-lookup"><span data-stu-id="835e0-137">Remarks</span></span>

<span data-ttu-id="835e0-138">Este elemento é obrigatório no elemento [GetUserAvailabilityRequest](getuseravailabilityrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="835e0-138">This element is required in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md) element.</span></span> <span data-ttu-id="835e0-139">Esse elemento ocorre no máximo uma vez ou pelo menos zero vezes quando o elemento pai é o elemento [WorkingHours](workinghours-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="835e0-139">This element occurs at most once or at least zero times when the parent element is the [WorkingHours](workinghours-ex15websvcsotherref.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="835e0-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="835e0-140">Example</span></span>

<span data-ttu-id="835e0-141">O exemplo a seguir mostra parte de uma solicitação XML que identifica um deslocamento do UTC de 8 horas no aplicativo cliente.</span><span class="sxs-lookup"><span data-stu-id="835e0-141">The following example shows part of an XML request that identifies an offset from UTC of 8 hours in the client application.</span></span>
  
```XML
<TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="835e0-142">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="835e0-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="835e0-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="835e0-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="835e0-144">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="835e0-144">Schema Name</span></span>  <br/> |<span data-ttu-id="835e0-145">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="835e0-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="835e0-146">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="835e0-146">Validation File</span></span>  <br/> |<span data-ttu-id="835e0-147">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="835e0-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="835e0-148">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="835e0-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="835e0-149">False</span><span class="sxs-lookup"><span data-stu-id="835e0-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="835e0-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="835e0-150">See also</span></span>



[<span data-ttu-id="835e0-151">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="835e0-151">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="835e0-152">Bias</span><span class="sxs-lookup"><span data-stu-id="835e0-152">Bias</span></span>](bias.md)


[<span data-ttu-id="835e0-153">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="835e0-153">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

