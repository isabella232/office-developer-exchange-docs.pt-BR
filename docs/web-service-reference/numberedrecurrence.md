---
title: NumberedRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberedRecurrence
api_type:
- schema
ms.assetid: 53746909-ef21-4764-8715-a7769b943cca
description: O elemento NumberedRecurrence descreve a data de início e o número de ocorrências de um item recorrente.
ms.openlocfilehash: 01fbf831fa7ff378221d4db3d873af730ac564d8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824628"
---
# <a name="numberedrecurrence"></a><span data-ttu-id="917e2-103">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="917e2-103">NumberedRecurrence</span></span>

<span data-ttu-id="917e2-104">O elemento **NumberedRecurrence** descreve a data de início e o número de ocorrências de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="917e2-104">The **NumberedRecurrence** element describes the start date and the number of occurrences of a recurring item.</span></span> 
  
```xml
<NumberedRecurrence>
   <StartDate/>
   <NumberOfOccurrences/>
</NumberedRecurrence>
```

 <span data-ttu-id="917e2-105">**NumberedRecurrenceRangeType**</span><span class="sxs-lookup"><span data-stu-id="917e2-105">**NumberedRecurrenceRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="917e2-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="917e2-106">Attributes and elements</span></span>

<span data-ttu-id="917e2-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="917e2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="917e2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="917e2-108">Attributes</span></span>

<span data-ttu-id="917e2-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="917e2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="917e2-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="917e2-110">Child elements</span></span>

|<span data-ttu-id="917e2-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="917e2-111">**Element**</span></span>|<span data-ttu-id="917e2-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="917e2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="917e2-113">StartDate (recorrência)</span><span class="sxs-lookup"><span data-stu-id="917e2-113">StartDate (Recurrence)</span></span>](startdate-recurrence.md) <br/> |<span data-ttu-id="917e2-114">Representa a data de início de uma tarefa recorrente ou item de calendário.</span><span class="sxs-lookup"><span data-stu-id="917e2-114">Represents the start date of a recurring task or calendar item.</span></span>  <br/> |
|[<span data-ttu-id="917e2-115">NumberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="917e2-115">NumberOfOccurrences</span></span>](numberofoccurrences.md) <br/> |<span data-ttu-id="917e2-116">Contém o número de ocorrências de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="917e2-116">Contains the number of occurrences of a recurring item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="917e2-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="917e2-117">Parent elements</span></span>

|<span data-ttu-id="917e2-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="917e2-118">**Element**</span></span>|<span data-ttu-id="917e2-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="917e2-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="917e2-120">Recorrência (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="917e2-120">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="917e2-121">Contém o padrão de recorrência para itens de calendário e solicitações de reunião.</span><span class="sxs-lookup"><span data-stu-id="917e2-121">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="917e2-122">Recorrência (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="917e2-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="917e2-123">Contém informações de recorrência de tarefas recorrentes.</span><span class="sxs-lookup"><span data-stu-id="917e2-123">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="917e2-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="917e2-124">Remarks</span></span>

<span data-ttu-id="917e2-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="917e2-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="917e2-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="917e2-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="917e2-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="917e2-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="917e2-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="917e2-128">Schema name</span></span>  <br/> |<span data-ttu-id="917e2-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="917e2-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="917e2-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="917e2-130">Validation file</span></span>  <br/> |<span data-ttu-id="917e2-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="917e2-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="917e2-132">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="917e2-132">Can be empty</span></span>  <br/> |<span data-ttu-id="917e2-133">False</span><span class="sxs-lookup"><span data-stu-id="917e2-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="917e2-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="917e2-134">See also</span></span>



- [<span data-ttu-id="917e2-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="917e2-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

