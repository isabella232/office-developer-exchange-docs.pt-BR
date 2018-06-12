---
title: TimeWindow
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeWindow
api_type:
- schema
ms.assetid: 49c79266-353a-4036-a8e2-8a4660d0d8ea
description: O elemento TimeWindow identifica o intervalo de tempo consultado para as informações de disponibilidade do usuário.
ms.openlocfilehash: 05858b4d62b72b3ff9904c90652bb1bff78ceb41
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837749"
---
# <a name="timewindow"></a><span data-ttu-id="00d58-103">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="00d58-103">TimeWindow</span></span>

<span data-ttu-id="00d58-104">O elemento **TimeWindow** identifica o intervalo de tempo consultado para as informações de disponibilidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="00d58-104">The **TimeWindow** element identifies the time span queried for the user availability information.</span></span> 
  
[<span data-ttu-id="00d58-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="00d58-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="00d58-106">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="00d58-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
[<span data-ttu-id="00d58-107">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="00d58-107">TimeWindow</span></span>](timewindow.md)
  
```xml
<TimeWindow>
   <StartTime>dateTime</StartTime>
   <EndTime>dateTime</EndTime>
</TimeWindow>
```

 <span data-ttu-id="00d58-108">**Duração**</span><span class="sxs-lookup"><span data-stu-id="00d58-108">**Duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="00d58-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="00d58-109">Attributes and elements</span></span>

<span data-ttu-id="00d58-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="00d58-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00d58-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="00d58-111">Attributes</span></span>

<span data-ttu-id="00d58-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="00d58-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="00d58-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="00d58-113">Child elements</span></span>

|<span data-ttu-id="00d58-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="00d58-114">**Element**</span></span>|<span data-ttu-id="00d58-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="00d58-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00d58-116">StartTime</span><span class="sxs-lookup"><span data-stu-id="00d58-116">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="00d58-117">Representa o início de um período de tempo consultado para as informações de disponibilidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="00d58-117">Represents the start of a time span queried for the user availability information.</span></span>  <br/> |
|[<span data-ttu-id="00d58-118">EndTime</span><span class="sxs-lookup"><span data-stu-id="00d58-118">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="00d58-119">Representa o final de um período de tempo consultado para as informações de disponibilidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="00d58-119">Represents the end of a time span queried for the user availability information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="00d58-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="00d58-120">Parent elements</span></span>

|<span data-ttu-id="00d58-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="00d58-121">**Element**</span></span>|<span data-ttu-id="00d58-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="00d58-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00d58-123">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="00d58-123">FreeBusyViewOptions</span></span>](freebusyviewoptions.md) <br/> |<span data-ttu-id="00d58-124">Especifica o tipo de informações de disponibilidade retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="00d58-124">Specifies the type of free/busy information returned in the response.</span></span>  <br/> <span data-ttu-id="00d58-125">Este é o XPath a este elemento:</span><span class="sxs-lookup"><span data-stu-id="00d58-125">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="00d58-126">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="00d58-126">Remarks</span></span>

<span data-ttu-id="00d58-127">O valor máximo por este período é 42 dias.</span><span class="sxs-lookup"><span data-stu-id="00d58-127">The maximum value for this time period is 42 days.</span></span> <span data-ttu-id="00d58-128">Esse valor máximo pode ser modificado.</span><span class="sxs-lookup"><span data-stu-id="00d58-128">This maximum value can be modified.</span></span> <span data-ttu-id="00d58-129">Quaisquer solicitações para obter informações de disponibilidade do usuário além o valor máximo retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="00d58-129">Any requests for user availability information beyond the maximum value will return an error.</span></span> <span data-ttu-id="00d58-130">Se todos os compromissos parcialmente do intervalo de tempo definido pelos elementos [StartTime](starttime.md) e [EndTime](endtime.md) , esse compromisso está incluído na íntegra.</span><span class="sxs-lookup"><span data-stu-id="00d58-130">If any appointments are partially in the time span defined by the [StartTime](starttime.md) and [EndTime](endtime.md) elements, that appointment is included in its entirety.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="00d58-131">O esquema que descreve este elemento está localizado no diretório /EWS/ do computador que está executando o Microsoft® Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="00d58-131">The schema that describes this element is located in the /EWS/ directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="00d58-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="00d58-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00d58-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="00d58-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="00d58-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="00d58-134">Schema Name</span></span>  <br/> |<span data-ttu-id="00d58-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="00d58-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="00d58-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="00d58-136">Validation File</span></span>  <br/> |<span data-ttu-id="00d58-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="00d58-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="00d58-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="00d58-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="00d58-139">False</span><span class="sxs-lookup"><span data-stu-id="00d58-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="00d58-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="00d58-140">See also</span></span>



[<span data-ttu-id="00d58-141">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="00d58-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="00d58-142">Obtenção de disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="00d58-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

