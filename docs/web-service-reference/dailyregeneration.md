---
title: DailyRegeneration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DailyRegeneration
api_type:
- schema
ms.assetid: cafb57e4-c518-45e0-b565-2babd0dab1df
description: O elemento DailyRegeneration descreve a frequência, em dias, em que uma tarefa seja gerada novamente.
ms.openlocfilehash: 356f7fd2672b2ad87d17e597c52e9f12273ce3c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751672"
---
# <a name="dailyregeneration"></a><span data-ttu-id="66082-103">DailyRegeneration</span><span class="sxs-lookup"><span data-stu-id="66082-103">DailyRegeneration</span></span>

<span data-ttu-id="66082-104">O elemento **DailyRegeneration** descreve a frequência, em dias, em que uma tarefa seja gerada novamente.</span><span class="sxs-lookup"><span data-stu-id="66082-104">The **DailyRegeneration** element describes the frequency, in days, in which a task is regenerated.</span></span> 
  
```xml
<DailyRegeneration>
   <Interval/>
</DailyRegeneration>
```

<span data-ttu-id="66082-105">**DailyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="66082-105">**DailyRegeneratingPatternType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="66082-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="66082-106">Attributes and elements</span></span>

<span data-ttu-id="66082-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="66082-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="66082-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="66082-108">Attributes</span></span>

<span data-ttu-id="66082-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="66082-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="66082-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="66082-110">Child elements</span></span>

|<span data-ttu-id="66082-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="66082-111">**Element**</span></span>|<span data-ttu-id="66082-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="66082-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66082-113">Intervalo</span><span class="sxs-lookup"><span data-stu-id="66082-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="66082-114">Define o intervalo, em dias, entre dois itens recorrentes consecutivos.</span><span class="sxs-lookup"><span data-stu-id="66082-114">Defines the interval, in days, between two consecutive recurring items.</span></span> <span data-ttu-id="66082-115">O valor deve estar no intervalo de 1 a 999.</span><span class="sxs-lookup"><span data-stu-id="66082-115">The value must be in the range of 1 to 999.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="66082-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="66082-116">Parent elements</span></span>

|<span data-ttu-id="66082-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="66082-117">**Element**</span></span>|<span data-ttu-id="66082-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="66082-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66082-119">Recorrência (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="66082-119">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="66082-120">Contém informações de recorrência de tarefas recorrentes.</span><span class="sxs-lookup"><span data-stu-id="66082-120">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="66082-121">Comentários</span><span class="sxs-lookup"><span data-stu-id="66082-121">Remarks</span></span>

<span data-ttu-id="66082-122">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="66082-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="66082-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="66082-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="66082-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="66082-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="66082-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="66082-125">Schema name</span></span>  <br/> |<span data-ttu-id="66082-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="66082-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="66082-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="66082-127">Validation file</span></span>  <br/> |<span data-ttu-id="66082-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="66082-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="66082-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="66082-129">Can be empty</span></span>  <br/> |<span data-ttu-id="66082-130">False</span><span class="sxs-lookup"><span data-stu-id="66082-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="66082-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="66082-131">See also</span></span>

- [<span data-ttu-id="66082-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="66082-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

