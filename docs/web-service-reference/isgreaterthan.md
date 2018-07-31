---
title: IsGreaterThan
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsGreaterThan
api_type:
- schema
ms.assetid: a6e9d462-cfa7-40ec-903e-128c95050352
description: O elemento IsGreaterThan representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retorna true se a primeira propriedade for maior.
ms.openlocfilehash: dfa7c221bb04e59f1ae12eeb5b9f2e1f09aea3ce
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353487"
---
# <a name="isgreaterthan"></a><span data-ttu-id="570c1-103">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="570c1-103">IsGreaterThan</span></span>

<span data-ttu-id="570c1-104">O elemento **IsGreaterThan** representa uma expressão de pesquisa que compara uma propriedade com um valor de constante ou outra propriedade e retorna **true** se a primeira propriedade for maior.</span><span class="sxs-lookup"><span data-stu-id="570c1-104">The **IsGreaterThan** element represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is greater.</span></span> 
  
```xml
<IsGreaterThan>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsGreaterThan>
```

```xml
<IsGreaterThan>
   <IndexedFieldURI/> 
   <FieldURIOrConstant/>
</IsGreaterThan>
```

```xml
<IsGreaterThan>
   <ExtendedFieldURI/>
   <FieldURIOrConstant/>
</IsGreaterThan>
```

<span data-ttu-id="570c1-105">**IsGreaterThanType**</span><span class="sxs-lookup"><span data-stu-id="570c1-105">**IsGreaterThanType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="570c1-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="570c1-106">Attributes and elements</span></span>

<span data-ttu-id="570c1-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="570c1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="570c1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="570c1-108">Attributes</span></span>

<span data-ttu-id="570c1-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="570c1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="570c1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="570c1-110">Child elements</span></span>

|<span data-ttu-id="570c1-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="570c1-111">**Element**</span></span>|<span data-ttu-id="570c1-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="570c1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="570c1-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="570c1-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="570c1-114">Identifica as propriedades frequentemente referenciadas pelo URI.</span><span class="sxs-lookup"><span data-stu-id="570c1-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="570c1-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="570c1-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="570c1-116">Identifica a membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="570c1-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="570c1-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="570c1-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="570c1-118">Identifica as propriedades MAPI.</span><span class="sxs-lookup"><span data-stu-id="570c1-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="570c1-119">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="570c1-119">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="570c1-120">Representa uma propriedade ou um valor de constante a ser usado ao comparar com outra propriedade.</span><span class="sxs-lookup"><span data-stu-id="570c1-120">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="570c1-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="570c1-121">Parent elements</span></span>

|<span data-ttu-id="570c1-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="570c1-122">**Element**</span></span>|<span data-ttu-id="570c1-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="570c1-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="570c1-124">Restriction</span><span class="sxs-lookup"><span data-stu-id="570c1-124">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="570c1-125">Representa a restrição ou a consulta que é usada para filtrar itens ou pastas nas operações da pasta FindItem/FindFolder e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="570c1-125">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="570c1-126">Não</span><span class="sxs-lookup"><span data-stu-id="570c1-126">Not</span></span>](not.md) <br/> |<span data-ttu-id="570c1-127">Representa uma expressão de pesquisa que dispensa o valor booliano da expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="570c1-127">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="570c1-128">E</span><span class="sxs-lookup"><span data-stu-id="570c1-128">And</span></span>](and.md) <br/> |<span data-ttu-id="570c1-129">Representa uma expressão de pesquisa que permite realizar uma operação Boolean e entre dois ou mais expressões de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="570c1-129">Represents a search expression that enables you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="570c1-130">O resultado da operação e será **true** se todas as expressões de pesquisa contidas And forem **verdadeiras**.</span><span class="sxs-lookup"><span data-stu-id="570c1-130">The result of the And operation is **true** if all the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="570c1-131">Ou</span><span class="sxs-lookup"><span data-stu-id="570c1-131">Or</span></span>](or.md) <br/> |<span data-ttu-id="570c1-132">Representa uma expressão de pesquisa que realiza um OR lógico a expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="570c1-132">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="570c1-133">[Ou](or.md) retornará **true** se qualquer um dos seus filhos retornam **true**.</span><span class="sxs-lookup"><span data-stu-id="570c1-133">[Or](or.md) will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="570c1-134">Comentários</span><span class="sxs-lookup"><span data-stu-id="570c1-134">Remarks</span></span>

<span data-ttu-id="570c1-135">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="570c1-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="570c1-136">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="570c1-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="570c1-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="570c1-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="570c1-138">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="570c1-138">Schema Name</span></span>  <br/> |<span data-ttu-id="570c1-139">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="570c1-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="570c1-140">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="570c1-140">Validation File</span></span>  <br/> |<span data-ttu-id="570c1-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="570c1-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="570c1-142">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="570c1-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="570c1-143">False</span><span class="sxs-lookup"><span data-stu-id="570c1-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="570c1-144">Ver também</span><span class="sxs-lookup"><span data-stu-id="570c1-144">See also</span></span>

- [<span data-ttu-id="570c1-145">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="570c1-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

