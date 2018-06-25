---
title: DailyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DailyRecurrence
api_type:
- schema
ms.assetid: 0aaf265d-b723-49c6-8e9c-9ba60141e9ab
description: O elemento DailyRecurrence descreve a frequência, em dias, em que é um item de calendário ou uma tarefa recorrente.
ms.openlocfilehash: d02c1f7425372d60c10b40527dc5f0d65f923b45
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751668"
---
# <a name="dailyrecurrence"></a><span data-ttu-id="01d28-103">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="01d28-103">DailyRecurrence</span></span>

<span data-ttu-id="01d28-104">O elemento **DailyRecurrence** descreve a frequência, em dias, em que é um item de calendário ou uma tarefa recorrente.</span><span class="sxs-lookup"><span data-stu-id="01d28-104">The **DailyRecurrence** element describes the frequency, in days, in which a calendar item or a task recurs.</span></span> 
  
```xml
<DailyRecurrence>
   <Interval/>
</DailyRecurrence>
```

<span data-ttu-id="01d28-105">**DailyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="01d28-105">**DailyRecurrencePatternType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="01d28-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="01d28-106">Attributes and elements</span></span>

<span data-ttu-id="01d28-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="01d28-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01d28-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="01d28-108">Attributes</span></span>

<span data-ttu-id="01d28-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="01d28-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="01d28-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="01d28-110">Child elements</span></span>

|<span data-ttu-id="01d28-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="01d28-111">**Element**</span></span>|<span data-ttu-id="01d28-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="01d28-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01d28-113">Intervalo</span><span class="sxs-lookup"><span data-stu-id="01d28-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="01d28-114">Define o intervalo, em dias, entre dois itens recorrentes consecutivos.</span><span class="sxs-lookup"><span data-stu-id="01d28-114">Defines the interval, in days, between two consecutive recurring items.</span></span> <span data-ttu-id="01d28-115">O valor deve estar no intervalo entre 1 e 999.</span><span class="sxs-lookup"><span data-stu-id="01d28-115">The value must be in the range from 1 to 999.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="01d28-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="01d28-116">Parent elements</span></span>

|<span data-ttu-id="01d28-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="01d28-117">**Element**</span></span>|<span data-ttu-id="01d28-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="01d28-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01d28-119">Recorrência (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="01d28-119">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="01d28-120">Contém informações de recorrência de tarefas recorrentes.</span><span class="sxs-lookup"><span data-stu-id="01d28-120">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="01d28-121">Recorrência (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="01d28-121">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="01d28-122">Contém o padrão de recorrência para itens de calendário e solicitações de reunião.</span><span class="sxs-lookup"><span data-stu-id="01d28-122">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="01d28-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="01d28-123">Remarks</span></span>

<span data-ttu-id="01d28-124">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="01d28-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01d28-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="01d28-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01d28-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="01d28-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="01d28-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="01d28-127">Schema name</span></span>  <br/> |<span data-ttu-id="01d28-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="01d28-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="01d28-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="01d28-129">Validation file</span></span>  <br/> |<span data-ttu-id="01d28-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="01d28-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="01d28-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="01d28-131">Can be empty</span></span>  <br/> |<span data-ttu-id="01d28-132">False</span><span class="sxs-lookup"><span data-stu-id="01d28-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="01d28-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="01d28-133">See also</span></span>

- [<span data-ttu-id="01d28-134">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="01d28-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

