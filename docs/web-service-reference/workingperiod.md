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
description: O elemento WorkingPeriod contém a semana de trabalho dias e horas do usuário da caixa de correio.
ms.openlocfilehash: 0f2707bede5e49174ed62a35ba704e39c0c48e9f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838092"
---
# <a name="workingperiod"></a><span data-ttu-id="d334a-103">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="d334a-103">WorkingPeriod</span></span>

<span data-ttu-id="d334a-104">O elemento **WorkingPeriod** contém a semana de trabalho dias e horas do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d334a-104">The **WorkingPeriod** element contains the work week days and hours of the mailbox user.</span></span> 
  
[<span data-ttu-id="d334a-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d334a-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="d334a-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="d334a-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="d334a-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="d334a-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="d334a-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="d334a-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="d334a-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="d334a-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
[<span data-ttu-id="d334a-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="d334a-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
[<span data-ttu-id="d334a-111">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="d334a-111">WorkingPeriod</span></span>](workingperiod.md)
  
```xml
<WorkingPeriod>
   <DayOfWeek>...</DayOfWeek>
   <StartTimeInMinutes>...</StartTimeInMinutes>
   <EndTimeInMinutes>...</EndTimeInMinutes>
</WorkingPeriod>
```

 <span data-ttu-id="d334a-112">**WorkingPeriod**</span><span class="sxs-lookup"><span data-stu-id="d334a-112">**WorkingPeriod**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d334a-113">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d334a-113">Attributes and elements</span></span>

<span data-ttu-id="d334a-114">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d334a-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d334a-115">Atributos</span><span class="sxs-lookup"><span data-stu-id="d334a-115">Attributes</span></span>

<span data-ttu-id="d334a-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d334a-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d334a-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d334a-117">Child elements</span></span>

|<span data-ttu-id="d334a-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d334a-118">**Element**</span></span>|<span data-ttu-id="d334a-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d334a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d334a-120">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="d334a-120">DayOfWeek (WorkingPeriod)</span></span>](dayofweek-workingperiod.md) <br/> |<span data-ttu-id="d334a-121">Contém a lista de dias úteis agendados para o usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d334a-121">Contains the list of working days scheduled for the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="d334a-122">StartTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="d334a-122">StartTimeInMinutes</span></span>](starttimeinminutes.md) <br/> |<span data-ttu-id="d334a-123">Representa o início do dia útil para um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d334a-123">Represents the start of the working day for a mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="d334a-124">EndTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="d334a-124">EndTimeInMinutes</span></span>](endtimeinminutes.md) <br/> |<span data-ttu-id="d334a-125">Representa o final do dia útil para um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d334a-125">Represents the end of the working day for a mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d334a-126">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d334a-126">Parent elements</span></span>

|<span data-ttu-id="d334a-127">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d334a-127">**Element**</span></span>|<span data-ttu-id="d334a-128">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d334a-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d334a-129">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="d334a-129">WorkingPeriodArray</span></span>](workingperiodarray.md) <br/> |<span data-ttu-id="d334a-130">Contém informações do período para o usuário de caixa de correio de trabalhando.</span><span class="sxs-lookup"><span data-stu-id="d334a-130">Contains working period information for the mailbox user.</span></span>  <br/> <span data-ttu-id="d334a-131">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="d334a-131">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d334a-132">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="d334a-132">Remarks</span></span>

<span data-ttu-id="d334a-133">Todos os elementos filhos são listados na sequência em que ocorrem.</span><span class="sxs-lookup"><span data-stu-id="d334a-133">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="d334a-134">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="d334a-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d334a-135">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d334a-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d334a-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="d334a-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d334a-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d334a-137">Schema Name</span></span>  <br/> |<span data-ttu-id="d334a-138">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d334a-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="d334a-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d334a-139">Validation File</span></span>  <br/> |<span data-ttu-id="d334a-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d334a-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d334a-141">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d334a-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="d334a-142">False</span><span class="sxs-lookup"><span data-stu-id="d334a-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d334a-143">Ver também</span><span class="sxs-lookup"><span data-stu-id="d334a-143">See also</span></span>



[<span data-ttu-id="d334a-144">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="d334a-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="d334a-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d334a-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="d334a-146">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="d334a-146">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

