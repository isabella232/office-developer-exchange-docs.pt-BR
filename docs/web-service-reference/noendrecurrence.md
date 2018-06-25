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
description: O elemento NoEndRecurrence descreve a data de início de um padrão de recorrência do item que não tem uma data de término definidas.
ms.openlocfilehash: fc3eae170f5c07e31d7a80b45836efd07d74e543
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824537"
---
# <a name="noendrecurrence"></a><span data-ttu-id="471e8-103">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="471e8-103">NoEndRecurrence</span></span>

<span data-ttu-id="471e8-104">O elemento **NoEndRecurrence** descreve a data de início de um padrão de recorrência do item que não tem uma data de término definidas.</span><span class="sxs-lookup"><span data-stu-id="471e8-104">The **NoEndRecurrence** element describes the start date of an item recurrence pattern that does not have a defined end date.</span></span> 
  
```xml
<NoEndRecurrence>
   <StartDate/>
</NoEndRecurrence>
```

 <span data-ttu-id="471e8-105">**NoEndRecurrenceRangeType**</span><span class="sxs-lookup"><span data-stu-id="471e8-105">**NoEndRecurrenceRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="471e8-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="471e8-106">Attributes and elements</span></span>

<span data-ttu-id="471e8-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="471e8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="471e8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="471e8-108">Attributes</span></span>

<span data-ttu-id="471e8-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="471e8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="471e8-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="471e8-110">Child elements</span></span>

|<span data-ttu-id="471e8-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="471e8-111">**Element**</span></span>|<span data-ttu-id="471e8-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="471e8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="471e8-113">StartDate (recorrência)</span><span class="sxs-lookup"><span data-stu-id="471e8-113">StartDate (Recurrence)</span></span>](startdate-recurrence.md) <br/> |<span data-ttu-id="471e8-114">Representa a data de início de uma tarefa recorrente ou item de calendário.</span><span class="sxs-lookup"><span data-stu-id="471e8-114">Represents the start date of a recurring task or calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="471e8-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="471e8-115">Parent elements</span></span>

|<span data-ttu-id="471e8-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="471e8-116">**Element**</span></span>|<span data-ttu-id="471e8-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="471e8-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="471e8-118">Recorrência (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="471e8-118">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="471e8-119">Contém o padrão de recorrência para itens de calendário e solicitações de reunião.</span><span class="sxs-lookup"><span data-stu-id="471e8-119">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="471e8-120">Recorrência (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="471e8-120">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="471e8-121">Contém informações de recorrência de tarefas recorrentes.</span><span class="sxs-lookup"><span data-stu-id="471e8-121">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="471e8-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="471e8-122">Remarks</span></span>

<span data-ttu-id="471e8-123">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="471e8-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="471e8-124">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="471e8-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="471e8-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="471e8-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="471e8-126">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="471e8-126">Schema name</span></span>  <br/> |<span data-ttu-id="471e8-127">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="471e8-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="471e8-128">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="471e8-128">Validation file</span></span>  <br/> |<span data-ttu-id="471e8-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="471e8-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="471e8-130">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="471e8-130">Can be empty</span></span>  <br/> |<span data-ttu-id="471e8-131">False</span><span class="sxs-lookup"><span data-stu-id="471e8-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="471e8-132">Ver também</span><span class="sxs-lookup"><span data-stu-id="471e8-132">See also</span></span>



- [<span data-ttu-id="471e8-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="471e8-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

