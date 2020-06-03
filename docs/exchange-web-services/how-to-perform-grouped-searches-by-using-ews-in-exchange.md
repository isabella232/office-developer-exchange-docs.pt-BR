---
title: Executar pesquisas agrupadas usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 55de92eb-8e8b-4156-8ad9-dd3828024242
description: Descubra como realizar pesquisas agrupadas na API gerenciada do EWS ou no aplicativo EWS que direciona o Exchange.
ms.openlocfilehash: 65c6f75ea6b8ab848a263349dcceceead52fa210
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527908"
---
# <a name="perform-grouped-searches-by-using-ews-in-exchange"></a><span data-ttu-id="10292-103">Executar pesquisas agrupadas usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="10292-103">Perform grouped searches by using EWS in Exchange</span></span>

<span data-ttu-id="10292-104">Descubra como realizar pesquisas agrupadas na API gerenciada do EWS ou no aplicativo EWS que direciona o Exchange.</span><span class="sxs-lookup"><span data-stu-id="10292-104">Find out how to perform grouped searches in your EWS Managed API or EWS application that targets Exchange.</span></span>
  
<span data-ttu-id="10292-105">As pesquisas agrupadas são úteis, pois dão controle sobre como os resultados da pesquisa são organizados.</span><span class="sxs-lookup"><span data-stu-id="10292-105">Grouped searches are useful in that they gives you control over how search results are organized.</span></span> <span data-ttu-id="10292-106">Os resultados de pesquisa organizados podem tornar mais fácil para o aplicativo processar os resultados ou exibi-los para um usuário final de uma maneira gerenciável.</span><span class="sxs-lookup"><span data-stu-id="10292-106">Organized search results can make it easier for your application to process results or display them to an end user in a manageable way.</span></span>
  
<span data-ttu-id="10292-107">O agrupamento funciona colocando todos os itens dentro do conjunto de resultados que têm o mesmo valor de um campo específico em um grupo.</span><span class="sxs-lookup"><span data-stu-id="10292-107">Grouping works by putting all items within the result set that have the same value of a specific field into a group.</span></span> <span data-ttu-id="10292-108">Por exemplo, você pode agrupar seus resultados pelo remetente, e todos os itens da mesma pessoa estarão em um grupo separado, e os itens de cada grupo serão classificados de acordo com a ordem especificada no modo de exibição.</span><span class="sxs-lookup"><span data-stu-id="10292-108">For example, you can group your results by the sender, and all items from the same person will be in a separate group, and the items within each group will be sorted according to the order you specify on the view.</span></span> <span data-ttu-id="10292-109">Os grupos em si são classificados por um valor agregado com base em um campo que você escolher.</span><span class="sxs-lookup"><span data-stu-id="10292-109">The groups themselves are sorted by an aggregate value based on a field you choose.</span></span>
  
<span data-ttu-id="10292-110">**Tabela 1. Métodos da API gerenciada do EWS e operações do EWS para organizar os resultados da pesquisa**</span><span class="sxs-lookup"><span data-stu-id="10292-110">**Table 1. EWS Managed API methods and EWS operations for organizing search results**</span></span>

|<span data-ttu-id="10292-111">**Se você quiser...**</span><span class="sxs-lookup"><span data-stu-id="10292-111">**If you want to…**</span></span>|<span data-ttu-id="10292-112">**Na API gerenciada do EWS, use...**</span><span class="sxs-lookup"><span data-stu-id="10292-112">**In the EWS Managed API, use…**</span></span>|<span data-ttu-id="10292-113">**Em EWS, use...**</span><span class="sxs-lookup"><span data-stu-id="10292-113">**In EWS, use…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="10292-114">Organizar itens com o mesmo valor em uma propriedade específica em seus resultados em grupos</span><span class="sxs-lookup"><span data-stu-id="10292-114">Organize items with the same value in a specific property in your results into groups</span></span>  <br/> |[<span data-ttu-id="10292-115">Agrupamento. agrupar</span><span class="sxs-lookup"><span data-stu-id="10292-115">Grouping.GroupOn</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.groupon%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="10292-116">Elemento [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) como um filho do elemento [GroupBy](https://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="10292-116">[FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) element as a child of the [GroupBy](https://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="10292-117">Classificar itens dentro de cada grupo pelo valor em uma propriedade específica</span><span class="sxs-lookup"><span data-stu-id="10292-117">Sort items within each group by the value in a specific property</span></span>  <br/> |[<span data-ttu-id="10292-118">AllViews. OrderBy</span><span class="sxs-lookup"><span data-stu-id="10292-118">ItemView.OrderBy</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.orderby%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="10292-119">Elemento [SortOrder](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="10292-119">[SortOrder](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="10292-120">Classificar os grupos</span><span class="sxs-lookup"><span data-stu-id="10292-120">Sort the groups</span></span>  <br/> |[<span data-ttu-id="10292-121">Agrupamento. agregação</span><span class="sxs-lookup"><span data-stu-id="10292-121">Grouping.AggregateOn</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregateon%28v=exchg.80%29.aspx) <br/><br/> [<span data-ttu-id="10292-122">Agrupamento. AggregateType</span><span class="sxs-lookup"><span data-stu-id="10292-122">Grouping.AggregateType</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregatetype%28v=exchg.80%29.aspx) <br/><br/> [<span data-ttu-id="10292-123">GROUPING. SortDirection</span><span class="sxs-lookup"><span data-stu-id="10292-123">Grouping.SortDirection</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.sortdirection%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="10292-124">Elemento **FieldURI** como um filho do elemento [Aggregate](https://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="10292-124">**FieldURI** element as a child of the [AggregateOn](https://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx) element</span></span><br/><br/> <span data-ttu-id="10292-125">Atributo **Aggregate** no elemento **Aggregate**</span><span class="sxs-lookup"><span data-stu-id="10292-125">**Aggregate** attribute on the **AggregateOn** element</span></span><br/><br/><span data-ttu-id="10292-126">Atributo **Order** no elemento **GroupBy**</span><span class="sxs-lookup"><span data-stu-id="10292-126">**Order** attribute on the **GroupBy** element</span></span>  <br/> |
   
<span data-ttu-id="10292-127">Vamos dar um passo a passo.</span><span class="sxs-lookup"><span data-stu-id="10292-127">Let's take it step by step.</span></span>
  
## <a name="group-results-by-a-specific-property"></a><span data-ttu-id="10292-128">Agrupar resultados por uma propriedade específica</span><span class="sxs-lookup"><span data-stu-id="10292-128">Group results by a specific property</span></span>
<span data-ttu-id="10292-129"><a name="bk_GroupResults"> </a></span><span class="sxs-lookup"><span data-stu-id="10292-129"><a name="bk_GroupResults"> </a></span></span>

<span data-ttu-id="10292-130">A primeira etapa para usar o agrupamento é selecionar uma propriedade ou um atributo nos itens do repositório do Exchange, para agrupar por.</span><span class="sxs-lookup"><span data-stu-id="10292-130">The first step to using grouping is to select a property, or attribute on the items in the Exchange store, to group by.</span></span> <span data-ttu-id="10292-131">A API gerenciada do EWS expõe essas propriedades como classe nas classes correspondentes, enquanto o EWS as expõe como elementos XML.</span><span class="sxs-lookup"><span data-stu-id="10292-131">The EWS Managed API exposes these as class properties on the corresponding classes, while EWS exposes them as XML elements.</span></span> <span data-ttu-id="10292-132">Você pode escolher qualquer propriedade, incluindo propriedades personalizadas ou estendidas, mas é útil entender como os itens são agrupados com base no valor da propriedade que você escolher.</span><span class="sxs-lookup"><span data-stu-id="10292-132">You can choose any property, including custom or extended properties, but it is helpful to understand how items are grouped based on the value of the property you choose.</span></span> 

<span data-ttu-id="10292-133">Todos os itens que têm o mesmo valor na propriedade que você escolheu para agrupar serão agrupados.</span><span class="sxs-lookup"><span data-stu-id="10292-133">All items that have the same value in the property you choose to group by will be grouped together.</span></span> <span data-ttu-id="10292-134">Isso pode parecer óbvio, mas é um detalhe importante.</span><span class="sxs-lookup"><span data-stu-id="10292-134">This might seem obvious, but it is an important detail.</span></span> <span data-ttu-id="10292-135">Considere o que acontece se você agrupar por uma propriedade data/hora, como [Item. DateTimeReceived](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.datetimereceived%28v=exchg.80%29.aspx) na API gerenciada do EWS ou o elemento [DateTimeReceived](https://msdn.microsoft.com/library/8f489bd4-2434-4d0a-91fe-1b5ba7eb5765%28Office.15%29.aspx) no EWS.</span><span class="sxs-lookup"><span data-stu-id="10292-135">Consider what happens if you group by a date/time property, such as [Item.DateTimeReceived](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.datetimereceived%28v=exchg.80%29.aspx) in the EWS Managed API, or the [DateTimeReceived](https://msdn.microsoft.com/library/8f489bd4-2434-4d0a-91fe-1b5ba7eb5765%28Office.15%29.aspx) element in EWS.</span></span> <span data-ttu-id="10292-136">A intenção pode ser organizar os resultados em grupos, com cada grupo contendo itens do mesmo dia.</span><span class="sxs-lookup"><span data-stu-id="10292-136">The intent might be to organize the results into groups, with each group containing items from the same day.</span></span> <span data-ttu-id="10292-137">No entanto, o agrupamento examina o valor inteiro, que inclui a hora.</span><span class="sxs-lookup"><span data-stu-id="10292-137">However, grouping looks at the entire value, which includes the time.</span></span> 

<span data-ttu-id="10292-138">O resultado final é que os itens serão agrupados para que os itens recebidos ao mesmo tempo, até o segundo, estejam em seus próprios grupos.</span><span class="sxs-lookup"><span data-stu-id="10292-138">The end result is that the items will be grouped so that items received at the same time, down to the second, are in their own groups.</span></span> <span data-ttu-id="10292-139">Os resultados provavelmente serão classificados em um grande número de grupos com um pequeno número de itens em cada grupo.</span><span class="sxs-lookup"><span data-stu-id="10292-139">The results will most likely be sorted into a large number of groups with a small number of items in each group.</span></span> 
  
<span data-ttu-id="10292-140">Para obter um conjunto de resultados com um número menor de grupos e um maior número de itens em cada grupo, escolha uma propriedade que provavelmente tenha um número menor de valores, como [EmailMessage. from](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.from%28v=exchg.80%29.aspx) ou [Item. Categories](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.categories%28v=exchg.80%29.aspx) na API gerenciada do [EWS ou em](https://msdn.microsoft.com/library/5a52d644-3677-4049-874c-12bd5c3080dc%28Office.15%29.aspx) [categorias](https://msdn.microsoft.com/library/d84d4927-b524-4e62-bf3d-1f12fec8c21a%28Office.15%29.aspx) do EWS.</span><span class="sxs-lookup"><span data-stu-id="10292-140">To get a results set with a smaller number of groups and a larger number of items in each group, choose a property that is likely to have a smaller number of values, such as [EmailMessage.From](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.from%28v=exchg.80%29.aspx) or [Item.Categories](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.categories%28v=exchg.80%29.aspx) in the EWS Managed API, or [From](https://msdn.microsoft.com/library/5a52d644-3677-4049-874c-12bd5c3080dc%28Office.15%29.aspx) or [Categories](https://msdn.microsoft.com/library/d84d4927-b524-4e62-bf3d-1f12fec8c21a%28Office.15%29.aspx) in EWS.</span></span> <span data-ttu-id="10292-141">A figura a seguir mostra uma lista de emails que aparecem em uma caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="10292-141">The following figure shows a list of emails that appear in an Inbox.</span></span> 
  
<span data-ttu-id="10292-142">**Figura 1. Mensagens em uma caixa de entrada**</span><span class="sxs-lookup"><span data-stu-id="10292-142">**Figure 1. Messages in an Inbox**</span></span>

![A sample list of messages in a user's Inbox.](media/Ex15_GroupedSearch_MsgList.png)
  
<span data-ttu-id="10292-144">Se você agrupar os itens na Figura 1 pela propriedade **EmailMessage. from** , o resultado será dois grupos, um para mensagens enviadas por esperança bruto e um para mensagens enviadas por Sadie Daniels.</span><span class="sxs-lookup"><span data-stu-id="10292-144">If you group the items in Figure 1 by the **EmailMessage.From** property, the result will be two groups, one for messages sent by Hope Gross, and one for messages sent by Sadie Daniels.</span></span> 
  
<span data-ttu-id="10292-145">**Figura 2. Mensagens separadas em grupos com base na propriedade from**</span><span class="sxs-lookup"><span data-stu-id="10292-145">**Figure 2. Messages separated into groups based on the From property**</span></span>

![An image that shows messages sorted into two lists by the From property.](media/Ex15_GroupedSearch_SeparateGroups.png)
  
## <a name="sort-the-items-within-groups"></a><span data-ttu-id="10292-147">Classificar os itens dentro de grupos</span><span class="sxs-lookup"><span data-stu-id="10292-147">Sort the items within groups</span></span>
<span data-ttu-id="10292-148"><a name="bk_SortItems"> </a></span><span class="sxs-lookup"><span data-stu-id="10292-148"><a name="bk_SortItems"> </a></span></span>

<span data-ttu-id="10292-149">Você pode controlar como os itens são classificados dentro de cada grupo usando a propriedade ItemProperty [. OrderBy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.orderby%28v=exchg.80%29.aspx) na API gerenciada do EWS ou o elemento [SortOrder](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) em EWS.</span><span class="sxs-lookup"><span data-stu-id="10292-149">You can control how items are sorted within each group by using the [ItemView.OrderBy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.orderby%28v=exchg.80%29.aspx) property in the EWS Managed API, or the [SortOrder](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) element in EWS.</span></span> <span data-ttu-id="10292-150">A mesma ordenação se aplica a cada grupo.</span><span class="sxs-lookup"><span data-stu-id="10292-150">The same ordering applies to each group.</span></span> <span data-ttu-id="10292-151">Por exemplo, se você classificar os itens da Figura 1 pela propriedade **Item. DateTimeReceived** , em ordem decrescente, o item mais recentemente recebido de espero bruto será o primeiro no grupo de espera bruto e o item mais recentemente recebido de Sadie Daniels será o primeiro no grupo Sadie Daniels.</span><span class="sxs-lookup"><span data-stu-id="10292-151">For example, if you sort the items from Figure 1 by the **Item.DateTimeReceived** property, in descending order, the item most recently received from Hope Gross will be first in the Hope Gross group, and the item most recently received from Sadie Daniels will be first in the Sadie Daniels group.</span></span> <span data-ttu-id="10292-152">Convenientemente, os grupos na Figura 2 já estão classificados dessa forma.</span><span class="sxs-lookup"><span data-stu-id="10292-152">Conveniently, the groups in Figure 2 are already sorted this way.</span></span> 
  
## <a name="sort-the-groups"></a><span data-ttu-id="10292-153">Classificar os grupos</span><span class="sxs-lookup"><span data-stu-id="10292-153">Sort the groups</span></span>
<span data-ttu-id="10292-154"><a name="bk_SortGroups"> </a></span><span class="sxs-lookup"><span data-stu-id="10292-154"><a name="bk_SortGroups"> </a></span></span>

<span data-ttu-id="10292-155">Agora que você tem seus grupos liquidados, a etapa final é classificar os grupos por conta própria.</span><span class="sxs-lookup"><span data-stu-id="10292-155">Now that you have your groups settled, the final step is sorting the groups themselves.</span></span> <span data-ttu-id="10292-156">Como os grupos não possuem valores específicos, o processo de agrupamento precisa atribuir um valor de classificação a cada grupo.</span><span class="sxs-lookup"><span data-stu-id="10292-156">Because the groups themselves have no specific values, the grouping process has to assign a sort value to each group.</span></span> <span data-ttu-id="10292-157">Isso é feito por agregação dos valores de uma propriedade específica dentro de cada grupo, especificado pela propriedade [GROUPING. Aggregate](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregateon%28v=exchg.80%29.aspx) na API gerenciada do EWS ou o elemento [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) como um filho do elemento [Aggregate](https://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx) no EWS.</span><span class="sxs-lookup"><span data-stu-id="10292-157">This is done by aggregation of the values of a specific property within each group, specified by the [Grouping.AggregateOn](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregateon%28v=exchg.80%29.aspx) property in the EWS Managed API, or the [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) element as a child of the [AggregateOn](https://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx) element in EWS.</span></span> <span data-ttu-id="10292-158">A propriedade [GROUPING. AggregateType](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregatetype%28v=exchg.80%29.aspx) na API gerenciada do EWS (ou o atributo **Aggregate** no elemento **Aggregate** no EWS) especifica qual valor dos itens dentro de cada grupo é atribuído ao valor de classificação para o grupo, seja o maior valor ou o menor valor.</span><span class="sxs-lookup"><span data-stu-id="10292-158">The [Grouping.AggregateType](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregatetype%28v=exchg.80%29.aspx) property in the EWS Managed API (or the **Aggregate** attribute on the **AggregateOn** element in EWS) specifies which value from the items within each group is assigned to the sort value for the group — either the largest value or the smallest value.</span></span> <span data-ttu-id="10292-159">Por fim, a ordem de classificação (decrescente ou crescente) é especificada pela propriedade [GROUPING. SortDirection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.sortdirection%28v=exchg.80%29.aspx) na API gerenciada do EWS ou o atributo **Order** no elemento [GroupBy](https://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx) do EWS.</span><span class="sxs-lookup"><span data-stu-id="10292-159">Finally, the sort order (descending or ascending) is specified by the [Grouping.SortDirection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.sortdirection%28v=exchg.80%29.aspx) property in the EWS Managed API, or the **Order** attribute on the [GroupBy](https://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx) element in EWS.</span></span> 
  
<span data-ttu-id="10292-160">Por exemplo, se os grupos da Figura 2 são classificados por agregação na propriedade **Item. DateTimeReceived** , usando o menor valor e classificando em ordem decrescente, os itens são retornados na ordem na Figura 3 mostrada.</span><span class="sxs-lookup"><span data-stu-id="10292-160">For example, if the groups from Figure 2 are sorted by aggregating on the **Item.DateTimeReceived** property, using the smallest value, and sorting in descending order, the items are returned in the order in shown Figure 3.</span></span> 
  
<span data-ttu-id="10292-161">**Figura 3. Resultados de pesquisa agrupados com os grupos classificados pela Propriedade DateTimeReceived**</span><span class="sxs-lookup"><span data-stu-id="10292-161">**Figure 3. Grouped search results with the groups sorted by the DateTimeReceived property**</span></span>

![An image that shows a sorted lists of messages, grouped by the From property, with the groups sorted by the smallest received date/time.](media/Ex15_GroupedSearch_Results.png)
  
<span data-ttu-id="10292-163">As seções a seguir mostram como você pode extrair e classificar juntos no código.</span><span class="sxs-lookup"><span data-stu-id="10292-163">The next sections show you how you might pull grouping and sorting together in code.</span></span>
  
## <a name="example-perform-a-grouped-search-by-using-the-ews-managed-api"></a><span data-ttu-id="10292-164">Exemplo: executar uma pesquisa agrupada usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="10292-164">Example: Perform a grouped search by using the EWS Managed API</span></span>
<span data-ttu-id="10292-165"><a name="bk_GroupSearchEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="10292-165"><a name="bk_GroupSearchEWSMA"> </a></span></span>

<span data-ttu-id="10292-166">Os seguintes métodos de API gerenciada do EWS podem usar o agrupamento:</span><span class="sxs-lookup"><span data-stu-id="10292-166">The following EWS Managed API methods can use grouping:</span></span>
  
- [<span data-ttu-id="10292-167">ExchangeService. FindItems</span><span class="sxs-lookup"><span data-stu-id="10292-167">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="10292-168">Folder. FindItems</span><span class="sxs-lookup"><span data-stu-id="10292-168">Folder.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
<span data-ttu-id="10292-169">O exemplo a seguir usa o método **ExchangeService. FindItems** ; no entanto, as mesmas regras e conceitos se aplicam ao método **Folder. FindItems** .</span><span class="sxs-lookup"><span data-stu-id="10292-169">The following example uses the **ExchangeService.FindItems** method; however, the same rules and concepts apply to the **Folder.FindItems** method.</span></span> <span data-ttu-id="10292-170">Neste exemplo, um método chamado **GroupItemsByFrom** é definido.</span><span class="sxs-lookup"><span data-stu-id="10292-170">In this example, a method called **GroupItemsByFrom** is defined.</span></span> <span data-ttu-id="10292-171">Ele usa um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e um objeto [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) como parâmetros.</span><span class="sxs-lookup"><span data-stu-id="10292-171">It takes an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and a [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) object as parameters.</span></span> <span data-ttu-id="10292-172">Ele solicita os primeiros 50 itens na pasta, agrupados pela propriedade **EmailMessage. from** , classificados pela propriedade **Item. DateTimeReceived** em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="10292-172">It requests the first 50 items in the folder, grouped by the **EmailMessage.From** property, sorted by the **Item.DateTimeReceived** property in descending order.</span></span> <span data-ttu-id="10292-173">Os grupos em si são classificados pelo menor valor de propriedade **Item. DateTimeReceived** em seus itens, em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="10292-173">The groups themselves are sorted by the smallest **Item.DateTimeReceived** property value on their items, in descending order.</span></span> 
  
<span data-ttu-id="10292-174">Este exemplo pressupõe que o objeto **ExchangeService** tenha sido inicializado com valores válidos nas propriedades de [credenciais](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) e [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="10292-174">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
```cs
static void GroupItemsByFrom(ExchangeService service, WellKnownFolderName folder)
{
    // Limit the result set to 50 items.
    ItemView view = new ItemView(50);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.From,
                                       ItemSchema.Categories);
    // Item searches do not support Deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Specify the sorting done within the groups.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    // Configure grouping.
    Grouping groupByFrom = new Grouping();
    groupByFrom.GroupOn = EmailMessageSchema.From;
    groupByFrom.AggregateOn = ItemSchema.DateTimeReceived;
    groupByFrom.AggregateType = AggregateType.Minimum;
    groupByFrom.SortDirection = SortDirection.Descending;
    try
    {
        GroupedFindItemsResults<Item> results = service.FindItems(folder,
            view, groupByFrom);
        foreach (ItemGroup<Item> group in results.ItemGroups)
        {
            Console.WriteLine("Group: {0}", group.GroupIndex);
            foreach (Item item in group.Items)
            {
                if (item is EmailMessage)
                {
                    EmailMessage message = item as EmailMessage;
                    Console.WriteLine("From: {0}", message.From);
                    Console.WriteLine("Subject: {0}", message.Subject);
                    Console.WriteLine("Id: {0}\n", message.Id.ToString());
                }
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

## <a name="example-perform-a-grouped-search-by-using-ews"></a><span data-ttu-id="10292-175">Exemplo: executar uma pesquisa agrupada usando o EWS</span><span class="sxs-lookup"><span data-stu-id="10292-175">Example: Perform a grouped search by using EWS</span></span>
<span data-ttu-id="10292-176"><a name="bk_GroupSearchEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="10292-176"><a name="bk_GroupSearchEWS"> </a></span></span>

<span data-ttu-id="10292-177">O exemplo de solicitação a seguir mostra uma solicitação de [operação FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) para os primeiros 50 itens na pasta, agrupados pelo elemento **from** , classificados pelo elemento **DateTimeReceived** em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="10292-177">The following request example shows a [FindItem operation](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) request for the first 50 items in the folder, grouped by the **From** element, sorted by the **DateTimeReceived** element in descending order.</span></span> <span data-ttu-id="10292-178">Os grupos em si são classificados pelo menor valor do elemento **DateTimeReceived** em seus itens, em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="10292-178">The groups themselves are sorted by the smallest **DateTimeReceived** element value on their items, in descending order.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="message:From" />
          <t:FieldURI FieldURI="item:Categories" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="50" Offset="0" BasePoint="Beginning" />
      <m:GroupBy Order="Descending">
        <t:FieldURI FieldURI="message:From" />
        <t:AggregateOn Aggregate="Minimum">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:AggregateOn>
      </m:GroupBy>
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

<span data-ttu-id="10292-179">O servidor retorna a seguinte resposta.</span><span class="sxs-lookup"><span data-stu-id="10292-179">The server returns the following response.</span></span>
  
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
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="10" TotalItemsInView="8" IncludesLastItemInRange="true">
            <t:Groups>
              <t:GroupedItems>
                <t:GroupIndex>0</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Planning resources</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:41:05Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Timeline</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:40:37Z</t:DateTimeReceived>
                    <t:Categories>
                      <t:String>Project</t:String>
                    </t:Categories>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>For your perusal</t:Subject>
                    <t:DateTimeReceived>2013-11-20T21:51:16Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>meeting notes</t:Subject>
                    <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                    <t:Categories>
                      <t:String>Blue category</t:String>
                    </t:Categories>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Meeting notes</t:Subject>
                    <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
              <t:GroupedItems>
                <t:GroupIndex>1</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Query</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:43:15Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Hope Gross</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=9B55E4100C064D9D8C5F72FF36802ED3-HOPE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Update</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:42:33Z</t:DateTimeReceived>
                    <t:Categories>
                      <t:String>Project</t:String>
                      <t:String>Blue category</t:String>
                    </t:Categories>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Hope Gross</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=9B55E4100C064D9D8C5F72FF36802ED3-HOPE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>This cat is hilarious!</t:Subject>
                    <t:DateTimeReceived>2013-10-15T20:22:12Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Hope Gross</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=9B55E4100C064D9D8C5F72FF36802ED3-HOPE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
            </t:Groups>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="version-differences"></a><span data-ttu-id="10292-180">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="10292-180">Version differences</span></span>
<span data-ttu-id="10292-181"><a name="bk_VersionDiffs"> </a></span><span class="sxs-lookup"><span data-stu-id="10292-181"><a name="bk_VersionDiffs"> </a></span></span>

<span data-ttu-id="10292-182">As versões do Exchange que começam com a versão principal 15 e terminam com os elementos de **grupo** de retorno de 15.0.775.38 de saída (do tipo **GroupedItemsType**) no lugar dos elementos [GroupedItems](https://msdn.microsoft.com/library/53170df4-4272-4b37-b23f-cd8e2d4a7396%28Office.15%29.aspx) na resposta SOAP.</span><span class="sxs-lookup"><span data-stu-id="10292-182">Versions of Exchange starting with major version 15 and ending with build 15.0.775.38 return **Group** elements (of type **GroupedItemsType**) in place of [GroupedItems](https://msdn.microsoft.com/library/53170df4-4272-4b37-b23f-cd8e2d4a7396%28Office.15%29.aspx) elements in the SOAP response.</span></span> <span data-ttu-id="10292-183">Se você estiver usando a API gerenciada do EWS, isso fará com que a coleção [GroupedFindItemsResults. Dogroups](https://msdn.microsoft.com/library/office/dd633961%28v=exchg.80%29.aspx) contenha objetos 0.</span><span class="sxs-lookup"><span data-stu-id="10292-183">If you are using the EWS Managed API, this will cause the [GroupedFindItemsResults.ItemGroups](https://msdn.microsoft.com/library/office/dd633961%28v=exchg.80%29.aspx) collection to contain 0 objects.</span></span> <span data-ttu-id="10292-184">Se você estiver usando o EWS, os elementos de **grupo** devem ser tratados como elementos **GroupedItems** .</span><span class="sxs-lookup"><span data-stu-id="10292-184">If you are using EWS, **Group** elements should be handled as **GroupedItems** elements.</span></span> 
  
<span data-ttu-id="10292-185">As versões do Exchange que começam com a versão principal 15 retornam um **grupo** extra ou elementos **GroupedItems** com o atributo **xsi: nil** definido como **true** na resposta SOAP.</span><span class="sxs-lookup"><span data-stu-id="10292-185">Versions of Exchange starting with major version 15 return extra **Group** or **GroupedItems** elements with the **xsi:nil** attribute set to **true** in the SOAP response.</span></span> <span data-ttu-id="10292-186">Se você estiver usando a API gerenciada do EWS, esses elementos extras farão com que um [ServiceXmlDeserializationException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.servicexmldeserializationexception%28v=exchg.80%29.aspx) seja lançado.</span><span class="sxs-lookup"><span data-stu-id="10292-186">If you are using the EWS Managed API, these extra elements will cause a [ServiceXmlDeserializationException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.servicexmldeserializationexception%28v=exchg.80%29.aspx) to be thrown.</span></span> <span data-ttu-id="10292-187">Se você estiver usando o EWS, esses elementos extras deverão ser ignorados.</span><span class="sxs-lookup"><span data-stu-id="10292-187">If you are using EWS, these extra elements should be ignored.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="10292-188">Confira também</span><span class="sxs-lookup"><span data-stu-id="10292-188">See also</span></span>

- [<span data-ttu-id="10292-189">Pesquisar e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="10292-189">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)    
- [<span data-ttu-id="10292-190">ExchangeService. FindItems</span><span class="sxs-lookup"><span data-stu-id="10292-190">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="10292-191">Folder. FindItems</span><span class="sxs-lookup"><span data-stu-id="10292-191">Folder.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)   
- [<span data-ttu-id="10292-192">Classe de agrupamento</span><span class="sxs-lookup"><span data-stu-id="10292-192">Grouping class</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="10292-193">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="10292-193">FindItem operation</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

