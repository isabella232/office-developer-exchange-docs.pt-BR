---
title: Grupos
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Groups
api_type:
- schema
ms.assetid: 6b6b2d67-219d-4dfb-a4ed-d627b1cfb33f
description: O elemento de grupos contém uma coleção dos grupos que são encontrados com os critérios de pesquisa e a agregação de lista segura que é identificada na solicitação de operação FindItem.
ms.openlocfilehash: 406a1974899e89243f52ba7a56afcc172c4f3df6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823786"
---
# <a name="groups"></a><span data-ttu-id="d6a6c-103">Grupos</span><span class="sxs-lookup"><span data-stu-id="d6a6c-103">Groups</span></span>

<span data-ttu-id="d6a6c-104">O elemento de **grupos** contém uma coleção dos grupos que são encontrados com os critérios de pesquisa e a agregação de lista segura que é identificada na solicitação de [operação FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d6a6c-104">The **Groups** element contains a collection of groups that are found with the search and aggregation criteria that is identified in the [FindItem operation](finditem-operation.md) request.</span></span> 
  
```xml
<Groups>
   <GroupedItems/>
</Groups>
```

 <span data-ttu-id="d6a6c-105">**ArrayOfGroupedItemsType**</span><span class="sxs-lookup"><span data-stu-id="d6a6c-105">**ArrayOfGroupedItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d6a6c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d6a6c-106">Attributes and elements</span></span>

<span data-ttu-id="d6a6c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d6a6c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d6a6c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="d6a6c-108">Attributes</span></span>

<span data-ttu-id="d6a6c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d6a6c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d6a6c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d6a6c-110">Child elements</span></span>

|<span data-ttu-id="d6a6c-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d6a6c-111">**Element**</span></span>|<span data-ttu-id="d6a6c-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d6a6c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6a6c-113">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="d6a6c-113">GroupedItems</span></span>](groupeditems.md) <br/> |<span data-ttu-id="d6a6c-114">Representa uma coleção de itens que são o resultado de uma [operação FindItem](finditem-operation.md) de agrupada de chamadas.</span><span class="sxs-lookup"><span data-stu-id="d6a6c-114">Represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d6a6c-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d6a6c-115">Parent elements</span></span>

|<span data-ttu-id="d6a6c-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d6a6c-116">**Element**</span></span>|<span data-ttu-id="d6a6c-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d6a6c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6a6c-118">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="d6a6c-118">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md) <br/> |<span data-ttu-id="d6a6c-119">Contém os resultados de uma pesquisa de uma pasta raiz única durante uma operação de [operação FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d6a6c-119">Contains the results from a search of a single root folder during a [FindItem operation](finditem-operation.md) operation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d6a6c-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="d6a6c-120">Remarks</span></span>

<span data-ttu-id="d6a6c-121">Uma instância de [GroupedItems](groupeditems.md) ocorrerá para cada grupo distinto dentro do resultado.</span><span class="sxs-lookup"><span data-stu-id="d6a6c-121">One [GroupedItems](groupeditems.md) instance will occur for each distinct group within the result.</span></span> 
  
<span data-ttu-id="d6a6c-122">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="d6a6c-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d6a6c-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d6a6c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d6a6c-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="d6a6c-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d6a6c-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d6a6c-125">Schema name</span></span>  <br/> |<span data-ttu-id="d6a6c-126">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d6a6c-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="d6a6c-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d6a6c-127">Validation file</span></span>  <br/> |<span data-ttu-id="d6a6c-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d6a6c-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d6a6c-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d6a6c-129">Can be empty</span></span>  <br/> |<span data-ttu-id="d6a6c-130">False</span><span class="sxs-lookup"><span data-stu-id="d6a6c-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d6a6c-131">Ver também</span><span class="sxs-lookup"><span data-stu-id="d6a6c-131">See also</span></span>



[<span data-ttu-id="d6a6c-132">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="d6a6c-132">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="d6a6c-133">Localizando itens</span><span class="sxs-lookup"><span data-stu-id="d6a6c-133">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

