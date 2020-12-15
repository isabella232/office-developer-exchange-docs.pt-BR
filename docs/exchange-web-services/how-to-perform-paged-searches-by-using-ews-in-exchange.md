---
title: Executar pesquisas paginadas usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 64ed70e4-32eb-4c25-bfc4-43d1477296e5
description: Descubra como realizar pesquisas paginadas na sua API gerenciada EWS ou no aplicativo EWS direcionado para o Exchange.
localization_priority: Priority
ms.openlocfilehash: fa36a2ce77150f29e5a62876138c9693a3b4ab1f
ms.sourcegitcommit: 37d4ecd4f469690ba1de87baad2f2f58c40c96ba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49348819"
---
# <a name="perform-paged-searches-by-using-ews-in-exchange"></a><span data-ttu-id="d370e-103">Executar pesquisas paginadas usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d370e-103">Perform paged searches by using EWS in Exchange</span></span>

<span data-ttu-id="d370e-104">Descubra como realizar pesquisas paginadas na sua API gerenciada EWS ou no aplicativo EWS direcionado para o Exchange.</span><span class="sxs-lookup"><span data-stu-id="d370e-104">Find out how to perform paged searches in your EWS Managed API or EWS application that targets Exchange.</span></span>
  
<span data-ttu-id="d370e-105">A paginação é um recurso no EWS que permite controlar o tamanho dos resultados de uma pesquisa.</span><span class="sxs-lookup"><span data-stu-id="d370e-105">Paging is a feature in EWS that enables you to control the size of the results of a search.</span></span> <span data-ttu-id="d370e-106">Em vez de recuperar todo o conjunto de resultados em uma resposta do EWS, você pode recuperar conjuntos menores em várias respostas do EWS.</span><span class="sxs-lookup"><span data-stu-id="d370e-106">Rather than retrieve the entire result set in one EWS response, you can retrieve smaller sets in multiple EWS responses.</span></span> <span data-ttu-id="d370e-107">Por exemplo, considere um usuário com 10.000 mensagens de email na caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="d370e-107">For example, consider a user with 10,000 email messages in their Inbox.</span></span> <span data-ttu-id="d370e-108">Teoricamente, você pode recuperar todos os 10.000 emails em uma resposta muito grande, mas pode querer separá-los em fragmentos gerenciados mais facilmente por razões como largura de banda ou desempenho.</span><span class="sxs-lookup"><span data-stu-id="d370e-108">Hypothetically, you could retrieve all 10,000 emails in one very large response, but you might want to break that up into more manageable chunks for bandwidth or performance reasons.</span></span> <span data-ttu-id="d370e-109">A paginação oferece as ferramentas para fazer exatamente isso.</span><span class="sxs-lookup"><span data-stu-id="d370e-109">Paging gives you the tools to do just that.</span></span>
  
> [!NOTE]
> <span data-ttu-id="d370e-110">Embora você possa recuperar, teoricamente, os 10.000 itens em uma única solicitação, na verdade isso não é muito provável devido à limitação do EWS.</span><span class="sxs-lookup"><span data-stu-id="d370e-110">While you can hypothetically retrieve 10,000 items in one request, in reality, this is unlikely due to EWS throttling.</span></span> <span data-ttu-id="d370e-111">Para saber mais, confira [Limitação do EWS no Exchange](ews-throttling-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="d370e-111">To find out more, see [EWS throttling in Exchange](ews-throttling-in-exchange.md).</span></span> 
  
<span data-ttu-id="d370e-112">**Tabela 1. Parâmetros de paginação na API gerenciada do EWS e no EWS**</span><span class="sxs-lookup"><span data-stu-id="d370e-112">**Table 1. Paging parameters in the EWS Managed API and EWS**</span></span>

|<span data-ttu-id="d370e-113">**Para configurar ou recuperar o...**</span><span class="sxs-lookup"><span data-stu-id="d370e-113">**To configure or retrieve the…**</span></span>|<span data-ttu-id="d370e-114">**Na API Gerenciada do EWS, use...**</span><span class="sxs-lookup"><span data-stu-id="d370e-114">**In the EWS Managed API, use…**</span></span>|<span data-ttu-id="d370e-115">**No EWS, use...**</span><span class="sxs-lookup"><span data-stu-id="d370e-115">**In EWS, use…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d370e-116">Número máximo de itens ou pastas em uma resposta</span><span class="sxs-lookup"><span data-stu-id="d370e-116">Maximum number of items or folders in a response</span></span>  <br/> |<span data-ttu-id="d370e-117">O parâmetro **pageSize** para o [construtor ItemView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) ou o [construtor FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="d370e-117">The **pageSize** parameter to the [ItemView constructor](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) or the [FolderView constructor](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx)</span></span> <br/> <span data-ttu-id="d370e-118">Ou</span><span class="sxs-lookup"><span data-stu-id="d370e-118">Or</span></span>  <br/> <span data-ttu-id="d370e-119">A propriedade [PagedView.PageSize](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="d370e-119">The [PagedView.PageSize](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="d370e-120">O atributo **MaxEntriesReturned** no elemento [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou no elemento [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="d370e-120">The **MaxEntriesReturned** attribute on the [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element or the [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="d370e-121">Ponto de partida na lista de itens ou pastas</span><span class="sxs-lookup"><span data-stu-id="d370e-121">Starting point in the list of items or folders</span></span>  <br/> |<span data-ttu-id="d370e-122">O parâmetro **offsetBasePoint** para o construtor **ItemView** ou o construtor **FolderView**</span><span class="sxs-lookup"><span data-stu-id="d370e-122">The **offsetBasePoint** parameter to the **ItemView** constructor or the **FolderView** constructor</span></span>  <br/> <span data-ttu-id="d370e-123">Ou</span><span class="sxs-lookup"><span data-stu-id="d370e-123">Or</span></span>  <br/> <span data-ttu-id="d370e-124">A propriedade[PagedView.OffsetBasePoint](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="d370e-124">The [PagedView.OffsetBasePoint](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="d370e-125">O atributo **BasePoint** no elemento **IndexedPageItemView** ou no elemento **IndexedPageFolderView**</span><span class="sxs-lookup"><span data-stu-id="d370e-125">The **BasePoint** attribute on the **IndexedPageItemView** element or the **IndexedPageFolderView** element</span></span>  <br/> |
|<span data-ttu-id="d370e-126">Deslocamento a partir do ponto de partida</span><span class="sxs-lookup"><span data-stu-id="d370e-126">Offset from the starting point</span></span>  <br/> |<span data-ttu-id="d370e-127">O parâmetro **offset** para o construtor **ItemView** ou o construtor **FolderView**</span><span class="sxs-lookup"><span data-stu-id="d370e-127">The **offset** parameter to the **ItemView** constructor or the **FolderView** constructor</span></span>  <br/> <span data-ttu-id="d370e-128">Ou</span><span class="sxs-lookup"><span data-stu-id="d370e-128">Or</span></span>  <br/> <span data-ttu-id="d370e-129">A propriedade[PagedView.Offset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="d370e-129">The [PagedView.Offset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="d370e-130">O atributo **Offset** no elemento **IndexedPageItemView** ou no elemento **IndexedPageFolderView**</span><span class="sxs-lookup"><span data-stu-id="d370e-130">The **Offset** attribute on the **IndexedPageItemView** element or the **IndexedPageFolderView** element</span></span>  <br/> |
|<span data-ttu-id="d370e-131">Número total de resultados no servidor</span><span class="sxs-lookup"><span data-stu-id="d370e-131">Total number of results on the server</span></span>  <br/> |<span data-ttu-id="d370e-132">A propriedade [FindItemsResults.TotalCount](https://msdn.microsoft.com/library/dd635348%28v=exchg.80%29.aspx) ou a propriedade [FindFoldersResults.TotalCount](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="d370e-132">The [FindItemsResults.TotalCount](https://msdn.microsoft.com/library/dd635348%28v=exchg.80%29.aspx) property or the [FindFoldersResults.TotalCount](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="d370e-133">O atributo **TotalItemsInView** no elemento [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) ou o elemento [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="d370e-133">The **TotalItemsInView** attribute on the [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) element or the [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="d370e-134">Deslocamento do primeiro item ou pasta não incluída na resposta atual</span><span class="sxs-lookup"><span data-stu-id="d370e-134">Offset of first item or folder not included in current response</span></span>  <br/> |<span data-ttu-id="d370e-135">A propriedade [FindItemsResults.NextPageOffset](https://msdn.microsoft.com/library/ee693014%28v=exchg.80%29.aspx) ou a propriedade [FindFoldersResults.NextPageOffset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="d370e-135">The [FindItemsResults.NextPageOffset](https://msdn.microsoft.com/library/ee693014%28v=exchg.80%29.aspx) property or the [FindFoldersResults.NextPageOffset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="d370e-136">O atributo **IndexedPagingOffset** no elemento **RootFolder**</span><span class="sxs-lookup"><span data-stu-id="d370e-136">The **IndexedPagingOffset** attribute on the **RootFolder** element</span></span>  <br/> |
|<span data-ttu-id="d370e-137">Indicador de que a resposta inclui o último item ou pasta na lista</span><span class="sxs-lookup"><span data-stu-id="d370e-137">Indicator that response includes the last item or folder in the list</span></span>  <br/> |<span data-ttu-id="d370e-138">A propriedade [FindItemsResults.MoreAvailable](https://msdn.microsoft.com/library/dd635477%28v=exchg.80%29.aspx) ou a propriedade [FindFoldersResults.MoreAvailable](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="d370e-138">The [FindItemsResults.MoreAvailable](https://msdn.microsoft.com/library/dd635477%28v=exchg.80%29.aspx) property or the [FindFoldersResults.MoreAvailable](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="d370e-139">O atributo **IncludesLastItemInRange** no elemento **RootFolder**</span><span class="sxs-lookup"><span data-stu-id="d370e-139">The **IncludesLastItemInRange** attribute on the **RootFolder** element</span></span>  <br/> |
   
## <a name="how-paging-works"></a><span data-ttu-id="d370e-140">Como funciona a paginação</span><span class="sxs-lookup"><span data-stu-id="d370e-140">How paging works</span></span>
<span data-ttu-id="d370e-141"><a name="bk_HowPagingWorks"> </a></span><span class="sxs-lookup"><span data-stu-id="d370e-141"><a name="bk_HowPagingWorks"> </a></span></span>

<span data-ttu-id="d370e-142">Para entender como funciona a paginação, é útil imaginá-las em uma pasta como painéis alinhados lado a lado em um espaço fora da sua casa.</span><span class="sxs-lookup"><span data-stu-id="d370e-142">To understand how paging works, it's helpful to visualize the messages in a folder as billboards lined up side by side in a field outside your house.</span></span> <span data-ttu-id="d370e-143">Você pode ver alguns desses painéis por meio de uma janela mágica.</span><span class="sxs-lookup"><span data-stu-id="d370e-143">You can see some of these billboards through a magical window.</span></span> <span data-ttu-id="d370e-144">Você tem a capacidade de alterar o tamanho da janela (para ver mais ou menos painéis por vez) e para mover a janela (para controlar quais painéis você pode ver).</span><span class="sxs-lookup"><span data-stu-id="d370e-144">You have the ability to change the size of the window (to see more or fewer billboards at once) and to move the window (to control which billboards you can see).</span></span> <span data-ttu-id="d370e-145">Essa manipulação da janela é paginação.</span><span class="sxs-lookup"><span data-stu-id="d370e-145">This manipulation of the window is paging.</span></span> 
  
<span data-ttu-id="d370e-146">Ao enviar a solicitação para o servidor Exchange, você especifica o tamanho da janela em termos de número de itens a ser retornado.</span><span class="sxs-lookup"><span data-stu-id="d370e-146">When you send your request to the Exchange server, you specify the size of your window in terms of how many items to return.</span></span> <span data-ttu-id="d370e-147">Defina a posição da janela especificando um ponto inicial (o início da linha ou o fim da linha) e um deslocamento desse ponto inicial, expresso em um número de itens.</span><span class="sxs-lookup"><span data-stu-id="d370e-147">You set the position of the window by specifying a starting point (either the beginning of the line or the end of the line) and an offset from that starting point, expressed in a number of items.</span></span> <span data-ttu-id="d370e-148">O início da janela é o número de itens especificado pelo deslocamento do ponto de partida.</span><span class="sxs-lookup"><span data-stu-id="d370e-148">The beginning of the window is the number of items specified by the offset from the starting point.</span></span>
  
<span data-ttu-id="d370e-149">A paginação fica um pouco mais interessante na resposta do servidor, e como seu aplicativo pode usar essa resposta para modelar a próxima solicitação.</span><span class="sxs-lookup"><span data-stu-id="d370e-149">Where paging gets a bit more interesting is in the server's response, and how your application can use that response to shape its next request.</span></span> <span data-ttu-id="d370e-150">O servidor oferece três informações que você pode usar para determinar como configurar sua "janela" para a próxima solicitação:</span><span class="sxs-lookup"><span data-stu-id="d370e-150">The server gives you three pieces of information that you can use to determine how to configure your "window" for your next request:</span></span> 
  
- <span data-ttu-id="d370e-151">Se os resultados na resposta incluem o último item no conjunto de resultados geral no servidor.</span><span class="sxs-lookup"><span data-stu-id="d370e-151">Whether the results in the response include the last item in the overall result set on the server.</span></span>
    
- <span data-ttu-id="d370e-152">O número total de itens no resultado definido no servidor.</span><span class="sxs-lookup"><span data-stu-id="d370e-152">The total number of items in the result set on the server.</span></span>
    
- <span data-ttu-id="d370e-153">Qual o próximo valor de deslocamento deve ser, se você quiser avançar a janela para o próximo item no conjunto de resultados que não está incluído na resposta atual.</span><span class="sxs-lookup"><span data-stu-id="d370e-153">What the next offset value should be, if you want to advance your window to the next item in the result set that isn't included in the current response.</span></span>
    
<span data-ttu-id="d370e-154">Vejamos um exemplo simples.</span><span class="sxs-lookup"><span data-stu-id="d370e-154">Let's look at a simple example.</span></span> <span data-ttu-id="d370e-155">Imagine uma caixa de entrada com 15 mensagens.</span><span class="sxs-lookup"><span data-stu-id="d370e-155">Imagine an Inbox with 15 messages in it.</span></span> <span data-ttu-id="d370e-156">O aplicativo envia uma solicitação inicial para recuperar um máximo de dez itens, começando no início da lista de mensagens (portanto, o deslocamento é zero).</span><span class="sxs-lookup"><span data-stu-id="d370e-156">Your application sends an initial request to retrieve a maximum of 10 items, starting at the beginning of the list of messages (so the offset is zero).</span></span> <span data-ttu-id="d370e-157">O servidor responde com as dez primeiras mensagens e indica que a resposta não inclui o último item, que há um total de 15 itens e que o próximo deslocamento deve ser dez.</span><span class="sxs-lookup"><span data-stu-id="d370e-157">The server responds with the first 10 messages, and indicates that the response does not include the last item, that there are a total of 15 items, and that the next offset should be 10.</span></span>
  
<span data-ttu-id="d370e-158">**Figura 1. Solicitar dez itens com deslocamento zero desde o início de uma lista de 15 itens**</span><span class="sxs-lookup"><span data-stu-id="d370e-158">**Figure 1. Requesting 10 items at offset 0 from the beginning of a list of 15 items**</span></span>

![Um diagrama mostrando os resultados da solicitação de dez itens com deslocamento zero no início de uma lista de 15 itens.](media/Ex15_PagedSearch_FirstPage.png)
  
<span data-ttu-id="d370e-160">Em seguida, o aplicativo reenvia a mesma solicitação para o servidor, com a única alteração sendo o deslocamento para dez.</span><span class="sxs-lookup"><span data-stu-id="d370e-160">Your application then resends the same request to the server, with the only change being that the offset is now 10.</span></span> <span data-ttu-id="d370e-161">O servidor retorna os últimos cinco itens e indica que a resposta inclui o último item, que há um total de 15 itens e que o próximo deslocamento deve ser 15 (no entanto, você chegou ao fim, por isso, não haverá um deslocamento próximo).</span><span class="sxs-lookup"><span data-stu-id="d370e-161">The server returns the last five items, and indicates that the response does include the last item, that there are a total of 15 items, and that the next offset should be 15 (though of course, you've reached the end, so there won't be a next offset.)</span></span>
  
<span data-ttu-id="d370e-162">**Figura 2. Solicitar dez itens com deslocamento dez desde o início de uma lista de 15 itens**</span><span class="sxs-lookup"><span data-stu-id="d370e-162">**Figure 2. Requesting 10 items at offset 10 from the beginning of a list of 15 items**</span></span>

![Um diagrama mostrando os resultados da solicitação de dez itens com deslocamento dez no início de uma lista de 15 itens.](media/Ex15_PagedSearch_SecondPage.png)
  
## <a name="design-considerations-for-paging"></a><span data-ttu-id="d370e-164">Considerações de design para paginação</span><span class="sxs-lookup"><span data-stu-id="d370e-164">Design considerations for paging</span></span>
<span data-ttu-id="d370e-165"><a name="bk_DesignConsiderations"> </a></span><span class="sxs-lookup"><span data-stu-id="d370e-165"><a name="bk_DesignConsiderations"> </a></span></span>

<span data-ttu-id="d370e-166">Aproveitar ao máximo a paginação em seu aplicativo exige algumas considerações.</span><span class="sxs-lookup"><span data-stu-id="d370e-166">Making the most out of paging in your application does require some consideration.</span></span> <span data-ttu-id="d370e-167">Por exemplo, qual é o tamanho da "janela"?</span><span class="sxs-lookup"><span data-stu-id="d370e-167">For example, how large do you make your "window"?</span></span> <span data-ttu-id="d370e-168">O que fazer se os resultados no servidor mudarem enquanto você estiver movendo a "janela"?</span><span class="sxs-lookup"><span data-stu-id="d370e-168">What do you do if the results on the server change while you're moving your "window"?</span></span>
  
### <a name="determine-the-size-of-your-window"></a><span data-ttu-id="d370e-169">Determinar o tamanho da janela</span><span class="sxs-lookup"><span data-stu-id="d370e-169">Determine the size of your window</span></span>

<span data-ttu-id="d370e-170">Não existe um número único de entradas o qual todos os aplicativos devem usar.</span><span class="sxs-lookup"><span data-stu-id="d370e-170">There is no "one-size-fits-all" maximum number of entries that all applications should use.</span></span> <span data-ttu-id="d370e-171">Determinar o número ideal para o seu aplicativo depende de vários fatores diferentes.</span><span class="sxs-lookup"><span data-stu-id="d370e-171">Determining the number that's right for your application depends on several different factors.</span></span> <span data-ttu-id="d370e-172">No entanto, é útil lembrar das seguintes orientações:</span><span class="sxs-lookup"><span data-stu-id="d370e-172">However, it's helpful to keep the following guidelines in mind:</span></span>
  
- <span data-ttu-id="d370e-173">Por padrão, o Exchange limita o número máximo de itens que podem ser retornados em uma única solicitação para 1000.</span><span class="sxs-lookup"><span data-stu-id="d370e-173">By default, Exchange limits the maximum number of items that can be returned in a single request to 1000.</span></span>
    
- <span data-ttu-id="d370e-174">Definir o número máximo de entradas para um número maior resulta em enviar menos solicitações para obter todos os itens, ao custo de ter que esperar mais respostas.</span><span class="sxs-lookup"><span data-stu-id="d370e-174">Setting the maximum number of entries to a larger number results in having to send fewer requests to get all items, at the cost of having to wait longer for responses.</span></span>
    
- <span data-ttu-id="d370e-175">Definir o número máximo de entradas para um número menor resulta em tempos de resposta mais rápidos, ao custo de ter que enviar mais solicitações para obter todos os itens.</span><span class="sxs-lookup"><span data-stu-id="d370e-175">Setting the maximum number of entries to a smaller number results in quicker response times, at the cost of having to send more requests to get all items.</span></span>
    
### <a name="handling-changes-to-the-result-set"></a><span data-ttu-id="d370e-176">Processando alterações para o conjunto de resultados</span><span class="sxs-lookup"><span data-stu-id="d370e-176">Handling changes to the result set</span></span>

<span data-ttu-id="d370e-177">No exemplo anterior simples nesse artigo, o número de itens na caixa de entrada do usuário permanecia constante.</span><span class="sxs-lookup"><span data-stu-id="d370e-177">In the simple example earlier in this article, the number of items in the user's Inbox remained constant.</span></span> <span data-ttu-id="d370e-178">No entanto, na realidade, o número de itens em uma caixa de entrada pode ser alterado frequentemente.</span><span class="sxs-lookup"><span data-stu-id="d370e-178">However, in reality, the number of items in an Inbox can change frequently.</span></span> <span data-ttu-id="d370e-179">Novas mensagens podem chegar e os itens podem ser excluídos ou movidos a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="d370e-179">New messages can arrive and items can be deleted or moved at any time.</span></span> <span data-ttu-id="d370e-180">Mas como isso afeta a paginação?</span><span class="sxs-lookup"><span data-stu-id="d370e-180">But how does this impact paging?</span></span> <span data-ttu-id="d370e-181">Modifiquemos o exemplo anterior de cenário para descobrir.</span><span class="sxs-lookup"><span data-stu-id="d370e-181">Let's modify the earlier example scenario to find out.</span></span>
  
<span data-ttu-id="d370e-182">Vamos começar novamente com os 15 itens na caixa de entrada do usuário e enviar a mesma solicitação inicial.</span><span class="sxs-lookup"><span data-stu-id="d370e-182">We'll start again with the 15 items in the user's Inbox, and send the same initial request.</span></span> <span data-ttu-id="d370e-183">Como antes, o servidor responde com as dez primeiras mensagens e indica que a resposta não inclui o último item, que há um total de 15 itens e que o próximo deslocamento deve ser dez, conforme mostrado na Figura 1.</span><span class="sxs-lookup"><span data-stu-id="d370e-183">As before, the server responds with the first 10 messages, and indicates that the response does not include the last item, that there are a total of 15 items, and that the next offset should be 10, as shown in Figure 1.</span></span>
  
<span data-ttu-id="d370e-184">Agora, enquanto o seu aplicativo processa esses dez itens, uma nova mensagem chega na caixa de entrada e é adicionada ao conjunto de resultados no servidor.</span><span class="sxs-lookup"><span data-stu-id="d370e-184">Now, while your application is processing those 10 items, a new message arrives in the Inbox and is added to the result set on the server.</span></span> <span data-ttu-id="d370e-185">O aplicativo reenvia a mesma solicitação para o servidor (somente com o deslocamento definido como 10).</span><span class="sxs-lookup"><span data-stu-id="d370e-185">Your application resends the same request to the server (only with the offset set to 10).</span></span> <span data-ttu-id="d370e-186">Desta vez, o servidor recebe seis itens e indica que há um total de 16 itens no conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="d370e-186">This time the server gets back six items, and indicates that there are a total of 16 items in the result set.</span></span>
  
<span data-ttu-id="d370e-187">Neste ponto, você deve estar se perguntando se esse isso é realmente um problema.</span><span class="sxs-lookup"><span data-stu-id="d370e-187">At this point you might be wondering if this is even a problem.</span></span> <span data-ttu-id="d370e-188">Afinal, você tem 16 itens nas duas respostas, então por que toda essa preocupação?</span><span class="sxs-lookup"><span data-stu-id="d370e-188">After all, you got 16 items back over the two responses, so why all the fuss?</span></span> <span data-ttu-id="d370e-189">A resposta depende de onde o novo item será posicionado.</span><span class="sxs-lookup"><span data-stu-id="d370e-189">The answer depends on where in the list the new item is placed.</span></span> <span data-ttu-id="d370e-190">Se a lista for classificada para que os itens mais antigos (por data/hora de recebimento) sejam os primeiros, não há nenhuma causa para se preocupar com esse cenário.</span><span class="sxs-lookup"><span data-stu-id="d370e-190">If the list is sorted so that the oldest items (by received date/time) are first, there's no cause for concern in this scenario.</span></span> <span data-ttu-id="d370e-191">O novo item será posicionado no final da lista e será incluído na segunda resposta.</span><span class="sxs-lookup"><span data-stu-id="d370e-191">The new item will be placed at the end of the list, and will be included in the second response.</span></span>
  
<span data-ttu-id="d370e-192">**Figura 3. Solicitar dez itens com deslocamento dez desde o início de uma lista com 16 itens, com o 16º item na lista sendo novo**</span><span class="sxs-lookup"><span data-stu-id="d370e-192">**Figure 3. Requesting 10 items at offset 10 from the beginning of a list of 16 items, with the 16th item in the list being new**</span></span>

![A diagram showing the results of requesting 10 items at offset 10 from the beginning of a list of 16 items when the 16th item was added to the end of the list.](media/Ex15_PagedSearch_SecondPage_NewItemEnd.png)
  
<span data-ttu-id="d370e-194">A história é diferente se a lista for classificada para que os itens mais recentes apareçam primeiro.</span><span class="sxs-lookup"><span data-stu-id="d370e-194">If the list is sorted so that the newest items are first, it's a different story.</span></span> <span data-ttu-id="d370e-195">Nesse caso, o primeiro item na segunda solicitação seria o último item da solicitação anterior mais os cinco itens restantes dos 15 itens originais.</span><span class="sxs-lookup"><span data-stu-id="d370e-195">In this case, the first item in the second request would be the last item from the previous request plus the remaining five items from the original 15.</span></span> <span data-ttu-id="d370e-196">Para colocá-lo em termos da nossa janela mágica imaginária, você mudou a posição da janela para 10, mas os próprios painéis também mudaram 1 posição.</span><span class="sxs-lookup"><span data-stu-id="d370e-196">To put it in terms of our imaginary magical window, you shifted your window's position by 10, but the billboards themselves also shifted by 1.</span></span>
  
<span data-ttu-id="d370e-197">**Figura 4. Solicitar dez itens com deslocamento dez desde o início de uma lista com 16 itens, com o primeiro item da lista sendo novo**</span><span class="sxs-lookup"><span data-stu-id="d370e-197">**Figure 4. Requesting 10 items at offset 10 from the beginning of a list of 16 items, with the first item in the list being new**</span></span>

![A diagram showing the results of asking for 10 items at offset 10 from the beginning of a list of 16 items when the 16th item was added to the beginning of the list.](media/Ex15_PagedSearch_SecondPage_NewItemBeginning.png)
  
<span data-ttu-id="d370e-199">Uma maneira de detectar uma alteração nos resultados no servidor é usar o conceito de um item de âncora.</span><span class="sxs-lookup"><span data-stu-id="d370e-199">One way to detect a change to the results on the server is to use the concept of an anchor item.</span></span> <span data-ttu-id="d370e-200">Um item de âncora é um item adicional na resposta que não é processado juntamente com o restante dos resultados, mas é usado para comparar com os próximos resultados para ver se os itens propriamente ditos foram deslocados.</span><span class="sxs-lookup"><span data-stu-id="d370e-200">An anchor item is an additional item in your response that is not processed along with the rest of the results, but is used to compare with the next results to see if the items themselves have shifted.</span></span> <span data-ttu-id="d370e-201">Retomando o nosso exemplo, se o aplicativo estiver usando um tamanho de "janela" dez, você, na verdade, define o número máximo de itens a serem retornados para 11.</span><span class="sxs-lookup"><span data-stu-id="d370e-201">Building again on our simple example, if your application is using a "window" size of 10, you actually set the maximum number of items to return to 11.</span></span> <span data-ttu-id="d370e-202">O aplicativo processa os primeiros dez itens na resposta como de costume.</span><span class="sxs-lookup"><span data-stu-id="d370e-202">Your application processes the first 10 items in the response as usual.</span></span> <span data-ttu-id="d370e-203">Para o último item, você salva o identificador do item como uma âncora e emite a próxima solicitação com um deslocamento dez.</span><span class="sxs-lookup"><span data-stu-id="d370e-203">For the last item, you save the item's identifier as an anchor, then issue the next request with an offset of 10.</span></span> <span data-ttu-id="d370e-204">Se os dados não forem alterados, o primeiro item na segunda resposta deve ter um identificador de item que corresponda à âncora.</span><span class="sxs-lookup"><span data-stu-id="d370e-204">If the data has not changed, the first item in the second response should have an item identifier that matches the anchor.</span></span> <span data-ttu-id="d370e-205">Se os identificadores de item não corresponderem, você saberá que os dados foram removidos ou inseridos nas partes da lista que já se encontravam "paginados".</span><span class="sxs-lookup"><span data-stu-id="d370e-205">If the item identifiers don't match, you know that the data has been removed or inserted in the parts of the list you have already "paged" over.</span></span>
  
<span data-ttu-id="d370e-206">Mesmo quando souber que os dados foram alterados, ainda será preciso decidir como reagir.</span><span class="sxs-lookup"><span data-stu-id="d370e-206">Even when you know that the data has changed, you still need to decide how to react.</span></span> <span data-ttu-id="d370e-207">Não há uma única resposta para essa pergunta.</span><span class="sxs-lookup"><span data-stu-id="d370e-207">There isn't a one-size-fits-all answer for this question either.</span></span> <span data-ttu-id="d370e-208">Suas ações dependerão da natureza do aplicativo e de quanto será importante capturar todos os itens.</span><span class="sxs-lookup"><span data-stu-id="d370e-208">Your actions will depend on the nature of your application and how critical it is to capture all items.</span></span> <span data-ttu-id="d370e-209">Você pode ignorá-la completamente, reiniciar o processo do começo ou controlar novamente e tentar detectar onde ocorreu a alteração.</span><span class="sxs-lookup"><span data-stu-id="d370e-209">You might ignore it altogether, restart the process from the beginning, or back track and try to detect where the change happened.</span></span>
  
## <a name="example-perform-a-paged-search-by-using-the-ews-managed-api"></a><span data-ttu-id="d370e-210">Exemplo: executar uma pesquisa de paginação usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="d370e-210">Example: Perform a paged search by using the EWS Managed API</span></span>
<span data-ttu-id="d370e-211"><a name="bk_PagedSearchEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="d370e-211"><a name="bk_PagedSearchEWSMA"> </a></span></span>

<span data-ttu-id="d370e-212">A paginação é compatível com os seguintes métodos da API gerenciada do EWS:</span><span class="sxs-lookup"><span data-stu-id="d370e-212">Paging is supported by the following EWS Managed API methods:</span></span>
  
- [<span data-ttu-id="d370e-213">ExchangeService.FindFolders</span><span class="sxs-lookup"><span data-stu-id="d370e-213">ExchangeService.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="d370e-214">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="d370e-214">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="d370e-215">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="d370e-215">Folder.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="d370e-216">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="d370e-216">Folder.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
<span data-ttu-id="d370e-217">Se você estiver usando a API gerenciada do EWS, seu aplicativo configurará a paginação com a classe [ItemView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) ou [FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx), e receberá informações do servidor em relação à paginação da classe [FindItemsResults](https://msdn.microsoft.com/library/dd635381%28v=exchg.80%29.aspx) ou [FindFoldersResults](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="d370e-217">If you are using the EWS Managed API, your application configures paging with the [ItemView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) or [FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) class and receives information from the server regarding paging from the [FindItemsResults](https://msdn.microsoft.com/library/dd635381%28v=exchg.80%29.aspx) or [FindFoldersResults](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx) class.</span></span> 
  
<span data-ttu-id="d370e-218">O exemplo a seguir recupera todos os itens de uma pasta usando uma pesquisa de paginação que retorna cinco itens em cada resposta.</span><span class="sxs-lookup"><span data-stu-id="d370e-218">The following example retrieves all the items in a folder using a paged search that returns five items in each response.</span></span> <span data-ttu-id="d370e-219">Ele também recupera um item adicional para servir como uma âncora para detectar alterações nos resultados no servidor.</span><span class="sxs-lookup"><span data-stu-id="d370e-219">It also retrieves an additional item to serve as an anchor to detect changes to the results on the server.</span></span> 
  
<span data-ttu-id="d370e-220">Este exemplo supõe que o objeto **ExchangeService** tenha sido inicializado com valores válidos nas propriedades [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) e [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="d370e-220">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void PageSearchItems(ExchangeService service, WellKnownFolderName folder)
{
    int pageSize = 5;
    int offset = 0;
    // Request one more item than your actual pageSize.
    // This will be used to detect a change to the result
    // set while paging.
    ItemView view = new ItemView(pageSize + 1, offset);
    view.PropertySet = new PropertySet(ItemSchema.Subject);
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    view.Traversal = ItemTraversal.Shallow;
    bool moreItems = true;
    ItemId anchorId = null;
    while (moreItems)
    {
        try
        {
            FindItemsResults<Item> results = service.FindItems(folder, view);
            moreItems = results.MoreAvailable;
            if (moreItems && anchorId != null)
            {
                // Check the first result to make sure it matches
                // the last result (anchor) from the previous page.
                // If it doesn't, that means that something was added
                // or deleted since you started the search.
                if (results.Items.First<Item>().Id != anchorId)
                {
                    Console.WriteLine("The collection has changed while paging. Some results may be missed.");
                }
            }
            if (moreItems)
                view.Offset += pageSize;
                
            anchorId = results.Items.Last<Item>().Id;
            
            // Because you're including an additional item on the end of your results
            // as an anchor, you don't want to display it.
            // Set the number to loop as the smaller value between
            // the number of items in the collection and the page size.
            int displayCount = 0;
            if ((results.MoreAvailable == false && results.Items.Count > pageSize) || (results.Items.Count < pageSize))
            {
                displayCount = results.Items.Count;
            }
            else
            {
                displayCount = pageSize;
            }
            
            for (int i = 0; i < displayCount; i++)
            {
                Item item = results.Items[i];
                Console.WriteLine("Subject: {0}", item.Subject);
                Console.WriteLine("Id: {0}\n", item.Id.ToString());
            }
        }
        catch (Exception ex)
        {
            Console.WriteLine("Exception while paging results: {0}", ex.Message);
        }
    }
}
```

## <a name="example-perform-a-paged-search-by-using-ews"></a><span data-ttu-id="d370e-221">Exemplo: executar uma pesquisa de paginação usando o EWS</span><span class="sxs-lookup"><span data-stu-id="d370e-221">Example: Perform a paged search by using EWS</span></span>
<span data-ttu-id="d370e-222"><a name="bk_PagedSearchEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="d370e-222"><a name="bk_PagedSearchEWS"> </a></span></span>

<span data-ttu-id="d370e-223">A paginação é compatível com as seguintes operações do EWS:</span><span class="sxs-lookup"><span data-stu-id="d370e-223">Paging is supported by the following EWS operations:</span></span>
  
- [<span data-ttu-id="d370e-224">FindFolder</span><span class="sxs-lookup"><span data-stu-id="d370e-224">FindFolder</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [<span data-ttu-id="d370e-225">FindItem</span><span class="sxs-lookup"><span data-stu-id="d370e-225">FindItem</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
<span data-ttu-id="d370e-226">Se você estiver usando o EWS, seu aplicativo configura a paginação com o elemento [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) e recebe informações do servidor de paginação do elemento [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) ou [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="d370e-226">If you're using EWS, your application configures paging with the [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element or the [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) element and receives information from the server regarding paging from the [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) element or the [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) element.</span></span> 
  
<span data-ttu-id="d370e-227">Neste exemplo de solicitação, uma solicitação **FindItem** é enviada para um máximo de seis itens, começando com um deslocamento de zero do início da lista de itens na caixa de entrada do usuário.</span><span class="sxs-lookup"><span data-stu-id="d370e-227">In this request example, a **FindItem** request is sent for a maximum of six items, starting at an offset of zero from the beginning of the list of items in the user's Inbox.</span></span> 
  
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
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="6" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="d370e-228">O servidor retorna esta resposta, a qual contém seis itens.</span><span class="sxs-lookup"><span data-stu-id="d370e-228">The server returns the following response, which contains six items.</span></span> <span data-ttu-id="d370e-229">A resposta também indica que há um total de oito itens nos resultados no servidor e que o último item na lista de resultados não está presente nesta resposta.</span><span class="sxs-lookup"><span data-stu-id="d370e-229">The response also indicates that there are a total of eight items in the results on the server, and that the last item in the results list is not present in this response.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
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
          <m:RootFolder IndexedPagingOffset="6" TotalItemsInView="8" IncludesLastItemInRange="false">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Query</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Update</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Planning resources</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Timeline</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>For your perusal</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>meeting notes</t:Subject>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="d370e-230">Neste exemplo, a mesma solicitação é enviada, mas desta vez, o atributo **Offset** é alterado para cinco, o que indica que o servidor deve retornar no máximo seis itens que começam no deslocamento cinco do começo.</span><span class="sxs-lookup"><span data-stu-id="d370e-230">In this example, the same request is sent, but this time, the **Offset** attribute is changed to five, which indicates that the server should return at most six items starting at offset five from the beginning.</span></span> 
  
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
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="6" Offset="5" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="d370e-231">O servidor envia essa resposta, a qual contém três itens.</span><span class="sxs-lookup"><span data-stu-id="d370e-231">The server sends the following response, which contains three items.</span></span> <span data-ttu-id="d370e-232">A resposta também indica que o total de número de itens nos resultados no servidor ainda é oito, e que o último item na lista de resultados está presente nessa resposta.</span><span class="sxs-lookup"><span data-stu-id="d370e-232">The response also indicates that the total number of items in the results on the server is still eight, and that the last item in the results list is included in this response.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
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
          <m:RootFolder IndexedPagingOffset="8" TotalItemsInView="8" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>meeting notes</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Meeting notes</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>This cat is hilarious!</t:Subject>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="d370e-233">Confira também</span><span class="sxs-lookup"><span data-stu-id="d370e-233">See also</span></span>


- [<span data-ttu-id="d370e-234">Pesquisa e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d370e-234">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)
    
- [<span data-ttu-id="d370e-235">Método ExchangeService.FindFolders</span><span class="sxs-lookup"><span data-stu-id="d370e-235">ExchangeService.FindFolders method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="d370e-236">Método ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="d370e-236">ExchangeService.FindItems method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="d370e-237">Método Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="d370e-237">Folder.FindFolders method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="d370e-238">Método Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="d370e-238">Folder.FindFolders method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="d370e-239">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="d370e-239">FindFolder operation</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [<span data-ttu-id="d370e-240">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="d370e-240">FindItem operation</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- [<span data-ttu-id="d370e-241">Limitação do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d370e-241">EWS throttling in Exchange</span></span>](ews-throttling-in-exchange.md)
    

