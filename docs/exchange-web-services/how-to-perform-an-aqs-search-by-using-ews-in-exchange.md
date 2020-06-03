---
title: Executar uma pesquisa do AQS usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: c136901a-313e-4adf-a223-1d090d16917a
description: Descubra como Pesquisar cadeias de caracteres de consulta e AQS em sua API gerenciada do EWS ou aplicativo do EWS.
localization_priority: Priority
ms.openlocfilehash: 9f611a8d90c6baf0f307897735c6366c82bb63c8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455713"
---
# <a name="perform-an-aqs-search-by-using-ews-in-exchange"></a><span data-ttu-id="a4c27-103">Executar uma pesquisa do AQS usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a4c27-103">Perform an AQS search by using EWS in Exchange</span></span>

<span data-ttu-id="a4c27-104">Descubra como Pesquisar cadeias de caracteres de consulta e AQS em sua API gerenciada do EWS ou aplicativo do EWS.</span><span class="sxs-lookup"><span data-stu-id="a4c27-104">Find out how to search with query strings and AQS in your EWS Managed API or EWS application.</span></span>
  
<span data-ttu-id="a4c27-105">As cadeias de caracteres de consulta oferecem uma alternativa aos [filtros de pesquisa](how-to-use-search-filters-with-ews-in-exchange.md) para expressar critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a4c27-105">Query strings provide an alternative to [search filters](how-to-use-search-filters-with-ews-in-exchange.md) for expressing search criteria.</span></span> <span data-ttu-id="a4c27-106">A maior vantagem de usar cadeias de caracteres de consulta é que você não precisa especificar uma única propriedade a Pesquisar.</span><span class="sxs-lookup"><span data-stu-id="a4c27-106">The biggest advantage to using query strings is that you are not required to specify a single property to search.</span></span> <span data-ttu-id="a4c27-107">Você pode simplesmente fornecer um valor e a pesquisa será aplicada a todos os campos usados com frequência nos itens.</span><span class="sxs-lookup"><span data-stu-id="a4c27-107">You can just provide a value, and the search will apply to all commonly used fields on the items.</span></span> <span data-ttu-id="a4c27-108">Você também pode refinar sua pesquisa usando a sintaxe de consulta avançada (AQS) em vez de um valor simples.</span><span class="sxs-lookup"><span data-stu-id="a4c27-108">You can also refine your search by using Advanced Query Syntax (AQS) instead of a simple value.</span></span> <span data-ttu-id="a4c27-109">No entanto, as cadeias de caracteres de consulta têm as seguintes limitações que você deve estar ciente antes de adicioná-las à caixa de ferramentas:</span><span class="sxs-lookup"><span data-stu-id="a4c27-109">However, query strings have the following limitations that you should be aware of before you add them to your toolbox:</span></span> 
  
- <span data-ttu-id="a4c27-110">**Capacidade limitada de Pesquisar propriedades específicas.**</span><span class="sxs-lookup"><span data-stu-id="a4c27-110">**Limited ability to search specific properties.**</span></span> <span data-ttu-id="a4c27-111">Quando você pesquisa com um valor simples em uma cadeia de caracteres de consulta, a pesquisa é executada em todas as propriedades indexadas.</span><span class="sxs-lookup"><span data-stu-id="a4c27-111">When you search with a simple value in a query string, the search is performed against all indexed properties.</span></span> <span data-ttu-id="a4c27-112">Você pode refinar sua pesquisa a propriedades específicas, mas as propriedades disponíveis para uso em uma cadeia de caracteres AQS são limitadas.</span><span class="sxs-lookup"><span data-stu-id="a4c27-112">You can refine your search to specific properties, but the properties available to use in an AQS string are limited.</span></span> <span data-ttu-id="a4c27-113">Se a propriedade que você deseja Pesquisar não é uma das propriedades que estão disponíveis para o AQS, considere usar um filtro de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a4c27-113">If the property you want to search isn't one of the properties that are available for AQS, consider using a search filter.</span></span> 
    
- <span data-ttu-id="a4c27-114">**Propriedades personalizadas não são pesquisadas.**</span><span class="sxs-lookup"><span data-stu-id="a4c27-114">**Custom properties aren't searched.**</span></span> <span data-ttu-id="a4c27-115">Pesquisas de cadeia de caracteres de consulta são realizadas em um índice e as propriedades personalizadas não são incluídas nesse índice.</span><span class="sxs-lookup"><span data-stu-id="a4c27-115">Query string searches are performed against an index, and custom properties are not included in that index.</span></span> <span data-ttu-id="a4c27-116">Se você precisar pesquisar Propriedades personalizadas, use um filtro de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a4c27-116">If you need to search custom properties, use a search filter instead.</span></span> 
    
- <span data-ttu-id="a4c27-117">**Controle limitado para pesquisas de cadeia de caracteres.**</span><span class="sxs-lookup"><span data-stu-id="a4c27-117">**Limited control for string searches.**</span></span> <span data-ttu-id="a4c27-118">Pesquisas de cadeia de caracteres de consulta sempre ignoram maiúsculas e são sempre subcadeias de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a4c27-118">Query string searches always ignore case, and are always substring searches.</span></span> <span data-ttu-id="a4c27-119">Se você deseja fazer pesquisas de diferenciação de maiúsculas e minúsculas, prefixo ou correspondência exata, use um filtro de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a4c27-119">If you want to do case-sensitive, prefix, or exact match searches, use a search filter.</span></span> 
    
- <span data-ttu-id="a4c27-120">**Não disponível para pastas ou pastas de pesquisa.**</span><span class="sxs-lookup"><span data-stu-id="a4c27-120">**Not available for folders or search folders.**</span></span> <span data-ttu-id="a4c27-121">As operações do EWS para pesquisa de pastas não são compatíveis com o uso de uma cadeia de caracteres de consulta.</span><span class="sxs-lookup"><span data-stu-id="a4c27-121">The EWS operations for searching for folders don't support using a query string.</span></span> <span data-ttu-id="a4c27-122">Além disso, as pastas de pesquisa não dão suporte a sequências de consulta.</span><span class="sxs-lookup"><span data-stu-id="a4c27-122">Additionally, search folders don't support query strings.</span></span> <span data-ttu-id="a4c27-123">Em ambos os casos, um filtro de pesquisa é sua única opção.</span><span class="sxs-lookup"><span data-stu-id="a4c27-123">In both cases, a search filter is your only option.</span></span> 
    
## <a name="creating-a-query-string"></a><span data-ttu-id="a4c27-124">Criar uma cadeia de caracteres de consulta</span><span class="sxs-lookup"><span data-stu-id="a4c27-124">Creating a query string</span></span>
<span data-ttu-id="a4c27-125"><a name="bk_CreateQueryString"> </a></span><span class="sxs-lookup"><span data-stu-id="a4c27-125"><a name="bk_CreateQueryString"> </a></span></span>

<span data-ttu-id="a4c27-126">As cadeias de caracteres de consulta na API gerenciada do EWS e no EWS são interpretadas como um subconjunto da sintaxe AQS.</span><span class="sxs-lookup"><span data-stu-id="a4c27-126">Query strings in the EWS Managed API and EWS are interpreted as a subset of AQS syntax.</span></span> <span data-ttu-id="a4c27-127">As cadeias de caracteres AQS são compostas de valores ou pares de palavra-chave/valor, separados por dois-pontos (:).</span><span class="sxs-lookup"><span data-stu-id="a4c27-127">AQS strings are composed of either values or keyword/value pairs, separated by a colon (:).</span></span>
  
`keyword:value`

<span data-ttu-id="a4c27-128">Quando um valor é especificado sem uma palavra-chave, todas as propriedades indexadas são pesquisadas quanto ao valor.</span><span class="sxs-lookup"><span data-stu-id="a4c27-128">When a value is specified without a keyword, all indexed properties are searched for the value.</span></span> <span data-ttu-id="a4c27-129">Se uma palavra-chave estiver emparelhada com um valor, a palavra-chave especificará uma propriedade para pesquisar o valor correspondente.</span><span class="sxs-lookup"><span data-stu-id="a4c27-129">If a keyword is paired with a value, the keyword specifies a property to search for the corresponding value.</span></span>
  
<span data-ttu-id="a4c27-130">**Tabela 1. Palavras-chave AQS suportadas**</span><span class="sxs-lookup"><span data-stu-id="a4c27-130">**Table 1. Supported AQS keywords**</span></span>

|<span data-ttu-id="a4c27-131">**Chaves**</span><span class="sxs-lookup"><span data-stu-id="a4c27-131">**Keyword**</span></span>|<span data-ttu-id="a4c27-132">**Value type**</span><span class="sxs-lookup"><span data-stu-id="a4c27-132">**Value type**</span></span>|<span data-ttu-id="a4c27-133">**Exemplo**</span><span class="sxs-lookup"><span data-stu-id="a4c27-133">**Example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a4c27-134">subject</span><span class="sxs-lookup"><span data-stu-id="a4c27-134">subject</span></span>  <br/> |<span data-ttu-id="a4c27-135">String</span><span class="sxs-lookup"><span data-stu-id="a4c27-135">String</span></span>  <br/> |<span data-ttu-id="a4c27-136">Assunto: projeto</span><span class="sxs-lookup"><span data-stu-id="a4c27-136">subject:project</span></span>  <br/> |
|<span data-ttu-id="a4c27-137">corpo</span><span class="sxs-lookup"><span data-stu-id="a4c27-137">body</span></span>  <br/> |<span data-ttu-id="a4c27-138">String</span><span class="sxs-lookup"><span data-stu-id="a4c27-138">String</span></span>  <br/> |<span data-ttu-id="a4c27-139">corpo: números de vendas</span><span class="sxs-lookup"><span data-stu-id="a4c27-139">body:sales figures</span></span>  <br/> |
|<span data-ttu-id="a4c27-140">anexo</span><span class="sxs-lookup"><span data-stu-id="a4c27-140">attachment</span></span>  <br/> |<span data-ttu-id="a4c27-141">String</span><span class="sxs-lookup"><span data-stu-id="a4c27-141">String</span></span>  <br/> |<span data-ttu-id="a4c27-142">Anexo: relatório</span><span class="sxs-lookup"><span data-stu-id="a4c27-142">attachment:report</span></span>  <br/> |
|<span data-ttu-id="a4c27-143">para</span><span class="sxs-lookup"><span data-stu-id="a4c27-143">to</span></span>  <br/> |<span data-ttu-id="a4c27-144">String</span><span class="sxs-lookup"><span data-stu-id="a4c27-144">String</span></span>  <br/> |<span data-ttu-id="a4c27-145">para: "Sadie Daniels"</span><span class="sxs-lookup"><span data-stu-id="a4c27-145">to:"Sadie Daniels"</span></span>  <br/> |
|<span data-ttu-id="a4c27-146">from</span><span class="sxs-lookup"><span data-stu-id="a4c27-146">from</span></span>  <br/> |<span data-ttu-id="a4c27-147">String</span><span class="sxs-lookup"><span data-stu-id="a4c27-147">String</span></span>  <br/> |<span data-ttu-id="a4c27-148">de: Espero</span><span class="sxs-lookup"><span data-stu-id="a4c27-148">from:hope</span></span>  <br/> |
|<span data-ttu-id="a4c27-149">cc</span><span class="sxs-lookup"><span data-stu-id="a4c27-149">cc</span></span>  <br/> |<span data-ttu-id="a4c27-150">String</span><span class="sxs-lookup"><span data-stu-id="a4c27-150">String</span></span>  <br/> |<span data-ttu-id="a4c27-151">CC: "Ronnie Sturgis"</span><span class="sxs-lookup"><span data-stu-id="a4c27-151">cc:"Ronnie Sturgis"</span></span>  <br/> |
|<span data-ttu-id="a4c27-152">bcc</span><span class="sxs-lookup"><span data-stu-id="a4c27-152">bcc</span></span>  <br/> |<span data-ttu-id="a4c27-153">String</span><span class="sxs-lookup"><span data-stu-id="a4c27-153">String</span></span>  <br/> |<span data-ttu-id="a4c27-154">CCO: Mack</span><span class="sxs-lookup"><span data-stu-id="a4c27-154">bcc:mack</span></span>  <br/> |
|<span data-ttu-id="a4c27-155">participants</span><span class="sxs-lookup"><span data-stu-id="a4c27-155">participants</span></span>  <br/> |<span data-ttu-id="a4c27-156">String</span><span class="sxs-lookup"><span data-stu-id="a4c27-156">String</span></span>  <br/> |<span data-ttu-id="a4c27-157">participantes: Sadie</span><span class="sxs-lookup"><span data-stu-id="a4c27-157">participants:sadie</span></span>  <br/> |
|<span data-ttu-id="a4c27-158">category</span><span class="sxs-lookup"><span data-stu-id="a4c27-158">category</span></span>  <br/> |<span data-ttu-id="a4c27-159">String</span><span class="sxs-lookup"><span data-stu-id="a4c27-159">String</span></span>  <br/> |<span data-ttu-id="a4c27-160">Categoria: projeto</span><span class="sxs-lookup"><span data-stu-id="a4c27-160">category:project</span></span>  <br/> |
|<span data-ttu-id="a4c27-161">importance</span><span class="sxs-lookup"><span data-stu-id="a4c27-161">importance</span></span>  <br/> |<span data-ttu-id="a4c27-162">String</span><span class="sxs-lookup"><span data-stu-id="a4c27-162">String</span></span>  <br/> |<span data-ttu-id="a4c27-163">prioridade: alta</span><span class="sxs-lookup"><span data-stu-id="a4c27-163">importance:high</span></span>  <br/> |
|<span data-ttu-id="a4c27-164">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4c27-164">kind</span></span>  <br/> |<span data-ttu-id="a4c27-165">Tipo de item</span><span class="sxs-lookup"><span data-stu-id="a4c27-165">Item type</span></span>  <br/> |<span data-ttu-id="a4c27-166">tipo: reuniões</span><span class="sxs-lookup"><span data-stu-id="a4c27-166">kind:meetings</span></span>  <br/> |
|<span data-ttu-id="a4c27-167">enviado</span><span class="sxs-lookup"><span data-stu-id="a4c27-167">sent</span></span>  <br/> |<span data-ttu-id="a4c27-168">Data</span><span class="sxs-lookup"><span data-stu-id="a4c27-168">Date</span></span>  <br/> |<span data-ttu-id="a4c27-169">enviado: 12/10/2013</span><span class="sxs-lookup"><span data-stu-id="a4c27-169">sent:12/10/2013</span></span>  <br/> |
|<span data-ttu-id="a4c27-170">recebido</span><span class="sxs-lookup"><span data-stu-id="a4c27-170">received</span></span>  <br/> |<span data-ttu-id="a4c27-171">Data</span><span class="sxs-lookup"><span data-stu-id="a4c27-171">Date</span></span>  <br/> |<span data-ttu-id="a4c27-172">recebido: ontem</span><span class="sxs-lookup"><span data-stu-id="a4c27-172">received:yesterday</span></span>  <br/> |
|<span data-ttu-id="a4c27-173">HasAttachment</span><span class="sxs-lookup"><span data-stu-id="a4c27-173">hasattachment</span></span>  <br/> |<span data-ttu-id="a4c27-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="a4c27-174">Boolean</span></span>  <br/> |<span data-ttu-id="a4c27-175">Tem anexo: true</span><span class="sxs-lookup"><span data-stu-id="a4c27-175">Has attachment:true</span></span>  <br/> |
|<span data-ttu-id="a4c27-176">issinalizado</span><span class="sxs-lookup"><span data-stu-id="a4c27-176">isflagged</span></span>  <br/> |<span data-ttu-id="a4c27-177">Booliano</span><span class="sxs-lookup"><span data-stu-id="a4c27-177">Boolean</span></span>  <br/> |<span data-ttu-id="a4c27-178">issinalizado: true</span><span class="sxs-lookup"><span data-stu-id="a4c27-178">isflagged:true</span></span>  <br/> |
|<span data-ttu-id="a4c27-179">IsRead</span><span class="sxs-lookup"><span data-stu-id="a4c27-179">isread</span></span>  <br/> |<span data-ttu-id="a4c27-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="a4c27-180">Boolean</span></span>  <br/> |<span data-ttu-id="a4c27-181">IsRead: false</span><span class="sxs-lookup"><span data-stu-id="a4c27-181">isread:false</span></span>  <br/> |
|<span data-ttu-id="a4c27-182">size</span><span class="sxs-lookup"><span data-stu-id="a4c27-182">size</span></span>  <br/> |<span data-ttu-id="a4c27-183">Número</span><span class="sxs-lookup"><span data-stu-id="a4c27-183">Number</span></span>  <br/> |<span data-ttu-id="a4c27-184">Tamanho: \> 5000</span><span class="sxs-lookup"><span data-stu-id="a4c27-184">size:\>5000</span></span>  <br/> |
   
<span data-ttu-id="a4c27-185">Vamos dar uma olhada em como os diferentes tipos de valor funcionam.</span><span class="sxs-lookup"><span data-stu-id="a4c27-185">Let's take a look at how the different value types work.</span></span>
  
### <a name="using-a-string-value-type"></a><span data-ttu-id="a4c27-186">Usando um tipo de valor de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a4c27-186">Using a string value type</span></span>

<span data-ttu-id="a4c27-187">Os tipos de valores de cadeia de caracteres são, por padrão, pesquisados como prefixo as pesquisas que não diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="a4c27-187">String value types are by default searched as prefix substring searches that are not case-sensitive.</span></span> <span data-ttu-id="a4c27-188">Isso significa que a pesquisa por assunto: Project corresponderia a qualquer um dos seguintes assuntos:</span><span class="sxs-lookup"><span data-stu-id="a4c27-188">That means that searching for subject:project would match any of the following subjects:</span></span> 
  
- <span data-ttu-id="a4c27-189">Notas da reunião do projeto</span><span class="sxs-lookup"><span data-stu-id="a4c27-189">Project meeting notes</span></span>
    
- <span data-ttu-id="a4c27-190">Você tem os planos do projeto?</span><span class="sxs-lookup"><span data-stu-id="a4c27-190">Do you have the project plans?</span></span>
    
- <span data-ttu-id="a4c27-191">Projeções de vendas de dezembro</span><span class="sxs-lookup"><span data-stu-id="a4c27-191">December sales projections</span></span>
    
<span data-ttu-id="a4c27-192">Você pode alterar a pesquisa para exigir a palavra inteira em vez de coincidir prefixos, colocando a cadeia de caracteres entre aspas.</span><span class="sxs-lookup"><span data-stu-id="a4c27-192">You can change the search to require the whole word rather than matching prefixes by enclosing the string in quotation marks.</span></span> <span data-ttu-id="a4c27-193">Pesquisando o assunto: "projeto" eliminaria o valor "projeções de vendas de dezembro" da lista de correspondências.</span><span class="sxs-lookup"><span data-stu-id="a4c27-193">Searching for subject:"project" would eliminate the "December sales projections" value from the list of matches.</span></span> <span data-ttu-id="a4c27-194">Observe que o valor ainda não diferencia maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="a4c27-194">Note that the value is still not case-sensitive.</span></span> 
  
<span data-ttu-id="a4c27-195">Se você usar várias palavras em uma cadeia de caracteres de consulta, uma correspondência exigirá que ambas as palavras apareçam nos campos pesquisados.</span><span class="sxs-lookup"><span data-stu-id="a4c27-195">If you use multiple words in a query string, a match requires that both words appear in the searched fields.</span></span> <span data-ttu-id="a4c27-196">Por exemplo, a pesquisa por assunto: o plano de projeto corresponderia a qualquer um dos seguintes assuntos:</span><span class="sxs-lookup"><span data-stu-id="a4c27-196">For example, searching for subject:project plan would match any of the following subjects:</span></span> 
  
- <span data-ttu-id="a4c27-197">Plano de projeto</span><span class="sxs-lookup"><span data-stu-id="a4c27-197">Project plan</span></span>
    
- <span data-ttu-id="a4c27-198">Você tem os planos do projeto?</span><span class="sxs-lookup"><span data-stu-id="a4c27-198">Do you have the project plans?</span></span>
    
- <span data-ttu-id="a4c27-199">Envie-me o plano para o nosso projeto</span><span class="sxs-lookup"><span data-stu-id="a4c27-199">Please send me the plan for our project</span></span>
    
- <span data-ttu-id="a4c27-200">Planejar Marcos de projeto</span><span class="sxs-lookup"><span data-stu-id="a4c27-200">Planning project milestones</span></span>
    
<span data-ttu-id="a4c27-201">Se você incluir várias palavras entre aspas, elas serão tratadas como uma única frase.</span><span class="sxs-lookup"><span data-stu-id="a4c27-201">If you enclose multiple words in quotation marks, they are treated as a single phrase.</span></span> <span data-ttu-id="a4c27-202">Pesquisando o assunto: "plano de projeto" só corresponderia ao assunto "plano do projeto" da lista anterior.</span><span class="sxs-lookup"><span data-stu-id="a4c27-202">Searching for subject:"project plan" would only match the "Project plan" subject from the previous list.</span></span> 
  
### <a name="using-an-item-type-value-type"></a><span data-ttu-id="a4c27-203">Usando um tipo de valor de tipo de item</span><span class="sxs-lookup"><span data-stu-id="a4c27-203">Using an item type value type</span></span>

<span data-ttu-id="a4c27-204">Você pode usar os seguintes valores de tipo de item com a palavra-chave **Kind** para limitar os resultados da pesquisa a apenas um tipo específico de item, como email ou solicitações de reunião:</span><span class="sxs-lookup"><span data-stu-id="a4c27-204">You can use the following item type values with the **kind** keyword to limit your search results to only a specific type of item, such as email or meeting requests:</span></span> 
  
- <span data-ttu-id="a4c27-205">contacts</span><span class="sxs-lookup"><span data-stu-id="a4c27-205">contacts</span></span>    
- <span data-ttu-id="a4c27-206">docs</span><span class="sxs-lookup"><span data-stu-id="a4c27-206">docs</span></span>    
- <span data-ttu-id="a4c27-207">email</span><span class="sxs-lookup"><span data-stu-id="a4c27-207">email</span></span>    
- <span data-ttu-id="a4c27-208">fax</span><span class="sxs-lookup"><span data-stu-id="a4c27-208">faxes</span></span>    
- <span data-ttu-id="a4c27-209">im (corresponde a mensagens instantâneas)</span><span class="sxs-lookup"><span data-stu-id="a4c27-209">im (corresponds to instant messages)</span></span>    
- <span data-ttu-id="a4c27-210">diários</span><span class="sxs-lookup"><span data-stu-id="a4c27-210">journals</span></span>    
- <span data-ttu-id="a4c27-211">reuniões (corresponde a compromissos e solicitações de reunião)</span><span class="sxs-lookup"><span data-stu-id="a4c27-211">meetings (corresponds to appointments and meeting requests)</span></span>    
- <span data-ttu-id="a4c27-212">notes</span><span class="sxs-lookup"><span data-stu-id="a4c27-212">notes</span></span>    
- <span data-ttu-id="a4c27-213">postagens</span><span class="sxs-lookup"><span data-stu-id="a4c27-213">posts</span></span>    
- <span data-ttu-id="a4c27-214">rssfeeds</span><span class="sxs-lookup"><span data-stu-id="a4c27-214">rssfeeds</span></span>    
- <span data-ttu-id="a4c27-215">tarefas</span><span class="sxs-lookup"><span data-stu-id="a4c27-215">tasks</span></span>    
- <span data-ttu-id="a4c27-216">postal</span><span class="sxs-lookup"><span data-stu-id="a4c27-216">voicemail</span></span>
    
### <a name="using-a-date-value-type"></a><span data-ttu-id="a4c27-217">Usando um tipo de valor de data</span><span class="sxs-lookup"><span data-stu-id="a4c27-217">Using a date value type</span></span>

<span data-ttu-id="a4c27-218">Você pode Pesquisar tipos de valor de data de várias maneiras diferentes.</span><span class="sxs-lookup"><span data-stu-id="a4c27-218">You can search date value types in a number of different ways.</span></span> <span data-ttu-id="a4c27-219">O mais simples é Pesquisar uma data específica.</span><span class="sxs-lookup"><span data-stu-id="a4c27-219">The simplest is to search for a specific date.</span></span> <span data-ttu-id="a4c27-220">Pesquisa com recebido: 12/11/2013 retornará todos os itens recebidos em 11 de dezembro de 2013.</span><span class="sxs-lookup"><span data-stu-id="a4c27-220">Searching with received:12/11/2013 will return all items received on December 11, 2013.</span></span> <span data-ttu-id="a4c27-221">No entanto, você também pode ser menos específico.</span><span class="sxs-lookup"><span data-stu-id="a4c27-221">However, you can also be less specific.</span></span> <span data-ttu-id="a4c27-222">Pesquisa com recebido: 12/11 retornará todos os itens recebidos em 11 de dezembro do ano atual.</span><span class="sxs-lookup"><span data-stu-id="a4c27-222">Searching with received:12/11 will return all items received on December 11 of the current year.</span></span> 
  
<span data-ttu-id="a4c27-223">Outra opção é usar os nomes dos meses.</span><span class="sxs-lookup"><span data-stu-id="a4c27-223">Another option is to use the month names.</span></span> <span data-ttu-id="a4c27-224">Você pode pesquisar com recebido: 11 de dezembro de 2013 ou dezembro 11 para obter os mesmos resultados recebidos: 12/11/2013 e recebidos: 12/11, respectivamente.</span><span class="sxs-lookup"><span data-stu-id="a4c27-224">You can search with received:December 11, 2013 or December 11 to get the same results as received:12/11/2013 and received:12/11, respectively.</span></span> <span data-ttu-id="a4c27-225">Você também pode pesquisar com recebido: dezembro para obter todos os itens recebidos no mês de dezembro, no ano atual.</span><span class="sxs-lookup"><span data-stu-id="a4c27-225">You can also search with received:December to get all items received in the month of December, in the current year.</span></span> 
  
<span data-ttu-id="a4c27-226">O uso dos nomes dos dias da semana também é uma opção.</span><span class="sxs-lookup"><span data-stu-id="a4c27-226">Using the names of the days of the week is also an option.</span></span> <span data-ttu-id="a4c27-227">Pesquisa com recebido: terça-feira retornará todos os itens recebidos na terça-feira da semana atual.</span><span class="sxs-lookup"><span data-stu-id="a4c27-227">Searching with received:Tuesday will return all items received on Tuesday of the current week.</span></span> 
  
<span data-ttu-id="a4c27-228">Os tipos de valores de data também oferecem suporte a um conjunto de palavras-chave para pesquisas em relação à hora atual.</span><span class="sxs-lookup"><span data-stu-id="a4c27-228">Date value types also support a set of keywords for searches relative to the current time.</span></span> <span data-ttu-id="a4c27-229">Há suporte para as seguintes palavras-chave:</span><span class="sxs-lookup"><span data-stu-id="a4c27-229">The following keywords are supported:</span></span>
  
- <span data-ttu-id="a4c27-230">hoje</span><span class="sxs-lookup"><span data-stu-id="a4c27-230">today</span></span>  
- <span data-ttu-id="a4c27-231">tomorrow</span><span class="sxs-lookup"><span data-stu-id="a4c27-231">tomorrow</span></span>
- <span data-ttu-id="a4c27-232">ontem</span><span class="sxs-lookup"><span data-stu-id="a4c27-232">yesterday</span></span>
- <span data-ttu-id="a4c27-233">esta semana</span><span class="sxs-lookup"><span data-stu-id="a4c27-233">this week</span></span>    
- <span data-ttu-id="a4c27-234">A semana passada</span><span class="sxs-lookup"><span data-stu-id="a4c27-234">last week</span></span>    
- <span data-ttu-id="a4c27-235">próximo mês</span><span class="sxs-lookup"><span data-stu-id="a4c27-235">next month</span></span>    
- <span data-ttu-id="a4c27-236">mês passado</span><span class="sxs-lookup"><span data-stu-id="a4c27-236">past month</span></span>    
- <span data-ttu-id="a4c27-237">próximo ano</span><span class="sxs-lookup"><span data-stu-id="a4c27-237">coming year</span></span>
    
<span data-ttu-id="a4c27-238">Os tipos de valor de data também podem ser comparados com operadores relacionais, como maior ou menor que, ou especificados como um intervalo com o operador de intervalo **..**. Por exemplo, recebido: \> 11/30/2013, enviado: \> = ontem e recebido: 12/1/2013.. hoje são todas as cadeias de caracteres de consulta válidas.</span><span class="sxs-lookup"><span data-stu-id="a4c27-238">Date value types can also be compared with relational operators like greater than or less than, or specified as a range with the range operator **..**. For example, received:\>11/30/2013, sent:\>=yesterday, and received:12/1/2013..today are all valid query strings.</span></span> 
  
### <a name="using-a-boolean-value-type"></a><span data-ttu-id="a4c27-239">Usando um tipo de valor Boolean</span><span class="sxs-lookup"><span data-stu-id="a4c27-239">Using a Boolean value type</span></span>

<span data-ttu-id="a4c27-240">Os tipos de valor Boolean podem ser "true" ou "false".</span><span class="sxs-lookup"><span data-stu-id="a4c27-240">Boolean value types can be "true" or "false".</span></span> <span data-ttu-id="a4c27-241">Os valores não diferenciam maiúsculas de minúsculas, portanto, IsRead: false produzirá os mesmos resultados que IsRead: FALSE.</span><span class="sxs-lookup"><span data-stu-id="a4c27-241">The values are not case-sensitive, so isread:false will produce the same results as isread:FALSE.</span></span>
  
### <a name="using-a-number-value-type"></a><span data-ttu-id="a4c27-242">Usando um tipo de valor de número</span><span class="sxs-lookup"><span data-stu-id="a4c27-242">Using a number value type</span></span>

<span data-ttu-id="a4c27-243">Os tipos de valor numérico podem ser pesquisados como correspondências exatas, mas também podem ser pesquisados usando operadores relacionais, como maior ou menor que.</span><span class="sxs-lookup"><span data-stu-id="a4c27-243">Number value types can be searched as exact matches, but they can also be searched using relational operators like greater than or less than.</span></span> <span data-ttu-id="a4c27-244">Por exemplo, tamanho: 10000 retornará apenas os itens que têm um tamanho de exatamente 10000 bytes, mas tamanho: \> = 10000 retornará itens com um tamanho maior ou igual a 10000 bytes.</span><span class="sxs-lookup"><span data-stu-id="a4c27-244">For example, size:10000 will return only items that have a size of exactly 10000 bytes, but size:\>=10000 will return items that have a size greater than or equal to 10000 bytes.</span></span> <span data-ttu-id="a4c27-245">Você também pode especificar um intervalo usando o operador de intervalo ( **..**).</span><span class="sxs-lookup"><span data-stu-id="a4c27-245">You can also specify a range by using the range operator ( **..**).</span></span> <span data-ttu-id="a4c27-246">Por exemplo, tamanho: 7000.. 8000 retornará itens que têm um tamanho entre 7000 e 8000.</span><span class="sxs-lookup"><span data-stu-id="a4c27-246">For example, size:7000..8000 will return items that have a size between 7000 and 8000.</span></span> 
  
### <a name="using-logical-operators"></a><span data-ttu-id="a4c27-247">Usando operadores lógicos</span><span class="sxs-lookup"><span data-stu-id="a4c27-247">Using logical operators</span></span>

<span data-ttu-id="a4c27-248">As cadeias de caracteres de consulta dão suporte aos seguintes operadores lógicos.</span><span class="sxs-lookup"><span data-stu-id="a4c27-248">Query strings support the following logical operators.</span></span>
  
<span data-ttu-id="a4c27-249">**Tabela 2. Operadores lógicos suportados**</span><span class="sxs-lookup"><span data-stu-id="a4c27-249">**Table 2. Supported logical operators**</span></span>

|<span data-ttu-id="a4c27-250">**Operator**</span><span class="sxs-lookup"><span data-stu-id="a4c27-250">**Operator**</span></span>|<span data-ttu-id="a4c27-251">**Exemplos**</span><span class="sxs-lookup"><span data-stu-id="a4c27-251">**Examples**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a4c27-252">E</span><span class="sxs-lookup"><span data-stu-id="a4c27-252">AND</span></span>  <br/> |<span data-ttu-id="a4c27-253">Project e de: "Sadie Daniels"</span><span class="sxs-lookup"><span data-stu-id="a4c27-253">project AND from:"Sadie Daniels"</span></span>  <br/> <span data-ttu-id="a4c27-254">Assunto: (projeto e plano)</span><span class="sxs-lookup"><span data-stu-id="a4c27-254">subject:(project AND plan)</span></span>  <br/> |
|<span data-ttu-id="a4c27-255">OU</span><span class="sxs-lookup"><span data-stu-id="a4c27-255">OR</span></span>  <br/> |<span data-ttu-id="a4c27-256">Assunto: reunião ou de: "Espero bruto"</span><span class="sxs-lookup"><span data-stu-id="a4c27-256">subject:meeting OR from:"Hope Gross"</span></span>  <br/> <span data-ttu-id="a4c27-257">de:("Sadie Daniels" ou "esperança bruto")</span><span class="sxs-lookup"><span data-stu-id="a4c27-257">from:("Sadie Daniels" OR "Hope Gross")</span></span>  <br/> |
|<span data-ttu-id="a4c27-258">NÃO</span><span class="sxs-lookup"><span data-stu-id="a4c27-258">NOT</span></span>  <br/> |<span data-ttu-id="a4c27-259">Não de: "Ronnie Sturgis"</span><span class="sxs-lookup"><span data-stu-id="a4c27-259">NOT from:"Ronnie Sturgis"</span></span>  <br/> <span data-ttu-id="a4c27-260">recebido: não hoje</span><span class="sxs-lookup"><span data-stu-id="a4c27-260">received:NOT today</span></span>  <br/> |
   
<span data-ttu-id="a4c27-261">Observe que você pode usar esses operadores para participar de vários critérios juntos ou para unir vários valores em um único par de palavra-chave/valor juntos.</span><span class="sxs-lookup"><span data-stu-id="a4c27-261">Notice that you can use these operators to join multiple criteria together or to join multiple values within a single keyword/value pair together.</span></span> <span data-ttu-id="a4c27-262">No entanto, ao unir vários valores em um único par de palavra-chave/valor, você deve usar parênteses para incluir os vários valores.</span><span class="sxs-lookup"><span data-stu-id="a4c27-262">However, when joining multiple values in a single keyword/value pair, you should use parentheses to enclose the multiple values.</span></span> <span data-ttu-id="a4c27-263">Para entender por que, considere Pesquisar de: "Sadie Daniels" ou "esperança bruto".</span><span class="sxs-lookup"><span data-stu-id="a4c27-263">To understand why, consider searching with from:"Sadie Daniels" OR "Hope Gross".</span></span> <span data-ttu-id="a4c27-264">Na verdade, essa pesquisa é interpretada como o seguinte critério:</span><span class="sxs-lookup"><span data-stu-id="a4c27-264">This search actually is interpreted as the following criteria:</span></span>
  
- <span data-ttu-id="a4c27-265">O item é de Sadie Daniels ou</span><span class="sxs-lookup"><span data-stu-id="a4c27-265">The item is from Sadie Daniels, OR</span></span>
    
- <span data-ttu-id="a4c27-266">O item tem a frase "Espero bruto" em qualquer uma das propriedades indexadas.</span><span class="sxs-lookup"><span data-stu-id="a4c27-266">The item has the phrase "Hope Gross" in any of its indexed properties.</span></span>
    
<span data-ttu-id="a4c27-267">Por outro lado, de:("Sadie Daniels" ou "Espero bruto") é interpretado como:</span><span class="sxs-lookup"><span data-stu-id="a4c27-267">In contrast, from:("Sadie Daniels" OR "Hope Gross") is interpreted as:</span></span> 
  
- <span data-ttu-id="a4c27-268">O item é de Sadie Daniels ou</span><span class="sxs-lookup"><span data-stu-id="a4c27-268">The item is from Sadie Daniels, OR</span></span>
    
- <span data-ttu-id="a4c27-269">O item é de esperança bruto</span><span class="sxs-lookup"><span data-stu-id="a4c27-269">The item is from Hope Gross</span></span>
    
<span data-ttu-id="a4c27-270">O operador padrão quando vários critérios são especificados, mas nenhum operador lógico está incluído é e.</span><span class="sxs-lookup"><span data-stu-id="a4c27-270">The default operator when multiple criteria are specified but no logical operator is included is AND.</span></span> <span data-ttu-id="a4c27-271">Por exemplo, tem anexo: verdadeiro assunto: o projeto é equivalente a: Attachment: true e subject: Project.</span><span class="sxs-lookup"><span data-stu-id="a4c27-271">For example, has attachment:true subject:project is equivalent to has:attachment:true AND subject:project.</span></span>
  
## <a name="example-find-items-by-using-a-query-string-and-the-ews-managed-api"></a><span data-ttu-id="a4c27-272">Exemplo: localizar itens usando uma cadeia de caracteres de consulta e a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="a4c27-272">Example: Find items by using a query string and the EWS Managed API</span></span>
<span data-ttu-id="a4c27-273"><a name="bk_ExampleEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="a4c27-273"><a name="bk_ExampleEWSMA"> </a></span></span>

<span data-ttu-id="a4c27-274">Neste exemplo, um método chamado **SearchWithQueryString** é definido.</span><span class="sxs-lookup"><span data-stu-id="a4c27-274">In this example, a method called **SearchWithQueryString** is defined.</span></span> <span data-ttu-id="a4c27-275">Ele usa um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , um objeto [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) e um objeto **String** que representa a cadeia de caracteres de consulta como parâmetros.</span><span class="sxs-lookup"><span data-stu-id="a4c27-275">It takes an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, a [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) object, and a **string** object that represents the query string as parameters.</span></span> <span data-ttu-id="a4c27-276">Este exemplo pressupõe que o objeto **ExchangeService** tenha sido inicializado com valores válidos nas propriedades de [credenciais](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) e [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="a4c27-276">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void SearchWithQueryString(ExchangeService service, WellKnownFolderName folder, string queryString)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       ItemSchema.Size,
                                       ItemSchema.Importance,
                                       EmailMessageSchema.IsRead);
    // Item searches do not support Deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Sorting
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        // Execute the search based on the query string.
        // Example: "subject:project plan"
        FindItemsResults<Item> results = service.FindItems(folder, queryString, view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Received: {0}", item.DateTimeReceived.ToString());
            Console.WriteLine("Size: {0}", item.Size.ToString());
            Console.WriteLine("Importance: {0}", item.Importance.ToString());
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

<span data-ttu-id="a4c27-277">Você pode usar esse método para pesquisar todos os itens com a frase "plano de projeto" no assunto, conforme mostrado neste exemplo.</span><span class="sxs-lookup"><span data-stu-id="a4c27-277">You can use this method to search for all items with the phrase "project plan" in the subject, as shown in this example.</span></span>
  
```cs
string queryString = "subject:\"project plan\"";
SearchWithQueryString(service, WellKnownFolderName.Inbox, queryString);
```

## <a name="example-find-items-by-using-a-query-string-and-ews"></a><span data-ttu-id="a4c27-278">Exemplo: localizar itens usando uma cadeia de caracteres de consulta e EWS</span><span class="sxs-lookup"><span data-stu-id="a4c27-278">Example: Find items by using a query string and EWS</span></span>
<span data-ttu-id="a4c27-279"><a name="bk_ExampleEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="a4c27-279"><a name="bk_ExampleEWS"> </a></span></span>

<span data-ttu-id="a4c27-280">Neste exemplo, uma solicitação SOAP [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) localiza todos os itens na caixa de entrada com a frase "plano do projeto" no assunto.</span><span class="sxs-lookup"><span data-stu-id="a4c27-280">In this example, a SOAP [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) request finds all items in the Inbox with the phrase "project plan" in the subject.</span></span> 
  
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
          <t:FieldURI FieldURI="item:Size" />
          <t:FieldURI FieldURI="item:Importance" />
          <t:FieldURI FieldURI="message:IsRead" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
      <m:QueryString>subject:"project plan"</m:QueryString>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="a4c27-281">O exemplo a seguir mostra a resposta do servidor com os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a4c27-281">The following example shows the response from the server with the search results.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>project plan</t:Subject>
                <t:DateTimeReceived>2013-12-11T15:42:02Z</t:DateTimeReceived>
                <t:Size>7406</t:Size>
                <t:Importance>Normal</t:Importance>
                <t:IsRead>false</t:IsRead>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="a4c27-282">Confira também</span><span class="sxs-lookup"><span data-stu-id="a4c27-282">See also</span></span>

- [<span data-ttu-id="a4c27-283">Pesquisar e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a4c27-283">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)    
- [<span data-ttu-id="a4c27-284">Usar filtros de pesquisa com o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a4c27-284">Use search filters with EWS in Exchange</span></span>](how-to-use-search-filters-with-ews-in-exchange.md)    
- [<span data-ttu-id="a4c27-285">ExchangeService. FindItems</span><span class="sxs-lookup"><span data-stu-id="a4c27-285">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="a4c27-286">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="a4c27-286">FindItem operation</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

