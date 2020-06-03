---
title: Contém
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Contains
api_type:
- schema
ms.assetid: 476d059d-c243-43e9-b475-319fc413ade2
description: O elemento Contains representa uma expressão de pesquisa que determina se uma determinada propriedade contém o valor da cadeia de caracteres constante fornecido.
ms.openlocfilehash: 79529bd752bcbce954ae3c8b0085c203b4eb8777
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527114"
---
# <a name="contains"></a><span data-ttu-id="6fdc3-103">Contém</span><span class="sxs-lookup"><span data-stu-id="6fdc3-103">Contains</span></span>

<span data-ttu-id="6fdc3-104">O elemento **Contains** representa uma expressão de pesquisa que determina se uma determinada propriedade contém o valor da cadeia de caracteres constante fornecido.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-104">The **Contains** element represents a search expression that determines whether a given property contains the supplied constant string value.</span></span> 
  
```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <FieldURI/>
   <Constant/>
</Contains>
```

```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <ExtendedFieldURI/>
   <Constant/>
</Contains>
```

```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <IndexedFieldURI/>
   <Constant/>
</Contains>
```


<span data-ttu-id="6fdc3-105">**ContainsExpressionType**</span><span class="sxs-lookup"><span data-stu-id="6fdc3-105">**ContainsExpressionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6fdc3-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6fdc3-106">Attributes and elements</span></span>

<span data-ttu-id="6fdc3-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6fdc3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6fdc3-108">Attributes</span></span>

|<span data-ttu-id="6fdc3-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="6fdc3-109">**Attribute**</span></span>|<span data-ttu-id="6fdc3-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6fdc3-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6fdc3-111">**ContainmentMode**</span><span class="sxs-lookup"><span data-stu-id="6fdc3-111">**ContainmentMode**</span></span> <br/> |<span data-ttu-id="6fdc3-112">Identifica os limites de uma pesquisa.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-112">Identifies the boundaries of a search.</span></span>  <br/> |
|<span data-ttu-id="6fdc3-113">**ContainmentComparison**</span><span class="sxs-lookup"><span data-stu-id="6fdc3-113">**ContainmentComparison**</span></span> <br/> |<span data-ttu-id="6fdc3-114">Determina se a pesquisa ignora casos e espaços.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-114">Determines whether the search ignores cases and spaces.</span></span>  <br/> |
   
#### <a name="containmentmode-attribute-values"></a><span data-ttu-id="6fdc3-115">Valores de atributo ContainmentMode</span><span class="sxs-lookup"><span data-stu-id="6fdc3-115">ContainmentMode attribute values</span></span>

|<span data-ttu-id="6fdc3-116">**Valor**</span><span class="sxs-lookup"><span data-stu-id="6fdc3-116">**Value**</span></span>|<span data-ttu-id="6fdc3-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6fdc3-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6fdc3-118">Fullstring</span><span class="sxs-lookup"><span data-stu-id="6fdc3-118">FullString</span></span>  <br/> |<span data-ttu-id="6fdc3-119">A comparação é entre a cadeia de caracteres completa e a constante.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-119">The comparison is between the full string and the constant.</span></span> <span data-ttu-id="6fdc3-120">O valor da propriedade e a constante fornecida são exatamente os mesmos.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-120">The property value and the supplied constant are precisely the same.</span></span>  <br/> |
|<span data-ttu-id="6fdc3-121">Precedidas</span><span class="sxs-lookup"><span data-stu-id="6fdc3-121">Prefixed</span></span>  <br/> |<span data-ttu-id="6fdc3-122">A comparação é entre o prefixo de cadeia de caracteres e a constante.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-122">The comparison is between the string prefix and the constant.</span></span>  <br/> |
|<span data-ttu-id="6fdc3-123">SUBSTRING</span><span class="sxs-lookup"><span data-stu-id="6fdc3-123">Substring</span></span>  <br/> |<span data-ttu-id="6fdc3-124">A comparação é entre uma subcadeia de caracteres e a constante.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-124">The comparison is between a substring of the string and the constant.</span></span>  <br/> |
|<span data-ttu-id="6fdc3-125">PrefixOnWords</span><span class="sxs-lookup"><span data-stu-id="6fdc3-125">PrefixOnWords</span></span>  <br/> |<span data-ttu-id="6fdc3-126">A comparação é entre um prefixo em palavras individuais na cadeia de caracteres e a constante.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-126">The comparison is between a prefix on individual words in the string and the constant.</span></span>  <br/> |
|<span data-ttu-id="6fdc3-127">ExactPhrase</span><span class="sxs-lookup"><span data-stu-id="6fdc3-127">ExactPhrase</span></span>  <br/> |<span data-ttu-id="6fdc3-128">A comparação é entre uma frase exata na cadeia de caracteres e a constante.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-128">The comparison is between an exact phrase in the string and the constant.</span></span>  <br/> |
   
#### <a name="containmentcomparison-attribute-values"></a><span data-ttu-id="6fdc3-129">Valores de atributo ContainmentComparison</span><span class="sxs-lookup"><span data-stu-id="6fdc3-129">ContainmentComparison attribute values</span></span>

|<span data-ttu-id="6fdc3-130">**Valor**</span><span class="sxs-lookup"><span data-stu-id="6fdc3-130">**Value**</span></span>|<span data-ttu-id="6fdc3-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6fdc3-131">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6fdc3-132">Exata</span><span class="sxs-lookup"><span data-stu-id="6fdc3-132">Exact</span></span>  <br/> |<span data-ttu-id="6fdc3-133">A comparação deve ser exata.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-133">The comparison must be exact.</span></span>  <br/> |
|<span data-ttu-id="6fdc3-134">IgnoreCase</span><span class="sxs-lookup"><span data-stu-id="6fdc3-134">IgnoreCase</span></span>  <br/> |<span data-ttu-id="6fdc3-135">A comparação ignora a capitalização.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-135">The comparison ignores casing.</span></span>  <br/> |
|<span data-ttu-id="6fdc3-136">IgnoreNonSpacingCharacters</span><span class="sxs-lookup"><span data-stu-id="6fdc3-136">IgnoreNonSpacingCharacters</span></span>  <br/> |<span data-ttu-id="6fdc3-137">A comparação ignora os caracteres sem espaçamento.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-137">The comparison ignores non-spacing characters.</span></span>  <br/> |
|<span data-ttu-id="6fdc3-138">Afastado</span><span class="sxs-lookup"><span data-stu-id="6fdc3-138">Loose</span></span>  <br/> |<span data-ttu-id="6fdc3-139">A ser removido.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-139">To be removed.</span></span>  <br/> |
|<span data-ttu-id="6fdc3-140">IgnoreCaseAndNonSpacingCharacters</span><span class="sxs-lookup"><span data-stu-id="6fdc3-140">IgnoreCaseAndNonSpacingCharacters</span></span>  <br/> |<span data-ttu-id="6fdc3-141">A comparação ignora caracteres de capitalização e sem espaçamento.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-141">The comparison ignores casing and non-spacing characters.</span></span>  <br/> |
|<span data-ttu-id="6fdc3-142">LooseAndIgnoreCase</span><span class="sxs-lookup"><span data-stu-id="6fdc3-142">LooseAndIgnoreCase</span></span>  <br/> |<span data-ttu-id="6fdc3-143">A ser removido.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-143">To be removed.</span></span>  <br/> |
|<span data-ttu-id="6fdc3-144">LooseAndIgnoreNonSpace</span><span class="sxs-lookup"><span data-stu-id="6fdc3-144">LooseAndIgnoreNonSpace</span></span>  <br/> |<span data-ttu-id="6fdc3-145">A ser removido.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-145">To be removed.</span></span>  <br/> |
|<span data-ttu-id="6fdc3-146">LooseAndIgnoreCaseAndIgnoreNonSpace</span><span class="sxs-lookup"><span data-stu-id="6fdc3-146">LooseAndIgnoreCaseAndIgnoreNonSpace</span></span>  <br/> |<span data-ttu-id="6fdc3-147">A ser removido.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-147">To be removed.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6fdc3-148">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6fdc3-148">Child elements</span></span>

|<span data-ttu-id="6fdc3-149">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6fdc3-149">**Element**</span></span>|<span data-ttu-id="6fdc3-150">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6fdc3-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6fdc3-151">FieldURI</span><span class="sxs-lookup"><span data-stu-id="6fdc3-151">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="6fdc3-152">Identifica as propriedades com frequência referenciadas por URI.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-152">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="6fdc3-153">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="6fdc3-153">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="6fdc3-154">Identifica membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-154">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="6fdc3-155">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="6fdc3-155">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="6fdc3-156">Identifica as propriedades MAPI.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-156">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="6fdc3-157">Constante</span><span class="sxs-lookup"><span data-stu-id="6fdc3-157">Constant</span></span>](constant.md) <br/> |<span data-ttu-id="6fdc3-158">Identifica um valor constante em uma restrição.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-158">Identifies a constant value in a restriction.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6fdc3-159">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6fdc3-159">Parent elements</span></span>

|<span data-ttu-id="6fdc3-160">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6fdc3-160">**Element**</span></span>|<span data-ttu-id="6fdc3-161">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6fdc3-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6fdc3-162">Restriction</span><span class="sxs-lookup"><span data-stu-id="6fdc3-162">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="6fdc3-163">Representa a restrição ou a consulta usada para filtrar itens ou pastas no FindItem/FindFolder e operações de pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-163">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="6fdc3-164">Not</span><span class="sxs-lookup"><span data-stu-id="6fdc3-164">Not</span></span>](not.md) <br/> |<span data-ttu-id="6fdc3-165">Representa uma expressão de pesquisa que nega o valor booliano da expressão de pesquisa que ela contém.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-165">Represents a search expression that negates the Boolean value of the search expression it contains.</span></span>  <br/> |
|[<span data-ttu-id="6fdc3-166">And</span><span class="sxs-lookup"><span data-stu-id="6fdc3-166">And</span></span>](and.md) <br/> |<span data-ttu-id="6fdc3-167">Representa uma expressão de pesquisa que permite executar um Boolean e uma operação entre duas ou mais expressões de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-167">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="6fdc3-168">O resultado da operação and será **true** se todas as expressões de pesquisa contidas no e forem **true**.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-168">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="6fdc3-169">Or</span><span class="sxs-lookup"><span data-stu-id="6fdc3-169">Or</span></span>](or.md) <br/> |<span data-ttu-id="6fdc3-170">Representa uma expressão de pesquisa que executa uma expressão lógica ou na expressão de pesquisa que ela contém.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-170">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="6fdc3-171">O elemento [ou](or.md) retornará **true** se qualquer um dos seus filhos retornar **true**.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-171">The [Or](or.md) element will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6fdc3-172">Comentários</span><span class="sxs-lookup"><span data-stu-id="6fdc3-172">Remarks</span></span>

<span data-ttu-id="6fdc3-173">Os atributos são usados para determinar como os elementos são correspondidos.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-173">The attributes are used to determine how the elements are matched.</span></span>
  
<span data-ttu-id="6fdc3-174">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="6fdc3-174">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6fdc3-175">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6fdc3-175">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6fdc3-176">Namespace</span><span class="sxs-lookup"><span data-stu-id="6fdc3-176">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6fdc3-177">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6fdc3-177">Schema Name</span></span>  <br/> |<span data-ttu-id="6fdc3-178">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="6fdc3-178">Types schema</span></span>  <br/> |
|<span data-ttu-id="6fdc3-179">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6fdc3-179">Validation File</span></span>  <br/> |<span data-ttu-id="6fdc3-180">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6fdc3-180">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6fdc3-181">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6fdc3-181">Can be Empty</span></span>  <br/> |<span data-ttu-id="6fdc3-182">False</span><span class="sxs-lookup"><span data-stu-id="6fdc3-182">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6fdc3-183">Confira também</span><span class="sxs-lookup"><span data-stu-id="6fdc3-183">See also</span></span>

- [<span data-ttu-id="6fdc3-184">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6fdc3-184">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

