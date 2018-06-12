---
title: StartTimeInMinutes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartTimeInMinutes
api_type:
- schema
ms.assetid: 0fb60a78-6e79-4601-8e2f-5bd245c46d69
description: O elemento StartTimeInMinutes representa o início do dia útil para um usuário de caixa de correio.
ms.openlocfilehash: f3f1d26731d0406ff8a0fd45fc0243a9feabf886
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825558"
---
# <a name="starttimeinminutes"></a><span data-ttu-id="cf45d-103">StartTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="cf45d-103">StartTimeInMinutes</span></span>

<span data-ttu-id="cf45d-104">O elemento **StartTimeInMinutes** representa o início do dia útil para um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="cf45d-104">The **StartTimeInMinutes** element represents the start of the working day for a mailbox user.</span></span> 
  
- [<span data-ttu-id="cf45d-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="cf45d-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
- [<span data-ttu-id="cf45d-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="cf45d-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
- [<span data-ttu-id="cf45d-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="cf45d-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
- [<span data-ttu-id="cf45d-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="cf45d-108">FreeBusyView</span></span>](freebusyview.md)
  
- [<span data-ttu-id="cf45d-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="cf45d-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
- [<span data-ttu-id="cf45d-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="cf45d-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
- [<span data-ttu-id="cf45d-111">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="cf45d-111">WorkingPeriod</span></span>](workingperiod.md)
  
- [<span data-ttu-id="cf45d-112">StartTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="cf45d-112">StartTimeInMinutes</span></span>](starttimeinminutes.md)
  
```xml
<StartTimeInMinutes>...</StartTimeInMinutes>
```

<span data-ttu-id="cf45d-113">**int**</span><span class="sxs-lookup"><span data-stu-id="cf45d-113">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="cf45d-114">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="cf45d-114">Attributes and elements</span></span>

<span data-ttu-id="cf45d-115">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cf45d-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf45d-116">Atributos</span><span class="sxs-lookup"><span data-stu-id="cf45d-116">Attributes</span></span>

<span data-ttu-id="cf45d-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cf45d-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf45d-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cf45d-118">Child elements</span></span>

<span data-ttu-id="cf45d-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cf45d-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cf45d-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cf45d-120">Parent elements</span></span>

|<span data-ttu-id="cf45d-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cf45d-121">**Element**</span></span>|<span data-ttu-id="cf45d-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cf45d-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf45d-123">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="cf45d-123">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="cf45d-124">Contém a semana de trabalho dias e horas do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="cf45d-124">Contains the work week days and hours of the mailbox user.</span></span>  <br/> <span data-ttu-id="cf45d-125">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="cf45d-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cf45d-126">Text value</span><span class="sxs-lookup"><span data-stu-id="cf45d-126">Text value</span></span>

<span data-ttu-id="cf45d-127">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="cf45d-127">A text value is required.</span></span> <span data-ttu-id="cf45d-128">O valor de texto representa o início do dia útil por quantos minutos decorridos desde o início do dia.</span><span class="sxs-lookup"><span data-stu-id="cf45d-128">The text value represents the start of the working day by how many minutes have elapsed since the day began.</span></span> <span data-ttu-id="cf45d-129">Por exemplo, uma hora de início das 8: 00</span><span class="sxs-lookup"><span data-stu-id="cf45d-129">For example, a start time of 8 A.M.</span></span> <span data-ttu-id="cf45d-130">é representado por 480 minutos.</span><span class="sxs-lookup"><span data-stu-id="cf45d-130">is represented by 480 minutes.</span></span>
  
<span data-ttu-id="cf45d-131">O intervalo de valores possíveis para esse elemento é de 0 a 1440.</span><span class="sxs-lookup"><span data-stu-id="cf45d-131">The range of possible values for this element is 0 to 1440.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cf45d-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="cf45d-132">Remarks</span></span>

<span data-ttu-id="cf45d-133">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="cf45d-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cf45d-134">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="cf45d-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf45d-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="cf45d-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cf45d-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cf45d-136">Schema Name</span></span>  <br/> |<span data-ttu-id="cf45d-137">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="cf45d-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="cf45d-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cf45d-138">Validation File</span></span>  <br/> |<span data-ttu-id="cf45d-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cf45d-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cf45d-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="cf45d-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="cf45d-141">False</span><span class="sxs-lookup"><span data-stu-id="cf45d-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cf45d-142">Ver também</span><span class="sxs-lookup"><span data-stu-id="cf45d-142">See also</span></span>

- [<span data-ttu-id="cf45d-143">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="cf45d-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="cf45d-144">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="cf45d-144">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="cf45d-145">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="cf45d-145">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

