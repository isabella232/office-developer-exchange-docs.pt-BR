---
title: TimeOffset
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeOffset
api_type:
- schema
ms.assetid: b70bf498-cc3a-4fa6-8236-514acb973b33
description: O elemento TimeOffset representa o deslocamento de tempo do tempo Universal Coordenado (UTC) para a transição de fuso horário.
ms.openlocfilehash: 46b1b2c8eec9bae871b4dafe43036e9d725075ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837725"
---
# <a name="timeoffset"></a><span data-ttu-id="01c32-103">TimeOffset</span><span class="sxs-lookup"><span data-stu-id="01c32-103">TimeOffset</span></span>

<span data-ttu-id="01c32-104">O elemento **TimeOffset** representa o deslocamento de tempo do tempo Universal Coordenado (UTC) para a transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="01c32-104">The **TimeOffset** element represents the time offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span> 
  
```XML
<TimeOffset/>
```

 <span data-ttu-id="01c32-105">**duration**</span><span class="sxs-lookup"><span data-stu-id="01c32-105">**duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="01c32-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="01c32-106">Attributes and elements</span></span>

<span data-ttu-id="01c32-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="01c32-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01c32-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="01c32-108">Attributes</span></span>

<span data-ttu-id="01c32-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="01c32-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="01c32-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="01c32-110">Child elements</span></span>

<span data-ttu-id="01c32-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="01c32-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="01c32-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="01c32-112">Parent elements</span></span>

|<span data-ttu-id="01c32-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="01c32-113">**Element**</span></span>|<span data-ttu-id="01c32-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="01c32-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01c32-115">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="01c32-115">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="01c32-116">Representa uma transição de fuso horário que ocorre em uma data específica de cada ano.</span><span class="sxs-lookup"><span data-stu-id="01c32-116">Represents a time zone transition that occurs on a specific date each year.</span></span>  <br/> |
|[<span data-ttu-id="01c32-117">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="01c32-117">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="01c32-118">Representa uma transição de fuso horário que ocorre no mesmo dia cada ano.</span><span class="sxs-lookup"><span data-stu-id="01c32-118">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="01c32-119">Text value</span><span class="sxs-lookup"><span data-stu-id="01c32-119">Text value</span></span>

<span data-ttu-id="01c32-120">O valor de texto do elemento **TimeOffset** é uma duração que especifica o deslocamento de tempo de UTC para a transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="01c32-120">The text value of the **TimeOffset** element is a duration that specifies the time offset from UTC for the time zone transition.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="01c32-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="01c32-121">Remarks</span></span>

<span data-ttu-id="01c32-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="01c32-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01c32-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="01c32-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01c32-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="01c32-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="01c32-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="01c32-125">Schema Name</span></span>  <br/> |<span data-ttu-id="01c32-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="01c32-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="01c32-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="01c32-127">Validation File</span></span>  <br/> |<span data-ttu-id="01c32-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="01c32-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="01c32-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="01c32-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="01c32-130">False</span><span class="sxs-lookup"><span data-stu-id="01c32-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="01c32-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="01c32-131">See also</span></span>



- [<span data-ttu-id="01c32-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="01c32-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

