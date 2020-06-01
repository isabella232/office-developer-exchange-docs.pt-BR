---
title: WorkingPeriod
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WorkingPeriod
api_type:
- schema
ms.assetid: 3b4e48af-9880-42b9-a0dc-dae7ac43c264
description: O elemento WorkingPeriod contém os dias e as horas da semana de trabalho do usuário da caixa de correio.
ms.openlocfilehash: 5c217169fb193d4bb6dae4e18570873d55de6127
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459676"
---
# <a name="workingperiod"></a><span data-ttu-id="e3074-103">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="e3074-103">WorkingPeriod</span></span>

<span data-ttu-id="e3074-104">O elemento **WorkingPeriod** contém os dias e as horas da semana de trabalho do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e3074-104">The **WorkingPeriod** element contains the work week days and hours of the mailbox user.</span></span> 
  
[<span data-ttu-id="e3074-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="e3074-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="e3074-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="e3074-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="e3074-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="e3074-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="e3074-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="e3074-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="e3074-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="e3074-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
[<span data-ttu-id="e3074-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="e3074-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
[<span data-ttu-id="e3074-111">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="e3074-111">WorkingPeriod</span></span>](workingperiod.md)
  
```xml
<WorkingPeriod>
   <DayOfWeek>...</DayOfWeek>
   <StartTimeInMinutes>...</StartTimeInMinutes>
   <EndTimeInMinutes>...</EndTimeInMinutes>
</WorkingPeriod>
```

 <span data-ttu-id="e3074-112">**WorkingPeriod**</span><span class="sxs-lookup"><span data-stu-id="e3074-112">**WorkingPeriod**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e3074-113">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="e3074-113">Attributes and elements</span></span>

<span data-ttu-id="e3074-114">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e3074-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e3074-115">Atributos</span><span class="sxs-lookup"><span data-stu-id="e3074-115">Attributes</span></span>

<span data-ttu-id="e3074-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e3074-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e3074-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e3074-117">Child elements</span></span>

|<span data-ttu-id="e3074-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e3074-118">**Element**</span></span>|<span data-ttu-id="e3074-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e3074-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3074-120">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="e3074-120">DayOfWeek (WorkingPeriod)</span></span>](dayofweek-workingperiod.md) <br/> |<span data-ttu-id="e3074-121">Contém a lista de dias úteis agendados para o usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e3074-121">Contains the list of working days scheduled for the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="e3074-122">StartTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="e3074-122">StartTimeInMinutes</span></span>](starttimeinminutes.md) <br/> |<span data-ttu-id="e3074-123">Representa o início do dia útil de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e3074-123">Represents the start of the working day for a mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="e3074-124">EndTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="e3074-124">EndTimeInMinutes</span></span>](endtimeinminutes.md) <br/> |<span data-ttu-id="e3074-125">Representa o final do dia útil de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e3074-125">Represents the end of the working day for a mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e3074-126">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e3074-126">Parent elements</span></span>

|<span data-ttu-id="e3074-127">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e3074-127">**Element**</span></span>|<span data-ttu-id="e3074-128">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e3074-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3074-129">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="e3074-129">WorkingPeriodArray</span></span>](workingperiodarray.md) <br/> |<span data-ttu-id="e3074-130">Contém informações de período de trabalho para o usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e3074-130">Contains working period information for the mailbox user.</span></span>  <br/> <span data-ttu-id="e3074-131">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="e3074-131">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e3074-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="e3074-132">Remarks</span></span>

<span data-ttu-id="e3074-133">Todos os elementos filho são listados na sequência em que ocorrem.</span><span class="sxs-lookup"><span data-stu-id="e3074-133">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="e3074-134">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="e3074-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e3074-135">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="e3074-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e3074-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="e3074-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e3074-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e3074-137">Schema Name</span></span>  <br/> |<span data-ttu-id="e3074-138">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e3074-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="e3074-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e3074-139">Validation File</span></span>  <br/> |<span data-ttu-id="e3074-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e3074-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e3074-141">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e3074-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="e3074-142">False</span><span class="sxs-lookup"><span data-stu-id="e3074-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e3074-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="e3074-143">See also</span></span>



[<span data-ttu-id="e3074-144">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="e3074-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="e3074-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="e3074-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="e3074-146">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="e3074-146">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

