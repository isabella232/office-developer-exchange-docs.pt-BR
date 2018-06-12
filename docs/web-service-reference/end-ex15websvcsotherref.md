---
title: End
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
description: O elemento final representa o fim de uma duração.
ms.openlocfilehash: 90eea4fc545fae083e5675225665e517b502ba6f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752052"
---
# <a name="end"></a><span data-ttu-id="43f2a-103">End</span><span class="sxs-lookup"><span data-stu-id="43f2a-103">End</span></span>

<span data-ttu-id="43f2a-104">O elemento **final** representa o fim de uma duração.</span><span class="sxs-lookup"><span data-stu-id="43f2a-104">The **End** element represents the end of a duration.</span></span> 
  
```xml
<End/>
```

 <span data-ttu-id="43f2a-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="43f2a-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="43f2a-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="43f2a-106">Attributes and elements</span></span>

<span data-ttu-id="43f2a-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="43f2a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="43f2a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="43f2a-108">Attributes</span></span>

<span data-ttu-id="43f2a-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="43f2a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="43f2a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="43f2a-110">Child elements</span></span>

<span data-ttu-id="43f2a-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="43f2a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="43f2a-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="43f2a-112">Parent elements</span></span>

|<span data-ttu-id="43f2a-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="43f2a-113">**Element**</span></span>|<span data-ttu-id="43f2a-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="43f2a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="43f2a-115">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="43f2a-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="43f2a-116">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="43f2a-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="43f2a-117">FirstOccurrence</span><span class="sxs-lookup"><span data-stu-id="43f2a-117">FirstOccurrence</span></span>](firstoccurrence.md) <br/> |<span data-ttu-id="43f2a-118">Representa a primeira ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="43f2a-118">Represents the first occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="43f2a-119">LastOccurrence</span><span class="sxs-lookup"><span data-stu-id="43f2a-119">LastOccurrence</span></span>](lastoccurrence.md) <br/> |<span data-ttu-id="43f2a-120">Representa a última ocorrência de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="43f2a-120">Represents the last occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="43f2a-121">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="43f2a-121">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="43f2a-122">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="43f2a-122">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="43f2a-123">Ocorrência</span><span class="sxs-lookup"><span data-stu-id="43f2a-123">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="43f2a-124">Representa uma única ocorrência de modificação de um item de calendário recorrente.</span><span class="sxs-lookup"><span data-stu-id="43f2a-124">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="43f2a-125">Text value</span><span class="sxs-lookup"><span data-stu-id="43f2a-125">Text value</span></span>

<span data-ttu-id="43f2a-126">O valor de texto representa o fim de uma duração.</span><span class="sxs-lookup"><span data-stu-id="43f2a-126">The text value represents the end of a duration.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="43f2a-127">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="43f2a-127">Remarks</span></span>

<span data-ttu-id="43f2a-128">A operação UpdateItem pode definir a hora de [início](start.md) e **término** de um item de armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="43f2a-128">The UpdateItem operation can set the [Start](start.md) and **End** time of an Exchange store item.</span></span> <span data-ttu-id="43f2a-129">Em uma solicitação de UpdateItem, você pode definir a hora de [início](start.md) sem também definir a hora de **término** .</span><span class="sxs-lookup"><span data-stu-id="43f2a-129">In an UpdateItem request, you can set the [Start](start.md) time without also setting the **End** time.</span></span> <span data-ttu-id="43f2a-130">Isso pode causar um erro se a hora de [início](start.md) é posterior à hora de **término** .</span><span class="sxs-lookup"><span data-stu-id="43f2a-130">This can cause an error if the [Start](start.md) time is later than the **End** time.</span></span> <span data-ttu-id="43f2a-131">Lembre-se de que os aplicativos cliente devem executar ajustes à hora de **término** quando a hora de [início](start.md) for alterada para preservar a duração.</span><span class="sxs-lookup"><span data-stu-id="43f2a-131">Be aware that client applications must perform adjustments to the **End** time when that [Start](start.md) time is changed in order to preserve the duration.</span></span> 
  
 <span data-ttu-id="43f2a-132">**Observação** As informações de deslocamento do fuso horário serão perdidas se as datas de [início](start.md) e **término** do item mestre recorrente não tiver uma data que é igual a primeira ocorrência de um padrão de recorrência semanal.</span><span class="sxs-lookup"><span data-stu-id="43f2a-132">**Note** The time zone offset information is lost if the [Start](start.md) and **End** dates of the recurring master item do not have a date that is equal to the first occurrence of a weekly recurrence pattern.</span></span> 
  
<span data-ttu-id="43f2a-133">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="43f2a-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="43f2a-134">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="43f2a-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="43f2a-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="43f2a-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="43f2a-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="43f2a-136">Schema Name</span></span>  <br/> |<span data-ttu-id="43f2a-137">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="43f2a-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="43f2a-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="43f2a-138">Validation File</span></span>  <br/> |<span data-ttu-id="43f2a-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="43f2a-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="43f2a-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="43f2a-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="43f2a-141">False</span><span class="sxs-lookup"><span data-stu-id="43f2a-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="43f2a-142">Ver também</span><span class="sxs-lookup"><span data-stu-id="43f2a-142">See also</span></span>



[<span data-ttu-id="43f2a-143">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="43f2a-143">WeeklyRecurrence</span></span>](weeklyrecurrence.md)
  
 <span data-ttu-id="43f2a-144">**End**</span><span class="sxs-lookup"><span data-stu-id="43f2a-144">**End**</span></span>


- [<span data-ttu-id="43f2a-145">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="43f2a-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

