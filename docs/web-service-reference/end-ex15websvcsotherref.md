---
title: Final
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- End
api_type:
- schema
ms.assetid: 72329821-32ff-495d-b6e5-fdc011003c2e
description: O elemento final representa o final de uma duração.
ms.openlocfilehash: d36f555d2ac9c0c1d82053029720ec17a53f2d92
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456140"
---
# <a name="end"></a><span data-ttu-id="05079-103">Final</span><span class="sxs-lookup"><span data-stu-id="05079-103">End</span></span>

<span data-ttu-id="05079-104">O elemento **final** representa o final de uma duração.</span><span class="sxs-lookup"><span data-stu-id="05079-104">The **End** element represents the end of a duration.</span></span> 
  
```xml
<End/>
```

 <span data-ttu-id="05079-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="05079-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="05079-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="05079-106">Attributes and elements</span></span>

<span data-ttu-id="05079-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="05079-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05079-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="05079-108">Attributes</span></span>

<span data-ttu-id="05079-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="05079-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05079-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="05079-110">Child elements</span></span>

<span data-ttu-id="05079-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="05079-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="05079-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="05079-112">Parent elements</span></span>

|<span data-ttu-id="05079-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="05079-113">**Element**</span></span>|<span data-ttu-id="05079-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="05079-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05079-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="05079-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="05079-116">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="05079-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="05079-117">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="05079-117">FirstOccurrence</span></span>](firstoccurrence.md) <br/> |<span data-ttu-id="05079-118">Representa a primeira ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="05079-118">Represents the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="05079-119">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="05079-119">LastOccurrence</span></span>](lastoccurrence.md) <br/> |<span data-ttu-id="05079-120">Representa a última ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="05079-120">Represents the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="05079-121">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="05079-121">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="05079-122">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="05079-122">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="05079-123">Ocorrência</span><span class="sxs-lookup"><span data-stu-id="05079-123">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="05079-124">Representa uma única ocorrência modificada de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="05079-124">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="05079-125">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="05079-125">Text value</span></span>

<span data-ttu-id="05079-126">O valor de texto representa o final de uma duração.</span><span class="sxs-lookup"><span data-stu-id="05079-126">The text value represents the end of a duration.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="05079-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="05079-127">Remarks</span></span>

<span data-ttu-id="05079-128">A operação UpdateItem pode definir a hora de [início](start.md) e de **término** de um item do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="05079-128">The UpdateItem operation can set the [Start](start.md) and **End** time of an Exchange store item.</span></span> <span data-ttu-id="05079-129">Em uma solicitação UpdateItem, você pode definir a hora de [início](start.md) sem definir a hora de **término** .</span><span class="sxs-lookup"><span data-stu-id="05079-129">In an UpdateItem request, you can set the [Start](start.md) time without also setting the **End** time.</span></span> <span data-ttu-id="05079-130">Isso pode causar um erro se a hora de [início](start.md) for posterior à hora de **término** .</span><span class="sxs-lookup"><span data-stu-id="05079-130">This can cause an error if the [Start](start.md) time is later than the **End** time.</span></span> <span data-ttu-id="05079-131">Lembre-se de que os aplicativos cliente devem realizar ajustes na hora de **término** em que a hora de [início](start.md) é alterada para preservar a duração.</span><span class="sxs-lookup"><span data-stu-id="05079-131">Be aware that client applications must perform adjustments to the **End** time when that [Start](start.md) time is changed in order to preserve the duration.</span></span> 
  
 <span data-ttu-id="05079-132">**Observação** As informações de deslocamento de fuso horário serão perdidas se as datas de [início](start.md) e **término** do item mestre recorrente não tiverem uma data igual à primeira ocorrência de um padrão de recorrência semanal.</span><span class="sxs-lookup"><span data-stu-id="05079-132">**Note** The time zone offset information is lost if the [Start](start.md) and **End** dates of the recurring master item do not have a date that is equal to the first occurrence of a weekly recurrence pattern.</span></span> 
  
<span data-ttu-id="05079-133">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="05079-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05079-134">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="05079-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05079-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="05079-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="05079-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="05079-136">Schema Name</span></span>  <br/> |<span data-ttu-id="05079-137">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="05079-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="05079-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="05079-138">Validation File</span></span>  <br/> |<span data-ttu-id="05079-139">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="05079-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="05079-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="05079-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="05079-141">False</span><span class="sxs-lookup"><span data-stu-id="05079-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="05079-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="05079-142">See also</span></span>



[<span data-ttu-id="05079-143">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="05079-143">WeeklyRecurrence</span></span>](weeklyrecurrence.md)
  
 <span data-ttu-id="05079-144">**End**</span><span class="sxs-lookup"><span data-stu-id="05079-144">**End**</span></span>


- [<span data-ttu-id="05079-145">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="05079-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

