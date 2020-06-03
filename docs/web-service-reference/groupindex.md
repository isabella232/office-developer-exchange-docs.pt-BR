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
description: O elemento GroupIndex representa o valor da propriedade que é usado para agrupar itens para o grupo atual de itens em uma chamada de operação FindItem.
ms.openlocfilehash: 05f303be92885a15dddf85c85251af04910d835c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530265"
---
# <a name="groupindex"></a><span data-ttu-id="a94fd-103">GroupIndex</span><span class="sxs-lookup"><span data-stu-id="a94fd-103">GroupIndex</span></span>

<span data-ttu-id="a94fd-104">O elemento **GroupIndex** representa o valor da propriedade que é usado para agrupar itens para o grupo atual de itens em uma chamada de [operação FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a94fd-104">The **GroupIndex** element represents the property value that is used to group items for the current group of items in a [FindItem operation](finditem-operation.md) call.</span></span> 
  
[<span data-ttu-id="a94fd-105">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="a94fd-105">FindItemResponse</span></span>](finditemresponse.md)
  
[<span data-ttu-id="a94fd-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a94fd-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="a94fd-107">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a94fd-107">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
  
[<span data-ttu-id="a94fd-108">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="a94fd-108">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
  
[<span data-ttu-id="a94fd-109">Grupos</span><span class="sxs-lookup"><span data-stu-id="a94fd-109">Groups</span></span>](groups.md)
  
[<span data-ttu-id="a94fd-110">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="a94fd-110">GroupedItems</span></span>](groupeditems.md)
  
[<span data-ttu-id="a94fd-111">GroupIndex</span><span class="sxs-lookup"><span data-stu-id="a94fd-111">GroupIndex</span></span>](groupindex.md)
  
```xml
<GroupIndex/>
```

 <span data-ttu-id="a94fd-112">**cadeia de caracteres**</span><span class="sxs-lookup"><span data-stu-id="a94fd-112">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a94fd-113">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="a94fd-113">Attributes and elements</span></span>

<span data-ttu-id="a94fd-114">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a94fd-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a94fd-115">Atributos</span><span class="sxs-lookup"><span data-stu-id="a94fd-115">Attributes</span></span>

<span data-ttu-id="a94fd-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a94fd-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a94fd-117">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a94fd-117">Child elements</span></span>

<span data-ttu-id="a94fd-118">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a94fd-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a94fd-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a94fd-119">Parent elements</span></span>

|<span data-ttu-id="a94fd-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a94fd-120">**Element**</span></span>|<span data-ttu-id="a94fd-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a94fd-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a94fd-122">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="a94fd-122">GroupedItems</span></span>](groupeditems.md) <br/> |<span data-ttu-id="a94fd-123">Representa uma coleção de itens que são o resultado de uma chamada de [operação FindItem](finditem-operation.md) agrupada.</span><span class="sxs-lookup"><span data-stu-id="a94fd-123">Represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> <span data-ttu-id="a94fd-124">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="a94fd-124">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItemResponse/ResponseMessages/FindItemResponseMessage/RootFolder/Groups/GroupedItems[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a94fd-125">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="a94fd-125">Text value</span></span>

<span data-ttu-id="a94fd-126">Um valor de texto é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a94fd-126">A text value is required.</span></span> <span data-ttu-id="a94fd-127">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a94fd-127">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a94fd-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="a94fd-128">Remarks</span></span>

<span data-ttu-id="a94fd-129">Esse elemento ocorre somente em uma resposta de [operação FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a94fd-129">This element only occurs in a [FindItem operation](finditem-operation.md) response.</span></span> 
  
<span data-ttu-id="a94fd-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="a94fd-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a94fd-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="a94fd-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a94fd-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="a94fd-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a94fd-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a94fd-133">Schema name</span></span>  <br/> |<span data-ttu-id="a94fd-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a94fd-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="a94fd-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a94fd-135">Validation file</span></span>  <br/> |<span data-ttu-id="a94fd-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a94fd-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a94fd-137">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="a94fd-137">Can be empty</span></span>  <br/> |<span data-ttu-id="a94fd-138">False</span><span class="sxs-lookup"><span data-stu-id="a94fd-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a94fd-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="a94fd-139">See also</span></span>



[<span data-ttu-id="a94fd-140">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="a94fd-140">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="a94fd-141">Localizar itens</span><span class="sxs-lookup"><span data-stu-id="a94fd-141">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

