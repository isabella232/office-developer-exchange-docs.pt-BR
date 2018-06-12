---
title: Restrição
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Restriction
api_type:
- schema
ms.assetid: 77f19014-d112-4999-8e83-ecc32a117a73
description: O elemento de restrição representa a restrição ou a consulta que é usada para filtrar itens ou pastas nas operações da pasta FindItem/FindFolder e pesquisa.
ms.openlocfilehash: 6b5702696db29910ae476a370bf362fe6a036ae7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825213"
---
# <a name="restriction"></a><span data-ttu-id="0216f-103">Restrição</span><span class="sxs-lookup"><span data-stu-id="0216f-103">Restriction</span></span>

<span data-ttu-id="0216f-104">O elemento de **restrição** representa a restrição ou a consulta que é usada para filtrar itens ou pastas nas operações da pasta FindItem/FindFolder e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="0216f-104">The **Restriction** element represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span> 
  
```xml
<Restriction>
   <SearchExpression/>
</Restriction>
```

 <span data-ttu-id="0216f-105">**RestrictionType**</span><span class="sxs-lookup"><span data-stu-id="0216f-105">**RestrictionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0216f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0216f-106">Attributes and elements</span></span>

<span data-ttu-id="0216f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0216f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0216f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0216f-108">Attributes</span></span>

<span data-ttu-id="0216f-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0216f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0216f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0216f-110">Child elements</span></span>

|<span data-ttu-id="0216f-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0216f-111">**Element**</span></span>|<span data-ttu-id="0216f-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0216f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0216f-113">E</span><span class="sxs-lookup"><span data-stu-id="0216f-113">And</span></span>](and.md) <br/> |<span data-ttu-id="0216f-114">Representa uma expressão de pesquisa que permite realizar uma operação de booleano **e** entre dois ou mais expressões de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="0216f-114">Represents a search expression that enables you to perform a Boolean **AND** operation between two or more search expressions.</span></span>  <br/> |
|[<span data-ttu-id="0216f-115">Contém</span><span class="sxs-lookup"><span data-stu-id="0216f-115">Contains</span></span>](contains.md) <br/> |<span data-ttu-id="0216f-116">Representa uma expressão de pesquisa que determina se uma determinada propriedade contém o valor de cadeia de caracteres constante fornecido.</span><span class="sxs-lookup"><span data-stu-id="0216f-116">Represents a search expression that determines whether a given property contains the supplied constant string value.</span></span>  <br/> |
|[<span data-ttu-id="0216f-117">Exclui</span><span class="sxs-lookup"><span data-stu-id="0216f-117">Excludes</span></span>](excludes.md) <br/> |<span data-ttu-id="0216f-118">Executa uma máscara de bit a bit das propriedades.</span><span class="sxs-lookup"><span data-stu-id="0216f-118">Performs a bitwise mask of the properties.</span></span>  <br/> |
|[<span data-ttu-id="0216f-119">Existe</span><span class="sxs-lookup"><span data-stu-id="0216f-119">Exists</span></span>](exists.md) <br/> |<span data-ttu-id="0216f-120">Representa uma expressão de pesquisa que retornará **true** se a propriedade fornecida existir em um item.</span><span class="sxs-lookup"><span data-stu-id="0216f-120">Represents a search expression that returns **true** if the supplied property exists on an item.</span></span>  <br/> |
|[<span data-ttu-id="0216f-121">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="0216f-121">IsEqualTo</span></span>](isequalto.md) <br/> |<span data-ttu-id="0216f-122">Representa uma expressão de pesquisa que compara uma propriedade com a um valor de constante ou outra propriedade e será avaliada como **true** , se eles forem iguais.</span><span class="sxs-lookup"><span data-stu-id="0216f-122">Represents a search expression that compares a property with either a constant value or another property and evaluates to **true** if they are equal.</span></span>  <br/> |
|[<span data-ttu-id="0216f-123">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="0216f-123">IsGreaterThan</span></span>](isgreaterthan.md) <br/> |<span data-ttu-id="0216f-124">Representa uma expressão de pesquisa que compara uma propriedade com um valor de constante ou outra propriedade e retorna **true** se a primeira propriedade for maior que o valor ou a propriedade.</span><span class="sxs-lookup"><span data-stu-id="0216f-124">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is greater than the value or property.</span></span>  <br/> |
|[<span data-ttu-id="0216f-125">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="0216f-125">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md) <br/> |<span data-ttu-id="0216f-126">Representa uma expressão de pesquisa que compara uma propriedade com um valor de constante ou outra propriedade e retorna **true** se a propriedade primeira for maior que ou igual ao valor ou propriedade.</span><span class="sxs-lookup"><span data-stu-id="0216f-126">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is greater than or equal to the value or property.</span></span>  <br/> |
|[<span data-ttu-id="0216f-127">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="0216f-127">IsLessThan</span></span>](islessthan.md) <br/> |<span data-ttu-id="0216f-128">Representa uma expressão de pesquisa que compara uma propriedade com um valor de constante ou outra propriedade e retorna **true** se a primeira propriedade for menor que o valor ou a propriedade.</span><span class="sxs-lookup"><span data-stu-id="0216f-128">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is less than the value or property.</span></span>  <br/> |
|[<span data-ttu-id="0216f-129">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="0216f-129">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md) <br/> |<span data-ttu-id="0216f-130">Representa uma expressão de pesquisa que compara uma propriedade com um valor de constante ou outra propriedade e retorna **true** se a primeira propriedade for menor ou igual ao valor ou propriedade.</span><span class="sxs-lookup"><span data-stu-id="0216f-130">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is less than or equal to the value or property.</span></span>  <br/> |
|[<span data-ttu-id="0216f-131">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="0216f-131">IsNotEqualTo</span></span>](isnotequalto.md) <br/> |<span data-ttu-id="0216f-132">Representa uma expressão de pesquisa que compara uma propriedade com um valor de constante ou outra propriedade e retorna **true** se os valores não são iguais.</span><span class="sxs-lookup"><span data-stu-id="0216f-132">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the values are not the same.</span></span>  <br/> |
|[<span data-ttu-id="0216f-133">Não</span><span class="sxs-lookup"><span data-stu-id="0216f-133">Not</span></span>](not.md) <br/> |<span data-ttu-id="0216f-134">Representa uma expressão de pesquisa que dispensa o valor booliano da expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="0216f-134">Represents a search expression that negates the Boolean value of the search expression it contains.</span></span>  <br/> |
|[<span data-ttu-id="0216f-135">Ou</span><span class="sxs-lookup"><span data-stu-id="0216f-135">Or</span></span>](or.md) <br/> |<span data-ttu-id="0216f-136">Representa uma expressão de pesquisa que executa uma operação **OR** lógica a expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="0216f-136">Represents a search expression that performs a logical **OR** operation on the search expression it contains.</span></span> <span data-ttu-id="0216f-137">O elemento **ou** retornará **true** se qualquer um dos seus filhos retornam **true**.</span><span class="sxs-lookup"><span data-stu-id="0216f-137">The **Or** element will return **true** if any of its children return **true**.</span></span>  <br/> |
|[<span data-ttu-id="0216f-138">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="0216f-138">SearchExpression</span></span>](searchexpression.md) <br/> |<span data-ttu-id="0216f-139">Representa o elemento substituído dentro de uma restrição.</span><span class="sxs-lookup"><span data-stu-id="0216f-139">Represents the substituted element within a restriction.</span></span> <span data-ttu-id="0216f-140">Este elemento não é usado em um documento de instância XML.</span><span class="sxs-lookup"><span data-stu-id="0216f-140">This element is not used in an XML instance document.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0216f-141">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0216f-141">Parent elements</span></span>

|<span data-ttu-id="0216f-142">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0216f-142">**Element**</span></span>|<span data-ttu-id="0216f-143">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0216f-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0216f-144">FindFolder</span><span class="sxs-lookup"><span data-stu-id="0216f-144">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="0216f-145">Define uma solicitação para identificar pastas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0216f-145">Defines a request to identify folders in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0216f-146">FindItem</span><span class="sxs-lookup"><span data-stu-id="0216f-146">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="0216f-147">Define uma solicitação para localizar itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0216f-147">Defines a request to find items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0216f-148">SearchParameters</span><span class="sxs-lookup"><span data-stu-id="0216f-148">SearchParameters</span></span>](searchparameters.md) <br/> |<span data-ttu-id="0216f-149">Representa os parâmetros que definem a uma pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="0216f-149">Represents the parameters that define a search folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0216f-150">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="0216f-150">Remarks</span></span>

<span data-ttu-id="0216f-151">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="0216f-151">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0216f-152">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0216f-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0216f-153">Namespace</span><span class="sxs-lookup"><span data-stu-id="0216f-153">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0216f-154">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0216f-154">Schema Name</span></span>  <br/> |<span data-ttu-id="0216f-155">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0216f-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="0216f-156">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0216f-156">Validation File</span></span>  <br/> |<span data-ttu-id="0216f-157">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0216f-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0216f-158">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0216f-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="0216f-159">False</span><span class="sxs-lookup"><span data-stu-id="0216f-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0216f-160">Ver também</span><span class="sxs-lookup"><span data-stu-id="0216f-160">See also</span></span>



- [<span data-ttu-id="0216f-161">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0216f-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

