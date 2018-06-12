---
title: StartDate (recorrência)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartDate
api_type:
- schema
ms.assetid: bd65ac06-b3ac-4c9b-9568-3e4dc94378e7
description: O elemento StartDate representa a data de início de uma tarefa recorrente ou item de calendário.
ms.openlocfilehash: 6a38e63bbcf010ab6dca8f66440a2b0a559cf88d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825551"
---
# <a name="startdate-recurrence"></a><span data-ttu-id="10900-103">StartDate (recorrência)</span><span class="sxs-lookup"><span data-stu-id="10900-103">StartDate (Recurrence)</span></span>

<span data-ttu-id="10900-104">O elemento **StartDate** representa a data de início de uma tarefa recorrente ou item de calendário.</span><span class="sxs-lookup"><span data-stu-id="10900-104">The **StartDate** element represents the start date of a recurring task or calendar item.</span></span> 
  
```xml
<StartDate/>
```

<span data-ttu-id="10900-105">**Date**</span><span class="sxs-lookup"><span data-stu-id="10900-105">**Date**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="10900-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="10900-106">Attributes and elements</span></span>

<span data-ttu-id="10900-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="10900-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="10900-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="10900-108">Attributes</span></span>

<span data-ttu-id="10900-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="10900-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="10900-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="10900-110">Child elements</span></span>

<span data-ttu-id="10900-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="10900-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="10900-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="10900-112">Parent elements</span></span>

|<span data-ttu-id="10900-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="10900-113">**Element**</span></span>|<span data-ttu-id="10900-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="10900-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="10900-115">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="10900-115">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="10900-116">Descreve a data de início e a data final do padrão de recorrência de um item.</span><span class="sxs-lookup"><span data-stu-id="10900-116">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="10900-117">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="10900-117">NoEndRecurrence</span></span>](noendrecurrence.md) <br/> |<span data-ttu-id="10900-118">Descreve a data de início de um padrão de recorrência do item que não tem uma data de término definidas.</span><span class="sxs-lookup"><span data-stu-id="10900-118">Describes the start date of an item recurrence pattern that does not have a defined end date.</span></span>  <br/> |
|[<span data-ttu-id="10900-119">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="10900-119">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="10900-120">Descreve a data de início e o número de ocorrências de um item recorrente.</span><span class="sxs-lookup"><span data-stu-id="10900-120">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="10900-121">Text value</span><span class="sxs-lookup"><span data-stu-id="10900-121">Text value</span></span>

<span data-ttu-id="10900-122">Se este elemento for usado, será necessário um valor de texto que representa uma data.</span><span class="sxs-lookup"><span data-stu-id="10900-122">A text value that represents a date is required if this element is used.</span></span> <span data-ttu-id="10900-123">O valor não pode ser menor do que 1 de abr de 1601 00:00:00.</span><span class="sxs-lookup"><span data-stu-id="10900-123">The value cannot be less than Apr, 1, 1601 00:00:00.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="10900-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="10900-124">Remarks</span></span>

<span data-ttu-id="10900-125">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="10900-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="10900-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="10900-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="10900-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="10900-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="10900-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="10900-128">Schema name</span></span>  <br/> |<span data-ttu-id="10900-129">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="10900-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="10900-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="10900-130">Validation file</span></span>  <br/> |<span data-ttu-id="10900-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="10900-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="10900-132">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="10900-132">Can be empty</span></span>  <br/> |<span data-ttu-id="10900-133">False</span><span class="sxs-lookup"><span data-stu-id="10900-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="10900-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="10900-134">See also</span></span>

- [<span data-ttu-id="10900-135">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="10900-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

