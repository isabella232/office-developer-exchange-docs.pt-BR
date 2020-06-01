---
title: MonthlyRegeneration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MonthlyRegeneration
api_type:
- schema
ms.assetid: 9a52ca97-a663-41fe-b61a-61d8c53833ca
description: O elemento MonthlyRegeneration descreve a frequência, em meses, da qual a tarefa é gerada novamente.
ms.openlocfilehash: c941bc2606790646d2797df27c854996901c0bc6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462735"
---
# <a name="monthlyregeneration"></a><span data-ttu-id="8f0ec-103">MonthlyRegeneration</span><span class="sxs-lookup"><span data-stu-id="8f0ec-103">MonthlyRegeneration</span></span>

<span data-ttu-id="8f0ec-104">O elemento **MonthlyRegeneration** descreve a frequência, em meses, da qual a tarefa é gerada novamente.</span><span class="sxs-lookup"><span data-stu-id="8f0ec-104">The **MonthlyRegeneration** element describes the frequency, in months, of which task is regenerated.</span></span> 
  
```xml
<MonthlyRegeneration>
   <Interval/>
</MonthlyRegeneration>
```

 <span data-ttu-id="8f0ec-105">**MonthlyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="8f0ec-105">**MonthlyRegeneratingPatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8f0ec-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8f0ec-106">Attributes and elements</span></span>

<span data-ttu-id="8f0ec-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8f0ec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8f0ec-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8f0ec-108">Attributes</span></span>

<span data-ttu-id="8f0ec-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8f0ec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8f0ec-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8f0ec-110">Child elements</span></span>

|<span data-ttu-id="8f0ec-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8f0ec-111">**Element**</span></span>|<span data-ttu-id="8f0ec-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8f0ec-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8f0ec-113">Intervalo</span><span class="sxs-lookup"><span data-stu-id="8f0ec-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="8f0ec-114">Define o intervalo, em meses, entre dois itens recorrentes consecutivos.</span><span class="sxs-lookup"><span data-stu-id="8f0ec-114">Defines the interval, in months, between two consecutive recurring items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8f0ec-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8f0ec-115">Parent elements</span></span>

|<span data-ttu-id="8f0ec-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8f0ec-116">**Element**</span></span>|<span data-ttu-id="8f0ec-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8f0ec-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8f0ec-118">Recorrência (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="8f0ec-118">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="8f0ec-119">Contém informações de recorrência para tarefas recorrentes.</span><span class="sxs-lookup"><span data-stu-id="8f0ec-119">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8f0ec-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="8f0ec-120">Remarks</span></span>

<span data-ttu-id="8f0ec-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="8f0ec-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8f0ec-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="8f0ec-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8f0ec-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="8f0ec-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8f0ec-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8f0ec-124">Schema name</span></span>  <br/> |<span data-ttu-id="8f0ec-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8f0ec-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="8f0ec-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8f0ec-126">Validation file</span></span>  <br/> |<span data-ttu-id="8f0ec-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8f0ec-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8f0ec-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="8f0ec-128">Can be empty</span></span>  <br/> |<span data-ttu-id="8f0ec-129">False</span><span class="sxs-lookup"><span data-stu-id="8f0ec-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8f0ec-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="8f0ec-130">See also</span></span>



- [<span data-ttu-id="8f0ec-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8f0ec-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

