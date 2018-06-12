---
title: EndTimeInMinutes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndTimeInMinutes
api_type:
- schema
ms.assetid: ef05bdda-7a66-44db-bb73-a2ce8316c257
description: O elemento EndTimeInMinutes representa o final do dia útil para um usuário de caixa de correio.
ms.openlocfilehash: 2885d810512eb0e575aa25b4f38d28332a10b8f2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752082"
---
# <a name="endtimeinminutes"></a><span data-ttu-id="046ff-103">EndTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="046ff-103">EndTimeInMinutes</span></span>

<span data-ttu-id="046ff-104">O elemento **EndTimeInMinutes** representa o final do dia útil para um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="046ff-104">The **EndTimeInMinutes** element represents the end of the working day for a mailbox user.</span></span> 
  
[<span data-ttu-id="046ff-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="046ff-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="046ff-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="046ff-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="046ff-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="046ff-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="046ff-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="046ff-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="046ff-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="046ff-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
[<span data-ttu-id="046ff-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="046ff-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
[<span data-ttu-id="046ff-111">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="046ff-111">WorkingPeriod</span></span>](workingperiod.md)
  
[<span data-ttu-id="046ff-112">EndTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="046ff-112">EndTimeInMinutes</span></span>](endtimeinminutes.md)
  
```xml
<StartTimeInMinutes>...</StartTimeInMinutes>
```

 <span data-ttu-id="046ff-113">**int**</span><span class="sxs-lookup"><span data-stu-id="046ff-113">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="046ff-114">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="046ff-114">Attributes and elements</span></span>

<span data-ttu-id="046ff-115">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="046ff-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="046ff-116">Atributos</span><span class="sxs-lookup"><span data-stu-id="046ff-116">Attributes</span></span>

<span data-ttu-id="046ff-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="046ff-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="046ff-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="046ff-118">Child elements</span></span>

<span data-ttu-id="046ff-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="046ff-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="046ff-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="046ff-120">Parent elements</span></span>

|<span data-ttu-id="046ff-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="046ff-121">**Element**</span></span>|<span data-ttu-id="046ff-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="046ff-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="046ff-123">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="046ff-123">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="046ff-124">Contém a semana de trabalho dias e horas do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="046ff-124">Contains the work week days and hours of the mailbox user.</span></span>  <br/> <span data-ttu-id="046ff-125">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="046ff-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="046ff-126">Text value</span><span class="sxs-lookup"><span data-stu-id="046ff-126">Text value</span></span>

<span data-ttu-id="046ff-127">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="046ff-127">A text value is required.</span></span> <span data-ttu-id="046ff-128">O valor de texto representa o final do dia útil por quantos minutos decorridos desde o início do dia.</span><span class="sxs-lookup"><span data-stu-id="046ff-128">The text value represents the end of the working day by how many minutes have elapsed since the day began.</span></span> <span data-ttu-id="046ff-129">Por exemplo, uma hora de término das 18h00</span><span class="sxs-lookup"><span data-stu-id="046ff-129">For example, an end time of 6 P.M.</span></span> <span data-ttu-id="046ff-130">é representado por 1080 minutos.</span><span class="sxs-lookup"><span data-stu-id="046ff-130">is represented by 1080 minutes.</span></span>
  
<span data-ttu-id="046ff-131">O intervalo de valores possíveis para esse elemento é de 0 a 1440.</span><span class="sxs-lookup"><span data-stu-id="046ff-131">The range of possible values for this element is 0 to 1440.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="046ff-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="046ff-132">Remarks</span></span>

<span data-ttu-id="046ff-133">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="046ff-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="046ff-134">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="046ff-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="046ff-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="046ff-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="046ff-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="046ff-136">Schema Name</span></span>  <br/> |<span data-ttu-id="046ff-137">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="046ff-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="046ff-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="046ff-138">Validation File</span></span>  <br/> |<span data-ttu-id="046ff-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="046ff-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="046ff-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="046ff-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="046ff-141">False</span><span class="sxs-lookup"><span data-stu-id="046ff-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="046ff-142">Ver também</span><span class="sxs-lookup"><span data-stu-id="046ff-142">See also</span></span>



[<span data-ttu-id="046ff-143">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="046ff-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="046ff-144">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="046ff-144">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="046ff-145">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="046ff-145">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

