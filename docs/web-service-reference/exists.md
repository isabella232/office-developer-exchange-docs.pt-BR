---
title: Existe
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Exists
api_type:
- schema
ms.assetid: 55d568bd-8dbc-4d50-b9d7-54b74a54d4b5
description: O elemento Exists representa uma expressão de pesquisa que retornará true se a propriedade fornecida existir em um item.
ms.openlocfilehash: d30f4b505afcac32afbfeaf2289c964ba145668e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752136"
---
# <a name="exists"></a><span data-ttu-id="0a8e5-103">Existe</span><span class="sxs-lookup"><span data-stu-id="0a8e5-103">Exists</span></span>

<span data-ttu-id="0a8e5-104">O elemento **Exists** representa uma expressão de pesquisa que retornará **true** se a propriedade fornecida existir em um item.</span><span class="sxs-lookup"><span data-stu-id="0a8e5-104">The **Exists** element represents a search expression that returns **true** if the supplied property exists on an item.</span></span> 
  
```xml
<Exists>
   <Path/>
</Exists>
```

 <span data-ttu-id="0a8e5-105">**ExistsType**</span><span class="sxs-lookup"><span data-stu-id="0a8e5-105">**ExistsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0a8e5-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0a8e5-106">Attributes and elements</span></span>

<span data-ttu-id="0a8e5-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0a8e5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0a8e5-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0a8e5-108">Attributes</span></span>

<span data-ttu-id="0a8e5-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0a8e5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0a8e5-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0a8e5-110">Child elements</span></span>

|<span data-ttu-id="0a8e5-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0a8e5-111">**Element**</span></span>|<span data-ttu-id="0a8e5-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0a8e5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a8e5-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="0a8e5-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="0a8e5-114">Identifica as propriedades frequentemente referenciadas pelo URI.</span><span class="sxs-lookup"><span data-stu-id="0a8e5-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="0a8e5-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="0a8e5-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="0a8e5-116">Identifica a membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="0a8e5-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="0a8e5-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="0a8e5-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="0a8e5-118">Identifica as propriedades MAPI.</span><span class="sxs-lookup"><span data-stu-id="0a8e5-118">Identifies MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0a8e5-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0a8e5-119">Parent elements</span></span>

|<span data-ttu-id="0a8e5-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0a8e5-120">**Element**</span></span>|<span data-ttu-id="0a8e5-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0a8e5-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a8e5-122">Restriction</span><span class="sxs-lookup"><span data-stu-id="0a8e5-122">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="0a8e5-123">Representa a restrição ou a consulta que é usada para filtrar itens ou pastas nas operações da pasta FindItem/FindFolder e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="0a8e5-123">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="0a8e5-124">Não</span><span class="sxs-lookup"><span data-stu-id="0a8e5-124">Not</span></span>](not.md) <br/> |<span data-ttu-id="0a8e5-125">Representa uma expressão de pesquisa que dispensa o valor booliano da expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="0a8e5-125">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="0a8e5-126">E</span><span class="sxs-lookup"><span data-stu-id="0a8e5-126">And</span></span>](and.md) <br/> |<span data-ttu-id="0a8e5-127">Representa uma expressão de pesquisa que permite realizar uma operação Boolean e entre dois ou mais expressões de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="0a8e5-127">Represents a search expression that enables you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="0a8e5-128">O resultado da operação e será **true** se todas as expressões de pesquisa contidas And forem **verdadeiras**.</span><span class="sxs-lookup"><span data-stu-id="0a8e5-128">The result of the And operation is **true** if all the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="0a8e5-129">Ou</span><span class="sxs-lookup"><span data-stu-id="0a8e5-129">Or</span></span>](or.md) <br/> |<span data-ttu-id="0a8e5-130">Representa uma expressão de pesquisa que realiza um OR lógico a expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="0a8e5-130">Represents a search expression that performs a logical OR on the search expression that it contains.</span></span> <span data-ttu-id="0a8e5-131">[Ou](or.md) retornará **true** se qualquer um dos seus filhos retornam **true**.</span><span class="sxs-lookup"><span data-stu-id="0a8e5-131">[Or](or.md) will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0a8e5-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="0a8e5-132">Remarks</span></span>

<span data-ttu-id="0a8e5-133">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="0a8e5-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0a8e5-134">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0a8e5-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0a8e5-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="0a8e5-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0a8e5-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0a8e5-136">Schema Name</span></span>  <br/> |<span data-ttu-id="0a8e5-137">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0a8e5-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="0a8e5-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0a8e5-138">Validation File</span></span>  <br/> |<span data-ttu-id="0a8e5-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0a8e5-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0a8e5-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0a8e5-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="0a8e5-141">False</span><span class="sxs-lookup"><span data-stu-id="0a8e5-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0a8e5-142">Ver também</span><span class="sxs-lookup"><span data-stu-id="0a8e5-142">See also</span></span>



- [<span data-ttu-id="0a8e5-143">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0a8e5-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

