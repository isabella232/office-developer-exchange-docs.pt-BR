---
title: GroupedItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupedItems
api_type:
- schema
ms.assetid: 53170df4-4272-4b37-b23f-cd8e2d4a7396
description: O elemento GroupedItems representa uma coleção de itens que são o resultado de uma chamada de operação FindItem agrupada.
ms.openlocfilehash: f8aed9b78fc54307f44b96a45e5c31a4cc76ab50
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823756"
---
# <a name="groupeditems"></a><span data-ttu-id="54212-103">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="54212-103">GroupedItems</span></span>

<span data-ttu-id="54212-104">O elemento **GroupedItems** representa uma coleção de itens que são o resultado de uma [operação FindItem](finditem-operation.md) de agrupadas chamada.</span><span class="sxs-lookup"><span data-stu-id="54212-104">The **GroupedItems** element represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span> 
  
[<span data-ttu-id="54212-105">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="54212-105">FindItemResponse</span></span>](finditemresponse.md)
  
[<span data-ttu-id="54212-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="54212-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="54212-107">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="54212-107">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
  
[<span data-ttu-id="54212-108">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="54212-108">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
  
[<span data-ttu-id="54212-109">Grupos</span><span class="sxs-lookup"><span data-stu-id="54212-109">Groups</span></span>](groups.md)
  
[<span data-ttu-id="54212-110">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="54212-110">GroupedItems</span></span>](groupeditems.md)
  
```xml
<GroupedItems>
   <GroupIndex/>
   <Items/>
</GroupedItems>
```

 <span data-ttu-id="54212-111">**GroupedItemsType**</span><span class="sxs-lookup"><span data-stu-id="54212-111">**GroupedItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54212-112">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="54212-112">Attributes and elements</span></span>

<span data-ttu-id="54212-113">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="54212-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54212-114">Atributos</span><span class="sxs-lookup"><span data-stu-id="54212-114">Attributes</span></span>

<span data-ttu-id="54212-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="54212-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54212-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="54212-116">Child elements</span></span>

|<span data-ttu-id="54212-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="54212-117">**Element**</span></span>|<span data-ttu-id="54212-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="54212-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54212-119">GroupIndex</span><span class="sxs-lookup"><span data-stu-id="54212-119">GroupIndex</span></span>](groupindex.md) <br/> |<span data-ttu-id="54212-120">Representa o valor da propriedade é usada para agrupar itens em uma agrupadas [FindItem operação](finditem-operation.md) chamada.</span><span class="sxs-lookup"><span data-stu-id="54212-120">Represents the property value that is used to group items in a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> |
|[<span data-ttu-id="54212-121">Items</span><span class="sxs-lookup"><span data-stu-id="54212-121">Items</span></span>](items.md) <br/> |<span data-ttu-id="54212-122">Contém uma matriz de itens agrupados.</span><span class="sxs-lookup"><span data-stu-id="54212-122">Contains an array of grouped items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="54212-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="54212-123">Parent elements</span></span>

|<span data-ttu-id="54212-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="54212-124">**Element**</span></span>|<span data-ttu-id="54212-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="54212-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54212-126">Grupos</span><span class="sxs-lookup"><span data-stu-id="54212-126">Groups</span></span>](groups.md) <br/> |<span data-ttu-id="54212-127">Contém uma coleção dos grupos que são encontrados com os critérios de pesquisa e a agregação de lista segura é identificada na solicitação de [operação FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="54212-127">Contains a collection of groups that are found with the search and aggregation criteria that is identified in the [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="54212-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="54212-128">Remarks</span></span>

<span data-ttu-id="54212-129">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="54212-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54212-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="54212-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54212-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="54212-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="54212-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="54212-132">Schema name</span></span>  <br/> |<span data-ttu-id="54212-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="54212-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="54212-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="54212-134">Validation file</span></span>  <br/> |<span data-ttu-id="54212-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="54212-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="54212-136">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="54212-136">Can be empty</span></span>  <br/> |<span data-ttu-id="54212-137">False</span><span class="sxs-lookup"><span data-stu-id="54212-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="54212-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="54212-138">See also</span></span>



[<span data-ttu-id="54212-139">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="54212-139">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="54212-140">Localizando itens</span><span class="sxs-lookup"><span data-stu-id="54212-140">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

