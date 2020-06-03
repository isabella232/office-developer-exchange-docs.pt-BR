---
title: IsEqualTo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsEqualTo
api_type:
- schema
ms.assetid: 48e7e067-049c-4184-8026-071e6f558e8a
description: O elemento IsEqualTo representa uma expressão de pesquisa que compara uma propriedade com um valor constante ou outra propriedade e é avaliada como true se elas forem iguais.
ms.openlocfilehash: 857192443ab0520bb26ead399bc5364cc862a4fb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455293"
---
# <a name="isequalto"></a><span data-ttu-id="c029b-103">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="c029b-103">IsEqualTo</span></span>

<span data-ttu-id="c029b-104">O elemento **IsEqualTo** representa uma expressão de pesquisa que compara uma propriedade com um valor constante ou outra propriedade e é avaliada como true se elas forem iguais.</span><span class="sxs-lookup"><span data-stu-id="c029b-104">The **IsEqualTo** element represents a search expression that compares a property with either a constant value or another property and evaluates to true if they are equal.</span></span> 
  
```xml
<IsEqualTo>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsEqualTo>
```

```xml
<IsEqualTo>
   <ExtendedFieldURI/>
   <FieldURIOrConstant/>
</IsEqualTo>
```

```xml
<IsEqualTo>
   <IndexedFieldURI/> 
   <FieldURIOrConstant/>
</IsEqualTo>
```

<span data-ttu-id="c029b-105">**IsEqualToType**</span><span class="sxs-lookup"><span data-stu-id="c029b-105">**IsEqualToType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c029b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c029b-106">Attributes and elements</span></span>

<span data-ttu-id="c029b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c029b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c029b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c029b-108">Attributes</span></span>

<span data-ttu-id="c029b-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c029b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c029b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c029b-110">Child elements</span></span>

|<span data-ttu-id="c029b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c029b-111">**Element**</span></span>|<span data-ttu-id="c029b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c029b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c029b-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="c029b-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="c029b-114">Identifica as propriedades com frequência referenciadas por URI.</span><span class="sxs-lookup"><span data-stu-id="c029b-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="c029b-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="c029b-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="c029b-116">Identifica membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="c029b-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="c029b-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="c029b-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="c029b-118">Identifica as propriedades MAPI.</span><span class="sxs-lookup"><span data-stu-id="c029b-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="c029b-119">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="c029b-119">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="c029b-120">Representa uma propriedade ou um valor de constante a ser usado ao comparar com outra propriedade.</span><span class="sxs-lookup"><span data-stu-id="c029b-120">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c029b-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c029b-121">Parent elements</span></span>

|<span data-ttu-id="c029b-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c029b-122">**Element**</span></span>|<span data-ttu-id="c029b-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c029b-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c029b-124">Restriction</span><span class="sxs-lookup"><span data-stu-id="c029b-124">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="c029b-125">Representa a restrição ou a consulta usada para filtrar itens ou pastas no FindItem/FindFolder e operações de pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="c029b-125">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="c029b-126">Not</span><span class="sxs-lookup"><span data-stu-id="c029b-126">Not</span></span>](not.md) <br/> |<span data-ttu-id="c029b-127">Representa uma expressão de pesquisa que nega o valor booliano da expressão de pesquisa que ela contém.</span><span class="sxs-lookup"><span data-stu-id="c029b-127">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="c029b-128">And</span><span class="sxs-lookup"><span data-stu-id="c029b-128">And</span></span>](and.md) <br/> |<span data-ttu-id="c029b-129">Representa uma expressão de pesquisa que permite executar um Boolean e uma operação entre duas ou mais expressões de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="c029b-129">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="c029b-130">O resultado da operação and será **true** se todas as expressões de pesquisa contidas no e forem **true**.</span><span class="sxs-lookup"><span data-stu-id="c029b-130">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="c029b-131">Or</span><span class="sxs-lookup"><span data-stu-id="c029b-131">Or</span></span>](or.md) <br/> |<span data-ttu-id="c029b-132">Representa uma expressão de pesquisa que executa uma expressão lógica ou na expressão de pesquisa que ela contém.</span><span class="sxs-lookup"><span data-stu-id="c029b-132">Represents a search expression that performs a logical OR on the search expression that it contains.</span></span> <span data-ttu-id="c029b-133">[Ou](or.md) retornará true se qualquer um dos seus filhos retornar true.</span><span class="sxs-lookup"><span data-stu-id="c029b-133">[Or](or.md) will return true if any of its children return true.</span></span> <span data-ttu-id="c029b-134">**Ou** deve ter dois ou mais filhos.</span><span class="sxs-lookup"><span data-stu-id="c029b-134">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c029b-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="c029b-135">Remarks</span></span>

<span data-ttu-id="c029b-136">Para realizar comparações de cadeia de caracteres, considere usar o elemento [Contains](contains.md) , pois fornece opções para correspondência de parâmetros, como maiúsculas e minúsculas e espaços em branco.</span><span class="sxs-lookup"><span data-stu-id="c029b-136">To perform string comparisons, consider using the [Contains](contains.md) element, as it provides options for matching parameters, such as case and white space.</span></span> <span data-ttu-id="c029b-137">Use o elemento [não](not.md) em conjunto com o elemento [Contains](contains.md) para negar o resultado.</span><span class="sxs-lookup"><span data-stu-id="c029b-137">Use the [Not](not.md) element in conjunction with the [Contains](contains.md) element to negate the result.</span></span> 
  
<span data-ttu-id="c029b-138">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="c029b-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c029b-139">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c029b-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c029b-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="c029b-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c029b-141">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c029b-141">Schema Name</span></span>  <br/> |<span data-ttu-id="c029b-142">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c029b-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="c029b-143">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c029b-143">Validation File</span></span>  <br/> |<span data-ttu-id="c029b-144">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c029b-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c029b-145">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c029b-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="c029b-146">False</span><span class="sxs-lookup"><span data-stu-id="c029b-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c029b-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="c029b-147">See also</span></span>

- [<span data-ttu-id="c029b-148">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c029b-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

