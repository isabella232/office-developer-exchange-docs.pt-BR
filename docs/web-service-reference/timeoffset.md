---
title: Timeoffset
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
description: O elemento timeoffset representa a diferença de tempo do UTC (tempo Universal Coordenado) para a transição de fuso horário.
ms.openlocfilehash: 8cfd43477f0548227204da9ebc6d7e9307786845
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460285"
---
# <a name="timeoffset"></a><span data-ttu-id="5b2f7-103">Timeoffset</span><span class="sxs-lookup"><span data-stu-id="5b2f7-103">TimeOffset</span></span>

<span data-ttu-id="5b2f7-104">O elemento **timeoffset** representa a diferença de tempo do UTC (tempo Universal Coordenado) para a transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="5b2f7-104">The **TimeOffset** element represents the time offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span> 
  
```XML
<TimeOffset/>
```

 <span data-ttu-id="5b2f7-105">**duration**</span><span class="sxs-lookup"><span data-stu-id="5b2f7-105">**duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5b2f7-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5b2f7-106">Attributes and elements</span></span>

<span data-ttu-id="5b2f7-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5b2f7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5b2f7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5b2f7-108">Attributes</span></span>

<span data-ttu-id="5b2f7-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5b2f7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5b2f7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5b2f7-110">Child elements</span></span>

<span data-ttu-id="5b2f7-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5b2f7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5b2f7-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5b2f7-112">Parent elements</span></span>

|<span data-ttu-id="5b2f7-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5b2f7-113">**Element**</span></span>|<span data-ttu-id="5b2f7-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5b2f7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5b2f7-115">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="5b2f7-115">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="5b2f7-116">Representa uma transição de fuso horário que ocorre em uma data específica por ano.</span><span class="sxs-lookup"><span data-stu-id="5b2f7-116">Represents a time zone transition that occurs on a specific date each year.</span></span>  <br/> |
|[<span data-ttu-id="5b2f7-117">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="5b2f7-117">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="5b2f7-118">Representa uma transição de fuso horário que ocorre no mesmo dia a cada ano.</span><span class="sxs-lookup"><span data-stu-id="5b2f7-118">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5b2f7-119">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="5b2f7-119">Text value</span></span>

<span data-ttu-id="5b2f7-120">O valor de texto do elemento **timeoffset** é uma duração que especifica a diferença de tempo do UTC para a transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="5b2f7-120">The text value of the **TimeOffset** element is a duration that specifies the time offset from UTC for the time zone transition.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5b2f7-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="5b2f7-121">Remarks</span></span>

<span data-ttu-id="5b2f7-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5b2f7-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5b2f7-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5b2f7-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5b2f7-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="5b2f7-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5b2f7-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5b2f7-125">Schema Name</span></span>  <br/> |<span data-ttu-id="5b2f7-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5b2f7-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="5b2f7-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5b2f7-127">Validation File</span></span>  <br/> |<span data-ttu-id="5b2f7-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5b2f7-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5b2f7-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5b2f7-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="5b2f7-130">False</span><span class="sxs-lookup"><span data-stu-id="5b2f7-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5b2f7-131">Confira também</span><span class="sxs-lookup"><span data-stu-id="5b2f7-131">See also</span></span>



- [<span data-ttu-id="5b2f7-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="5b2f7-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

