---
title: YearlyRegeneration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- YearlyRegeneration
api_type:
- schema
ms.assetid: 23538bca-738e-4319-944e-f459ff8a7eba
description: O elemento YearlyRegeneration descreve a frequência, em anos, em que uma tarefa é gerada novamente.
ms.openlocfilehash: 7a6796c433bc54d145d5a769e01f9bba46897735
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457876"
---
# <a name="yearlyregeneration"></a><span data-ttu-id="ffcfa-103">YearlyRegeneration</span><span class="sxs-lookup"><span data-stu-id="ffcfa-103">YearlyRegeneration</span></span>

<span data-ttu-id="ffcfa-104">O elemento **YearlyRegeneration** descreve a frequência, em anos, em que uma tarefa é gerada novamente.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-104">The **YearlyRegeneration** element describes the frequency, in years, in which a task is regenerated.</span></span> 
  
```xml
<YearlyRegeneratingPatternType>
   <Interval/>
</YearlyRegeneratingPatternType>
```

<span data-ttu-id="ffcfa-105">**YearlyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="ffcfa-105">**YearlyRegeneratingPatternType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ffcfa-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ffcfa-106">Attributes and elements</span></span>

<span data-ttu-id="ffcfa-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ffcfa-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ffcfa-108">Attributes</span></span>

<span data-ttu-id="ffcfa-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ffcfa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ffcfa-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ffcfa-110">Child elements</span></span>

|<span data-ttu-id="ffcfa-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ffcfa-111">**Element**</span></span>|<span data-ttu-id="ffcfa-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ffcfa-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ffcfa-113">Intervalo</span><span class="sxs-lookup"><span data-stu-id="ffcfa-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="ffcfa-114">Define o intervalo, em anos, durante o qual uma nova tarefa é regenerada após a conclusão da tarefa.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-114">Defines the interval, in years, during which a new task is regenerated after the completion of the task.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ffcfa-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ffcfa-115">Parent elements</span></span>

|<span data-ttu-id="ffcfa-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ffcfa-116">**Element**</span></span>|<span data-ttu-id="ffcfa-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ffcfa-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ffcfa-118">Recorrência (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="ffcfa-118">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="ffcfa-119">Contém informações de recorrência para tarefas recorrentes.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-119">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ffcfa-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="ffcfa-120">Remarks</span></span>

<span data-ttu-id="ffcfa-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="ffcfa-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="ffcfa-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ffcfa-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ffcfa-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="ffcfa-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ffcfa-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ffcfa-124">Schema Name</span></span>  <br/> |<span data-ttu-id="ffcfa-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ffcfa-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="ffcfa-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ffcfa-126">Validation File</span></span>  <br/> |<span data-ttu-id="ffcfa-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ffcfa-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ffcfa-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ffcfa-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="ffcfa-129">False</span><span class="sxs-lookup"><span data-stu-id="ffcfa-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ffcfa-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="ffcfa-130">See also</span></span>

- [<span data-ttu-id="ffcfa-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ffcfa-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

