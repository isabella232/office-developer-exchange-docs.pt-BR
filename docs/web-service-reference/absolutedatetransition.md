---
title: AbsoluteDateTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AbsoluteDateTransition
api_type:
- schema
ms.assetid: 8f5731eb-bed0-45bf-ba89-4aaf20c34a39
description: O elemento AbsoluteDateTransition representa uma transição de fuso horário que ocorre em uma data específica e, em um momento específico.
ms.openlocfilehash: 1e9e5f3f2269814a82b827efe46c71a172e21348
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751034"
---
# <a name="absolutedatetransition"></a><span data-ttu-id="1b28e-103">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="1b28e-103">AbsoluteDateTransition</span></span>

<span data-ttu-id="1b28e-104">O elemento **AbsoluteDateTransition** representa uma transição de fuso horário que ocorre em uma data específica e, em um momento específico.</span><span class="sxs-lookup"><span data-stu-id="1b28e-104">The **AbsoluteDateTransition** element represents a time zone transition that occurs on a specific date and at a specific time.</span></span> 
  
```xml
<AbsoluteDateTransition>
   <To/>
   <DateTime/>
</AbsoluteDateTransition>
```

<span data-ttu-id="1b28e-105">**AbsoluteDateTransitionType**</span><span class="sxs-lookup"><span data-stu-id="1b28e-105">**AbsoluteDateTransitionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1b28e-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="1b28e-106">Attributes and elements</span></span>

<span data-ttu-id="1b28e-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1b28e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1b28e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1b28e-108">Attributes</span></span>

<span data-ttu-id="1b28e-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1b28e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1b28e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1b28e-110">Child elements</span></span>

|<span data-ttu-id="1b28e-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1b28e-111">**Element**</span></span>|<span data-ttu-id="1b28e-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1b28e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b28e-113">To</span><span class="sxs-lookup"><span data-stu-id="1b28e-113">To</span></span>](to.md) <br/> |<span data-ttu-id="1b28e-114">Especifica o [período](period.md) ou [TransitionsGroup](transitionsgroup.md) que é o destino da transição fuso horário.</span><span class="sxs-lookup"><span data-stu-id="1b28e-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="1b28e-115">DateTime</span><span class="sxs-lookup"><span data-stu-id="1b28e-115">DateTime</span></span>](datetime.md) <br/> |<span data-ttu-id="1b28e-116">Representa a data e hora em que ocorre a transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="1b28e-116">Represents the date and time at which the time zone transition occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1b28e-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1b28e-117">Parent elements</span></span>

|<span data-ttu-id="1b28e-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1b28e-118">**Element**</span></span>|<span data-ttu-id="1b28e-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1b28e-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b28e-120">Transições</span><span class="sxs-lookup"><span data-stu-id="1b28e-120">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="1b28e-121">Representa uma coleção de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="1b28e-121">Represents a collection of time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="1b28e-122">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="1b28e-122">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="1b28e-123">Representa uma coleção de transições de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="1b28e-123">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1b28e-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="1b28e-124">Remarks</span></span>

<span data-ttu-id="1b28e-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b28e-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1b28e-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="1b28e-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1b28e-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="1b28e-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1b28e-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1b28e-128">Schema Name</span></span>  <br/> |<span data-ttu-id="1b28e-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="1b28e-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="1b28e-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1b28e-130">Validation File</span></span>  <br/> |<span data-ttu-id="1b28e-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1b28e-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1b28e-132">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1b28e-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="1b28e-133">False</span><span class="sxs-lookup"><span data-stu-id="1b28e-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1b28e-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="1b28e-134">See also</span></span>

- [<span data-ttu-id="1b28e-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1b28e-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

