---
title: Mês (transição de fuso horário)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Month
api_type:
- schema
ms.assetid: 5e6aac75-366d-43d0-8ccb-956285474662
description: O elemento de mês representa o mês em que ocorre a transição de fuso horário.
ms.openlocfilehash: 887bd750b9cad1e28e6f7603c7b3289da8f8dc07
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824483"
---
# <a name="month-time-zone-transition"></a><span data-ttu-id="40eb9-103">Mês (transição de fuso horário)</span><span class="sxs-lookup"><span data-stu-id="40eb9-103">Month (Time Zone Transition)</span></span>

<span data-ttu-id="40eb9-104">O elemento de **mês** representa o mês em que ocorre a transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="40eb9-104">The **Month** element represents the month in which the time zone transition occurs.</span></span> 
  
```xml
<Month/>
```

 <span data-ttu-id="40eb9-105">**int**</span><span class="sxs-lookup"><span data-stu-id="40eb9-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="40eb9-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="40eb9-106">Attributes and elements</span></span>

<span data-ttu-id="40eb9-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="40eb9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="40eb9-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="40eb9-108">Attributes</span></span>

<span data-ttu-id="40eb9-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="40eb9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="40eb9-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="40eb9-110">Child elements</span></span>

<span data-ttu-id="40eb9-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="40eb9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="40eb9-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="40eb9-112">Parent elements</span></span>

|<span data-ttu-id="40eb9-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="40eb9-113">**Element**</span></span>|<span data-ttu-id="40eb9-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="40eb9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40eb9-115">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="40eb9-115">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="40eb9-116">Representa uma transição de fuso horário que ocorre em uma data específica de cada ano.</span><span class="sxs-lookup"><span data-stu-id="40eb9-116">Represents a time zone transition that occurs on a specific date each year.</span></span>  <br/> |
|[<span data-ttu-id="40eb9-117">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="40eb9-117">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="40eb9-118">Representa uma transição de fuso horário que ocorre no mesmo dia cada ano.</span><span class="sxs-lookup"><span data-stu-id="40eb9-118">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="40eb9-119">Text value</span><span class="sxs-lookup"><span data-stu-id="40eb9-119">Text value</span></span>

<span data-ttu-id="40eb9-120">O valor de texto é um inteiro que representa o mês em que ocorre a transição de fuso horário.</span><span class="sxs-lookup"><span data-stu-id="40eb9-120">The text value is an integer that represents the month in which the time zone transition occurs.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="40eb9-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="40eb9-121">Remarks</span></span>

<span data-ttu-id="40eb9-122">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="40eb9-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="40eb9-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="40eb9-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="40eb9-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="40eb9-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="40eb9-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="40eb9-125">Schema Name</span></span>  <br/> |<span data-ttu-id="40eb9-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="40eb9-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="40eb9-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="40eb9-127">Validation File</span></span>  <br/> |<span data-ttu-id="40eb9-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="40eb9-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="40eb9-129">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="40eb9-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="40eb9-130">False</span><span class="sxs-lookup"><span data-stu-id="40eb9-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="40eb9-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="40eb9-131">See also</span></span>



- [<span data-ttu-id="40eb9-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="40eb9-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

