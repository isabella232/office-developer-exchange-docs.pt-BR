---
title: WorkingPeriodArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WorkingPeriodArray
api_type:
- schema
ms.assetid: 3a3f6393-eacc-4734-b6c9-b67023fe2830
description: O elemento WorkingPeriodArray contém trabalhando informações do período para o usuário de caixa de correio.
ms.openlocfilehash: 02712f05dc3373a532d769f476341b78ad25a79c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838091"
---
# <a name="workingperiodarray"></a><span data-ttu-id="aae5e-103">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="aae5e-103">WorkingPeriodArray</span></span>

<span data-ttu-id="aae5e-104">O elemento **WorkingPeriodArray** contém trabalhando informações do período para o usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="aae5e-104">The **WorkingPeriodArray** element contains working period information for the mailbox user.</span></span> 
  
[<span data-ttu-id="aae5e-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="aae5e-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="aae5e-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="aae5e-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="aae5e-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="aae5e-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="aae5e-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="aae5e-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="aae5e-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="aae5e-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
[<span data-ttu-id="aae5e-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="aae5e-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
```xml
<WorkingPeriodArray>
   <WorkingPeriod>...</WorkingPeriod>
</WorkingPeriodArray>
```

 <span data-ttu-id="aae5e-111">**ArrayOfWorkingPeriod**</span><span class="sxs-lookup"><span data-stu-id="aae5e-111">**ArrayOfWorkingPeriod**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aae5e-112">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="aae5e-112">Attributes and elements</span></span>

<span data-ttu-id="aae5e-113">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="aae5e-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aae5e-114">Atributos</span><span class="sxs-lookup"><span data-stu-id="aae5e-114">Attributes</span></span>

<span data-ttu-id="aae5e-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="aae5e-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aae5e-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="aae5e-116">Child elements</span></span>

|<span data-ttu-id="aae5e-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="aae5e-117">**Element**</span></span>|<span data-ttu-id="aae5e-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aae5e-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aae5e-119">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="aae5e-119">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="aae5e-120">Contém a semana de trabalho dias e horas do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="aae5e-120">Contains the work week days and hours of the mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aae5e-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="aae5e-121">Parent elements</span></span>

|<span data-ttu-id="aae5e-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="aae5e-122">**Element**</span></span>|<span data-ttu-id="aae5e-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="aae5e-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aae5e-124">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="aae5e-124">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md) <br/> |<span data-ttu-id="aae5e-125">Representa as configurações de fuso horário e o horário de trabalho para o usuário de caixa de correio solicitada.</span><span class="sxs-lookup"><span data-stu-id="aae5e-125">Represents the time zone settings and working hours for the requested mailbox user.</span></span>  <br/> <span data-ttu-id="aae5e-126">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="aae5e-126">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aae5e-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="aae5e-127">Remarks</span></span>

<span data-ttu-id="aae5e-128">Esse elemento é necessário se o elemento [WorkingHours](workinghours-ex15websvcsotherref.md) é usado.</span><span class="sxs-lookup"><span data-stu-id="aae5e-128">This element is required if the [WorkingHours](workinghours-ex15websvcsotherref.md) element is used.</span></span> <span data-ttu-id="aae5e-129">Todos os elementos filhos são listados na sequência em que ocorrem.</span><span class="sxs-lookup"><span data-stu-id="aae5e-129">All the child elements are listed in the sequence in which they occur.</span></span> 
  
<span data-ttu-id="aae5e-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="aae5e-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aae5e-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="aae5e-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aae5e-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="aae5e-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aae5e-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="aae5e-133">Schema Name</span></span>  <br/> |<span data-ttu-id="aae5e-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="aae5e-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="aae5e-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="aae5e-135">Validation File</span></span>  <br/> |<span data-ttu-id="aae5e-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="aae5e-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aae5e-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="aae5e-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="aae5e-138">False</span><span class="sxs-lookup"><span data-stu-id="aae5e-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aae5e-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="aae5e-139">See also</span></span>



[<span data-ttu-id="aae5e-140">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="aae5e-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="aae5e-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="aae5e-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="aae5e-142">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="aae5e-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

