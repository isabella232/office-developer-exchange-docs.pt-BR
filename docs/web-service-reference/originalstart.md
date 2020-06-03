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
ms.openlocfilehash: 5346a65c432b8e96cb95e412e3e88fbc40ce36e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462364"
---
# <a name="originalstart"></a><span data-ttu-id="f4374-103">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="f4374-103">OriginalStart</span></span>

<span data-ttu-id="f4374-104">O elemento **OriginalStart** representa a hora de início original de um item de calendário.</span><span class="sxs-lookup"><span data-stu-id="f4374-104">The **OriginalStart** element represents the original start time of a calendar item.</span></span> 
  
```xml
<OriginalStart/>
```

 <span data-ttu-id="f4374-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="f4374-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f4374-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f4374-106">Attributes and elements</span></span>

<span data-ttu-id="f4374-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f4374-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f4374-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f4374-108">Attributes</span></span>

<span data-ttu-id="f4374-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f4374-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f4374-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f4374-110">Child elements</span></span>

<span data-ttu-id="f4374-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f4374-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f4374-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f4374-112">Parent elements</span></span>

|<span data-ttu-id="f4374-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f4374-113">**Element**</span></span>|<span data-ttu-id="f4374-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f4374-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4374-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="f4374-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="f4374-116">Representa um item de calendário no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f4374-116">Represents a calendar item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f4374-117">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="f4374-117">FirstOccurrence</span></span>](firstoccurrence.md) <br/> |<span data-ttu-id="f4374-118">Representa a primeira ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="f4374-118">Represents the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="f4374-119">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="f4374-119">LastOccurrence</span></span>](lastoccurrence.md) <br/> |<span data-ttu-id="f4374-120">Representa a última ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="f4374-120">Represents the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="f4374-121">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="f4374-121">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="f4374-122">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f4374-122">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f4374-123">Ocorrência</span><span class="sxs-lookup"><span data-stu-id="f4374-123">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="f4374-124">Representa uma única ocorrência modificada de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="f4374-124">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f4374-125">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="f4374-125">Text value</span></span>

<span data-ttu-id="f4374-126">Um valor de texto que representa uma data e hora será necessário se esse elemento for usado.</span><span class="sxs-lookup"><span data-stu-id="f4374-126">A text value that represents a date and time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f4374-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="f4374-127">Remarks</span></span>

<span data-ttu-id="f4374-128">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f4374-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f4374-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f4374-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f4374-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="f4374-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f4374-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f4374-131">Schema Name</span></span>  <br/> |<span data-ttu-id="f4374-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f4374-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="f4374-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f4374-133">Validation File</span></span>  <br/> |<span data-ttu-id="f4374-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f4374-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f4374-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f4374-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="f4374-136">False</span><span class="sxs-lookup"><span data-stu-id="f4374-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f4374-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="f4374-137">See also</span></span>



- [<span data-ttu-id="f4374-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f4374-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

