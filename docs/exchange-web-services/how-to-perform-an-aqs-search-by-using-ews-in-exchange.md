---
title: Executar uma pesquisa AQS, usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c136901a-313e-4adf-a223-1d090d16917a
description: Descubra como pesquisar com cadeias de caracteres de consulta e AQS na sua API gerenciada de EWS ou aplicativos do EWS.
ms.openlocfilehash: dc859e24fa80cd5627477182979c9cc9527818d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750823"
---
# <a name="perform-an-aqs-search-by-using-ews-in-exchange"></a><span data-ttu-id="8a41e-103">Executar uma pesquisa AQS, usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8a41e-103">Perform an AQS search by using EWS in Exchange</span></span>

<span data-ttu-id="8a41e-104">Descubra como pesquisar com cadeias de caracteres de consulta e AQS na sua API gerenciada de EWS ou aplicativos do EWS.</span><span class="sxs-lookup"><span data-stu-id="8a41e-104">Find out how to search with query strings and AQS in your EWS Managed API or EWS application.</span></span>
  
<span data-ttu-id="8a41e-105">Cadeias de caracteres de consulta fornecem uma alternativa para [filtros de pesquisa](how-to-use-search-filters-with-ews-in-exchange.md) para expressar critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="8a41e-105">Query strings provide an alternative to [search filters](how-to-use-search-filters-with-ews-in-exchange.md) for expressing search criteria.</span></span> <span data-ttu-id="8a41e-106">A maior vantagem ao uso de cadeias de caracteres de consulta é que não são necessários para especificar uma única propriedade a ser pesquisado.</span><span class="sxs-lookup"><span data-stu-id="8a41e-106">The biggest advantage to using query strings is that you are not required to specify a single property to search.</span></span> <span data-ttu-id="8a41e-107">Você pode simplesmente fornecer um valor e a pesquisa se aplicará a todos os campos comumente usados nos itens.</span><span class="sxs-lookup"><span data-stu-id="8a41e-107">You can just provide a value, and the search will apply to all commonly used fields on the items.</span></span> <span data-ttu-id="8a41e-108">Você também pode refinar sua pesquisa usando a sintaxe de consulta avançada (AQS) em vez de um valor simple.</span><span class="sxs-lookup"><span data-stu-id="8a41e-108">You can also refine your search by using Advanced Query Syntax (AQS) instead of a simple value.</span></span> <span data-ttu-id="8a41e-109">No entanto, as cadeias de caracteres de consulta têm as seguintes limitações que você deve estar ciente antes de adicioná-los à sua caixa de ferramentas:</span><span class="sxs-lookup"><span data-stu-id="8a41e-109">However, query strings have the following limitations that you should be aware of before you add them to your toolbox:</span></span> 
  
- <span data-ttu-id="8a41e-110">**Capacidade limitada de propriedades específicas de pesquisa.**</span><span class="sxs-lookup"><span data-stu-id="8a41e-110">**Limited ability to search specific properties.**</span></span> <span data-ttu-id="8a41e-111">Quando você pesquisa com um valor simple em uma cadeia de caracteres de consulta, a pesquisa é executada em relação a todas as propriedades indexadas.</span><span class="sxs-lookup"><span data-stu-id="8a41e-111">When you search with a simple value in a query string, the search is performed against all indexed properties.</span></span> <span data-ttu-id="8a41e-112">Você pode refinar a pesquisa às propriedades específicas, mas as propriedades disponíveis para serem usados em uma cadeia de caracteres AQS são limitadas.</span><span class="sxs-lookup"><span data-stu-id="8a41e-112">You can refine your search to specific properties, but the properties available to use in an AQS string are limited.</span></span> <span data-ttu-id="8a41e-113">Se a propriedade que você deseja pesquisar não for uma das propriedades disponíveis para AQS, considere o uso de um filtro de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="8a41e-113">If the property you want to search isn't one of the properties that are available for AQS, consider using a search filter.</span></span> 
    
- <span data-ttu-id="8a41e-114">**Propriedades personalizadas não são pesquisadas.**</span><span class="sxs-lookup"><span data-stu-id="8a41e-114">**Custom properties aren't searched.**</span></span> <span data-ttu-id="8a41e-115">As pesquisas de cadeia de caracteres de consulta são executadas em relação a um índice e propriedades personalizadas não são incluídas no índice.</span><span class="sxs-lookup"><span data-stu-id="8a41e-115">Query string searches are performed against an index, and custom properties are not included in that index.</span></span> <span data-ttu-id="8a41e-116">Se você precisar propriedades personalizadas de pesquisa, use um filtro de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="8a41e-116">If you need to search custom properties, use a search filter instead.</span></span> 
    
- <span data-ttu-id="8a41e-117">**Controle limitado cadeia de caracteres de pesquisa.**</span><span class="sxs-lookup"><span data-stu-id="8a41e-117">**Limited control for string searches.**</span></span> <span data-ttu-id="8a41e-118">As pesquisas de cadeia de caracteres de consulta sempre Ignorar maiusculas e minúsculas e são sempre pesquisas de subsequência.</span><span class="sxs-lookup"><span data-stu-id="8a41e-118">Query string searches always ignore case, and are always substring searches.</span></span> <span data-ttu-id="8a41e-119">Se você deseja fazer diferencia maiusculas de minúsculas, o prefixo ou pesquisas de correspondência exata, usam um filtro de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="8a41e-119">If you want to do case-sensitive, prefix, or exact match searches, use a search filter.</span></span> 
    
- <span data-ttu-id="8a41e-120">**Não disponível para pastas ou pastas de pesquisa.**</span><span class="sxs-lookup"><span data-stu-id="8a41e-120">**Not available for folders or search folders.**</span></span> <span data-ttu-id="8a41e-121">As operações de EWS para a procura de pastas não suportam o uso uma cadeia de caracteres de consulta.</span><span class="sxs-lookup"><span data-stu-id="8a41e-121">The EWS operations for searching for folders don't support using a query string.</span></span> <span data-ttu-id="8a41e-122">Além disso, as pastas de pesquisa não oferecem suporte a cadeias de caracteres de consulta.</span><span class="sxs-lookup"><span data-stu-id="8a41e-122">Additionally, search folders don't support query strings.</span></span> <span data-ttu-id="8a41e-123">Em ambos os casos, um filtro de pesquisa é a única opção.</span><span class="sxs-lookup"><span data-stu-id="8a41e-123">In both cases, a search filter is your only option.</span></span> 
    
## <a name="creating-a-query-string"></a><span data-ttu-id="8a41e-124">Criando uma cadeia de caracteres de consulta</span><span class="sxs-lookup"><span data-stu-id="8a41e-124">Creating a query string</span></span>
<span data-ttu-id="8a41e-125"><a name="bk_CreateQueryString"> </a></span><span class="sxs-lookup"><span data-stu-id="8a41e-125"></span></span>

<span data-ttu-id="8a41e-126">Cadeias de caracteres de consulta na API gerenciada de EWS e EWS são interpretadas como um subconjunto da sintaxe AQS.</span><span class="sxs-lookup"><span data-stu-id="8a41e-126">Query strings in the EWS Managed API and EWS are interpreted as a subset of AQS syntax.</span></span> <span data-ttu-id="8a41e-127">Cadeias de caracteres AQS são compostas de valores ou pares de palavra-chave/valor, separados por dois pontos (:).</span><span class="sxs-lookup"><span data-stu-id="8a41e-127">AQS strings are composed of either values or keyword/value pairs, separated by a colon (:).</span></span>
  
`keyword:value`

<span data-ttu-id="8a41e-128">Quando um valor for especificado, sem uma palavra-chave, todas as propriedades indexadas são pesquisadas para o valor.</span><span class="sxs-lookup"><span data-stu-id="8a41e-128">When a value is specified without a keyword, all indexed properties are searched for the value.</span></span> <span data-ttu-id="8a41e-129">Se uma palavra-chave é emparelhada com um valor, a palavra-chave especifica uma propriedade para procurar o valor correspondente.</span><span class="sxs-lookup"><span data-stu-id="8a41e-129">If a keyword is paired with a value, the keyword specifies a property to search for the corresponding value.</span></span>
  
<span data-ttu-id="8a41e-130">**Tabela 1. Palavras-chave AQS com suporte**</span><span class="sxs-lookup"><span data-stu-id="8a41e-130">**Table 1. Supported AQS keywords**</span></span>

|<span data-ttu-id="8a41e-131">**Palavra-chave**</span><span class="sxs-lookup"><span data-stu-id="8a41e-131">**Keyword**</span></span>|<span data-ttu-id="8a41e-132">**Value type**</span><span class="sxs-lookup"><span data-stu-id="8a41e-132">**Value type**</span></span>|<span data-ttu-id="8a41e-133">**Exemplo**</span><span class="sxs-lookup"><span data-stu-id="8a41e-133">**Example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="8a41e-134">subject</span><span class="sxs-lookup"><span data-stu-id="8a41e-134">subject</span></span>  <br/> |<span data-ttu-id="8a41e-135">String</span><span class="sxs-lookup"><span data-stu-id="8a41e-135">String</span></span>  <br/> |<span data-ttu-id="8a41e-136">Assunto: project</span><span class="sxs-lookup"><span data-stu-id="8a41e-136">subject:project</span></span>  <br/> |
|<span data-ttu-id="8a41e-137">body</span><span class="sxs-lookup"><span data-stu-id="8a41e-137">body</span></span>  <br/> |<span data-ttu-id="8a41e-138">String</span><span class="sxs-lookup"><span data-stu-id="8a41e-138">String</span></span>  <br/> |<span data-ttu-id="8a41e-139">ilustrações de sales de corpo:</span><span class="sxs-lookup"><span data-stu-id="8a41e-139">body:sales figures</span></span>  <br/> |
|<span data-ttu-id="8a41e-140">anexo</span><span class="sxs-lookup"><span data-stu-id="8a41e-140">attachment</span></span>  <br/> |<span data-ttu-id="8a41e-141">String</span><span class="sxs-lookup"><span data-stu-id="8a41e-141">String</span></span>  <br/> |<span data-ttu-id="8a41e-142">anexo: relatório</span><span class="sxs-lookup"><span data-stu-id="8a41e-142">attachment:report</span></span>  <br/> |
|<span data-ttu-id="8a41e-143">para</span><span class="sxs-lookup"><span data-stu-id="8a41e-143">to</span></span>  <br/> |<span data-ttu-id="8a41e-144">String</span><span class="sxs-lookup"><span data-stu-id="8a41e-144">String</span></span>  <br/> |<span data-ttu-id="8a41e-145">para: "Sadie Daniels"</span><span class="sxs-lookup"><span data-stu-id="8a41e-145">to:"Sadie Daniels"</span></span>  <br/> |
|<span data-ttu-id="8a41e-146">from</span><span class="sxs-lookup"><span data-stu-id="8a41e-146">from</span></span>  <br/> |<span data-ttu-id="8a41e-147">String</span><span class="sxs-lookup"><span data-stu-id="8a41e-147">String</span></span>  <br/> |<span data-ttu-id="8a41e-148">de:, esperamos</span><span class="sxs-lookup"><span data-stu-id="8a41e-148">from:hope</span></span>  <br/> |
|<span data-ttu-id="8a41e-149">cc</span><span class="sxs-lookup"><span data-stu-id="8a41e-149">cc</span></span>  <br/> |<span data-ttu-id="8a41e-150">String</span><span class="sxs-lookup"><span data-stu-id="8a41e-150">String</span></span>  <br/> |<span data-ttu-id="8a41e-151">cc: "Ronnie Sturgis"</span><span class="sxs-lookup"><span data-stu-id="8a41e-151">cc:"Ronnie Sturgis"</span></span>  <br/> |
|<span data-ttu-id="8a41e-152">bcc</span><span class="sxs-lookup"><span data-stu-id="8a41e-152">bcc</span></span>  <br/> |<span data-ttu-id="8a41e-153">String</span><span class="sxs-lookup"><span data-stu-id="8a41e-153">String</span></span>  <br/> |<span data-ttu-id="8a41e-154">BCC:mack</span><span class="sxs-lookup"><span data-stu-id="8a41e-154">bcc:mack</span></span>  <br/> |
|<span data-ttu-id="8a41e-155">participantes</span><span class="sxs-lookup"><span data-stu-id="8a41e-155">participants</span></span>  <br/> |<span data-ttu-id="8a41e-156">String</span><span class="sxs-lookup"><span data-stu-id="8a41e-156">String</span></span>  <br/> |<span data-ttu-id="8a41e-157">participantes: sadie</span><span class="sxs-lookup"><span data-stu-id="8a41e-157">participants:sadie</span></span>  <br/> |
|<span data-ttu-id="8a41e-158">Ferramentas para desenvolvedores</span><span class="sxs-lookup"><span data-stu-id="8a41e-158">category</span></span>  <br/> |<span data-ttu-id="8a41e-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a41e-159">String</span></span>  <br/> |<span data-ttu-id="8a41e-160">projeto de categoria:</span><span class="sxs-lookup"><span data-stu-id="8a41e-160">category:project</span></span>  <br/> |
|<span data-ttu-id="8a41e-161">importance</span><span class="sxs-lookup"><span data-stu-id="8a41e-161">importance</span></span>  <br/> |<span data-ttu-id="8a41e-162">String</span><span class="sxs-lookup"><span data-stu-id="8a41e-162">String</span></span>  <br/> |<span data-ttu-id="8a41e-163">importância: alta</span><span class="sxs-lookup"><span data-stu-id="8a41e-163">importance:high</span></span>  <br/> |
|<span data-ttu-id="8a41e-164">tipo</span><span class="sxs-lookup"><span data-stu-id="8a41e-164">kind</span></span>  <br/> |<span data-ttu-id="8a41e-165">Tipo de item</span><span class="sxs-lookup"><span data-stu-id="8a41e-165">Item type</span></span>  <br/> |<span data-ttu-id="8a41e-166">reuniões do tipo:</span><span class="sxs-lookup"><span data-stu-id="8a41e-166">kind:meetings</span></span>  <br/> |
|<span data-ttu-id="8a41e-167">enviado</span><span class="sxs-lookup"><span data-stu-id="8a41e-167">sent</span></span>  <br/> |<span data-ttu-id="8a41e-168">Data</span><span class="sxs-lookup"><span data-stu-id="8a41e-168">Date</span></span>  <br/> |<span data-ttu-id="8a41e-169">enviados: 12/10/2013</span><span class="sxs-lookup"><span data-stu-id="8a41e-169">sent:12/10/2013</span></span>  <br/> |
|<span data-ttu-id="8a41e-170">recebido</span><span class="sxs-lookup"><span data-stu-id="8a41e-170">received</span></span>  <br/> |<span data-ttu-id="8a41e-171">Data</span><span class="sxs-lookup"><span data-stu-id="8a41e-171">Date</span></span>  <br/> |<span data-ttu-id="8a41e-172">recebidos: ontem</span><span class="sxs-lookup"><span data-stu-id="8a41e-172">received:yesterday</span></span>  <br/> |
|<span data-ttu-id="8a41e-173">hasattachment</span><span class="sxs-lookup"><span data-stu-id="8a41e-173">hasattachment</span></span>  <br/> |<span data-ttu-id="8a41e-174">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a41e-174">Boolean</span></span>  <br/> |<span data-ttu-id="8a41e-175">Tem anexo: true</span><span class="sxs-lookup"><span data-stu-id="8a41e-175">Has attachment:true</span></span>  <br/> |
|<span data-ttu-id="8a41e-176">está sinalizado</span><span class="sxs-lookup"><span data-stu-id="8a41e-176">isflagged</span></span>  <br/> |<span data-ttu-id="8a41e-177">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a41e-177">Boolean</span></span>  <br/> |<span data-ttu-id="8a41e-178">isflagged:True</span><span class="sxs-lookup"><span data-stu-id="8a41e-178">isflagged:true</span></span>  <br/> |
|<span data-ttu-id="8a41e-179">foi lido</span><span class="sxs-lookup"><span data-stu-id="8a41e-179">isread</span></span>  <br/> |<span data-ttu-id="8a41e-180">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a41e-180">Boolean</span></span>  <br/> |<span data-ttu-id="8a41e-181">isread:False</span><span class="sxs-lookup"><span data-stu-id="8a41e-181">isread:false</span></span>  <br/> |
|<span data-ttu-id="8a41e-182">size</span><span class="sxs-lookup"><span data-stu-id="8a41e-182">size</span></span>  <br/> |<span data-ttu-id="8a41e-183">Número</span><span class="sxs-lookup"><span data-stu-id="8a41e-183">Number</span></span>  <br/> |<span data-ttu-id="8a41e-184">Tamanho:\>5000</span><span class="sxs-lookup"><span data-stu-id="8a41e-184">size:\>5000</span></span>  <br/> |
   
<span data-ttu-id="8a41e-185">Vamos dar uma olhada em como os tipos de valores diferentes funcionam.</span><span class="sxs-lookup"><span data-stu-id="8a41e-185">Let's take a look at how the different value types work.</span></span>
  
### <a name="using-a-string-value-type"></a><span data-ttu-id="8a41e-186">Usando um tipo de valor de cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a41e-186">Using a string value type</span></span>

<span data-ttu-id="8a41e-187">Tipos de valores de cadeia de caracteres são por padrão pesquisada como pesquisas de subcadeia de caracteres de prefixo que não diferenciam maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="8a41e-187">String value types are by default searched as prefix substring searches that are not case-sensitive.</span></span> <span data-ttu-id="8a41e-188">Isso significa que procurando por assunto: project encontraria como correspondente qualquer um dos seguintes assuntos:</span><span class="sxs-lookup"><span data-stu-id="8a41e-188">That means that searching for subject:project would match any of the following subjects:</span></span> 
  
- <span data-ttu-id="8a41e-189">Notas de reunião de projeto</span><span class="sxs-lookup"><span data-stu-id="8a41e-189">Project meeting notes</span></span>
    
- <span data-ttu-id="8a41e-190">Você tem os planos de projeto?</span><span class="sxs-lookup"><span data-stu-id="8a41e-190">Do you have the project plans?</span></span>
    
- <span data-ttu-id="8a41e-191">Projeções de vendas de dezembro</span><span class="sxs-lookup"><span data-stu-id="8a41e-191">December sales projections</span></span>
    
<span data-ttu-id="8a41e-192">Você pode alterar a pesquisa para exigir a palavra inteira em vez de prefixos correspondentes colocando-se a cadeia de caracteres entre aspas.</span><span class="sxs-lookup"><span data-stu-id="8a41e-192">You can change the search to require the whole word rather than matching prefixes by enclosing the string in quotation marks.</span></span> <span data-ttu-id="8a41e-193">Procurando por assunto: "projeto" seria eliminar o valor de "Projeções de vendas de dezembro" da lista de correspondências.</span><span class="sxs-lookup"><span data-stu-id="8a41e-193">Searching for subject:"project" would eliminate the "December sales projections" value from the list of matches.</span></span> <span data-ttu-id="8a41e-194">Observe que o valor é ainda não diferencia maiusculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="8a41e-194">Note that the value is still not case-sensitive.</span></span> 
  
<span data-ttu-id="8a41e-195">Se você usar várias palavras em uma cadeia de caracteres de consulta, uma correspondência requer que ambas as palavras aparecem nos campos pesquisados.</span><span class="sxs-lookup"><span data-stu-id="8a41e-195">If you use multiple words in a query string, a match requires that both words appear in the searched fields.</span></span> <span data-ttu-id="8a41e-196">Por exemplo, procurando o plano de projeto de assunto: encontraria como correspondente qualquer um dos seguintes assuntos:</span><span class="sxs-lookup"><span data-stu-id="8a41e-196">For example, searching for subject:project plan would match any of the following subjects:</span></span> 
  
- <span data-ttu-id="8a41e-197">Plano de projeto</span><span class="sxs-lookup"><span data-stu-id="8a41e-197">Project plan</span></span>
    
- <span data-ttu-id="8a41e-198">Você tem os planos de projeto?</span><span class="sxs-lookup"><span data-stu-id="8a41e-198">Do you have the project plans?</span></span>
    
- <span data-ttu-id="8a41e-199">Oriente-me o plano para nosso projeto</span><span class="sxs-lookup"><span data-stu-id="8a41e-199">Please send me the plan for our project</span></span>
    
- <span data-ttu-id="8a41e-200">Planejando as etapas do projeto</span><span class="sxs-lookup"><span data-stu-id="8a41e-200">Planning project milestones</span></span>
    
<span data-ttu-id="8a41e-201">Se você colocar várias palavras entre aspas, eles são tratados como uma única frase.</span><span class="sxs-lookup"><span data-stu-id="8a41e-201">If you enclose multiple words in quotation marks, they are treated as a single phrase.</span></span> <span data-ttu-id="8a41e-202">Procurando por assunto: "plano de projeto" encontraria como correspondente apenas o assunto "Plano de projeto" da lista anterior.</span><span class="sxs-lookup"><span data-stu-id="8a41e-202">Searching for subject:"project plan" would only match the "Project plan" subject from the previous list.</span></span> 
  
### <a name="using-an-item-type-value-type"></a><span data-ttu-id="8a41e-203">Usando um tipo de valor de tipo de item</span><span class="sxs-lookup"><span data-stu-id="8a41e-203">Using an item type value type</span></span>

<span data-ttu-id="8a41e-204">Você pode usar os seguintes valores de tipo de item com a palavra-chave de **tipo** para limitar os resultados de pesquisa a apenas um tipo específico de item, como email ou solicitações de reunião:</span><span class="sxs-lookup"><span data-stu-id="8a41e-204">You can use the following item type values with the **kind** keyword to limit your search results to only a specific type of item, such as email or meeting requests:</span></span> 
  
- <span data-ttu-id="8a41e-205">contatos</span><span class="sxs-lookup"><span data-stu-id="8a41e-205">contacts</span></span>    
- <span data-ttu-id="8a41e-206">documentos</span><span class="sxs-lookup"><span data-stu-id="8a41e-206">docs</span></span>    
- <span data-ttu-id="8a41e-207">email</span><span class="sxs-lookup"><span data-stu-id="8a41e-207">email</span></span>    
- <span data-ttu-id="8a41e-208">aparelhos de fax</span><span class="sxs-lookup"><span data-stu-id="8a41e-208">faxes</span></span>    
- <span data-ttu-id="8a41e-209">IM (corresponde a mensagens instantâneas)</span><span class="sxs-lookup"><span data-stu-id="8a41e-209">im (corresponds to instant messages)</span></span>    
- <span data-ttu-id="8a41e-210">diários</span><span class="sxs-lookup"><span data-stu-id="8a41e-210">journals</span></span>    
- <span data-ttu-id="8a41e-211">reuniões (corresponde à compromissos e solicitações de reunião)</span><span class="sxs-lookup"><span data-stu-id="8a41e-211">meetings (corresponds to appointments and meeting requests)</span></span>    
- <span data-ttu-id="8a41e-212">Observações</span><span class="sxs-lookup"><span data-stu-id="8a41e-212">notes</span></span>    
- <span data-ttu-id="8a41e-213">postagens</span><span class="sxs-lookup"><span data-stu-id="8a41e-213">posts</span></span>    
- <span data-ttu-id="8a41e-214">rssfeeds</span><span class="sxs-lookup"><span data-stu-id="8a41e-214">rssfeeds</span></span>    
- <span data-ttu-id="8a41e-215">tarefas</span><span class="sxs-lookup"><span data-stu-id="8a41e-215">tasks</span></span>    
- <span data-ttu-id="8a41e-216">caixa postal</span><span class="sxs-lookup"><span data-stu-id="8a41e-216">voicemail</span></span>
    
### <a name="using-a-date-value-type"></a><span data-ttu-id="8a41e-217">Usando um tipo de valor de data</span><span class="sxs-lookup"><span data-stu-id="8a41e-217">Using a date value type</span></span>

<span data-ttu-id="8a41e-218">Você pode pesquisar os tipos de valores de data em um número de formas diferentes.</span><span class="sxs-lookup"><span data-stu-id="8a41e-218">You can search date value types in a number of different ways.</span></span> <span data-ttu-id="8a41e-219">É o mais simples para procurar uma data específica.</span><span class="sxs-lookup"><span data-stu-id="8a41e-219">The simplest is to search for a specific date.</span></span> <span data-ttu-id="8a41e-220">Pesquisando com recebidos: 12/11/2013 retornará todos os itens recebidos em 11 de dezembro de 2013.</span><span class="sxs-lookup"><span data-stu-id="8a41e-220">Searching with received:12/11/2013 will return all items received on December 11, 2013.</span></span> <span data-ttu-id="8a41e-221">No entanto, você também pode ser menos específico.</span><span class="sxs-lookup"><span data-stu-id="8a41e-221">However, you can also be less specific.</span></span> <span data-ttu-id="8a41e-222">Pesquisando com recebidos: 12/11 retornará todos os itens recebidos em 11 de dezembro do ano atual.</span><span class="sxs-lookup"><span data-stu-id="8a41e-222">Searching with received:12/11 will return all items received on December 11 of the current year.</span></span> 
  
<span data-ttu-id="8a41e-223">Outra opção é usar os nomes dos meses.</span><span class="sxs-lookup"><span data-stu-id="8a41e-223">Another option is to use the month names.</span></span> <span data-ttu-id="8a41e-224">Você pode pesquisar com recebidos: 11 de dezembro de 2013 ou em 11 de dezembro para obter os mesmos resultados como recebido: 12/11/2013 e recebidos: 12/11, respectivamente.</span><span class="sxs-lookup"><span data-stu-id="8a41e-224">You can search with received:December 11, 2013 or December 11 to get the same results as received:12/11/2013 and received:12/11, respectively.</span></span> <span data-ttu-id="8a41e-225">Você também pode pesquisar com recebidos: dezembro para obter todos os itens recebidos no mês de dezembro, no ano atual.</span><span class="sxs-lookup"><span data-stu-id="8a41e-225">You can also search with received:December to get all items received in the month of December, in the current year.</span></span> 
  
<span data-ttu-id="8a41e-226">Também é uma opção usando os nomes dos dias da semana.</span><span class="sxs-lookup"><span data-stu-id="8a41e-226">Using the names of the days of the week is also an option.</span></span> <span data-ttu-id="8a41e-227">Pesquisando com recebidos: terça-feira retornará todos os itens recebidos na terça-feira da semana atual.</span><span class="sxs-lookup"><span data-stu-id="8a41e-227">Searching with received:Tuesday will return all items received on Tuesday of the current week.</span></span> 
  
<span data-ttu-id="8a41e-228">Tipos de valores de data também suportam um conjunto de palavras-chave para pesquisas em relação a hora atual.</span><span class="sxs-lookup"><span data-stu-id="8a41e-228">Date value types also support a set of keywords for searches relative to the current time.</span></span> <span data-ttu-id="8a41e-229">Há suporte para as seguintes palavras-chave:</span><span class="sxs-lookup"><span data-stu-id="8a41e-229">The following keywords are supported:</span></span>
  
- <span data-ttu-id="8a41e-230">hoje</span><span class="sxs-lookup"><span data-stu-id="8a41e-230">today</span></span>  
- <span data-ttu-id="8a41e-231">tomorrow</span><span class="sxs-lookup"><span data-stu-id="8a41e-231">tomorrow</span></span>
- <span data-ttu-id="8a41e-232">ontem</span><span class="sxs-lookup"><span data-stu-id="8a41e-232">yesterday</span></span>
- <span data-ttu-id="8a41e-233">esta semana</span><span class="sxs-lookup"><span data-stu-id="8a41e-233">this week</span></span>    
- <span data-ttu-id="8a41e-234">A semana passada</span><span class="sxs-lookup"><span data-stu-id="8a41e-234">last week</span></span>    
- <span data-ttu-id="8a41e-235">próximo mês</span><span class="sxs-lookup"><span data-stu-id="8a41e-235">next month</span></span>    
- <span data-ttu-id="8a41e-236">mês passado</span><span class="sxs-lookup"><span data-stu-id="8a41e-236">past month</span></span>    
- <span data-ttu-id="8a41e-237">próximo ano</span><span class="sxs-lookup"><span data-stu-id="8a41e-237">coming year</span></span>
    
<span data-ttu-id="8a41e-238">Tipos de valores de data também podem ser comparados com os operadores relacionais como maior ou menor que, ou especificado como um intervalo com o operador de intervalo **.**. Por exemplo, recebido:\>30/11/2013, enviados:\>= ontem, e received:12/1/2013..today são todas as cadeias de caracteres de consulta válido.</span><span class="sxs-lookup"><span data-stu-id="8a41e-238">Date value types can also be compared with relational operators like greater than or less than, or specified as a range with the range operator **..**. For example, received:\>11/30/2013, sent:\>=yesterday, and received:12/1/2013..today are all valid query strings.</span></span> 
  
### <a name="using-a-boolean-value-type"></a><span data-ttu-id="8a41e-239">Usando um tipo de valor booleano</span><span class="sxs-lookup"><span data-stu-id="8a41e-239">Using a Boolean value type</span></span>

<span data-ttu-id="8a41e-240">Tipos de valor booleano podem ser "verdadeiro" ou "falso".</span><span class="sxs-lookup"><span data-stu-id="8a41e-240">Boolean value types can be "true" or "false".</span></span> <span data-ttu-id="8a41e-241">Os valores não diferenciam maiusculas de minúsculas, portanto isread:false produzirá os mesmos resultados que isread:FALSE.</span><span class="sxs-lookup"><span data-stu-id="8a41e-241">The values are not case-sensitive, so isread:false will produce the same results as isread:FALSE.</span></span>
  
### <a name="using-a-number-value-type"></a><span data-ttu-id="8a41e-242">Usando um tipo de valor de número</span><span class="sxs-lookup"><span data-stu-id="8a41e-242">Using a number value type</span></span>

<span data-ttu-id="8a41e-243">Tipos de valor de número podem ser pesquisados como correspondências exatas, mas eles também podem ser pesquisados usando operadores relacionais como maior ou menor que.</span><span class="sxs-lookup"><span data-stu-id="8a41e-243">Number value types can be searched as exact matches, but they can also be searched using relational operators like greater than or less than.</span></span> <span data-ttu-id="8a41e-244">Por exemplo, tamanho: 10000 retornará apenas os itens que tenham um tamanho de exatamente 10000 bytes, mas tamanho:\>= 10000 retornará os itens que tenham um tamanho maior ou igual a 10000 bytes.</span><span class="sxs-lookup"><span data-stu-id="8a41e-244">For example, size:10000 will return only items that have a size of exactly 10000 bytes, but size:\>=10000 will return items that have a size greater than or equal to 10000 bytes.</span></span> <span data-ttu-id="8a41e-245">Você também pode especificar um intervalo usando o operador de intervalo ( **.**).</span><span class="sxs-lookup"><span data-stu-id="8a41e-245">You can also specify a range by using the range operator ( **..**).</span></span> <span data-ttu-id="8a41e-246">Por exemplo, tamanho: 7000..8000 retornará os itens que tenham um tamanho entre 7000 e 8000.</span><span class="sxs-lookup"><span data-stu-id="8a41e-246">For example, size:7000..8000 will return items that have a size between 7000 and 8000.</span></span> 
  
### <a name="using-logical-operators"></a><span data-ttu-id="8a41e-247">Usando operadores lógicos</span><span class="sxs-lookup"><span data-stu-id="8a41e-247">Using logical operators</span></span>

<span data-ttu-id="8a41e-248">Cadeias de caracteres de consulta suportam os seguintes operadores lógicos.</span><span class="sxs-lookup"><span data-stu-id="8a41e-248">Query strings support the following logical operators.</span></span>
  
<span data-ttu-id="8a41e-249">**Tabela 2. Suporte para os operadores lógicos**</span><span class="sxs-lookup"><span data-stu-id="8a41e-249">**Table 2. Supported logical operators**</span></span>

|<span data-ttu-id="8a41e-250">**Operador**</span><span class="sxs-lookup"><span data-stu-id="8a41e-250">**Operator**</span></span>|<span data-ttu-id="8a41e-251">**Exemplos**</span><span class="sxs-lookup"><span data-stu-id="8a41e-251">**Examples**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8a41e-252">E</span><span class="sxs-lookup"><span data-stu-id="8a41e-252">AND</span></span>  <br/> |<span data-ttu-id="8a41e-253">projeto e de: "Sadie Daniels"</span><span class="sxs-lookup"><span data-stu-id="8a41e-253">project AND from:"Sadie Daniels"</span></span>  <br/> <span data-ttu-id="8a41e-254">Assunto:(project AND plan)</span><span class="sxs-lookup"><span data-stu-id="8a41e-254">subject:(project AND plan)</span></span>  <br/> |
|<span data-ttu-id="8a41e-255">OU</span><span class="sxs-lookup"><span data-stu-id="8a41e-255">OR</span></span>  <br/> |<span data-ttu-id="8a41e-256">Assunto: reunião ou de: "Espero bruta"</span><span class="sxs-lookup"><span data-stu-id="8a41e-256">subject:meeting OR from:"Hope Gross"</span></span>  <br/> <span data-ttu-id="8a41e-257">de: ("Sadie Daniels" ou "Valor bruto, esperamos")</span><span class="sxs-lookup"><span data-stu-id="8a41e-257">from:("Sadie Daniels" OR "Hope Gross")</span></span>  <br/> |
|<span data-ttu-id="8a41e-258">NÃO</span><span class="sxs-lookup"><span data-stu-id="8a41e-258">NOT</span></span>  <br/> |<span data-ttu-id="8a41e-259">NÃO de: "Ronnie Sturgis"</span><span class="sxs-lookup"><span data-stu-id="8a41e-259">NOT from:"Ronnie Sturgis"</span></span>  <br/> <span data-ttu-id="8a41e-260">recebidos: não hoje</span><span class="sxs-lookup"><span data-stu-id="8a41e-260">received:NOT today</span></span>  <br/> |
   
<span data-ttu-id="8a41e-261">Observe que você pode usar esses operadores para unir vários critérios ou unir vários valores dentro de um par de palavra-chave/valor único.</span><span class="sxs-lookup"><span data-stu-id="8a41e-261">Notice that you can use these operators to join multiple criteria together or to join multiple values within a single keyword/value pair together.</span></span> <span data-ttu-id="8a41e-262">No entanto, ao unir vários valores em um par de palavra-chave/valor único, você deve usar parênteses para delimitar vários valores.</span><span class="sxs-lookup"><span data-stu-id="8a41e-262">However, when joining multiple values in a single keyword/value pair, you should use parentheses to enclose the multiple values.</span></span> <span data-ttu-id="8a41e-263">Para entender o porquê, considere a pesquisa com a partir de: "Sadie Daniels" ou "Espero bruto".</span><span class="sxs-lookup"><span data-stu-id="8a41e-263">To understand why, consider searching with from:"Sadie Daniels" OR "Hope Gross".</span></span> <span data-ttu-id="8a41e-264">Na verdade, essa pesquisa será interpretada como os seguintes critérios:</span><span class="sxs-lookup"><span data-stu-id="8a41e-264">This search actually is interpreted as the following criteria:</span></span>
  
- <span data-ttu-id="8a41e-265">O item é de Sadie Daniels, OR</span><span class="sxs-lookup"><span data-stu-id="8a41e-265">The item is from Sadie Daniels, OR</span></span>
    
- <span data-ttu-id="8a41e-266">O item tem a frase "Espero bruta" em qualquer uma das suas propriedades indexadas.</span><span class="sxs-lookup"><span data-stu-id="8a41e-266">The item has the phrase "Hope Gross" in any of its indexed properties.</span></span>
    
<span data-ttu-id="8a41e-267">Por outro lado, a partir: ("Sadie Daniels" ou "Espero bruta") será interpretada como:</span><span class="sxs-lookup"><span data-stu-id="8a41e-267">In contrast, from:("Sadie Daniels" OR "Hope Gross") is interpreted as:</span></span> 
  
- <span data-ttu-id="8a41e-268">O item é de Sadie Daniels, OR</span><span class="sxs-lookup"><span data-stu-id="8a41e-268">The item is from Sadie Daniels, OR</span></span>
    
- <span data-ttu-id="8a41e-269">O item é de espero bruta</span><span class="sxs-lookup"><span data-stu-id="8a41e-269">The item is from Hope Gross</span></span>
    
<span data-ttu-id="8a41e-270">O operador padrão quando vários critérios são especificados, mas nenhum operador lógico é incluído é and.</span><span class="sxs-lookup"><span data-stu-id="8a41e-270">The default operator when multiple criteria are specified but no logical operator is included is AND.</span></span> <span data-ttu-id="8a41e-271">Por exemplo, tem anexo: true assunto: project é equivalente à tem: anexo: true e assunto: project.</span><span class="sxs-lookup"><span data-stu-id="8a41e-271">For example, has attachment:true subject:project is equivalent to has:attachment:true AND subject:project.</span></span>
  
## <a name="example-find-items-by-using-a-query-string-and-the-ews-managed-api"></a><span data-ttu-id="8a41e-272">Exemplo: Localizar itens usando uma cadeia de caracteres de consulta e a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="8a41e-272">Example: Find items by using a query string and the EWS Managed API</span></span>
<span data-ttu-id="8a41e-273"><a name="bk_ExampleEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="8a41e-273"></span></span>

<span data-ttu-id="8a41e-274">Neste exemplo, um método chamado **SearchWithQueryString** é definido.</span><span class="sxs-lookup"><span data-stu-id="8a41e-274">In this example, a method called **SearchWithQueryString** is defined.</span></span> <span data-ttu-id="8a41e-275">Que leva a um objeto [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , um objeto [WellKnownFolderName](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) e um objeto de **cadeia de caracteres** que representa a cadeia de caracteres de consulta como parâmetros.</span><span class="sxs-lookup"><span data-stu-id="8a41e-275">It takes an [ExchangeService](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, a [WellKnownFolderName](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) object, and a **string** object that represents the query string as parameters.</span></span> <span data-ttu-id="8a41e-276">Este exemplo pressupõe que o objeto **ExchangeService** foi inicializado com valores válidos nas propriedades [credenciais](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) e [Url](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8a41e-276">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
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

<span data-ttu-id="8a41e-277">Você pode usar esse método para procurar todos os itens com a frase "plano de projeto" no assunto, conforme mostrado neste exemplo.</span><span class="sxs-lookup"><span data-stu-id="8a41e-277">You can use this method to search for all items with the phrase "project plan" in the subject, as shown in this example.</span></span>
  
```cs
string queryString = "subject:\"project plan\"";
SearchWithQueryString(service, WellKnownFolderName.Inbox, queryString);
```

## <a name="example-find-items-by-using-a-query-string-and-ews"></a><span data-ttu-id="8a41e-278">Exemplo: Localizar itens usando uma cadeia de caracteres de consulta e o EWS</span><span class="sxs-lookup"><span data-stu-id="8a41e-278">Example: Find items by using a query string and EWS</span></span>
<span data-ttu-id="8a41e-279"><a name="bk_ExampleEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="8a41e-279"></span></span>

<span data-ttu-id="8a41e-280">Neste exemplo, uma solicitação SOAP [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) localiza todos os itens na caixa de entrada com a frase "plano de projeto" no assunto.</span><span class="sxs-lookup"><span data-stu-id="8a41e-280">In this example, a SOAP [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) request finds all items in the Inbox with the phrase "project plan" in the subject.</span></span> 
  
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

<span data-ttu-id="8a41e-281">O exemplo a seguir mostra a resposta do servidor com os resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="8a41e-281">The following example shows the response from the server with the search results.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="see-also"></a><span data-ttu-id="8a41e-282">Confira também</span><span class="sxs-lookup"><span data-stu-id="8a41e-282">See also</span></span>

- [<span data-ttu-id="8a41e-283">Pesquisa e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8a41e-283">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)    
- [<span data-ttu-id="8a41e-284">Use os filtros de pesquisa com o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8a41e-284">Use search filters with EWS in Exchange</span></span>](how-to-use-search-filters-with-ews-in-exchange.md)    
- [<span data-ttu-id="8a41e-285">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="8a41e-285">ExchangeService.FindItems</span></span>](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="8a41e-286">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="8a41e-286">FindItem operation</span></span>](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

