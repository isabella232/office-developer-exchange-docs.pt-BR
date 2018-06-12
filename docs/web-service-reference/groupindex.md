---
title: GroupIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupIndex
api_type:
- schema
ms.assetid: 7a596ff7-6cc3-4626-a52c-538a92202337
description: O elemento GroupIndex representa o valor da propriedade é usado para agrupar itens para o grupo atual de itens em uma chamada de operação FindItem.
ms.openlocfilehash: 8b23f5142a15c099c30209ea48cd04f4af4e8c6a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823762"
---
# <a name="groupindex"></a><span data-ttu-id="dc116-103">GroupIndex</span><span class="sxs-lookup"><span data-stu-id="dc116-103">GroupIndex</span></span>

<span data-ttu-id="dc116-104">O elemento **GroupIndex** representa o valor da propriedade é usado para agrupar itens para o grupo atual de itens em uma chamada de [operação FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="dc116-104">The **GroupIndex** element represents the property value that is used to group items for the current group of items in a [FindItem operation](finditem-operation.md) call.</span></span> 
  
[<span data-ttu-id="dc116-105">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="dc116-105">FindItemResponse</span></span>](finditemresponse.md)
  
[<span data-ttu-id="dc116-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="dc116-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="dc116-107">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="dc116-107">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
  
[<span data-ttu-id="dc116-108">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="dc116-108">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
  
[<span data-ttu-id="dc116-109">Grupos</span><span class="sxs-lookup"><span data-stu-id="dc116-109">Groups</span></span>](groups.md)
  
[<span data-ttu-id="dc116-110">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="dc116-110">GroupedItems</span></span>](groupeditems.md)
  
[<span data-ttu-id="dc116-111">GroupIndex</span><span class="sxs-lookup"><span data-stu-id="dc116-111">GroupIndex</span></span>](groupindex.md)
  
```xml
<GroupIndex/>
```

 <span data-ttu-id="dc116-112">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="dc116-112">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dc116-113">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="dc116-113">Attributes and elements</span></span>

<span data-ttu-id="dc116-114">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="dc116-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dc116-115">Atributos</span><span class="sxs-lookup"><span data-stu-id="dc116-115">Attributes</span></span>

<span data-ttu-id="dc116-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="dc116-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dc116-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="dc116-117">Child elements</span></span>

<span data-ttu-id="dc116-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="dc116-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dc116-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="dc116-119">Parent elements</span></span>

|<span data-ttu-id="dc116-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dc116-120">**Element**</span></span>|<span data-ttu-id="dc116-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dc116-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc116-122">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="dc116-122">GroupedItems</span></span>](groupeditems.md) <br/> |<span data-ttu-id="dc116-123">Representa uma coleção de itens que são o resultado de uma [operação FindItem](finditem-operation.md) de agrupada de chamadas.</span><span class="sxs-lookup"><span data-stu-id="dc116-123">Represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> <span data-ttu-id="dc116-124">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="dc116-124">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItemResponse/ResponseMessages/FindItemResponseMessage/RootFolder/Groups/GroupedItems[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dc116-125">Text value</span><span class="sxs-lookup"><span data-stu-id="dc116-125">Text value</span></span>

<span data-ttu-id="dc116-126">É necessário um valor de texto.</span><span class="sxs-lookup"><span data-stu-id="dc116-126">A text value is required.</span></span> <span data-ttu-id="dc116-127">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="dc116-127">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dc116-128">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="dc116-128">Remarks</span></span>

<span data-ttu-id="dc116-129">Esse elemento só ocorre em uma resposta de [operação FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="dc116-129">This element only occurs in a [FindItem operation](finditem-operation.md) response.</span></span> 
  
<span data-ttu-id="dc116-130">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="dc116-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dc116-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="dc116-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dc116-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="dc116-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dc116-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="dc116-133">Schema name</span></span>  <br/> |<span data-ttu-id="dc116-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="dc116-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="dc116-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="dc116-135">Validation file</span></span>  <br/> |<span data-ttu-id="dc116-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dc116-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dc116-137">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="dc116-137">Can be empty</span></span>  <br/> |<span data-ttu-id="dc116-138">False</span><span class="sxs-lookup"><span data-stu-id="dc116-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dc116-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="dc116-139">See also</span></span>



[<span data-ttu-id="dc116-140">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="dc116-140">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="dc116-141">Localizando itens</span><span class="sxs-lookup"><span data-stu-id="dc116-141">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

