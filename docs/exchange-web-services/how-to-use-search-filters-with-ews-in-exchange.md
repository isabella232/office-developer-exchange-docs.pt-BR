---
title: Usar filtros de pesquisa com o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 20fc6d2d-41c2-4490-98b8-c52513977fef
description: Descubra como usar filtros de pesquisa com a API gerenciada do EWS ou o EWS no Exchange.
localization_priority: Priority
ms.openlocfilehash: 04a74ec92d4bced8abd58d164a1c186d6405e679
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455832"
---
# <a name="use-search-filters-with-ews-in-exchange"></a><span data-ttu-id="d0b3a-103">Usar filtros de pesquisa com o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d0b3a-103">Use search filters with EWS in Exchange</span></span>

<span data-ttu-id="d0b3a-104">Descubra como usar filtros de pesquisa com a API gerenciada do EWS ou o EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-104">Find out how to use search filters with the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="d0b3a-105">Os filtros de pesquisa são a principal ferramenta para expressar os critérios de pesquisa na API gerenciada do EWS ou no aplicativo EWS.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-105">Search filters are the primary tool for expressing search criteria in your EWS Managed API or EWS application.</span></span> <span data-ttu-id="d0b3a-106">Recomendamos que você use os filtros de pesquisa, em oposição às [cadeias de caracteres de consulta](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md), para fazer o seguinte:</span><span class="sxs-lookup"><span data-stu-id="d0b3a-106">We recommend that you use search filters, as opposed to [query strings](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md), to do the following:</span></span>
  
- <span data-ttu-id="d0b3a-107">Pesquisar em uma propriedade específica ou em um conjunto de propriedades.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-107">Search on a specific property or set of properties.</span></span>  
- <span data-ttu-id="d0b3a-108">Pesquisa usando vários critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-108">Search using multiple search criteria.</span></span>
    
<span data-ttu-id="d0b3a-109">Os filtros de pesquisa são sua única opção se você estiver fazendo um dos seguintes:</span><span class="sxs-lookup"><span data-stu-id="d0b3a-109">Search filters are your only option if you are doing any of the following:</span></span>
  
- <span data-ttu-id="d0b3a-110">Pesquisando Propriedades personalizadas.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-110">Searching custom properties.</span></span>  
- <span data-ttu-id="d0b3a-111">Executar pesquisas de cadeia de caracteres que diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-111">Performing case-sensitive string searches.</span></span>  
- <span data-ttu-id="d0b3a-112">Executando pesquisas de cadeia de caracteres de correspondência exata ou prefixo.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-112">Performing prefix or exact match string searches.</span></span> 
- <span data-ttu-id="d0b3a-113">Executando pesquisas de bitmask.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-113">Performing bitmask searches.</span></span>
- <span data-ttu-id="d0b3a-114">Pesquisa de itens que tenham um conjunto de propriedades específico, independentemente do valor.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-114">Searching for items that have a specific property set, regardless of value.</span></span>
- <span data-ttu-id="d0b3a-115">Pesquisando pastas.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-115">Searching for folders.</span></span>
- <span data-ttu-id="d0b3a-116">Criar pastas de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-116">Creating search folders.</span></span>
    
## <a name="determine-what-type-of-search-filter-you-need"></a><span data-ttu-id="d0b3a-117">Determinar que tipo de filtro de pesquisa você precisa</span><span class="sxs-lookup"><span data-stu-id="d0b3a-117">Determine what type of search filter you need</span></span>
<span data-ttu-id="d0b3a-118"><a name="bk_SelectFilter"> </a></span><span class="sxs-lookup"><span data-stu-id="d0b3a-118"><a name="bk_SelectFilter"> </a></span></span>

<span data-ttu-id="d0b3a-119">Antes de criar um filtro de pesquisa, determine primeiro qual tipo de filtro você precisa.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-119">Before you create a search filter, first determine which type of filter you need.</span></span> <span data-ttu-id="d0b3a-120">Os tipos de filtro são implementados como classes descendentes da classe [SearchFilter](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) na API gerenciada do EWS e como elementos filho do elemento [Restriction](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) no EWS.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-120">The filter types are implemented as descendant classes of the [SearchFilter](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) class in the EWS Managed API, and as child elements of the [Restriction](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) element in EWS.</span></span> 
  
<span data-ttu-id="d0b3a-121">**Tabela 1. Tipos de filtros de pesquisa**</span><span class="sxs-lookup"><span data-stu-id="d0b3a-121">**Table 1. Types of search filters**</span></span>

|<span data-ttu-id="d0b3a-122">**Tipo de filtro**</span><span class="sxs-lookup"><span data-stu-id="d0b3a-122">**Filter type**</span></span>|<span data-ttu-id="d0b3a-123">**Classe de API gerenciada do EWS**</span><span class="sxs-lookup"><span data-stu-id="d0b3a-123">**EWS Managed API class**</span></span>|<span data-ttu-id="d0b3a-124">**Elemento do EWS**</span><span class="sxs-lookup"><span data-stu-id="d0b3a-124">**EWS element**</span></span>|<span data-ttu-id="d0b3a-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d0b3a-125">**Description**</span></span>|
|:-----|:-----|:-----|:-----|
|<span data-ttu-id="d0b3a-126">Contém filtro</span><span class="sxs-lookup"><span data-stu-id="d0b3a-126">Contains filter</span></span>  <br/> |[<span data-ttu-id="d0b3a-127">ContainsSubstring</span><span class="sxs-lookup"><span data-stu-id="d0b3a-127">ContainsSubstring</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d0b3a-128">Contém</span><span class="sxs-lookup"><span data-stu-id="d0b3a-128">Contains</span></span>](https://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) <br/> |<span data-ttu-id="d0b3a-129">O melhor tipo de filtro a ser usado para comparações de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-129">The best filter type to use for string comparisons.</span></span> <span data-ttu-id="d0b3a-130">Ele permite controlar a diferenciação entre maiúsculas e minúsculas, se deve ignorar o espaço em branco e definir o modo de confinamento.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-130">It allows you to control case sensitivity, whether to ignore whitespace, and set the containment mode.</span></span>  <br/> |
|<span data-ttu-id="d0b3a-131">Filtro de bitmask</span><span class="sxs-lookup"><span data-stu-id="d0b3a-131">Bitmask filter</span></span>  <br/> |[<span data-ttu-id="d0b3a-132">ExcludesBitmask</span><span class="sxs-lookup"><span data-stu-id="d0b3a-132">ExcludesBitmask</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.excludesbitmask%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d0b3a-133">Exclui</span><span class="sxs-lookup"><span data-stu-id="d0b3a-133">Excludes</span></span>](https://msdn.microsoft.com/library/bbaeddf6-9a67-4ee0-af99-7a7a5bbdc0e1%28Office.15%29.aspx) <br/> |<span data-ttu-id="d0b3a-134">Permite pesquisar Propriedades de inteiros como bitmasks e retornar apenas resultados que tenham bits correspondentes à desdefinição de bitmask especificada.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-134">Allows you to search integer properties as bitmasks and only return results that have bits corresponding to the specified bitmask unset.</span></span>  <br/> |
|<span data-ttu-id="d0b3a-135">Filtro existe</span><span class="sxs-lookup"><span data-stu-id="d0b3a-135">Exists filter</span></span>  <br/> |[<span data-ttu-id="d0b3a-136">Existe</span><span class="sxs-lookup"><span data-stu-id="d0b3a-136">Exists</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.exists%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d0b3a-137">Existe</span><span class="sxs-lookup"><span data-stu-id="d0b3a-137">Exists</span></span>](https://msdn.microsoft.com/library/55d568bd-8dbc-4d50-b9d7-54b74a54d4b5%28Office.15%29.aspx) <br/> |<span data-ttu-id="d0b3a-138">Retorna todos os itens que têm a propriedade especificada presente, independentemente do valor.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-138">Returns all items that have the specified property present, regardless of value.</span></span>  <br/> |
|<span data-ttu-id="d0b3a-139">Filtro de igualdade</span><span class="sxs-lookup"><span data-stu-id="d0b3a-139">Equality filter</span></span>  <br/> |[<span data-ttu-id="d0b3a-140">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="d0b3a-140">IsEqualTo</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isequalto%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="d0b3a-141">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="d0b3a-141">IsNotEqualTo</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isnotequalto%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d0b3a-142">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="d0b3a-142">IsEqualTo</span></span>](https://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx) <br/> [<span data-ttu-id="d0b3a-143">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="d0b3a-143">IsNotEqualTo</span></span>](https://msdn.microsoft.com/library/e2eff26c-3403-45cd-bb74-1eb98c7dbfcd%28Office.15%29.aspx) <br/> |<span data-ttu-id="d0b3a-144">Compara o valor da propriedade especificada com um valor de constante especificado ou o valor de outra propriedade e retorna todos os itens que têm um valor igual (no caso de um filtro **IsEqualTo** ) ou um valor não igual (no caso de um filtro **IsNotEqualTo** ).</span><span class="sxs-lookup"><span data-stu-id="d0b3a-144">Compares the value of the specified property with either a specified constant value or the value of another property and return all items that have an equal value (in the case of an **IsEqualTo** filter) or a non-equal value (in the case of an **IsNotEqualTo** filter).</span></span>  <br/> |
|<span data-ttu-id="d0b3a-145">Filtro de teste relacional</span><span class="sxs-lookup"><span data-stu-id="d0b3a-145">Relational testing filter</span></span>  <br/> |[<span data-ttu-id="d0b3a-146">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="d0b3a-146">IsGreaterThan</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthan%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="d0b3a-147">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="d0b3a-147">IsGreaterThanOrEqualTo</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthanorequalto%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="d0b3a-148">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="d0b3a-148">IsLessThan</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.islessthan%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="d0b3a-149">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="d0b3a-149">IsLessThanOrEqualTo</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.islessthanorequalto%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d0b3a-150">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="d0b3a-150">IsGreaterThan</span></span>](https://msdn.microsoft.com/library/a6e9d462-cfa7-40ec-903e-128c95050352%28Office.15%29.aspx) <br/> [<span data-ttu-id="d0b3a-151">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="d0b3a-151">IsGreaterThanOrEqualTo</span></span>](https://msdn.microsoft.com/library/373cc954-314d-40e2-be03-cc08aefc0d5b%28Office.15%29.aspx) <br/> [<span data-ttu-id="d0b3a-152">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="d0b3a-152">IsLessThan</span></span>](https://msdn.microsoft.com/library/2550469b-6e5d-45a5-9ecc-090d1b409296%28Office.15%29.aspx) <br/> [<span data-ttu-id="d0b3a-153">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="d0b3a-153">IsLessThanOrEqualTo</span></span>](https://msdn.microsoft.com/library/b5d85eb2-5e15-4d01-ad49-6289e735ad8a%28Office.15%29.aspx) <br/> |<span data-ttu-id="d0b3a-154">Retorna todos os itens que têm um valor para a propriedade especificada na relação apropriada para um valor de constante especificado ou outra propriedade.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-154">Returns all items that have a value for the specified property in the appropriate relation to either a specified constant value or another property.</span></span> <span data-ttu-id="d0b3a-155">Por exemplo, um filtro **IsGreaterThan** retorna todos os itens que têm um valor maior do que o valor especificado na propriedade especificada.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-155">For example, an **IsGreaterThan** filter returns all items that have a value that is greater than the specified value in the specified property.</span></span>  <br/> |
|<span data-ttu-id="d0b3a-156">Negando filtro</span><span class="sxs-lookup"><span data-stu-id="d0b3a-156">Negating filter</span></span>  <br/> |[<span data-ttu-id="d0b3a-157">Not</span><span class="sxs-lookup"><span data-stu-id="d0b3a-157">Not</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.not%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d0b3a-158">Not</span><span class="sxs-lookup"><span data-stu-id="d0b3a-158">Not</span></span>](https://msdn.microsoft.com/library/1aa16318-7e90-4b19-bce8-dd1a20a66223%28Office.15%29.aspx) <br/> |<span data-ttu-id="d0b3a-159">Nega o resultado dos outros filtros.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-159">Negates the result of the other filters.</span></span>  <br/> |
|<span data-ttu-id="d0b3a-160">Filtro composto</span><span class="sxs-lookup"><span data-stu-id="d0b3a-160">Compound filter</span></span>  <br/> |[<span data-ttu-id="d0b3a-161">SearchFilterCollection</span><span class="sxs-lookup"><span data-stu-id="d0b3a-161">SearchFilterCollection</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d0b3a-162">And</span><span class="sxs-lookup"><span data-stu-id="d0b3a-162">And</span></span>](https://msdn.microsoft.com/library/790246c2-37ad-49a8-91b9-6186d743b011%28Office.15%29.aspx) <br/> [<span data-ttu-id="d0b3a-163">Or</span><span class="sxs-lookup"><span data-stu-id="d0b3a-163">Or</span></span>](https://msdn.microsoft.com/library/4876d83a-73a3-4953-9d95-3048e6b76ccb%28Office.15%29.aspx) <br/> |<span data-ttu-id="d0b3a-164">Combina vários filtros, permitindo critérios de pesquisa mais complexos.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-164">Combines multiple filters, allowing for more complex search criteria.</span></span>  <br/> |
   
### <a name="contains-filter"></a><span data-ttu-id="d0b3a-165">Contém filtro</span><span class="sxs-lookup"><span data-stu-id="d0b3a-165">Contains filter</span></span>

<span data-ttu-id="d0b3a-166">Um filtro contém é a melhor opção para pesquisar Propriedades de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-166">A contains filter is the best choice for searching string properties.</span></span> <span data-ttu-id="d0b3a-167">Com um filtro Contains, você pode controlar os aspectos da correspondência de cadeia de caracteres, como diferenciação de maiúsculas e minúsculas e como o espaço em branco é tratado, definindo o modo de confinamento e o modo de comparação.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-167">With a contains filter, you can control aspects of string matching, like case sensitivity and how whitespace is treated, by setting the containment mode and the comparison mode.</span></span>
  
#### <a name="contains-filter-in-the-ews-managed-api"></a><span data-ttu-id="d0b3a-168">Contém o filtro na API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="d0b3a-168">Contains filter in the EWS Managed API</span></span>
<span data-ttu-id="d0b3a-169"><a name="bk_ContainsEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="d0b3a-169"><a name="bk_ContainsEWSMA"> </a></span></span>

<span data-ttu-id="d0b3a-170">Se você estiver usando a API gerenciada do EWS, defina o modo de contenção usando a propriedade [ContainmentMode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.containmentmode%28v=exchg.80%29.aspx) da classe [ContainsSubstring](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) e defina o modo de comparação usando a propriedade [comparisonmode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.comparisonmode%28v=exchg.80%29.aspx) da classe **ContainsSubstring** .</span><span class="sxs-lookup"><span data-stu-id="d0b3a-170">If you're using the EWS Managed API, you set the containment mode by using the [ContainmentMode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.containmentmode%28v=exchg.80%29.aspx) property of the [ContainsSubstring](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) class, and you set the comparison mode by using the [ComparisonMode](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.comparisonmode%28v=exchg.80%29.aspx) property of the **ContainsSubstring** class.</span></span> <span data-ttu-id="d0b3a-171">O exemplo a seguir mostra como criar um filtro de pesquisa que pesquisa o campo de assunto de itens da subcadeia de caracteres "anotações da reunião".</span><span class="sxs-lookup"><span data-stu-id="d0b3a-171">The following example shows you how to create a search filter that searches the subject field of items for the substring "meeting notes".</span></span> <span data-ttu-id="d0b3a-172">Este exemplo ignora maiúsculas e minúsculas, mas não ignora espaço em branco.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-172">This example ignores case, but does not ignore whitespace.</span></span> 
  
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

#### <a name="contains-filter-in-ews"></a><span data-ttu-id="d0b3a-173">Contém o filtro no EWS</span><span class="sxs-lookup"><span data-stu-id="d0b3a-173">Contains filter in EWS</span></span>
<span data-ttu-id="d0b3a-174"><a name="bk_ContainsEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="d0b3a-174"><a name="bk_ContainsEWSMA"> </a></span></span>

<span data-ttu-id="d0b3a-175">No EWS, você define o modo de contenção usando o atributo **ContainmentMode** no elemento [Contains](https://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) e define o modo de comparação usando o atributo **ContainmentComparison** no elemento **Contains** .</span><span class="sxs-lookup"><span data-stu-id="d0b3a-175">In EWS, you set the containment mode by using the **ContainmentMode** attribute on the [Contains](https://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) element, and you set the comparison mode by using the **ContainmentComparison** attribute on the **Contains** element.</span></span> <span data-ttu-id="d0b3a-176">O exemplo a seguir mostra como criar um filtro de pesquisa para pesquisar o campo de assunto de itens da subcadeia de caracteres "anotações da reunião".</span><span class="sxs-lookup"><span data-stu-id="d0b3a-176">The following example shows you how to create a search filter to search the subject field of items for the substring "meeting notes".</span></span> <span data-ttu-id="d0b3a-177">Este exemplo ignora maiúsculas e minúsculas, mas não ignora espaço em branco.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-177">This example ignores case, but does not ignore whitespace.</span></span> 
  
```XML
<t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
  <t:FieldURI FieldURI="item:Subject" />
  <t:Constant Value="meeting notes" />
</t:Contains>
```

### <a name="bitmask-filter"></a><span data-ttu-id="d0b3a-178">Filtro de bitmask</span><span class="sxs-lookup"><span data-stu-id="d0b3a-178">Bitmask filter</span></span>

<span data-ttu-id="d0b3a-179">Um filtro de bitmask permite que você pesquise Propriedades de inteiros como bitmasks e retorne resultados em que os bits específicos não são definidos no valor da propriedade especificada.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-179">A bitmask filter enables you to search integer properties as bitmasks, and return results where specific bits are not set in the value of the specified property.</span></span>
  
#### <a name="bitmask-filter-in-the-ews-managed-api"></a><span data-ttu-id="d0b3a-180">Filtro de bitmask na API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="d0b3a-180">Bitmask filter in the EWS Managed API</span></span>

<span data-ttu-id="d0b3a-181">O exemplo a seguir mostra como usar a API gerenciada do EWS para criar um filtro de pesquisa para retornar todos os itens que têm um valor na propriedade personalizada **ItemIndex** (definido no [exemplo: localizar itens usando um filtro de pesquisa e a seção de API gerenciada do EWS](#bk_ExampleEWSMA) deste artigo) que não têm o segundo conjunto (10 em binário) definido.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-181">The following example shows you how to use the EWS Managed API to create a search filter to return all items that have a value in the **ItemIndex** custom property (defined in the [Example: Find items by using a search filter and the EWS Managed API](#bk_ExampleEWSMA) section of this article) that do not have the second bit (10 in binary) set.</span></span> 
  
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

#### <a name="bitmask-filter-in-ews"></a><span data-ttu-id="d0b3a-182">Filtro de bitmask no EWS</span><span class="sxs-lookup"><span data-stu-id="d0b3a-182">Bitmask filter in EWS</span></span>

<span data-ttu-id="d0b3a-183">O exemplo a seguir mostra como usar o EWS para criar um filtro de pesquisa para retornar todos os itens que têm um valor na propriedade personalizada **ItemIndex** (definida no [exemplo: localizar itens usando um filtro de pesquisa e a seção de API gerenciada do EWS](#bk_ExampleEWSMA) deste artigo) que não têm o segundo conjunto (10 em binário) definido.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-183">The following example shows you how to use EWS to create a search filter to return all items that have a value in the **ItemIndex** custom property (defined in the [Example: Find items by using a search filter and the EWS Managed API](#bk_ExampleEWSMA) section of this article) that do not have the second bit (10 in binary) set.</span></span> 
  
```XML
<t:Excludes>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:Bitmask Value="2" />
</t:Excludes>
```

### <a name="exists-filter"></a><span data-ttu-id="d0b3a-184">Filtro existe</span><span class="sxs-lookup"><span data-stu-id="d0b3a-184">Exists filter</span></span>

<span data-ttu-id="d0b3a-185">Um filtro Exists permite pesquisar itens que tenham uma propriedade específica definida, independentemente do valor.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-185">An exists filter enables you to search for items that have a specific property set on them, regardless of the value.</span></span>
  
#### <a name="exists-filter-in-the-ews-managed-api"></a><span data-ttu-id="d0b3a-186">Existe filtro na API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="d0b3a-186">Exists filter in the EWS Managed API</span></span>

<span data-ttu-id="d0b3a-187">O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens que têm a propriedade personalizada **ItemIndex** definida.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-187">The following example shows you how to create a search filter to return all items that have the **ItemIndex** custom property set.</span></span> 
  
```cs
// Find all items that have the custom property set.
SearchFilter.Exists customPropSetFilter =
    new SearchFilter.Exists(customPropDefinition);
```

#### <a name="exists-filter-in-ews"></a><span data-ttu-id="d0b3a-188">Existe filtro no EWS</span><span class="sxs-lookup"><span data-stu-id="d0b3a-188">Exists filter in EWS</span></span>

<span data-ttu-id="d0b3a-189">O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens que têm a propriedade personalizada **ItemIndex** definida.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-189">The following example shows you how to create a search filter to return all items that have the **ItemIndex** custom property set.</span></span> 
  
```XML
<t:Exists>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
</t:Exists>
```

### <a name="equality-filter"></a><span data-ttu-id="d0b3a-190">Filtro de igualdade</span><span class="sxs-lookup"><span data-stu-id="d0b3a-190">Equality filter</span></span>

<span data-ttu-id="d0b3a-191">Os filtros de igualdade permitem pesquisar todos os itens que têm um valor para a propriedade especificada que seja igual a um valor específico ou não é igual a um valor específico.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-191">Equality filters enable you to search for all items that have a value for the specified property that either equals a specific value or does not equal a specific value.</span></span> <span data-ttu-id="d0b3a-192">O valor com o qual comparar pode ser um valor constante ou o valor de outra propriedade em cada item.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-192">The value to compare with can be either a constant value or the value of another property on each item.</span></span>
  
#### <a name="equality-filter-in-the-ews-managed-api"></a><span data-ttu-id="d0b3a-193">Filtro de igualdade na API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="d0b3a-193">Equality filter in the EWS Managed API</span></span>

<span data-ttu-id="d0b3a-194">O exemplo a seguir mostra como usar a API gerenciada do EWS para criar um filtro de pesquisa para retornar todos os itens que não tenham sido lidos.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-194">The following example shows you how to use the EWS Managed API to create a search filter to return all items that have not been read.</span></span>
  
```cs
// Find all items that are not marked as read.
SearchFilter.IsEqualTo unreadFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.IsRead, false);
```

<span data-ttu-id="d0b3a-195">O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens que têm um valor na propriedade **ItemIndex** que não seja igual ao tamanho do item.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-195">The following example shows you how to create a search filter to return all items that have a value in the **ItemIndex** property that is not equal to the size of the item.</span></span> 
  
```cs
// Find all items that are marked as read.
SearchFilter.IsNotEqualTo indexNotEqualToSizeFilter =
    new SearchFilter.IsNotEqualTo(customPropDefinition, ItemSchema.Size);
```

#### <a name="equality-filter-in-ews"></a><span data-ttu-id="d0b3a-196">Filtro de igualdade no EWS</span><span class="sxs-lookup"><span data-stu-id="d0b3a-196">Equality filter in EWS</span></span>

<span data-ttu-id="d0b3a-197">O exemplo a seguir mostra como usar o EWS para criar um filtro de pesquisa para retornar todos os itens que não tenham sido lidos.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-197">The following example shows you how to use EWS to create a search filter to return all items that have not been read.</span></span>
  
```XML
<t:IsEqualTo>
  <t:FieldURI FieldURI="message:IsRead" />
  <t:FieldURIOrConstant>
    <t:Constant Value="false" />
  </t:FieldURIOrConstant>
</t:IsEqualTo>
```

<span data-ttu-id="d0b3a-198">O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens que têm um valor na propriedade **ItemIndex** que não seja igual ao tamanho do item.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-198">The following example shows you how to create a search filter to return all items that have a value in the **ItemIndex** property that is not equal to the size of the item.</span></span> 
  
```XML
<t:IsNotEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:FieldURI FieldURI="item:Size" />
  </t:FieldURIOrConstant>
</t:IsNotEqualTo>
```

### <a name="relational-testing-filter"></a><span data-ttu-id="d0b3a-199">Filtro de teste relacional</span><span class="sxs-lookup"><span data-stu-id="d0b3a-199">Relational testing filter</span></span>

<span data-ttu-id="d0b3a-200">Os filtros de teste relacionais permitem pesquisar todos os itens que têm um valor na propriedade especificada que seja maior que ( \> ), maior ou igual a ( \> =), menor que ( \< ) ou menor que ou igual a ( \< =) um valor especificado.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-200">Relational testing filters enable you to search for all items that have a value in the specified property that is either greater than (\>), greater than or equal to (\>=), less than (\<), or less than or equal to (\<=) a specified value.</span></span> <span data-ttu-id="d0b3a-201">O valor com o qual comparar pode ser um valor constante ou o valor de outra propriedade em cada item.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-201">The value to compare with can be either a constant value or the value of another property on each item.</span></span>
  
#### <a name="relational-testing-filter-in-the-ews-managed-api"></a><span data-ttu-id="d0b3a-202">Filtro de teste relacional na API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="d0b3a-202">Relational testing filter in the EWS Managed API</span></span>

<span data-ttu-id="d0b3a-203">O exemplo a seguir mostra como usar a API gerenciada do EWS para criar filtros de pesquisa para retornar todos os itens com um valor na propriedade **ItemIndex** que tenha a relação especificada com o valor 3 da constante.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-203">The following example shows you how to use the EWS Managed API to create search filters to return all items with a value in the **ItemIndex** property that has the specified relationship to the constant value 3.</span></span> 
  
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

#### <a name="relational-testing-filter-in-ews"></a><span data-ttu-id="d0b3a-204">Filtro de teste relacional no EWS</span><span class="sxs-lookup"><span data-stu-id="d0b3a-204">Relational testing filter in EWS</span></span>

<span data-ttu-id="d0b3a-205">O exemplo a seguir mostra como usar o EWS para criar um filtro de pesquisa para retornar todos os itens com um valor na propriedade **ItemIndex** que seja maior do que o valor de constante 3.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-205">The following example shows you how to use EWS to create a search filter to return all items with a value in the **ItemIndex** property that is greater than the constant value 3.</span></span> 
  
```XML
<t:IsGreaterThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThan>
```

<span data-ttu-id="d0b3a-206">O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens com um valor na propriedade **ItemIndex** que seja maior ou igual ao valor de constante 3.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-206">The following example shows you how to create a search filter to return all items with a value in the **ItemIndex** property that is greater than or equal to the constant value 3.</span></span> 
  
```XML
<t:IsGreaterThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThanOrEqualTo>
```

<span data-ttu-id="d0b3a-207">O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens com um valor na propriedade **ItemIndex** que seja menor do que o valor de constante 3.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-207">The following example shows you how to create a search filter to return all items with a value in the **ItemIndex** property that is less than the constant value 3.</span></span> 
  
```XML
<t:IsLessThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThan>
```

<span data-ttu-id="d0b3a-208">O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens com um valor na propriedade **ItemIndex** que seja menor ou igual ao valor de constante 3.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-208">The following example shows you how to create a search filter to return all items with a value in the **ItemIndex** property that is less than or equal to the constant value 3.</span></span> 
  
```XML
<t:IsLessThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThanOrEqualTo>
```

### <a name="negating-filter"></a><span data-ttu-id="d0b3a-209">Negando filtro</span><span class="sxs-lookup"><span data-stu-id="d0b3a-209">Negating filter</span></span>

<span data-ttu-id="d0b3a-210">Um filtro de negação permite que você retenha outro filtro e obtenha os resultados opostos da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-210">A negating filter enables you to negate another filter and get the opposite search results.</span></span> <span data-ttu-id="d0b3a-211">Enquanto outros filtros retornam resultados que correspondam a critérios específicos, um filtro de negação retorna resultados que não coincidem com os critérios especificados pelo filtro ao qual é aplicado.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-211">While other filters return results that match specific criteria, a negating filter returns results that do not match the criteria specified by the filter it is applied to.</span></span>
  
#### <a name="negating-filter-in-the-ews-managed-api"></a><span data-ttu-id="d0b3a-212">Negando o filtro na API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="d0b3a-212">Negating filter in the EWS Managed API</span></span>

<span data-ttu-id="d0b3a-213">O exemplo a seguir mostra como usar a API gerenciada do EWS para criar um filtro de pesquisa para retornar todos os itens que não têm a subcadeia de caracteres "anotações da reunião" no assunto.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-213">The following example shows you how to use the EWS Managed API to create a search filter to return all items that do not have the substring "meeting notes" in the subject.</span></span>
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
SearchFilter.Not subjectNotFilter =
    new SearchFilter.Not(subjectFilter);
```

#### <a name="negating-filter-in-ews"></a><span data-ttu-id="d0b3a-214">Negando filtro no EWS</span><span class="sxs-lookup"><span data-stu-id="d0b3a-214">Negating filter in EWS</span></span>

<span data-ttu-id="d0b3a-215">O exemplo a seguir mostra como criar um filtro de pesquisa para retornar todos os itens que não têm a subcadeia de caracteres "anotações da reunião" no assunto.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-215">The following example shows you how to create a search filter to return all items that do not have the substring "meeting notes" in the subject.</span></span>
  
```XML
<t:Not>
  <t:Contains ContainmentMode="ExactPhrase" ContainmentComparison="IgnoreCase">
    <t:FieldURI FieldURI="item:Subject" />
    <t:Constant Value="meeting notes" />
  </t:Contains>
</t:Not>
```

### <a name="compound-filter"></a><span data-ttu-id="d0b3a-216">Filtro composto</span><span class="sxs-lookup"><span data-stu-id="d0b3a-216">Compound filter</span></span>

<span data-ttu-id="d0b3a-217">Um filtro composto permite combinar vários filtros para criar critérios de pesquisa mais complexos.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-217">A compound filter enables you to combine multiple filters to create more complex search criteria.</span></span> <span data-ttu-id="d0b3a-218">Você pode combinar critérios usando os operadores lógicos e ou.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-218">You can combine criteria by using the logical operators AND or OR.</span></span> <span data-ttu-id="d0b3a-219">Dessa forma, você pode realizar pesquisas como "todos os emails do Sadie Daniels que contêm" notas da reunião "no assunto".</span><span class="sxs-lookup"><span data-stu-id="d0b3a-219">In this way, you can perform searches like "all mail from Sadie Daniels that contains 'meeting notes' in the subject".</span></span>
  
#### <a name="compound-filter-in-the-ews-managed-api"></a><span data-ttu-id="d0b3a-220">Filtro composto na API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="d0b3a-220">Compound filter in the EWS Managed API</span></span>

<span data-ttu-id="d0b3a-221">O exemplo a seguir mostra como usar a API gerenciada do EWS para criar um filtro de pesquisa que retorna todos os itens enviados do Sadie Daniels e que contêm "notas da reunião" no assunto.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-221">The following example shows you how to use the EWS Managed API to create a search filter that returns all items that are sent from Sadie Daniels and contain "meeting notes" in the subject.</span></span>
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
EmailAddress manager = new EmailAddress("sadie@contoso.com");
SearchFilter.IsEqualTo fromManagerFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, fromManagerFilter);
```

#### <a name="compound-filter-in-ews"></a><span data-ttu-id="d0b3a-222">Filtro composto no EWS</span><span class="sxs-lookup"><span data-stu-id="d0b3a-222">Compound filter in EWS</span></span>

<span data-ttu-id="d0b3a-223">O exemplo a seguir mostra como usar o EWS para criar um filtro de pesquisa que retorna todos os itens que são enviados do Sadie Daniels e que contêm "notas da reunião" no assunto.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-223">The following example shows you how to use EWS to create a search filter that returns all items that are sent from Sadie Daniels and contain "meeting notes" in the subject.</span></span>
  
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

## <a name="example-find-items-by-using-a-search-filter-and-the-ews-managed-api"></a><span data-ttu-id="d0b3a-224">Exemplo: localizar itens usando um filtro de pesquisa e a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="d0b3a-224">Example: Find items by using a search filter and the EWS Managed API</span></span>
<span data-ttu-id="d0b3a-225"><a name="bk_ExampleEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="d0b3a-225"><a name="bk_ExampleEWSMA"> </a></span></span>

<span data-ttu-id="d0b3a-226">Os seguintes métodos de API gerenciada do EWS usam filtros de pesquisa:</span><span class="sxs-lookup"><span data-stu-id="d0b3a-226">The following EWS Managed API methods use search filters:</span></span>
  
- [<span data-ttu-id="d0b3a-227">ExchangeService. FindItems</span><span class="sxs-lookup"><span data-stu-id="d0b3a-227">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
- [<span data-ttu-id="d0b3a-228">ExchangeService. FindFolders</span><span class="sxs-lookup"><span data-stu-id="d0b3a-228">ExchangeService.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
- [<span data-ttu-id="d0b3a-229">Folder. FindFolders</span><span class="sxs-lookup"><span data-stu-id="d0b3a-229">Folder.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
- [<span data-ttu-id="d0b3a-230">Folder. FindItems</span><span class="sxs-lookup"><span data-stu-id="d0b3a-230">Folder.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
<span data-ttu-id="d0b3a-231">O exemplo a seguir usa o método **ExchangeService. FindItems** ; no entanto, as mesmas regras e conceitos se aplicam a todos os métodos.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-231">The following example uses the **ExchangeService.FindItems** method; however, the same rules and concepts apply to all the methods.</span></span> <span data-ttu-id="d0b3a-232">Neste exemplo, um método chamado **SearchWithFilter** é definido.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-232">In this example, a method called **SearchWithFilter** is defined.</span></span> <span data-ttu-id="d0b3a-233">Ele usa um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , um objeto [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) e um objeto [SearchFilter](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) como parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-233">It takes an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, a [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) object, and a [SearchFilter](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) object as parameters.</span></span> <span data-ttu-id="d0b3a-234">Este exemplo pressupõe que o objeto **ExchangeService** tenha sido inicializado com valores válidos nas propriedades de [credenciais](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) e [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d0b3a-234">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> <span data-ttu-id="d0b3a-235">A classe **SearchFilter** é a classe base para todos os diferentes filtros de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-235">The **SearchFilter** class is the base class for all the different search filters.</span></span> 
  
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

<span data-ttu-id="d0b3a-236">Você pode usar essa função com qualquer um dos filtros de pesquisa mostrados nos exemplos deste artigo.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-236">You can use this function with any of the search filters shown in the examples in this article.</span></span> <span data-ttu-id="d0b3a-237">Este exemplo usa um filtro composto para retornar todos os itens na caixa de entrada de Sadie Daniels com "notas da reunião" no assunto.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-237">This example uses a compound filter to return all items in the Inbox from Sadie Daniels with "meeting notes" in the subject.</span></span>
  
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

## <a name="example-find-an-item-by-using-a-search-filter-and-ews"></a><span data-ttu-id="d0b3a-238">Exemplo: localizar um item usando um filtro de pesquisa e o EWS</span><span class="sxs-lookup"><span data-stu-id="d0b3a-238">Example: Find an item by using a search filter and EWS</span></span>
<span data-ttu-id="d0b3a-239"><a name="bk_ExampleEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="d0b3a-239"><a name="bk_ExampleEWS"> </a></span></span>

<span data-ttu-id="d0b3a-240">As operações do EWS a seguir usam filtros de pesquisa:</span><span class="sxs-lookup"><span data-stu-id="d0b3a-240">The following EWS operations use search filters:</span></span>
  
- [<span data-ttu-id="d0b3a-241">FindFolder</span><span class="sxs-lookup"><span data-stu-id="d0b3a-241">FindFolder</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
- [<span data-ttu-id="d0b3a-242">FindItem</span><span class="sxs-lookup"><span data-stu-id="d0b3a-242">FindItem</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
<span data-ttu-id="d0b3a-243">O exemplo a seguir usa a operação **FindItem** ; no entanto, as mesmas regras e conceitos se aplicam às duas operações.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-243">The following example uses the **FindItem** operation; however, the same rules and concepts apply to both operations.</span></span> <span data-ttu-id="d0b3a-244">Os filtros de pesquisa estão contidos no elemento [Restriction](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) nas solicitações SOAP.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-244">Search filters are contained in the [Restriction](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) element in SOAP requests.</span></span> <span data-ttu-id="d0b3a-245">Este exemplo envia uma solicitação SOAP equivalente à pesquisa mostrada no exemplo anterior de API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-245">This example sends a SOAP request that is equivalent to the search that is shown in the preceding EWS Managed API example.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="d0b3a-246">O exemplo a seguir mostra a resposta do servidor, incluindo os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-246">The following example shows the response from the server, including the search results.</span></span>
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="next-steps"></a><span data-ttu-id="d0b3a-247">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="d0b3a-247">Next steps</span></span>
<span data-ttu-id="d0b3a-248"><a name="bk_ExampleEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="d0b3a-248"><a name="bk_ExampleEWS"> </a></span></span>

<span data-ttu-id="d0b3a-249">Agora que você está familiarizado com o uso de filtros de pesquisa em pesquisas básicas, é possível passar para técnicas de pesquisa mais avançadas.</span><span class="sxs-lookup"><span data-stu-id="d0b3a-249">Now that you're familiar with using search filters in basic searches, you can move on to more advanced search techniques.</span></span>
  
- [<span data-ttu-id="d0b3a-250">Executar pesquisas agrupadas usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d0b3a-250">Perform grouped searches by using EWS in Exchange</span></span>](how-to-perform-grouped-searches-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="d0b3a-251">Executar pesquisas paginadas usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d0b3a-251">Perform paged searches by using EWS in Exchange</span></span>](how-to-perform-paged-searches-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="d0b3a-252">Confira também</span><span class="sxs-lookup"><span data-stu-id="d0b3a-252">See also</span></span>

- [<span data-ttu-id="d0b3a-253">Pesquisar e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d0b3a-253">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)    
- [<span data-ttu-id="d0b3a-254">Executar uma pesquisa do AQS usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d0b3a-254">Perform an AQS search by using EWS in Exchange</span></span>](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)   
- [<span data-ttu-id="d0b3a-255">ExchangeService. FindItems</span><span class="sxs-lookup"><span data-stu-id="d0b3a-255">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="d0b3a-256">ExchangeService. FindFolders</span><span class="sxs-lookup"><span data-stu-id="d0b3a-256">ExchangeService.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="d0b3a-257">Folder. FindFolders</span><span class="sxs-lookup"><span data-stu-id="d0b3a-257">Folder.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="d0b3a-258">Folder. FindItems</span><span class="sxs-lookup"><span data-stu-id="d0b3a-258">Folder.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="d0b3a-259">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="d0b3a-259">FindFolder operation</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)   
- [<span data-ttu-id="d0b3a-260">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="d0b3a-260">FindItem operation</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

