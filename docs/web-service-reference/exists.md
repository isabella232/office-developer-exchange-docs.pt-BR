---
title: Saídas
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
description: O elemento Exists representa uma expressão de pesquisa que retorna true se a propriedade fornecida existir em um item.
ms.openlocfilehash: b5e7a24c5214574ef385cd6ffca87ed5f861c188
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456945"
---
# <a name="exists"></a><span data-ttu-id="f9fe6-103">Saídas</span><span class="sxs-lookup"><span data-stu-id="f9fe6-103">Exists</span></span>

<span data-ttu-id="f9fe6-104">O elemento **Exists** representa uma expressão de pesquisa que retorna **true** se a propriedade fornecida existir em um item.</span><span class="sxs-lookup"><span data-stu-id="f9fe6-104">The **Exists** element represents a search expression that returns **true** if the supplied property exists on an item.</span></span> 
  
```xml
<Exists>
   <Path/>
</Exists>
```

 <span data-ttu-id="f9fe6-105">**Existtype**</span><span class="sxs-lookup"><span data-stu-id="f9fe6-105">**ExistsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f9fe6-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f9fe6-106">Attributes and elements</span></span>

<span data-ttu-id="f9fe6-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f9fe6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f9fe6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f9fe6-108">Attributes</span></span>

<span data-ttu-id="f9fe6-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f9fe6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f9fe6-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f9fe6-110">Child elements</span></span>

|<span data-ttu-id="f9fe6-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f9fe6-111">**Element**</span></span>|<span data-ttu-id="f9fe6-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f9fe6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9fe6-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="f9fe6-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="f9fe6-114">Identifica as propriedades com frequência referenciadas por URI.</span><span class="sxs-lookup"><span data-stu-id="f9fe6-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="f9fe6-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="f9fe6-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="f9fe6-116">Identifica membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="f9fe6-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="f9fe6-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="f9fe6-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="f9fe6-118">Identifica as propriedades MAPI.</span><span class="sxs-lookup"><span data-stu-id="f9fe6-118">Identifies MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f9fe6-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f9fe6-119">Parent elements</span></span>

|<span data-ttu-id="f9fe6-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f9fe6-120">**Element**</span></span>|<span data-ttu-id="f9fe6-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f9fe6-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9fe6-122">Restriction</span><span class="sxs-lookup"><span data-stu-id="f9fe6-122">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="f9fe6-123">Representa a restrição ou a consulta usada para filtrar itens ou pastas no FindItem/FindFolder e operações de pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="f9fe6-123">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="f9fe6-124">Not</span><span class="sxs-lookup"><span data-stu-id="f9fe6-124">Not</span></span>](not.md) <br/> |<span data-ttu-id="f9fe6-125">Representa uma expressão de pesquisa que nega o valor booliano da expressão de pesquisa que ela contém.</span><span class="sxs-lookup"><span data-stu-id="f9fe6-125">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="f9fe6-126">And</span><span class="sxs-lookup"><span data-stu-id="f9fe6-126">And</span></span>](and.md) <br/> |<span data-ttu-id="f9fe6-127">Representa uma expressão de pesquisa que permite que você execute um Boolean e uma operação entre duas ou mais expressões de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="f9fe6-127">Represents a search expression that enables you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="f9fe6-128">O resultado da operação and será **true** se todas as expressões de pesquisa contidas no e forem **true**.</span><span class="sxs-lookup"><span data-stu-id="f9fe6-128">The result of the And operation is **true** if all the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="f9fe6-129">Or</span><span class="sxs-lookup"><span data-stu-id="f9fe6-129">Or</span></span>](or.md) <br/> |<span data-ttu-id="f9fe6-130">Representa uma expressão de pesquisa que executa uma expressão lógica ou na expressão de pesquisa que ela contém.</span><span class="sxs-lookup"><span data-stu-id="f9fe6-130">Represents a search expression that performs a logical OR on the search expression that it contains.</span></span> <span data-ttu-id="f9fe6-131">[Ou](or.md) retornará **true** se qualquer um dos seus filhos retornar **true**.</span><span class="sxs-lookup"><span data-stu-id="f9fe6-131">[Or](or.md) will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f9fe6-132">Comentários</span><span class="sxs-lookup"><span data-stu-id="f9fe6-132">Remarks</span></span>

<span data-ttu-id="f9fe6-133">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f9fe6-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f9fe6-134">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f9fe6-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f9fe6-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="f9fe6-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f9fe6-136">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f9fe6-136">Schema Name</span></span>  <br/> |<span data-ttu-id="f9fe6-137">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f9fe6-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="f9fe6-138">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f9fe6-138">Validation File</span></span>  <br/> |<span data-ttu-id="f9fe6-139">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f9fe6-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f9fe6-140">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f9fe6-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="f9fe6-141">False</span><span class="sxs-lookup"><span data-stu-id="f9fe6-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f9fe6-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="f9fe6-142">See also</span></span>



- [<span data-ttu-id="f9fe6-143">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f9fe6-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

