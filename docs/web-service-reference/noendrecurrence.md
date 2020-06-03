---
title: NoEndRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NoEndRecurrence
api_type:
- schema
ms.assetid: ab2ebd9c-388e-45f1-abf9-56e293ef123b
description: O elemento NoEndRecurrence descreve a data de início de um padrão de recorrência de item que não tem uma data de término definida.
ms.openlocfilehash: 31a3bd6ae2d7ce94debbeebc4fd4f536447433a7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466791"
---
# <a name="noendrecurrence"></a><span data-ttu-id="6e69f-103">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="6e69f-103">NoEndRecurrence</span></span>

<span data-ttu-id="6e69f-104">O elemento **NoEndRecurrence** descreve a data de início de um padrão de recorrência de item que não tem uma data de término definida.</span><span class="sxs-lookup"><span data-stu-id="6e69f-104">The **NoEndRecurrence** element describes the start date of an item recurrence pattern that does not have a defined end date.</span></span> 
  
```xml
<NoEndRecurrence>
   <StartDate/>
</NoEndRecurrence>
```

 <span data-ttu-id="6e69f-105">**NoEndRecurrenceRangeType**</span><span class="sxs-lookup"><span data-stu-id="6e69f-105">**NoEndRecurrenceRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e69f-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6e69f-106">Attributes and elements</span></span>

<span data-ttu-id="6e69f-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6e69f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e69f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6e69f-108">Attributes</span></span>

<span data-ttu-id="6e69f-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e69f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e69f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6e69f-110">Child elements</span></span>

|<span data-ttu-id="6e69f-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6e69f-111">**Element**</span></span>|<span data-ttu-id="6e69f-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6e69f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e69f-113">StartDate (recorrência)</span><span class="sxs-lookup"><span data-stu-id="6e69f-113">StartDate (Recurrence)</span></span>](startdate-recurrence.md) <br/> |<span data-ttu-id="6e69f-114">Representa a data de início de um item de calendário ou tarefa recorrente.</span><span class="sxs-lookup"><span data-stu-id="6e69f-114">Represents the start date of a recurring task or calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6e69f-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6e69f-115">Parent elements</span></span>

|<span data-ttu-id="6e69f-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6e69f-116">**Element**</span></span>|<span data-ttu-id="6e69f-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6e69f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e69f-118">Recurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="6e69f-118">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="6e69f-119">Contém o padrão de recorrência para itens de calendário e solicitações de reunião.</span><span class="sxs-lookup"><span data-stu-id="6e69f-119">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="6e69f-120">Recorrência (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="6e69f-120">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="6e69f-121">Contém informações de recorrência para tarefas recorrentes.</span><span class="sxs-lookup"><span data-stu-id="6e69f-121">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6e69f-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="6e69f-122">Remarks</span></span>

<span data-ttu-id="6e69f-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="6e69f-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e69f-124">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6e69f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e69f-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="6e69f-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6e69f-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6e69f-126">Schema name</span></span>  <br/> |<span data-ttu-id="6e69f-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="6e69f-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="6e69f-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6e69f-128">Validation file</span></span>  <br/> |<span data-ttu-id="6e69f-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6e69f-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6e69f-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="6e69f-130">Can be empty</span></span>  <br/> |<span data-ttu-id="6e69f-131">False</span><span class="sxs-lookup"><span data-stu-id="6e69f-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6e69f-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="6e69f-132">See also</span></span>



- [<span data-ttu-id="6e69f-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6e69f-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

