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
description: O elemento EndDate representa a data de término de uma tarefa recorrente ou um item de calendário que tenha o tipo de padrão de EndDateRecurrence.
ms.openlocfilehash: b8570a069fc0a2d05044a9c85ab2d5c39d70ccdf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752047"
---
# <a name="enddate-recurrence"></a><span data-ttu-id="fa622-103">EndDate (recorrência)</span><span class="sxs-lookup"><span data-stu-id="fa622-103">EndDate (Recurrence)</span></span>

<span data-ttu-id="fa622-104">O elemento **EndDate** representa a data de término de uma tarefa recorrente ou um item de calendário que tenha o tipo de padrão de EndDateRecurrence.</span><span class="sxs-lookup"><span data-stu-id="fa622-104">The **EndDate** element represents the end date of a recurring task or a calendar item that has the EndDateRecurrence pattern type.</span></span> 
  
```xml
<EndDate/>
```

 <span data-ttu-id="fa622-105">**Data**</span><span class="sxs-lookup"><span data-stu-id="fa622-105">**date**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fa622-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="fa622-106">Attributes and elements</span></span>

<span data-ttu-id="fa622-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fa622-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fa622-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="fa622-108">Attributes</span></span>

<span data-ttu-id="fa622-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fa622-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fa622-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fa622-110">Child elements</span></span>

<span data-ttu-id="fa622-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fa622-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fa622-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fa622-112">Parent elements</span></span>

|<span data-ttu-id="fa622-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fa622-113">**Element**</span></span>|<span data-ttu-id="fa622-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fa622-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa622-115">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="fa622-115">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="fa622-116">Descreve a data de início e a data final do padrão de recorrência de um item.</span><span class="sxs-lookup"><span data-stu-id="fa622-116">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fa622-117">Text value</span><span class="sxs-lookup"><span data-stu-id="fa622-117">Text value</span></span>

<span data-ttu-id="fa622-118">Se este elemento for usado, será necessário um valor de texto que representa uma data.</span><span class="sxs-lookup"><span data-stu-id="fa622-118">A text value that represents a date is required if this element is used.</span></span> <span data-ttu-id="fa622-119">O valor não pode ser maior que 1 de setembro de 4500 00:00:00.</span><span class="sxs-lookup"><span data-stu-id="fa622-119">The value cannot be larger than September 1, 4500 00:00:00.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fa622-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="fa622-120">Remarks</span></span>

<span data-ttu-id="fa622-121">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="fa622-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fa622-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="fa622-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fa622-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="fa622-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fa622-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fa622-124">Schema name</span></span>  <br/> |<span data-ttu-id="fa622-125">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="fa622-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="fa622-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fa622-126">Validation file</span></span>  <br/> |<span data-ttu-id="fa622-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fa622-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fa622-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="fa622-128">Can be empty</span></span>  <br/> |<span data-ttu-id="fa622-129">False</span><span class="sxs-lookup"><span data-stu-id="fa622-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fa622-130">Ver também</span><span class="sxs-lookup"><span data-stu-id="fa622-130">See also</span></span>



- [<span data-ttu-id="fa622-131">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fa622-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

