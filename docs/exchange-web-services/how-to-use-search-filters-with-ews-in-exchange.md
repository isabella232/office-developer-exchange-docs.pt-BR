---
title: Use os filtros de pesquisa com o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 20fc6d2d-41c2-4490-98b8-c52513977fef
description: Descubra como usar filtros de pesquisa com a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: 0652c36fd610c2f9dfe22b55323b368997137e0c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750849"
---
# <a name="use-search-filters-with-ews-in-exchange"></a><span data-ttu-id="50876-103">Use os filtros de pesquisa com o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="50876-103">Use search filters with EWS in Exchange</span></span>

<span data-ttu-id="50876-104">Descubra como usar filtros de pesquisa com a API gerenciada de EWS ou EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="50876-104">Find out how to use search filters with the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="50876-105">Os filtros de pesquisa são a ferramenta principal para expressar critérios de pesquisa na sua API gerenciada de EWS ou aplicativos do EWS.</span><span class="sxs-lookup"><span data-stu-id="50876-105">Search filters are the primary tool for expressing search criteria in your EWS Managed API or EWS application.</span></span> <span data-ttu-id="50876-106">Recomendamos que você use filtros de pesquisa, em vez de [cadeias de caracteres de consulta](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md), para fazer o seguinte:</span><span class="sxs-lookup"><span data-stu-id="50876-106">We recommend that you use search filters, as opposed to [query strings](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md), to do the following:</span></span>
  
- <span data-ttu-id="50876-107">Pesquisa em uma propriedade específica ou um conjunto de propriedades.</span><span class="sxs-lookup"><span data-stu-id="50876-107">Search on a specific property or set of properties.</span></span>  
- <span data-ttu-id="50876-108">Pesquise usando vários critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="50876-108">Search using multiple search criteria.</span></span>
    
<span data-ttu-id="50876-109">Filtros de pesquisa são a única opção se você estiver fazendo o seguinte:</span><span class="sxs-lookup"><span data-stu-id="50876-109">Search filters are your only option if you are doing any of the following:</span></span>
  
- <span data-ttu-id="50876-110">Pesquisa de propriedades personalizadas.</span><span class="sxs-lookup"><span data-stu-id="50876-110">Searching custom properties.</span></span>  
- <span data-ttu-id="50876-111">Realizar diferencia maiusculas de minúsculas cadeia de caracteres de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="50876-111">Performing case-sensitive string searches.</span></span>  
- <span data-ttu-id="50876-112">Realizando prefixo ou correspondência exata de cadeia de caracteres de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="50876-112">Performing prefix or exact match string searches.</span></span> 
- <span data-ttu-id="50876-113">Realizar bitmask pesquisa.</span><span class="sxs-lookup"><span data-stu-id="50876-113">Performing bitmask searches.</span></span>
- <span data-ttu-id="50876-114">Pesquisando itens que tenham uma propriedade específica definido, independentemente do valor.</span><span class="sxs-lookup"><span data-stu-id="50876-114">Searching for items that have a specific property set, regardless of value.</span></span>
- <span data-ttu-id="50876-115">Pesquisar pastas.</span><span class="sxs-lookup"><span data-stu-id="50876-115">Searching for folders.</span></span>
- <span data-ttu-id="50876-116">Criação de pastas de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="50876-116">Creating search folders.</span></span>
    
## <a name="determine-what-type-of-search-filter-you-need"></a><span data-ttu-id="50876-117">Determinar que tipo de filtro de pesquisa que você precisa</span><span class="sxs-lookup"><span data-stu-id="50876-117">Determine what type of search filter you need</span></span>
<span data-ttu-id="50876-118"><a name="bk_SelectFilter"> </a></span><span class="sxs-lookup"><span data-stu-id="50876-118"></span></span>

<span data-ttu-id="50876-119">Antes de criar um filtro de pesquisa, primeiro determine qual tipo de filtro que você precisa.</span><span class="sxs-lookup"><span data-stu-id="50876-119">Before you create a search filter, first determine which type of filter you need.</span></span> <span data-ttu-id="50876-120">Os tipos de filtro são implementados como classes descendentes da classe [SearchFilter](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) na API gerenciada do EWS e como elementos filho do elemento [restrição](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) no EWS.</span><span class="sxs-lookup"><span data-stu-id="50876-120">The filter types are implemented as descendant classes of the [SearchFilter](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) class in the EWS Managed API, and as child elements of the [Restriction](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) element in EWS.</span></span> 
  
<span data-ttu-id="50876-121">**Tabela 1. Tipos de filtros de pesquisa**</span><span class="sxs-lookup"><span data-stu-id="50876-121">**Table 1. Types of search filters**</span></span>

|<span data-ttu-id="50876-122">**Tipo de filtro**</span><span class="sxs-lookup"><span data-stu-id="50876-122">**Filter type**</span></span>|<span data-ttu-id="50876-123">**Classe de API gerenciada de EWS**</span><span class="sxs-lookup"><span data-stu-id="50876-123">**EWS Managed API class**</span></span>|<span data-ttu-id="50876-124">**Elemento EWS**</span><span class="sxs-lookup"><span data-stu-id="50876-124">**EWS element**</span></span>|<span data-ttu-id="50876-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="50876-125">**Description**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="50876-126">Contém o filtro</span><span class="sxs-lookup"><span data-stu-id="50876-126">Contains filter</span></span>  <br/> |[<span data-ttu-id="50876-127">ContainsSubstring</span><span class="sxs-lookup"><span data-stu-id="50876-127">ContainsSubstring</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="50876-128">Contém</span><span class="sxs-lookup"><span data-stu-id="50876-128">Contains</span></span>](http://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) <br/> |<span data-ttu-id="50876-129">O melhor tipo de filtro a ser usado para comparações de sequência.</span><span class="sxs-lookup"><span data-stu-id="50876-129">The best filter type to use for string comparisons.</span></span> <span data-ttu-id="50876-130">Ele permite que você controle a diferenciação de maiusculas, se deve ignorar espaço em branco e definir o modo de contenção.</span><span class="sxs-lookup"><span data-stu-id="50876-130">It allows you to control case sensitivity, whether to ignore whitespace, and set the containment mode.</span></span>  <br/> |
|<span data-ttu-id="50876-131">Filtro de bitmask</span><span class="sxs-lookup"><span data-stu-id="50876-131">Bitmask filter</span></span>  <br/> |[<span data-ttu-id="50876-132">ExcludesBitmask</span><span class="sxs-lookup"><span data-stu-id="50876-132">ExcludesBitmask</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.excludesbitmask%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="50876-133">Exclui</span><span class="sxs-lookup"><span data-stu-id="50876-133">Excludes</span></span>](http://msdn.microsoft.com/library/bbaeddf6-9a67-4ee0-af99-7a7a5bbdc0e1%28Office.15%29.aspx) <br/> |<span data-ttu-id="50876-134">Permite que você pesquise propriedades inteiro como bitmasks e retornar apenas resultados que tem bits correspondente para o bitmask especificado não definido.</span><span class="sxs-lookup"><span data-stu-id="50876-134">Allows you to search integer properties as bitmasks and only return results that have bits corresponding to the specified bitmask unset.</span></span>  <br/> |
|<span data-ttu-id="50876-135">Existe um filtro</span><span class="sxs-lookup"><span data-stu-id="50876-135">Exists filter</span></span>  <br/> |[<span data-ttu-id="50876-136">Existe</span><span class="sxs-lookup"><span data-stu-id="50876-136">Exists</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.exists%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="50876-137">Existe</span><span class="sxs-lookup"><span data-stu-id="50876-137">Exists</span></span>](http://msdn.microsoft.com/library/55d568bd-8dbc-4d50-b9d7-54b74a54d4b5%28Office.15%29.aspx) <br/> |<span data-ttu-id="50876-138">Retorna todos os itens que têm a presente, independentemente do valor de propriedade especificada.</span><span class="sxs-lookup"><span data-stu-id="50876-138">Returns all items that have the specified property present, regardless of value.</span></span>  <br/> |
|<span data-ttu-id="50876-139">Filtro de igualdade</span><span class="sxs-lookup"><span data-stu-id="50876-139">Equality filter</span></span>  <br/> |[<span data-ttu-id="50876-140">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="50876-140">IsEqualTo</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.isequalto%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="50876-141">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="50876-141">IsNotEqualTo</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.isnotequalto%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="50876-142">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="50876-142">IsEqualTo</span></span>](http://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx) <br/> [<span data-ttu-id="50876-143">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="50876-143">IsNotEqualTo</span></span>](http://msdn.microsoft.com/library/e2eff26c-3403-45cd-bb74-1eb98c7dbfcd%28Office.15%29.aspx) <br/> |<span data-ttu-id="50876-144">Compara o valor da propriedade especificada com um valor de constante especificado ou o valor da propriedade outro e retornar todos os itens que têm um valor igual a (no caso de um filtro **IsEqualTo** ) ou um valor de não-igual (no caso de um **IsNotEqualTo **filtro).</span><span class="sxs-lookup"><span data-stu-id="50876-144">Compares the value of the specified property with either a specified constant value or the value of another property and return all items that have an equal value (in the case of an **IsEqualTo** filter) or a non-equal value (in the case of an **IsNotEqualTo** filter).</span></span>  <br/> |
|<span data-ttu-id="50876-145">Filtro de teste relacional</span><span class="sxs-lookup"><span data-stu-id="50876-145">Relational testing filter</span></span>  <br/> |[<span data-ttu-id="50876-146">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="50876-146">IsGreaterThan</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthan%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="50876-147">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="50876-147">IsGreaterThanOrEqualTo</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthanorequalto%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="50876-148">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="50876-148">IsLessThan</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.islessthan%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="50876-149">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="50876-149">IsLessThanOrEqualTo</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.islessthanorequalto%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="50876-150">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="50876-150">IsGreaterThan</span></span>](http://msdn.microsoft.com/library/a6e9d462-cfa7-40ec-903e-128c95050352%28Office.15%29.aspx) <br/> [<span data-ttu-id="50876-151">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="50876-151">IsGreaterThanOrEqualTo</span></span>](http://msdn.microsoft.com/library/373cc954-314d-40e2-be03-cc08aefc0d5b%28Office.15%29.aspx) <br/> [<span data-ttu-id="50876-152">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="50876-152">IsLessThan</span></span>](http://msdn.microsoft.com/library/2550469b-6e5d-45a5-9ecc-090d1b409296%28Office.15%29.aspx) <br/> [<span data-ttu-id="50876-153">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="50876-153">IsLessThanOrEqualTo</span></span>](http://msdn.microsoft.com/library/b5d85eb2-5e15-4d01-ad49-6289e735ad8a%28Office.15%29.aspx) <br/> |<span data-ttu-id="50876-154">Retorna todos os itens que tenham um valor para a propriedade especificada na relação apropriada com um valor de constante especificado ou outra propriedade.</span><span class="sxs-lookup"><span data-stu-id="50876-154">Returns all items that have a value for the specified property in the appropriate relation to either a specified constant value or another property.</span></span> <span data-ttu-id="50876-155">Por exemplo, um filtro **IsGreaterThan** retorna todos os itens que têm um valor maior que o valor especificado na propriedade especificado.</span><span class="sxs-lookup"><span data-stu-id="50876-155">For example, an **IsGreaterThan** filter returns all items that have a value that is greater than the specified value in the specified property.</span></span>  <br/> |
|<span data-ttu-id="50876-156">Eliminando o filtro</span><span class="sxs-lookup"><span data-stu-id="50876-156">Negating filter</span></span>  <br/> |[<span data-ttu-id="50876-157">Não</span><span class="sxs-lookup"><span data-stu-id="50876-157">Not</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.not%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="50876-158">Não</span><span class="sxs-lookup"><span data-stu-id="50876-158">Not</span></span>](http://msdn.microsoft.com/library/1aa16318-7e90-4b19-bce8-dd1a20a66223%28Office.15%29.aspx) <br/> |<span data-ttu-id="50876-159">Dispensa o resultado dos outros filtros.</span><span class="sxs-lookup"><span data-stu-id="50876-159">Negates the result of the other filters.</span></span>  <br/> |
|<span data-ttu-id="50876-160">Filtro composto</span><span class="sxs-lookup"><span data-stu-id="50876-160">Compound filter</span></span>  <br/> |[<span data-ttu-id="50876-161">SearchFilterCollection</span><span class="sxs-lookup"><span data-stu-id="50876-161">SearchFilterCollection</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="50876-162">E</span><span class="sxs-lookup"><span data-stu-id="50876-162">And</span></span>](http://msdn.microsoft.com/library/790246c2-37ad-49a8-91b9-6186d743b011%28Office.15%29.aspx) <br/> [<span data-ttu-id="50876-163">Ou</span><span class="sxs-lookup"><span data-stu-id="50876-163">Or</span></span>](http://msdn.microsoft.com/library/4876d83a-73a3-4953-9d95-3048e6b76ccb%28Office.15%29.aspx) <br/> |<span data-ttu-id="50876-164">Combina vários filtros, permitindo critérios de pesquisa mais complexos.</span><span class="sxs-lookup"><span data-stu-id="50876-164">Combines multiple filters, allowing for more complex search criteria.</span></span>  <br/> |
   
### <a name="contains-filter"></a><span data-ttu-id="50876-165">Contém o filtro</span><span class="sxs-lookup"><span data-stu-id="50876-165">Contains filter</span></span>

<span data-ttu-id="50876-166">Contém um filtro é a melhor escolha para propriedades de cadeia de caracteres de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="50876-166">A contains filter is the best choice for searching string properties.</span></span> <span data-ttu-id="50876-167">Com um contém o filtro, você pode controlar os aspectos de correspondência de cadeia de caracteres, como diferenciação de maiusculas e como o espaço em branco é tratado, definindo o modo de contenção e o modo de comparação.</span><span class="sxs-lookup"><span data-stu-id="50876-167">With a contains filter, you can control aspects of string matching, like case sensitivity and how whitespace is treated, by setting the containment mode and the comparison mode.</span></span>
  
#### <a name="contains-filter-in-the-ews-managed-api"></a><span data-ttu-id="50876-168">Contém o filtro na API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="50876-168">Contains filter in the EWS Managed API</span></span>
<span data-ttu-id="50876-169"><a name="bk_ContainsEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="50876-169"></span></span>

<span data-ttu-id="50876-170">Se você estiver usando a API gerenciada de EWS, você definir o modo de contenção usando a propriedade [ContainmentMode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.containmentmode%28v=exchg.80%29.aspx) da classe [ContainsSubstring](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) e você definir o modo de comparação, usando a propriedade [ComparisonMode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.comparisonmode%28v=exchg.80%29.aspx) do ** ContainsSubstring** classe.</span><span class="sxs-lookup"><span data-stu-id="50876-170">If you're using the EWS Managed API, you set the containment mode by using the [ContainmentMode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.containmentmode%28v=exchg.80%29.aspx) property of the [ContainsSubstring](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) class, and you set the comparison mode by using the [ComparisonMode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.comparisonmode%28v=exchg.80%29.aspx) property of the **ContainsSubstring** class.</span></span> <span data-ttu-id="50876-171">O exemplo a seguir mostra como criar um filtro de pesquisa que pesquisa o campo de assunto de itens para a subcadeia de caracteres "notas de reunião".</span><span class="sxs-lookup"><span data-stu-id="50876-171">The following example shows you how to create a search filter that searches the subject field of items for the substring "meeting notes".</span></span> <span data-ttu-id="50876-172">Este exemplo diferencia maiusculas de minúsculas, mas não ignora espaço em branco.</span><span class="sxs-lookup"><span data-stu-id="50876-172">This example ignores case, but does not ignore whitespace.</span></span> 
  
```cs
// Find all items with a subject that contain the substring
// "meeting notes", regardless of case.
// Matches include:
//   - meeting notes
//   - Meeting Notes
//   - Here are my meeting notes
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
```

#### <a name="contains-filter-in-ews"></a><span data-ttu-id="50876-173">Contém o filtro no EWS</span><span class="sxs-lookup"><span data-stu-id="50876-173">Contains filter in EWS</span></span>
<span data-ttu-id="50876-174"><a name="bk_ContainsEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="50876-174"></span></span>

<span data-ttu-id="50876-175">Você definir o modo de contenção usando o atributo **ContainmentMode** no elemento [contém](http://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) no EWS, e você definir o modo de comparação, usando o atributo **ContainmentComparison** no elemento **contém** .</span><span class="sxs-lookup"><span data-stu-id="50876-175">In EWS, you set the containment mode by using the **ContainmentMode** attribute on the [Contains](http://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) element, and you set the comparison mode by using the **ContainmentComparison** attribute on the **Contains** element.</span></span> <span data-ttu-id="50876-176">O exemplo a seguir mostra como criar um filtro de pesquisa para pesquisar o campo de assunto de itens para a subcadeia de caracteres "notas de reunião".</span><span class="sxs-lookup"><span data-stu-id="50876-176">The following example shows you how to create a search filter to search the subject field of items for the substring "meeting notes".</span></span> <span data-ttu-id="50876-177">Este exemplo diferencia maiusculas de minúsculas, mas não ignora espaço em branco.</span><span class="sxs-lookup"><span data-stu-id="50876-177">This example ignores case, but does not ignore whitespace.</span></span> 
  
```XML
<t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
  <t:FieldURI FieldURI="item:Subject" />
  <t:Constant Value="meeting notes" />
</t:Contains>
```

### <a name="bitmask-filter"></a><span data-ttu-id="50876-178">Filtro de bitmask</span><span class="sxs-lookup"><span data-stu-id="50876-178">Bitmask filter</span></span>

<span data-ttu-id="50876-179">Um filtro de bitmask permite que você pesquise propriedades inteiro como bitmasks e retornar resultados onde os bits específicos não são definidos no valor da propriedade especificada.</span><span class="sxs-lookup"><span data-stu-id="50876-179">A bitmask filter enables you to search integer properties as bitmasks, and return results where specific bits are not set in the value of the specified property.</span></span>
  
#### <a name="bitmask-filter-in-the-ews-managed-api"></a><span data-ttu-id="50876-180">Filtro de bitmask na API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="50876-180">Bitmask filter in the EWS Managed API</span></span>

<span data-ttu-id="50876-181">O exemplo a seguir mostra como usar a API gerenciada de EWS para criar um filtro de pesquisa para retornar todos os itens que têm um valor na propriedade **ItemIndex** personalizada (definido no [exemplo: localizar itens usando um filtro de pesquisa e a API gerenciada de EWS](#bk_ExampleEWSMA) seção Este artigo) que não tenham o segundo bit (10 em binário) definida.</span><span class="sxs-lookup"><span data-stu-id="50876-181">The following example shows you how to use the EWS Managed API to create a search filter to return all items that have a value in the **ItemIndex** custom property (defined in the [Example: Find items by using a search filter and the EWS Managed API](#bk_ExampleEWSMA) section of this article) that do not have the second bit (10 in binary) set.</span></span> 
  
```cs
// Find all items with a value of the custom property that does not
// have the second bit (0010) set.
// Matches include:
//   - Property not set
//   - 1 (0001)
//   - 4 (0100)
//   - 5 (0101)
//   - 8 (1000)
SearchFilter.ExcludesBitmask bit2NotSetFilter = 
    new SearchFilter.ExcludesBitmask(customPropDefinition, 2);
```

#### <a name="bitmask-filter-in-ews"></a><span data-ttu-id="50876-182">Filtro de bitmask no EWS</span><span class="sxs-lookup"><span data-stu-id="50876-182">Bitmask filter in EWS</span></span>

<span data-ttu-id="50876-183">O exemplo a seguir mostra como usar o EWS para criar um filtro de pesquisa para retornar todos os itens que têm um valor na propriedade **ItemIndex** personalizada (definido no [exemplo: localizar itens usando um filtro de pesquisa e a API gerenciada de EWS](#bk_ExampleEWSMA) seção deste artigo) que não tenham o segundo bit (10 em binário) definida.</span><span class="sxs-lookup"><span data-stu-id="50876-183">The following example shows you how to use EWS to create a search filter to return all items that have a value in the **ItemIndex** custom property (defined in the [Example: Find items by using a search filter and the EWS Managed API](#bk_ExampleEWSMA) section of this article) that do not have the second bit (10 in binary) set.</span></span> 
  
```XML
<t:Excludes>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:Bitmask Value="2" />
</t:Excludes>
```

### <a name="exists-filter"></a><span data-ttu-id="50876-184">Existe um filtro</span><span class="sxs-lookup"><span data-stu-id="50876-184">Exists filter</span></span>

<span data-ttu-id="50876-185">Um existe filtro permite que você pesquise para itens que tenham uma propriedade específica definida neles, independente do valor.</span><span class="sxs-lookup"><span data-stu-id="50876-185">An exists filter enables you to search for items that have a specific property set on them, regardless of the value.</span></span>
  
#### <a name="exists-filter-in-the-ews-managed-api"></a><span data-ttu-id="50876-186">Existe um filtro na API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="50876-186">Exists filter in the EWS Managed API</span></span>

<span data-ttu-id="50876-187">O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens que possuem a propriedade personalizada do **ItemIndex** definido.</span><span class="sxs-lookup"><span data-stu-id="50876-187">The following example shows you how to create a search filter to return all items that have the **ItemIndex** custom property set.</span></span> 
  
```cs
// Find all items that have the custom property set.
SearchFilter.Exists customPropSetFilter =
    new SearchFilter.Exists(customPropDefinition);
```

#### <a name="exists-filter-in-ews"></a><span data-ttu-id="50876-188">Existe um filtro no EWS</span><span class="sxs-lookup"><span data-stu-id="50876-188">Exists filter in EWS</span></span>

<span data-ttu-id="50876-189">O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens que possuem a propriedade personalizada do **ItemIndex** definido.</span><span class="sxs-lookup"><span data-stu-id="50876-189">The following example shows you how to create a search filter to return all items that have the **ItemIndex** custom property set.</span></span> 
  
```XML
<t:Exists>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
</t:Exists>
```

### <a name="equality-filter"></a><span data-ttu-id="50876-190">Filtro de igualdade</span><span class="sxs-lookup"><span data-stu-id="50876-190">Equality filter</span></span>

<span data-ttu-id="50876-191">Filtros de igualdade permitem que você procurar todos os itens que têm um valor da propriedade especificado que é igual a um valor específico ou que não é igual a um valor específico.</span><span class="sxs-lookup"><span data-stu-id="50876-191">Equality filters enable you to search for all items that have a value for the specified property that either equals a specific value or does not equal a specific value.</span></span> <span data-ttu-id="50876-192">O valor a ser comparado com pode ser um valor de constante ou o valor da propriedade outra em cada item.</span><span class="sxs-lookup"><span data-stu-id="50876-192">The value to compare with can be either a constant value or the value of another property on each item.</span></span>
  
#### <a name="equality-filter-in-the-ews-managed-api"></a><span data-ttu-id="50876-193">Filtro de igualdade na API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="50876-193">Equality filter in the EWS Managed API</span></span>

<span data-ttu-id="50876-194">O exemplo a seguir mostra como usar a API gerenciada de EWS para criar um filtro de pesquisa para retornar todos os itens que não tenham sido lidas.</span><span class="sxs-lookup"><span data-stu-id="50876-194">The following example shows you how to use the EWS Managed API to create a search filter to return all items that have not been read.</span></span>
  
```cs
// Find all items that are not marked as read.
SearchFilter.IsEqualTo unreadFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.IsRead, false);
```

<span data-ttu-id="50876-195">O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens que têm um valor na propriedade **ItemIndex** que não é igual ao tamanho do item.</span><span class="sxs-lookup"><span data-stu-id="50876-195">The following example shows you how to create a search filter to return all items that have a value in the **ItemIndex** property that is not equal to the size of the item.</span></span> 
  
```cs
// Find all items that are marked as read.
SearchFilter.IsNotEqualTo indexNotEqualToSizeFilter =
    new SearchFilter.IsNotEqualTo(customPropDefinition, ItemSchema.Size);
```

#### <a name="equality-filter-in-ews"></a><span data-ttu-id="50876-196">Filtro de igualdade do EWS</span><span class="sxs-lookup"><span data-stu-id="50876-196">Equality filter in EWS</span></span>

<span data-ttu-id="50876-197">O exemplo a seguir mostra como usar o EWS para criar um filtro de pesquisa para retornar todos os itens que não tenham sido lidas.</span><span class="sxs-lookup"><span data-stu-id="50876-197">The following example shows you how to use EWS to create a search filter to return all items that have not been read.</span></span>
  
```XML
<t:IsEqualTo>
  <t:FieldURI FieldURI="message:IsRead" />
  <t:FieldURIOrConstant>
    <t:Constant Value="false" />
  </t:FieldURIOrConstant>
</t:IsEqualTo>
```

<span data-ttu-id="50876-198">O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens que têm um valor na propriedade **ItemIndex** que não é igual ao tamanho do item.</span><span class="sxs-lookup"><span data-stu-id="50876-198">The following example shows you how to create a search filter to return all items that have a value in the **ItemIndex** property that is not equal to the size of the item.</span></span> 
  
```XML
<t:IsNotEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:FieldURI FieldURI="item:Size" />
  </t:FieldURIOrConstant>
</t:IsNotEqualTo>
```

### <a name="relational-testing-filter"></a><span data-ttu-id="50876-199">Filtro de teste relacional</span><span class="sxs-lookup"><span data-stu-id="50876-199">Relational testing filter</span></span>

<span data-ttu-id="50876-200">Filtros de testes relacionais permitem que você procurar todos os itens que têm um valor na propriedade especificada que é maior que (\>), maior ou igual a (\>=), menor que (\<), ou menor ou igual a (\<=) um valor especificado.</span><span class="sxs-lookup"><span data-stu-id="50876-200">Relational testing filters enable you to search for all items that have a value in the specified property that is either greater than (\>), greater than or equal to (\>=), less than (\<), or less than or equal to (\<=) a specified value.</span></span> <span data-ttu-id="50876-201">O valor a ser comparado com pode ser um valor de constante ou o valor da propriedade outra em cada item.</span><span class="sxs-lookup"><span data-stu-id="50876-201">The value to compare with can be either a constant value or the value of another property on each item.</span></span>
  
#### <a name="relational-testing-filter-in-the-ews-managed-api"></a><span data-ttu-id="50876-202">Filtro de teste relacional na API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="50876-202">Relational testing filter in the EWS Managed API</span></span>

<span data-ttu-id="50876-203">O exemplo a seguir mostra como usar a API gerenciada de EWS para criar filtros de pesquisa para retornar todos os itens com um valor na propriedade **ItemIndex** que tem a relação especificada com o valor da constante 3.</span><span class="sxs-lookup"><span data-stu-id="50876-203">The following example shows you how to use the EWS Managed API to create search filters to return all items with a value in the **ItemIndex** property that has the specified relationship to the constant value 3.</span></span> 
  
```cs
// Find all items where the custom property value is > 3.
SearchFilter.IsGreaterThan greaterThanFilter =
    new SearchFilter.IsGreaterThan(customPropDefinition, 3);
// Find all items where the custom property value is >= 3.
SearchFilter.IsGreaterThanOrEqualTo greaterThanOrEqualFilter =
    new SearchFilter.IsGreaterThanOrEqualTo(customPropDefinition, ItemSchema.Size);
// Find all items where the custom property value is < 3.
SearchFilter.IsLessThan lessThanFilter =
    new SearchFilter.IsLessThan(customPropDefinition, 3);
// Find all items where the custom property value is <= 3.
SearchFilter.IsLessThanOrEqualTo lessThanOrEqualFilter =
    new SearchFilter.IsLessThanOrEqualTo(customPropDefinition, 3);
```

#### <a name="relational-testing-filter-in-ews"></a><span data-ttu-id="50876-204">Filtro de teste relacional do EWS</span><span class="sxs-lookup"><span data-stu-id="50876-204">Relational testing filter in EWS</span></span>

<span data-ttu-id="50876-205">O exemplo a seguir mostra como usar o EWS para criar um filtro de pesquisa para retornar todos os itens com um valor na propriedade **ItemIndex** que for maior do que o valor da constante 3.</span><span class="sxs-lookup"><span data-stu-id="50876-205">The following example shows you how to use EWS to create a search filter to return all items with a value in the **ItemIndex** property that is greater than the constant value 3.</span></span> 
  
```XML
<t:IsGreaterThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThan>
```

<span data-ttu-id="50876-206">O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens com um valor na propriedade **ItemIndex** que é maior que ou igual ao valor de constante 3.</span><span class="sxs-lookup"><span data-stu-id="50876-206">The following example shows you how to create a search filter to return all items with a value in the **ItemIndex** property that is greater than or equal to the constant value 3.</span></span> 
  
```XML
<t:IsGreaterThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThanOrEqualTo>
```

<span data-ttu-id="50876-207">O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens com um valor na propriedade **ItemIndex** menor que o valor da constante 3.</span><span class="sxs-lookup"><span data-stu-id="50876-207">The following example shows you how to create a search filter to return all items with a value in the **ItemIndex** property that is less than the constant value 3.</span></span> 
  
```XML
<t:IsLessThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThan>
```

<span data-ttu-id="50876-208">O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens com um valor na propriedade **ItemIndex** que for menor ou igual ao valor de constante 3.</span><span class="sxs-lookup"><span data-stu-id="50876-208">The following example shows you how to create a search filter to return all items with a value in the **ItemIndex** property that is less than or equal to the constant value 3.</span></span> 
  
```XML
<t:IsLessThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThanOrEqualTo>
```

### <a name="negating-filter"></a><span data-ttu-id="50876-209">Eliminando o filtro</span><span class="sxs-lookup"><span data-stu-id="50876-209">Negating filter</span></span>

<span data-ttu-id="50876-210">Um filtro negating permite que você negar a outro filtro e obter resultados da pesquisa oposto.</span><span class="sxs-lookup"><span data-stu-id="50876-210">A negating filter enables you to negate another filter and get the opposite search results.</span></span> <span data-ttu-id="50876-211">Enquanto outros filtros retornam resultados que correspondem a critérios específicos, um filtro negating retorna resultados que não correspondem aos critérios especificados pelo filtro a que for aplicado.</span><span class="sxs-lookup"><span data-stu-id="50876-211">While other filters return results that match specific criteria, a negating filter returns results that do not match the criteria specified by the filter it is applied to.</span></span>
  
#### <a name="negating-filter-in-the-ews-managed-api"></a><span data-ttu-id="50876-212">Eliminando o filtro na API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="50876-212">Negating filter in the EWS Managed API</span></span>

<span data-ttu-id="50876-213">O exemplo a seguir mostra como usar a API gerenciada de EWS para criar um filtro de pesquisa para retornar todos os itens que não têm a subcadeia de caracteres "notas de reunião" no assunto.</span><span class="sxs-lookup"><span data-stu-id="50876-213">The following example shows you how to use the EWS Managed API to create a search filter to return all items that do not have the substring "meeting notes" in the subject.</span></span>
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
SearchFilter.Not subjectNotFilter =
    new SearchFilter.Not(subjectFilter);
```

#### <a name="negating-filter-in-ews"></a><span data-ttu-id="50876-214">Eliminando o filtro no EWS</span><span class="sxs-lookup"><span data-stu-id="50876-214">Negating filter in EWS</span></span>

<span data-ttu-id="50876-215">O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens que não têm a subcadeia de caracteres "notas de reunião" no assunto.</span><span class="sxs-lookup"><span data-stu-id="50876-215">The following example shows you how to create a search filter to return all items that do not have the substring "meeting notes" in the subject.</span></span>
  
```XML
<t:Not>
  <t:Contains ContainmentMode="ExactPhrase" ContainmentComparison="IgnoreCase">
    <t:FieldURI FieldURI="item:Subject" />
    <t:Constant Value="meeting notes" />
  </t:Contains>
</t:Not>
```

### <a name="compound-filter"></a><span data-ttu-id="50876-216">Filtro composto</span><span class="sxs-lookup"><span data-stu-id="50876-216">Compound filter</span></span>

<span data-ttu-id="50876-217">Um filtro composto permite combinar vários filtros para criar critérios de pesquisa mais complexos.</span><span class="sxs-lookup"><span data-stu-id="50876-217">A compound filter enables you to combine multiple filters to create more complex search criteria.</span></span> <span data-ttu-id="50876-218">Você pode combinar os critérios usando operadores lógicos e ou OR.</span><span class="sxs-lookup"><span data-stu-id="50876-218">You can combine criteria by using the logical operators AND or OR.</span></span> <span data-ttu-id="50876-219">Dessa forma, você pode realizar pesquisas como "todos os emails de Sadie Daniels que contém 'Notas de reunião' no assunto".</span><span class="sxs-lookup"><span data-stu-id="50876-219">In this way, you can perform searches like "all mail from Sadie Daniels that contains 'meeting notes' in the subject".</span></span>
  
#### <a name="compound-filter-in-the-ews-managed-api"></a><span data-ttu-id="50876-220">Filtro composto na API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="50876-220">Compound filter in the EWS Managed API</span></span>

<span data-ttu-id="50876-221">O exemplo a seguir mostra como usar a API gerenciada de EWS para criar um filtro de pesquisa que retorna todos os itens que são enviados de Sadie Daniels e conter "notas de reunião" no assunto.</span><span class="sxs-lookup"><span data-stu-id="50876-221">The following example shows you how to use the EWS Managed API to create a search filter that returns all items that are sent from Sadie Daniels and contain "meeting notes" in the subject.</span></span>
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
EmailAddress manager = new EmailAddress("sadie@contoso.com");
SearchFilter.IsEqualTo fromManagerFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, fromManagerFilter);
```

#### <a name="compound-filter-in-ews"></a><span data-ttu-id="50876-222">Filtro composto no EWS</span><span class="sxs-lookup"><span data-stu-id="50876-222">Compound filter in EWS</span></span>

<span data-ttu-id="50876-223">O exemplo a seguir mostra como usar o EWS para criar um filtro de pesquisa que retorna todos os itens que são enviados de Sadie Daniels e contenham "notas de reunião" no assunto.</span><span class="sxs-lookup"><span data-stu-id="50876-223">The following example shows you how to use EWS to create a search filter that returns all items that are sent from Sadie Daniels and contain "meeting notes" in the subject.</span></span>
  
```XML
<t:And>
  <t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
    <t:FieldURI FieldURI="item:Subject" />
    <t:Constant Value="meeting notes" />
  </t:Contains>
  <t:IsEqualTo>
    <t:FieldURI FieldURI="message:Sender" />
    <t:FieldURIOrConstant>
      <t:Constant Value="sadie@fourthcoffee.com" />
    </t:FieldURIOrConstant>
  </t:IsEqualTo>
</t:And>
```

## <a name="example-find-items-by-using-a-search-filter-and-the-ews-managed-api"></a><span data-ttu-id="50876-224">Exemplo: Localizar itens usando um filtro de pesquisa e a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="50876-224">Example: Find items by using a search filter and the EWS Managed API</span></span>
<span data-ttu-id="50876-225"><a name="bk_ExampleEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="50876-225"></span></span>

<span data-ttu-id="50876-226">Os seguintes métodos de API gerenciada de EWS usar filtros de pesquisa:</span><span class="sxs-lookup"><span data-stu-id="50876-226">The following EWS Managed API methods use search filters:</span></span>
  
- [<span data-ttu-id="50876-227">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="50876-227">ExchangeService.FindItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
- [<span data-ttu-id="50876-228">ExchangeService.FindFolders</span><span class="sxs-lookup"><span data-stu-id="50876-228">ExchangeService.FindFolders</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
- [<span data-ttu-id="50876-229">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="50876-229">Folder.FindFolders</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
- [<span data-ttu-id="50876-230">Folder.FindItems</span><span class="sxs-lookup"><span data-stu-id="50876-230">Folder.FindItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
<span data-ttu-id="50876-231">O exemplo a seguir usa o método **ExchangeService.FindItems** ; No entanto, as mesmas regras e conceitos se aplicam a todos os métodos.</span><span class="sxs-lookup"><span data-stu-id="50876-231">The following example uses the **ExchangeService.FindItems** method; however, the same rules and concepts apply to all the methods.</span></span> <span data-ttu-id="50876-232">Neste exemplo, um método chamado **SearchWithFilter** é definido.</span><span class="sxs-lookup"><span data-stu-id="50876-232">In this example, a method called **SearchWithFilter** is defined.</span></span> <span data-ttu-id="50876-233">Ele usa um objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , um objeto [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) e um objeto [SearchFilter](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) como parâmetros.</span><span class="sxs-lookup"><span data-stu-id="50876-233">It takes an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, a [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) object, and a [SearchFilter](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) object as parameters.</span></span> <span data-ttu-id="50876-234">Este exemplo pressupõe que o objeto **ExchangeService** foi inicializado com valores válidos nas propriedades [credenciais](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) e [Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="50876-234">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> <span data-ttu-id="50876-235">A classe **SearchFilter** é a classe base para todos os filtros de pesquisa diferentes.</span><span class="sxs-lookup"><span data-stu-id="50876-235">The **SearchFilter** class is the base class for all the different search filters.</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data
private static Guid SearchTestGUID = new Guid("{AA3DF801-4FC7-401F-BBC1-7C93D6498C2E}");
private static ExtendedPropertyDefinition customPropDefinition =
        new ExtendedPropertyDefinition(SearchTestGUID, "ItemIndex", MapiPropertyType.Integer);
static void SearchWithFilter(ExchangeService service, WellKnownFolderName folder, SearchFilter filter)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    view.PropertySet = new PropertySet(ItemSchema.Subject, 
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.IsRead,
                                       customPropDefinition);
    // Item searches do not support Deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Sorting.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        FindItemsResults<Item> results = service.FindItems(folder, filter, view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Id: {0}", item.Id.ToString());
            if (item.ExtendedProperties.Count > 0 &&
                 item.ExtendedProperties[0].PropertyDefinition == customPropDefinition)
            {
                Console.WriteLine("Search Index: {0}", item.ExtendedProperties[0].Value);
            }
            if (item is EmailMessage)
            {
                EmailMessage message = item as EmailMessage;
                Console.WriteLine("Read: {0}", message.IsRead.ToString());
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

<span data-ttu-id="50876-236">Você pode usar essa função com qualquer um dos filtros de pesquisa que mostram os exemplos neste artigo.</span><span class="sxs-lookup"><span data-stu-id="50876-236">You can use this function with any of the search filters shown in the examples in this article.</span></span> <span data-ttu-id="50876-237">Este exemplo usa um filtro composto para retornar todos os itens na caixa de entrada de Sadie Daniels com "notas de reunião" no assunto.</span><span class="sxs-lookup"><span data-stu-id="50876-237">This example uses a compound filter to return all items in the Inbox from Sadie Daniels with "meeting notes" in the subject.</span></span>
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
EmailAddress manager = new EmailAddress("sadie@contoso.com");
SearchFilter.IsEqualTo fromManagerFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, greaterThanFilter);
SearchWithFilter(service, WellKnownFolderName.Inbox, compoundFilter);
```

## <a name="example-find-an-item-by-using-a-search-filter-and-ews"></a><span data-ttu-id="50876-238">Exemplo: Localizar um item usando um filtro de pesquisa e o EWS</span><span class="sxs-lookup"><span data-stu-id="50876-238">Example: Find an item by using a search filter and EWS</span></span>
<span data-ttu-id="50876-239"><a name="bk_ExampleEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="50876-239"></span></span>

<span data-ttu-id="50876-240">As seguintes operações de EWS usam filtros de pesquisa:</span><span class="sxs-lookup"><span data-stu-id="50876-240">The following EWS operations use search filters:</span></span>
  
- [<span data-ttu-id="50876-241">FindFolder</span><span class="sxs-lookup"><span data-stu-id="50876-241">FindFolder</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
- [<span data-ttu-id="50876-242">FindItem</span><span class="sxs-lookup"><span data-stu-id="50876-242">FindItem</span></span>](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
<span data-ttu-id="50876-243">O exemplo a seguir usa a operação **FindItem** ; No entanto, as mesmas regras e conceitos se aplicam a ambas as operações.</span><span class="sxs-lookup"><span data-stu-id="50876-243">The following example uses the **FindItem** operation; however, the same rules and concepts apply to both operations.</span></span> <span data-ttu-id="50876-244">Filtros de pesquisa estão contidos no elemento [restrição](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) no solicitações SOAP.</span><span class="sxs-lookup"><span data-stu-id="50876-244">Search filters are contained in the [Restriction](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) element in SOAP requests.</span></span> <span data-ttu-id="50876-245">Este exemplo envia uma solicitação SOAP que é equivalente à pesquisa que é mostrada no exemplo anterior EWS Managed API.</span><span class="sxs-lookup"><span data-stu-id="50876-245">This example sends a SOAP request that is equivalent to the search that is shown in the preceding EWS Managed API example.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="message:IsRead" />
          <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:And>
          <t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
            <t:FieldURI FieldURI="item:Subject" />
            <t:Constant Value="meeting notes" />
          </t:Contains>
          <t:IsEqualTo>
            <t:FieldURI FieldURI="message:Sender" />
            <t:FieldURIOrConstant>
              <t:Constant Value="sadie@contoso.com" />
            </t:FieldURIOrConstant>
          </t:IsEqualTo>
        </t:And>
      </m:Restriction>
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="50876-246">O exemplo a seguir mostra a resposta do servidor, incluindo os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="50876-246">The following example shows the response from the server, including the search results.</span></span>
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="3" TotalItemsInView="3" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>meeting notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>5</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Meeting Notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>6</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Meeting notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>7</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="next-steps"></a><span data-ttu-id="50876-247">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="50876-247">Next steps</span></span>
<span data-ttu-id="50876-248"><a name="bk_ExampleEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="50876-248"></span></span>

<span data-ttu-id="50876-249">Agora que você está familiarizado com o uso de filtros de pesquisa nas pesquisas básicas, você pode mover para técnicas mais avançadas de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="50876-249">Now that you're familiar with using search filters in basic searches, you can move on to more advanced search techniques.</span></span>
  
- [<span data-ttu-id="50876-250">Realizar pesquisas de agrupadas usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="50876-250">Perform grouped searches by using EWS in Exchange</span></span>](how-to-perform-grouped-searches-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="50876-251">Realizar pesquisas paginadas utilizando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="50876-251">Perform paged searches by using EWS in Exchange</span></span>](how-to-perform-paged-searches-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="50876-252">Confira também</span><span class="sxs-lookup"><span data-stu-id="50876-252">See also</span></span>

- [<span data-ttu-id="50876-253">Pesquisa e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="50876-253">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)    
- [<span data-ttu-id="50876-254">Executar uma pesquisa AQS, usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="50876-254">Perform an AQS search by using EWS in Exchange</span></span>](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)   
- [<span data-ttu-id="50876-255">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="50876-255">ExchangeService.FindItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="50876-256">ExchangeService.FindFolders</span><span class="sxs-lookup"><span data-stu-id="50876-256">ExchangeService.FindFolders</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="50876-257">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="50876-257">Folder.FindFolders</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="50876-258">Folder.FindItems</span><span class="sxs-lookup"><span data-stu-id="50876-258">Folder.FindItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="50876-259">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="50876-259">FindFolder operation</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)   
- [<span data-ttu-id="50876-260">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="50876-260">FindItem operation</span></span>](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

