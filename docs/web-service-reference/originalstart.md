---
title: OriginalStart
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OriginalStart
api_type:
- schema
ms.assetid: 4599dd34-15ee-4d57-b886-732081b50784
description: O elemento OriginalStart representa a hora de início original de um item de calendário.
ms.openlocfilehash: 9e5facb3df87ab08e05f23258abdf1767fae64e4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824668"
---
# <a name="originalstart"></a><span data-ttu-id="76eda-103">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="76eda-103">OriginalStart</span></span>

<span data-ttu-id="76eda-104">O elemento **OriginalStart** representa a hora de início original de um item de calendário.</span><span class="sxs-lookup"><span data-stu-id="76eda-104">The **OriginalStart** element represents the original start time of a calendar item.</span></span> 
  
```xml
<OriginalStart/>
```

 <span data-ttu-id="76eda-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="76eda-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="76eda-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="76eda-106">Attributes and elements</span></span>

<span data-ttu-id="76eda-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="76eda-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="76eda-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="76eda-108">Attributes</span></span>

<span data-ttu-id="76eda-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="76eda-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="76eda-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="76eda-110">Child elements</span></span>

<span data-ttu-id="76eda-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="76eda-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="76eda-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="76eda-112">Parent elements</span></span>

|<span data-ttu-id="76eda-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="76eda-113">**Element**</span></span>|<span data-ttu-id="76eda-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="76eda-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76eda-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="76eda-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="76eda-116">Representa um item de calendário no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="76eda-116">Represents a calendar item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="76eda-117">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="76eda-117">FirstOccurrence</span></span>](firstoccurrence.md) <br/> |<span data-ttu-id="76eda-118">Representa a primeira ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="76eda-118">Represents the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="76eda-119">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="76eda-119">LastOccurrence</span></span>](lastoccurrence.md) <br/> |<span data-ttu-id="76eda-120">Representa a última ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="76eda-120">Represents the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="76eda-121">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="76eda-121">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="76eda-122">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="76eda-122">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="76eda-123">Ocorrência</span><span class="sxs-lookup"><span data-stu-id="76eda-123">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="76eda-124">Representa uma única ocorrência de modificação de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="76eda-124">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="76eda-125">Text value</span><span class="sxs-lookup"><span data-stu-id="76eda-125">Text value</span></span>

<span data-ttu-id="76eda-126">Se este elemento for usado, será necessário um valor de texto que representa uma data e hora.</span><span class="sxs-lookup"><span data-stu-id="76eda-126">A text value that represents a date and time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="76eda-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="76eda-127">Remarks</span></span>

<span data-ttu-id="76eda-128">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="76eda-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="76eda-129">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="76eda-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="76eda-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="76eda-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="76eda-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="76eda-131">Schema Name</span></span>  <br/> |<span data-ttu-id="76eda-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="76eda-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="76eda-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="76eda-133">Validation File</span></span>  <br/> |<span data-ttu-id="76eda-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="76eda-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="76eda-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="76eda-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="76eda-136">False</span><span class="sxs-lookup"><span data-stu-id="76eda-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="76eda-137">Ver também</span><span class="sxs-lookup"><span data-stu-id="76eda-137">See also</span></span>



- [<span data-ttu-id="76eda-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="76eda-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

