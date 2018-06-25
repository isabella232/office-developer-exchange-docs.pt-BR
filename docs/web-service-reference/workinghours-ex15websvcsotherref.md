---
title: WorkingHours
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WorkingHours
api_type:
- schema
ms.assetid: bbe97777-f728-46c5-b2aa-565112c24f3a
description: O elemento WorkingHours representa as configurações de fuso horário e o horário de trabalho para o usuário de caixa de correio solicitada.
ms.openlocfilehash: c53779422b87adebed370a1ed88e4e91c7a2dcaf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838080"
---
# <a name="workinghours"></a><span data-ttu-id="d697a-103">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="d697a-103">WorkingHours</span></span>

<span data-ttu-id="d697a-104">O elemento **WorkingHours** representa as configurações de fuso horário e o horário de trabalho para o usuário de caixa de correio solicitada.</span><span class="sxs-lookup"><span data-stu-id="d697a-104">The **WorkingHours** element represents the time zone settings and working hours for the requested mailbox user.</span></span> 
  
[<span data-ttu-id="d697a-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d697a-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="d697a-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="d697a-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="d697a-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="d697a-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="d697a-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="d697a-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="d697a-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="d697a-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
```xml
<WorkingHours>
   <TimeZone>...</TimeZone>
   <WorkingPeriodArray>...</WorkingPeriodArray>
</WorkingHours>
```

 <span data-ttu-id="d697a-110">**WorkingHours**</span><span class="sxs-lookup"><span data-stu-id="d697a-110">**WorkingHours**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d697a-111">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d697a-111">Attributes and elements</span></span>

<span data-ttu-id="d697a-112">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d697a-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d697a-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="d697a-113">Attributes</span></span>

<span data-ttu-id="d697a-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d697a-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d697a-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d697a-115">Child elements</span></span>

|<span data-ttu-id="d697a-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d697a-116">**Element**</span></span>|<span data-ttu-id="d697a-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d697a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d697a-118">Fuso horário (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="d697a-118">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> |<span data-ttu-id="d697a-119">Contém os elementos que identificam as informações de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="d697a-119">Contains elements that identify time zone information.</span></span> <span data-ttu-id="d697a-120">Esse elemento também contém informações sobre a transição entre o período padrão e o horário de verão.</span><span class="sxs-lookup"><span data-stu-id="d697a-120">This element also contains information about the transition between standard time and daylight saving time.</span></span> <span data-ttu-id="d697a-121">Esse elemento é necessário se o elemento **WorkingHours** é usado.</span><span class="sxs-lookup"><span data-stu-id="d697a-121">This element is required if the **WorkingHours** element is used.</span></span>  <br/> |
|[<span data-ttu-id="d697a-122">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="d697a-122">WorkingPeriodArray</span></span>](workingperiodarray.md) <br/> |<span data-ttu-id="d697a-123">Contém informações do período para o usuário de caixa de correio de trabalhando.</span><span class="sxs-lookup"><span data-stu-id="d697a-123">Contains working period information for the mailbox user.</span></span> <span data-ttu-id="d697a-124">Esse elemento é necessário se o elemento **WorkingHours** é usado.</span><span class="sxs-lookup"><span data-stu-id="d697a-124">This element is required if the **WorkingHours** element is used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d697a-125">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d697a-125">Parent elements</span></span>

|<span data-ttu-id="d697a-126">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d697a-126">**Element**</span></span>|<span data-ttu-id="d697a-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d697a-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d697a-128">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="d697a-128">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="d697a-129">Contém informações de disponibilidade para um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="d697a-129">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="d697a-130">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="d697a-130">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d697a-131">Comentários</span><span class="sxs-lookup"><span data-stu-id="d697a-131">Remarks</span></span>

<span data-ttu-id="d697a-132">Todos os elementos filhos são listados na sequência em que ocorrem.</span><span class="sxs-lookup"><span data-stu-id="d697a-132">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="d697a-133">O nível de detalhes fornecidos por esse elemento depende as permissões concedidas para o solicitante.</span><span class="sxs-lookup"><span data-stu-id="d697a-133">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="d697a-134">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="d697a-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d697a-135">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d697a-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d697a-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="d697a-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d697a-137">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d697a-137">Schema Name</span></span>  <br/> |<span data-ttu-id="d697a-138">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d697a-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="d697a-139">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d697a-139">Validation File</span></span>  <br/> |<span data-ttu-id="d697a-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d697a-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d697a-141">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d697a-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="d697a-142">False</span><span class="sxs-lookup"><span data-stu-id="d697a-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d697a-143">Ver também</span><span class="sxs-lookup"><span data-stu-id="d697a-143">See also</span></span>



[<span data-ttu-id="d697a-144">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="d697a-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="d697a-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d697a-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="d697a-146">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="d697a-146">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

