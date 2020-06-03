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
description: O elemento WorkingPeriodArray contém informações de período de trabalho para o usuário da caixa de correio.
ms.openlocfilehash: a9ca55866a574c5208d8561fca6daf417867fef6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465195"
---
# <a name="workingperiodarray"></a><span data-ttu-id="50c47-103">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="50c47-103">WorkingPeriodArray</span></span>

<span data-ttu-id="50c47-104">O elemento **WorkingPeriodArray** contém informações de período de trabalho para o usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="50c47-104">The **WorkingPeriodArray** element contains working period information for the mailbox user.</span></span> 
  
[<span data-ttu-id="50c47-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="50c47-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="50c47-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="50c47-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="50c47-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="50c47-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="50c47-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="50c47-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="50c47-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="50c47-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
[<span data-ttu-id="50c47-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="50c47-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
```xml
<WorkingPeriodArray>
   <WorkingPeriod>...</WorkingPeriod>
</WorkingPeriodArray>
```

 <span data-ttu-id="50c47-111">**ArrayOfWorkingPeriod**</span><span class="sxs-lookup"><span data-stu-id="50c47-111">**ArrayOfWorkingPeriod**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="50c47-112">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="50c47-112">Attributes and elements</span></span>

<span data-ttu-id="50c47-113">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="50c47-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="50c47-114">Atributos</span><span class="sxs-lookup"><span data-stu-id="50c47-114">Attributes</span></span>

<span data-ttu-id="50c47-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="50c47-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="50c47-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="50c47-116">Child elements</span></span>

|<span data-ttu-id="50c47-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="50c47-117">**Element**</span></span>|<span data-ttu-id="50c47-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="50c47-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50c47-119">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="50c47-119">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="50c47-120">Contém os dias e as horas da semana de trabalho do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="50c47-120">Contains the work week days and hours of the mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="50c47-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="50c47-121">Parent elements</span></span>

|<span data-ttu-id="50c47-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="50c47-122">**Element**</span></span>|<span data-ttu-id="50c47-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="50c47-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50c47-124">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="50c47-124">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md) <br/> |<span data-ttu-id="50c47-125">Representa as configurações de fuso horário e as horas de trabalho do usuário de caixa de correio solicitado.</span><span class="sxs-lookup"><span data-stu-id="50c47-125">Represents the time zone settings and working hours for the requested mailbox user.</span></span>  <br/> <span data-ttu-id="50c47-126">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="50c47-126">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="50c47-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="50c47-127">Remarks</span></span>

<span data-ttu-id="50c47-128">Esse elemento é necessário se o elemento [WorkingHours](workinghours-ex15websvcsotherref.md) for usado.</span><span class="sxs-lookup"><span data-stu-id="50c47-128">This element is required if the [WorkingHours](workinghours-ex15websvcsotherref.md) element is used.</span></span> <span data-ttu-id="50c47-129">Todos os elementos filho são listados na sequência em que ocorrem.</span><span class="sxs-lookup"><span data-stu-id="50c47-129">All the child elements are listed in the sequence in which they occur.</span></span> 
  
<span data-ttu-id="50c47-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="50c47-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="50c47-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="50c47-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="50c47-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="50c47-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="50c47-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="50c47-133">Schema Name</span></span>  <br/> |<span data-ttu-id="50c47-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="50c47-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="50c47-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="50c47-135">Validation File</span></span>  <br/> |<span data-ttu-id="50c47-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="50c47-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="50c47-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="50c47-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="50c47-138">False</span><span class="sxs-lookup"><span data-stu-id="50c47-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="50c47-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="50c47-139">See also</span></span>



[<span data-ttu-id="50c47-140">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="50c47-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="50c47-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="50c47-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="50c47-142">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="50c47-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

