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
ms.openlocfilehash: 000674e5b0bad9deea5aa4ac78d41135a922c755
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465937"
---
# <a name="numberedrecurrence"></a><span data-ttu-id="20e73-103">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="20e73-103">NumberedRecurrence</span></span>

<span data-ttu-id="20e73-104">O elemento **NumberedRecurrence** descreve a data de início e o número de ocorrências de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="20e73-104">The **NumberedRecurrence** element describes the start date and the number of occurrences of a recurring item.</span></span> 
  
```xml
<NumberedRecurrence>
   <StartDate/>
   <NumberOfOccurrences/>
</NumberedRecurrence>
```

 <span data-ttu-id="20e73-105">**NumberedRecurrenceRangeType**</span><span class="sxs-lookup"><span data-stu-id="20e73-105">**NumberedRecurrenceRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="20e73-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="20e73-106">Attributes and elements</span></span>

<span data-ttu-id="20e73-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="20e73-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="20e73-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="20e73-108">Attributes</span></span>

<span data-ttu-id="20e73-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="20e73-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="20e73-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="20e73-110">Child elements</span></span>

|<span data-ttu-id="20e73-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="20e73-111">**Element**</span></span>|<span data-ttu-id="20e73-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="20e73-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20e73-113">StartDate (recorrência)</span><span class="sxs-lookup"><span data-stu-id="20e73-113">StartDate (Recurrence)</span></span>](startdate-recurrence.md) <br/> |<span data-ttu-id="20e73-114">Representa a data de início de um item de calendário ou tarefa recorrente.</span><span class="sxs-lookup"><span data-stu-id="20e73-114">Represents the start date of a recurring task or calendar item.</span></span>  <br/> |
|[<span data-ttu-id="20e73-115">NumberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="20e73-115">NumberOfOccurrences</span></span>](numberofoccurrences.md) <br/> |<span data-ttu-id="20e73-116">Contém o número de ocorrências de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="20e73-116">Contains the number of occurrences of a recurring item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="20e73-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="20e73-117">Parent elements</span></span>

|<span data-ttu-id="20e73-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="20e73-118">**Element**</span></span>|<span data-ttu-id="20e73-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="20e73-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20e73-120">Recurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="20e73-120">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="20e73-121">Contém o padrão de recorrência para itens de calendário e solicitações de reunião.</span><span class="sxs-lookup"><span data-stu-id="20e73-121">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="20e73-122">Recorrência (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="20e73-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="20e73-123">Contém informações de recorrência para tarefas recorrentes.</span><span class="sxs-lookup"><span data-stu-id="20e73-123">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="20e73-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="20e73-124">Remarks</span></span>

<span data-ttu-id="20e73-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="20e73-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="20e73-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="20e73-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="20e73-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="20e73-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="20e73-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="20e73-128">Schema name</span></span>  <br/> |<span data-ttu-id="20e73-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="20e73-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="20e73-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="20e73-130">Validation file</span></span>  <br/> |<span data-ttu-id="20e73-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="20e73-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="20e73-132">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="20e73-132">Can be empty</span></span>  <br/> |<span data-ttu-id="20e73-133">False</span><span class="sxs-lookup"><span data-stu-id="20e73-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="20e73-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="20e73-134">See also</span></span>



- [<span data-ttu-id="20e73-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="20e73-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

