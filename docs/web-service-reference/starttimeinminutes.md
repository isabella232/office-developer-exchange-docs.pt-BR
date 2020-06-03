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
description: O elemento StartTimeInMinutes representa o início do dia útil de um usuário de caixa de correio.
ms.openlocfilehash: b33cb12299a146b577dd17939a0585a15d50fb07
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458527"
---
# <a name="starttimeinminutes"></a><span data-ttu-id="6ae51-103">StartTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="6ae51-103">StartTimeInMinutes</span></span>

<span data-ttu-id="6ae51-104">O elemento **StartTimeInMinutes** representa o início do dia útil de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6ae51-104">The **StartTimeInMinutes** element represents the start of the working day for a mailbox user.</span></span> 
  
- [<span data-ttu-id="6ae51-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="6ae51-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
- [<span data-ttu-id="6ae51-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="6ae51-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
- [<span data-ttu-id="6ae51-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="6ae51-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
- [<span data-ttu-id="6ae51-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="6ae51-108">FreeBusyView</span></span>](freebusyview.md)
  
- [<span data-ttu-id="6ae51-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="6ae51-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
- [<span data-ttu-id="6ae51-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="6ae51-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
- [<span data-ttu-id="6ae51-111">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="6ae51-111">WorkingPeriod</span></span>](workingperiod.md)
  
- [<span data-ttu-id="6ae51-112">StartTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="6ae51-112">StartTimeInMinutes</span></span>](starttimeinminutes.md)
  
```xml
<StartTimeInMinutes>...</StartTimeInMinutes>
```

<span data-ttu-id="6ae51-113">**int**</span><span class="sxs-lookup"><span data-stu-id="6ae51-113">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6ae51-114">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6ae51-114">Attributes and elements</span></span>

<span data-ttu-id="6ae51-115">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6ae51-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6ae51-116">Atributos</span><span class="sxs-lookup"><span data-stu-id="6ae51-116">Attributes</span></span>

<span data-ttu-id="6ae51-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6ae51-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6ae51-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6ae51-118">Child elements</span></span>

<span data-ttu-id="6ae51-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6ae51-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6ae51-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6ae51-120">Parent elements</span></span>

|<span data-ttu-id="6ae51-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6ae51-121">**Element**</span></span>|<span data-ttu-id="6ae51-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6ae51-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6ae51-123">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="6ae51-123">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="6ae51-124">Contém os dias e as horas da semana de trabalho do usuário da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6ae51-124">Contains the work week days and hours of the mailbox user.</span></span>  <br/> <span data-ttu-id="6ae51-125">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="6ae51-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6ae51-126">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="6ae51-126">Text value</span></span>

<span data-ttu-id="6ae51-127">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ae51-127">A text value is required.</span></span> <span data-ttu-id="6ae51-128">O valor de texto representa o início do dia útil em quantos minutos foram decorridos desde o início do dia.</span><span class="sxs-lookup"><span data-stu-id="6ae51-128">The text value represents the start of the working day by how many minutes have elapsed since the day began.</span></span> <span data-ttu-id="6ae51-129">Por exemplo, um horário de início de 8 A.M.</span><span class="sxs-lookup"><span data-stu-id="6ae51-129">For example, a start time of 8 A.M.</span></span> <span data-ttu-id="6ae51-130">é representado por 480 minutos.</span><span class="sxs-lookup"><span data-stu-id="6ae51-130">is represented by 480 minutes.</span></span>
  
<span data-ttu-id="6ae51-131">O intervalo de valores possíveis para esse elemento é de 0 a 1440.</span><span class="sxs-lookup"><span data-stu-id="6ae51-131">The range of possible values for this element is 0 to 1440.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6ae51-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="6ae51-132">Remarks</span></span>

<span data-ttu-id="6ae51-133">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="6ae51-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6ae51-134">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6ae51-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6ae51-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="6ae51-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6ae51-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6ae51-136">Schema Name</span></span>  <br/> |<span data-ttu-id="6ae51-137">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="6ae51-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="6ae51-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6ae51-138">Validation File</span></span>  <br/> |<span data-ttu-id="6ae51-139">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6ae51-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6ae51-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6ae51-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="6ae51-141">False</span><span class="sxs-lookup"><span data-stu-id="6ae51-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6ae51-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="6ae51-142">See also</span></span>

- [<span data-ttu-id="6ae51-143">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="6ae51-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="6ae51-144">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="6ae51-144">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="6ae51-145">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="6ae51-145">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

