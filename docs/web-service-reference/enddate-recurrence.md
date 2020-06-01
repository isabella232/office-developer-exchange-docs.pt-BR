---
title: EndDate (recorrência)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndDate
api_type:
- schema
ms.assetid: 16026595-26f8-4770-8a6d-0d3e4157effd
description: O elemento EndDate representa a data de término de uma tarefa recorrente ou um item de calendário que tem o tipo de padrão EndDateRecurrence.
ms.openlocfilehash: 53d9b04faf1d8f740c858080b5fcbeadf577df0d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460159"
---
# <a name="enddate-recurrence"></a><span data-ttu-id="7a4f8-103">EndDate (recorrência)</span><span class="sxs-lookup"><span data-stu-id="7a4f8-103">EndDate (Recurrence)</span></span>

<span data-ttu-id="7a4f8-104">O elemento **EndDate** representa a data de término de uma tarefa recorrente ou um item de calendário que tem o tipo de padrão EndDateRecurrence.</span><span class="sxs-lookup"><span data-stu-id="7a4f8-104">The **EndDate** element represents the end date of a recurring task or a calendar item that has the EndDateRecurrence pattern type.</span></span> 
  
```xml
<EndDate/>
```

 <span data-ttu-id="7a4f8-105">**data**</span><span class="sxs-lookup"><span data-stu-id="7a4f8-105">**date**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7a4f8-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="7a4f8-106">Attributes and elements</span></span>

<span data-ttu-id="7a4f8-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7a4f8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a4f8-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7a4f8-108">Attributes</span></span>

<span data-ttu-id="7a4f8-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7a4f8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a4f8-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7a4f8-110">Child elements</span></span>

<span data-ttu-id="7a4f8-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7a4f8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7a4f8-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7a4f8-112">Parent elements</span></span>

|<span data-ttu-id="7a4f8-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7a4f8-113">**Element**</span></span>|<span data-ttu-id="7a4f8-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7a4f8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a4f8-115">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="7a4f8-115">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="7a4f8-116">Descreve a data de início e a data de término de um padrão de recorrência de item.</span><span class="sxs-lookup"><span data-stu-id="7a4f8-116">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7a4f8-117">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="7a4f8-117">Text value</span></span>

<span data-ttu-id="7a4f8-118">Um valor de texto que representa uma data é necessário se esse elemento for usado.</span><span class="sxs-lookup"><span data-stu-id="7a4f8-118">A text value that represents a date is required if this element is used.</span></span> <span data-ttu-id="7a4f8-119">O valor não pode ser maior que 1 de setembro de 4500 00:00:00.</span><span class="sxs-lookup"><span data-stu-id="7a4f8-119">The value cannot be larger than September 1, 4500 00:00:00.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7a4f8-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="7a4f8-120">Remarks</span></span>

<span data-ttu-id="7a4f8-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="7a4f8-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7a4f8-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="7a4f8-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a4f8-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="7a4f8-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7a4f8-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7a4f8-124">Schema name</span></span>  <br/> |<span data-ttu-id="7a4f8-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7a4f8-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="7a4f8-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7a4f8-126">Validation file</span></span>  <br/> |<span data-ttu-id="7a4f8-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7a4f8-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7a4f8-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="7a4f8-128">Can be empty</span></span>  <br/> |<span data-ttu-id="7a4f8-129">False</span><span class="sxs-lookup"><span data-stu-id="7a4f8-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7a4f8-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="7a4f8-130">See also</span></span>



- [<span data-ttu-id="7a4f8-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7a4f8-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

