---
title: WeeklyRegeneration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WeeklyRegeneration
api_type:
- schema
ms.assetid: f128fdaa-ca3d-4614-8e55-f25e76a67b6c
description: O elemento WeeklyRegeneration descreve a frequência, em semanas, em que uma tarefa seja gerada novamente.
ms.openlocfilehash: 36cd3cc5c180f2b2cf53708e7787d0595f518def
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838071"
---
# <a name="weeklyregeneration"></a><span data-ttu-id="8374b-103">WeeklyRegeneration</span><span class="sxs-lookup"><span data-stu-id="8374b-103">WeeklyRegeneration</span></span>

<span data-ttu-id="8374b-104">O elemento **WeeklyRegeneration** descreve a frequência, em semanas, em que uma tarefa seja gerada novamente.</span><span class="sxs-lookup"><span data-stu-id="8374b-104">The **WeeklyRegeneration** element describes the frequency, in weeks, in which a task is regenerated.</span></span> 
  
```xml
<WeeklyRegeneration>
   <Interval/>
</WeeklyRegeneration>
```

 <span data-ttu-id="8374b-105">**WeeklyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="8374b-105">**WeeklyRegeneratingPatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8374b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8374b-106">Attributes and elements</span></span>

<span data-ttu-id="8374b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8374b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8374b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8374b-108">Attributes</span></span>

<span data-ttu-id="8374b-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8374b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8374b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8374b-110">Child elements</span></span>

|<span data-ttu-id="8374b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8374b-111">**Element**</span></span>|<span data-ttu-id="8374b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8374b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8374b-113">Intervalo</span><span class="sxs-lookup"><span data-stu-id="8374b-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="8374b-114">Define o intervalo, em semanas, desde que a tarefa foi concluída, após o qual uma nova tarefa seja gerada novamente.</span><span class="sxs-lookup"><span data-stu-id="8374b-114">Defines the interval, in weeks, since the task was completed, after which a new task is regenerated.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8374b-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8374b-115">Parent elements</span></span>

|<span data-ttu-id="8374b-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8374b-116">**Element**</span></span>|<span data-ttu-id="8374b-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8374b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8374b-118">Recorrência (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="8374b-118">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="8374b-119">Contém informações de recorrência de tarefas recorrentes.</span><span class="sxs-lookup"><span data-stu-id="8374b-119">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8374b-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="8374b-120">Remarks</span></span>

<span data-ttu-id="8374b-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="8374b-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8374b-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8374b-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8374b-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="8374b-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8374b-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8374b-124">Schema Name</span></span>  <br/> |<span data-ttu-id="8374b-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8374b-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="8374b-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8374b-126">Validation File</span></span>  <br/> |<span data-ttu-id="8374b-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8374b-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8374b-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8374b-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="8374b-129">False</span><span class="sxs-lookup"><span data-stu-id="8374b-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8374b-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="8374b-130">See also</span></span>



- [<span data-ttu-id="8374b-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8374b-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

