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
ms.openlocfilehash: 5c66614520f9d616687d67ad609b3d55d9cf6571
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458926"
---
# <a name="timewindow"></a><span data-ttu-id="2cd14-103">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="2cd14-103">TimeWindow</span></span>

<span data-ttu-id="2cd14-104">O elemento **TimeWindow** identifica o intervalo de tempo consultado para as informações de disponibilidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="2cd14-104">The **TimeWindow** element identifies the time span queried for the user availability information.</span></span> 
  
[<span data-ttu-id="2cd14-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="2cd14-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="2cd14-106">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="2cd14-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
[<span data-ttu-id="2cd14-107">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="2cd14-107">TimeWindow</span></span>](timewindow.md)
  
```xml
<TimeWindow>
   <StartTime>dateTime</StartTime>
   <EndTime>dateTime</EndTime>
</TimeWindow>
```

 <span data-ttu-id="2cd14-108">**Duration**</span><span class="sxs-lookup"><span data-stu-id="2cd14-108">**Duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2cd14-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="2cd14-109">Attributes and elements</span></span>

<span data-ttu-id="2cd14-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="2cd14-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2cd14-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="2cd14-111">Attributes</span></span>

<span data-ttu-id="2cd14-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2cd14-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2cd14-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="2cd14-113">Child elements</span></span>

|<span data-ttu-id="2cd14-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2cd14-114">**Element**</span></span>|<span data-ttu-id="2cd14-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2cd14-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2cd14-116">StartTime</span><span class="sxs-lookup"><span data-stu-id="2cd14-116">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="2cd14-117">Representa o início de um período de tempo consultado para as informações de disponibilidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="2cd14-117">Represents the start of a time span queried for the user availability information.</span></span>  <br/> |
|[<span data-ttu-id="2cd14-118">EndTime</span><span class="sxs-lookup"><span data-stu-id="2cd14-118">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="2cd14-119">Representa o final de um período de tempo consultado para as informações de disponibilidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="2cd14-119">Represents the end of a time span queried for the user availability information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2cd14-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="2cd14-120">Parent elements</span></span>

|<span data-ttu-id="2cd14-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2cd14-121">**Element**</span></span>|<span data-ttu-id="2cd14-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2cd14-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2cd14-123">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="2cd14-123">FreeBusyViewOptions</span></span>](freebusyviewoptions.md) <br/> |<span data-ttu-id="2cd14-124">Especifica o tipo de informações de disponibilidade retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="2cd14-124">Specifies the type of free/busy information returned in the response.</span></span>  <br/> <span data-ttu-id="2cd14-125">Este é o XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="2cd14-125">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2cd14-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="2cd14-126">Remarks</span></span>

<span data-ttu-id="2cd14-127">O valor máximo para esse período de tempo é de 42 dias.</span><span class="sxs-lookup"><span data-stu-id="2cd14-127">The maximum value for this time period is 42 days.</span></span> <span data-ttu-id="2cd14-128">Esse valor máximo pode ser modificado.</span><span class="sxs-lookup"><span data-stu-id="2cd14-128">This maximum value can be modified.</span></span> <span data-ttu-id="2cd14-129">Todas as solicitações de informações de disponibilidade do usuário além do valor máximo retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="2cd14-129">Any requests for user availability information beyond the maximum value will return an error.</span></span> <span data-ttu-id="2cd14-130">Se algum compromisso estiver parcialmente no intervalo de tempo definido pelos elementos [StartTime](starttime.md) e [EndTime](endtime.md) , esse compromisso será incluído em sua totalidade.</span><span class="sxs-lookup"><span data-stu-id="2cd14-130">If any appointments are partially in the time span defined by the [StartTime](starttime.md) and [EndTime](endtime.md) elements, that appointment is included in its entirety.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="2cd14-131">O esquema que descreve este elemento está localizado no diretório/EWS/do computador que está executando o Microsoft® Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="2cd14-131">The schema that describes this element is located in the /EWS/ directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="2cd14-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="2cd14-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2cd14-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="2cd14-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2cd14-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="2cd14-134">Schema Name</span></span>  <br/> |<span data-ttu-id="2cd14-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="2cd14-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="2cd14-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="2cd14-136">Validation File</span></span>  <br/> |<span data-ttu-id="2cd14-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2cd14-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2cd14-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="2cd14-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="2cd14-139">False</span><span class="sxs-lookup"><span data-stu-id="2cd14-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2cd14-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="2cd14-140">See also</span></span>



[<span data-ttu-id="2cd14-141">Operação GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="2cd14-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="2cd14-142">Obtendo disponibilidade do usuário</span><span class="sxs-lookup"><span data-stu-id="2cd14-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

