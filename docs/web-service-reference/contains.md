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
description: O elemento contém representa uma expressão de pesquisa que determina se uma determinada propriedade contém o valor de cadeia de caracteres constante fornecido.
ms.openlocfilehash: 083efdf32cd32bea6964361b5b558480aa937280
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751468"
---
# <a name="contains"></a><span data-ttu-id="64c05-103">Contém</span><span class="sxs-lookup"><span data-stu-id="64c05-103">Contains</span></span>

<span data-ttu-id="64c05-104">O elemento **contém** representa uma expressão de pesquisa que determina se uma determinada propriedade contém o valor de cadeia de caracteres constante fornecido.</span><span class="sxs-lookup"><span data-stu-id="64c05-104">The **Contains** element represents a search expression that determines whether a given property contains the supplied constant string value.</span></span> 
  
```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <FieldURI/>
   <Constant/>
</Contains>
```

 <span data-ttu-id="64c05-105">**ContainsExpressionType**</span><span class="sxs-lookup"><span data-stu-id="64c05-105">**ContainsExpressionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="64c05-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="64c05-106">Attributes and elements</span></span>

<span data-ttu-id="64c05-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="64c05-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64c05-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="64c05-108">Attributes</span></span>

|<span data-ttu-id="64c05-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="64c05-109">**Attribute**</span></span>|<span data-ttu-id="64c05-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="64c05-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="64c05-111">**ContainmentMode**</span><span class="sxs-lookup"><span data-stu-id="64c05-111">**ContainmentMode**</span></span> <br/> |<span data-ttu-id="64c05-112">Identifica os limites de uma pesquisa.</span><span class="sxs-lookup"><span data-stu-id="64c05-112">Identifies the boundaries of a search.</span></span>  <br/> |
|<span data-ttu-id="64c05-113">**ContainmentComparison**</span><span class="sxs-lookup"><span data-stu-id="64c05-113">**ContainmentComparison**</span></span> <br/> |<span data-ttu-id="64c05-114">Determina se a pesquisa ignora casos e espaços.</span><span class="sxs-lookup"><span data-stu-id="64c05-114">Determines whether the search ignores cases and spaces.</span></span>  <br/> |
   
#### <a name="containmentmode-attribute-values"></a><span data-ttu-id="64c05-115">Valores de atributo ContainmentMode</span><span class="sxs-lookup"><span data-stu-id="64c05-115">ContainmentMode attribute values</span></span>

|<span data-ttu-id="64c05-116">**Valor**</span><span class="sxs-lookup"><span data-stu-id="64c05-116">**Value**</span></span>|<span data-ttu-id="64c05-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="64c05-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="64c05-118">FullString</span><span class="sxs-lookup"><span data-stu-id="64c05-118">FullString</span></span>  <br/> |<span data-ttu-id="64c05-119">A comparação é entre a cadeia de caracteres completa e a constante.</span><span class="sxs-lookup"><span data-stu-id="64c05-119">The comparison is between the full string and the constant.</span></span> <span data-ttu-id="64c05-120">O valor da propriedade e a constante fornecida com precisão são os mesmos.</span><span class="sxs-lookup"><span data-stu-id="64c05-120">The property value and the supplied constant are precisely the same.</span></span>  <br/> |
|<span data-ttu-id="64c05-121">O prefixo</span><span class="sxs-lookup"><span data-stu-id="64c05-121">Prefixed</span></span>  <br/> |<span data-ttu-id="64c05-122">A comparação é entre o prefixo de cadeia de caracteres e a constante.</span><span class="sxs-lookup"><span data-stu-id="64c05-122">The comparison is between the string prefix and the constant.</span></span>  <br/> |
|<span data-ttu-id="64c05-123">Subcadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="64c05-123">Substring</span></span>  <br/> |<span data-ttu-id="64c05-124">A comparação é entre uma subcadeia da cadeia de caracteres e a constante.</span><span class="sxs-lookup"><span data-stu-id="64c05-124">The comparison is between a substring of the string and the constant.</span></span>  <br/> |
|<span data-ttu-id="64c05-125">PrefixOnWords</span><span class="sxs-lookup"><span data-stu-id="64c05-125">PrefixOnWords</span></span>  <br/> |<span data-ttu-id="64c05-126">A comparação é entre um prefixo de palavras individuais na cadeia de caracteres e a constante.</span><span class="sxs-lookup"><span data-stu-id="64c05-126">The comparison is between a prefix on individual words in the string and the constant.</span></span>  <br/> |
|<span data-ttu-id="64c05-127">ExactPhrase</span><span class="sxs-lookup"><span data-stu-id="64c05-127">ExactPhrase</span></span>  <br/> |<span data-ttu-id="64c05-128">A comparação é entre uma frase exata na cadeia de caracteres e a constante.</span><span class="sxs-lookup"><span data-stu-id="64c05-128">The comparison is between an exact phrase in the string and the constant.</span></span>  <br/> |
   
#### <a name="containmentcomparison-attribute-values"></a><span data-ttu-id="64c05-129">Valores de atributo ContainmentComparison</span><span class="sxs-lookup"><span data-stu-id="64c05-129">ContainmentComparison attribute values</span></span>

|<span data-ttu-id="64c05-130">**Valor**</span><span class="sxs-lookup"><span data-stu-id="64c05-130">**Value**</span></span>|<span data-ttu-id="64c05-131">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="64c05-131">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="64c05-132">Exact</span><span class="sxs-lookup"><span data-stu-id="64c05-132">Exact</span></span>  <br/> |<span data-ttu-id="64c05-133">A comparação deve ser exata.</span><span class="sxs-lookup"><span data-stu-id="64c05-133">The comparison must be exact.</span></span>  <br/> |
|<span data-ttu-id="64c05-134">IgnoreCase</span><span class="sxs-lookup"><span data-stu-id="64c05-134">IgnoreCase</span></span>  <br/> |<span data-ttu-id="64c05-135">Comparação ignora maiusculas e minúsculas.</span><span class="sxs-lookup"><span data-stu-id="64c05-135">The comparison ignores casing.</span></span>  <br/> |
|<span data-ttu-id="64c05-136">IgnoreNonSpacingCharacters</span><span class="sxs-lookup"><span data-stu-id="64c05-136">IgnoreNonSpacingCharacters</span></span>  <br/> |<span data-ttu-id="64c05-137">Comparação ignora caracteres sem espaçamento.</span><span class="sxs-lookup"><span data-stu-id="64c05-137">The comparison ignores non-spacing characters.</span></span>  <br/> |
|<span data-ttu-id="64c05-138">Afastado</span><span class="sxs-lookup"><span data-stu-id="64c05-138">Loose</span></span>  <br/> |<span data-ttu-id="64c05-139">A ser removido.</span><span class="sxs-lookup"><span data-stu-id="64c05-139">To be removed.</span></span>  <br/> |
|<span data-ttu-id="64c05-140">IgnoreCaseAndNonSpacingCharacters</span><span class="sxs-lookup"><span data-stu-id="64c05-140">IgnoreCaseAndNonSpacingCharacters</span></span>  <br/> |<span data-ttu-id="64c05-141">Comparação ignora a cobertura e sem espaçamento de caracteres.</span><span class="sxs-lookup"><span data-stu-id="64c05-141">The comparison ignores casing and non-spacing characters.</span></span>  <br/> |
|<span data-ttu-id="64c05-142">LooseAndIgnoreCase</span><span class="sxs-lookup"><span data-stu-id="64c05-142">LooseAndIgnoreCase</span></span>  <br/> |<span data-ttu-id="64c05-143">A ser removido.</span><span class="sxs-lookup"><span data-stu-id="64c05-143">To be removed.</span></span>  <br/> |
|<span data-ttu-id="64c05-144">LooseAndIgnoreNonSpace</span><span class="sxs-lookup"><span data-stu-id="64c05-144">LooseAndIgnoreNonSpace</span></span>  <br/> |<span data-ttu-id="64c05-145">A ser removido.</span><span class="sxs-lookup"><span data-stu-id="64c05-145">To be removed.</span></span>  <br/> |
|<span data-ttu-id="64c05-146">LooseAndIgnoreCaseAndIgnoreNonSpace</span><span class="sxs-lookup"><span data-stu-id="64c05-146">LooseAndIgnoreCaseAndIgnoreNonSpace</span></span>  <br/> |<span data-ttu-id="64c05-147">A ser removido.</span><span class="sxs-lookup"><span data-stu-id="64c05-147">To be removed.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="64c05-148">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="64c05-148">Child elements</span></span>

|<span data-ttu-id="64c05-149">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="64c05-149">**Element**</span></span>|<span data-ttu-id="64c05-150">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="64c05-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64c05-151">FieldURI</span><span class="sxs-lookup"><span data-stu-id="64c05-151">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="64c05-152">Identifica as propriedades frequentemente referenciadas pelo URI.</span><span class="sxs-lookup"><span data-stu-id="64c05-152">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="64c05-153">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="64c05-153">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="64c05-154">Identifica a membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="64c05-154">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="64c05-155">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="64c05-155">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="64c05-156">Identifica as propriedades MAPI.</span><span class="sxs-lookup"><span data-stu-id="64c05-156">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="64c05-157">Constante</span><span class="sxs-lookup"><span data-stu-id="64c05-157">Constant</span></span>](constant.md) <br/> |<span data-ttu-id="64c05-158">Identifica um valor de constante em uma restrição.</span><span class="sxs-lookup"><span data-stu-id="64c05-158">Identifies a constant value in a restriction.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="64c05-159">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="64c05-159">Parent elements</span></span>

|<span data-ttu-id="64c05-160">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="64c05-160">**Element**</span></span>|<span data-ttu-id="64c05-161">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="64c05-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64c05-162">Restriction</span><span class="sxs-lookup"><span data-stu-id="64c05-162">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="64c05-163">Representa a restrição ou a consulta que é usada para filtrar itens ou pastas nas operações da pasta FindItem/FindFolder e pesquisa.</span><span class="sxs-lookup"><span data-stu-id="64c05-163">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="64c05-164">Não</span><span class="sxs-lookup"><span data-stu-id="64c05-164">Not</span></span>](not.md) <br/> |<span data-ttu-id="64c05-165">Representa uma expressão de pesquisa que dispensa o valor booliano da expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="64c05-165">Represents a search expression that negates the Boolean value of the search expression it contains.</span></span>  <br/> |
|[<span data-ttu-id="64c05-166">E</span><span class="sxs-lookup"><span data-stu-id="64c05-166">And</span></span>](and.md) <br/> |<span data-ttu-id="64c05-167">Representa uma expressão de pesquisa que permite realizar uma operação Boolean e entre dois ou mais expressões de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="64c05-167">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="64c05-168">O resultado da operação e será **true** se todas as expressões de pesquisa contidas And forem **verdadeiras**.</span><span class="sxs-lookup"><span data-stu-id="64c05-168">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="64c05-169">Ou</span><span class="sxs-lookup"><span data-stu-id="64c05-169">Or</span></span>](or.md) <br/> |<span data-ttu-id="64c05-170">Representa uma expressão de pesquisa que realiza um OR lógico a expressão de pesquisa que ele contém.</span><span class="sxs-lookup"><span data-stu-id="64c05-170">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="64c05-171">O elemento [ou](or.md) retornará **true** se qualquer um dos seus filhos retornam **true**.</span><span class="sxs-lookup"><span data-stu-id="64c05-171">The [Or](or.md) element will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="64c05-172">Comentários</span><span class="sxs-lookup"><span data-stu-id="64c05-172">Remarks</span></span>

<span data-ttu-id="64c05-173">Os atributos são usados para determinar como os elementos são correspondidos.</span><span class="sxs-lookup"><span data-stu-id="64c05-173">The attributes are used to determine how the elements are matched.</span></span>
  
<span data-ttu-id="64c05-174">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="64c05-174">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="64c05-175">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="64c05-175">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="64c05-176">Namespace</span><span class="sxs-lookup"><span data-stu-id="64c05-176">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="64c05-177">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="64c05-177">Schema Name</span></span>  <br/> |<span data-ttu-id="64c05-178">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="64c05-178">Types schema</span></span>  <br/> |
|<span data-ttu-id="64c05-179">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="64c05-179">Validation File</span></span>  <br/> |<span data-ttu-id="64c05-180">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="64c05-180">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="64c05-181">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="64c05-181">Can be Empty</span></span>  <br/> |<span data-ttu-id="64c05-182">False</span><span class="sxs-lookup"><span data-stu-id="64c05-182">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="64c05-183">Ver também</span><span class="sxs-lookup"><span data-stu-id="64c05-183">See also</span></span>



- [<span data-ttu-id="64c05-184">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="64c05-184">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

