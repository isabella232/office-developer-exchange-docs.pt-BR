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
ms.openlocfilehash: 0ee1ca3c6d0cf98e2daefa60a1cb1fd096cda478
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530808"
---
# <a name="groupeditems"></a><span data-ttu-id="d8d73-103">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="d8d73-103">GroupedItems</span></span>

<span data-ttu-id="d8d73-104">O elemento **GroupedItems** representa uma coleção de itens que são o resultado de uma chamada de [operação FindItem](finditem-operation.md) agrupada.</span><span class="sxs-lookup"><span data-stu-id="d8d73-104">The **GroupedItems** element represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span> 
  
[<span data-ttu-id="d8d73-105">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="d8d73-105">FindItemResponse</span></span>](finditemresponse.md)
  
[<span data-ttu-id="d8d73-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d8d73-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="d8d73-107">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d8d73-107">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
  
[<span data-ttu-id="d8d73-108">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="d8d73-108">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
  
[<span data-ttu-id="d8d73-109">Grupos</span><span class="sxs-lookup"><span data-stu-id="d8d73-109">Groups</span></span>](groups.md)
  
[<span data-ttu-id="d8d73-110">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="d8d73-110">GroupedItems</span></span>](groupeditems.md)
  
```xml
<GroupedItems>
   <GroupIndex/>
   <Items/>
</GroupedItems>
```

 <span data-ttu-id="d8d73-111">**GroupedItemsType**</span><span class="sxs-lookup"><span data-stu-id="d8d73-111">**GroupedItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8d73-112">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d8d73-112">Attributes and elements</span></span>

<span data-ttu-id="d8d73-113">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d8d73-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8d73-114">Atributos</span><span class="sxs-lookup"><span data-stu-id="d8d73-114">Attributes</span></span>

<span data-ttu-id="d8d73-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d8d73-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8d73-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d8d73-116">Child elements</span></span>

|<span data-ttu-id="d8d73-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d8d73-117">**Element**</span></span>|<span data-ttu-id="d8d73-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d8d73-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8d73-119">GroupIndex</span><span class="sxs-lookup"><span data-stu-id="d8d73-119">GroupIndex</span></span>](groupindex.md) <br/> |<span data-ttu-id="d8d73-120">Representa o valor da propriedade que é usado para agrupar itens em uma chamada de [operação FindItem](finditem-operation.md) agrupada.</span><span class="sxs-lookup"><span data-stu-id="d8d73-120">Represents the property value that is used to group items in a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> |
|[<span data-ttu-id="d8d73-121">Itens</span><span class="sxs-lookup"><span data-stu-id="d8d73-121">Items</span></span>](items.md) <br/> |<span data-ttu-id="d8d73-122">Contém uma matriz de itens agrupados.</span><span class="sxs-lookup"><span data-stu-id="d8d73-122">Contains an array of grouped items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d8d73-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d8d73-123">Parent elements</span></span>

|<span data-ttu-id="d8d73-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d8d73-124">**Element**</span></span>|<span data-ttu-id="d8d73-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d8d73-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8d73-126">Grupos</span><span class="sxs-lookup"><span data-stu-id="d8d73-126">Groups</span></span>](groups.md) <br/> |<span data-ttu-id="d8d73-127">Contém uma coleção de grupos que são encontrados com os critérios de pesquisa e agregação identificados na solicitação de [operação FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d8d73-127">Contains a collection of groups that are found with the search and aggregation criteria that is identified in the [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d8d73-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="d8d73-128">Remarks</span></span>

<span data-ttu-id="d8d73-129">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="d8d73-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8d73-130">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d8d73-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8d73-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="d8d73-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d8d73-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d8d73-132">Schema name</span></span>  <br/> |<span data-ttu-id="d8d73-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d8d73-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="d8d73-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d8d73-134">Validation file</span></span>  <br/> |<span data-ttu-id="d8d73-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d8d73-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d8d73-136">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d8d73-136">Can be empty</span></span>  <br/> |<span data-ttu-id="d8d73-137">False</span><span class="sxs-lookup"><span data-stu-id="d8d73-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d8d73-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="d8d73-138">See also</span></span>



[<span data-ttu-id="d8d73-139">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="d8d73-139">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="d8d73-140">Localizar itens</span><span class="sxs-lookup"><span data-stu-id="d8d73-140">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

