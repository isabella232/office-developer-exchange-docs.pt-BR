---
title: IsNotEqualTo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsNotEqualTo
api_type:
- schema
ms.assetid: e2eff26c-3403-45cd-bb74-1eb98c7dbfcd
description: O elemento IsNotEqualTo representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e retorna true se os valores não são iguais.
ms.openlocfilehash: c11f5ba5b8c0672bba0b9ae2a76211ac7d5d94ad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824059"
---
# <a name="isnotequalto"></a><span data-ttu-id="1dab2-103">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="1dab2-103">IsNotEqualTo</span></span>

<span data-ttu-id="1dab2-104">O elemento **IsNotEqualTo** representa uma expressão de pesquisa que compara uma propriedade com um valor de constante ou outra propriedade e retorna **true** se os valores não são iguais.</span><span class="sxs-lookup"><span data-stu-id="1dab2-104">The **IsNotEqualTo** element represents a search expression that compares a property with either a constant value or another property and returns **true** if the values are not the same.</span></span> 
  
```xml
<IsNotEqualTo>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsNotEqualTo>
```

 <span data-ttu-id="1dab2-105">**IsNotEqualToType**</span><span class="sxs-lookup"><span data-stu-id="1dab2-105">**IsNotEqualToType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1dab2-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="1dab2-106">Attributes and elements</span></span>

<span data-ttu-id="1dab2-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="1dab2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1dab2-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="1dab2-108">Attributes</span></span>

<span data-ttu-id="1dab2-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="1dab2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1dab2-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="1dab2-110">Child elements</span></span>

|<span data-ttu-id="1dab2-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1dab2-111">**Element**</span></span>|<span data-ttu-id="1dab2-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1dab2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1dab2-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="1dab2-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="1dab2-114">Identifica as propriedades frequentemente referenciadas pelo URI.</span><span class="sxs-lookup"><span data-stu-id="1dab2-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="1dab2-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="1dab2-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="1dab2-116">Identifica a membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="1dab2-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="1dab2-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="1dab2-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="1dab2-118">Identifica as propriedades MAPI.</span><span class="sxs-lookup"><span data-stu-id="1dab2-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="1dab2-119">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="1dab2-119">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="1dab2-120">Representa uma propriedade ou um valor de constante a ser usado ao comparar com outra propriedade.</span><span class="sxs-lookup"><span data-stu-id="1dab2-120">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1dab2-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="1dab2-121">Parent elements</span></span>

|<span data-ttu-id="1dab2-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="1dab2-122">**Element**</span></span>|<span data-ttu-id="1dab2-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1dab2-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1dab2-124">Restriction</span><span class="sxs-lookup"><span data-stu-id="1dab2-124">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="1dab2-125">Representa a restrição ou a consulta que é usada para filtrar itens ou pastas nas operações da pasta FindItem/FindFolder e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="1dab2-125">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="1dab2-126">Não</span><span class="sxs-lookup"><span data-stu-id="1dab2-126">Not</span></span>](not.md) <br/> |<span data-ttu-id="1dab2-127">Representa uma expressão de pesquisa que dispensa o valor booliano da expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="1dab2-127">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="1dab2-128">E</span><span class="sxs-lookup"><span data-stu-id="1dab2-128">And</span></span>](and.md) <br/> |<span data-ttu-id="1dab2-129">Representa uma expressão de pesquisa que permite realizar uma operação Boolean e entre dois ou mais expressões de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="1dab2-129">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="1dab2-130">O resultado da operação e será **true** se todas as expressões de pesquisa contidas And forem **verdadeiras**.</span><span class="sxs-lookup"><span data-stu-id="1dab2-130">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="1dab2-131">Ou</span><span class="sxs-lookup"><span data-stu-id="1dab2-131">Or</span></span>](or.md) <br/> |<span data-ttu-id="1dab2-132">Representa uma expressão de pesquisa que realiza um OR lógico a expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="1dab2-132">Represents a search expression that performs a logical OR on the search expression that it contains.</span></span> <span data-ttu-id="1dab2-133">[Ou](or.md) retornará **true** se qualquer um dos seus filhos retornam **true**.</span><span class="sxs-lookup"><span data-stu-id="1dab2-133">[Or](or.md) will return **true** if any of its children return **true**.</span></span> <span data-ttu-id="1dab2-134">**Ou** deve ter dois ou mais filhos.</span><span class="sxs-lookup"><span data-stu-id="1dab2-134">**Or** must have two or more children.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1dab2-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="1dab2-135">Remarks</span></span>

<span data-ttu-id="1dab2-136">Para executar comparações de sequência, considere o uso do elemento [contém](contains.md) , como ele fornece opções para os parâmetros correspondentes como caso e espaços em branco.</span><span class="sxs-lookup"><span data-stu-id="1dab2-136">To perform string comparisons, consider using the [Contains](contains.md) element, as it provides options for matching parameters such as case and white space.</span></span> <span data-ttu-id="1dab2-137">Use o elemento [não](not.md) em conjunto com o elemento [contém](contains.md) para negar o resultado.</span><span class="sxs-lookup"><span data-stu-id="1dab2-137">Use the [Not](not.md) element in conjunction with the [Contains](contains.md) element to negate the result.</span></span> 
  
<span data-ttu-id="1dab2-138">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="1dab2-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1dab2-139">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="1dab2-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1dab2-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="1dab2-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1dab2-141">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="1dab2-141">Schema Name</span></span>  <br/> |<span data-ttu-id="1dab2-142">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="1dab2-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="1dab2-143">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="1dab2-143">Validation File</span></span>  <br/> |<span data-ttu-id="1dab2-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1dab2-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1dab2-145">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="1dab2-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="1dab2-146">False</span><span class="sxs-lookup"><span data-stu-id="1dab2-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1dab2-147">Ver também</span><span class="sxs-lookup"><span data-stu-id="1dab2-147">See also</span></span>



- [<span data-ttu-id="1dab2-148">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1dab2-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

