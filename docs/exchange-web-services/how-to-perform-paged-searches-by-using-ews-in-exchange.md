---
title: Executar pesquisas paginadas usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 64ed70e4-32eb-4c25-bfc4-43d1477296e5
description: Descubra como realizar pesquisas paginadas em sua API gerenciada do EWS ou aplicativo EWS que tem como alvo o Exchange.
localization_priority: Priority
ms.openlocfilehash: 2b608584918c936f62883b8b444d59c05c5952ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456821"
---
# <a name="perform-paged-searches-by-using-ews-in-exchange"></a><span data-ttu-id="ae149-103">Executar pesquisas paginadas usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ae149-103">Perform paged searches by using EWS in Exchange</span></span>

<span data-ttu-id="ae149-104">Descubra como realizar pesquisas paginadas em sua API gerenciada do EWS ou aplicativo EWS que tem como alvo o Exchange.</span><span class="sxs-lookup"><span data-stu-id="ae149-104">Find out how to perform paged searches in your EWS Managed API or EWS application that targets Exchange.</span></span>
  
<span data-ttu-id="ae149-105">Paginação é um recurso do EWS que permite controlar o tamanho dos resultados de uma pesquisa.</span><span class="sxs-lookup"><span data-stu-id="ae149-105">Paging is a feature in EWS that enables you to control the size of the results of a search.</span></span> <span data-ttu-id="ae149-106">Em vez de recuperar todo o conjunto de resultados em uma resposta do EWS, você pode recuperar conjuntos menores em várias respostas do EWS.</span><span class="sxs-lookup"><span data-stu-id="ae149-106">Rather than retrieve the entire result set in one EWS response, you can retrieve smaller sets in multiple EWS responses.</span></span> <span data-ttu-id="ae149-107">Por exemplo, considere um usuário com 10.000 mensagens de email na caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="ae149-107">For example, consider a user with 10,000 email messages in their Inbox.</span></span> <span data-ttu-id="ae149-108">De forma hipotética, você pode recuperar todos os emails 10.000 em uma resposta muito grande, mas você pode querer desmembrar isso em partes mais gerenciáveis para fins de largura de banda ou desempenho.</span><span class="sxs-lookup"><span data-stu-id="ae149-108">Hypothetically, you could retrieve all 10,000 emails in one very large response, but you might want to break that up into more manageable chunks for bandwidth or performance reasons.</span></span> <span data-ttu-id="ae149-109">A paginação fornece as ferramentas para fazer exatamente isso.</span><span class="sxs-lookup"><span data-stu-id="ae149-109">Paging gives you the tools to do just that.</span></span>
  
> [!NOTE]
> <span data-ttu-id="ae149-110">Embora você possa recuperar de fato 10.000 itens em uma única solicitação, na realidade, isso é improvável devido à limitação do EWS.</span><span class="sxs-lookup"><span data-stu-id="ae149-110">While you can hypothetically retrieve 10,000 items in one request, in reality, this is unlikely due to EWS throttling.</span></span> <span data-ttu-id="ae149-111">Para saber mais, confira [limitação do EWS no Exchange](ews-throttling-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="ae149-111">To find out more, see [EWS throttling in Exchange](ews-throttling-in-exchange.md).</span></span> 
  
<span data-ttu-id="ae149-112">**Tabela 1. Parâmetros de paginação na API gerenciada do EWS e EWS**</span><span class="sxs-lookup"><span data-stu-id="ae149-112">**Table 1. Paging parameters in the EWS Managed API and EWS**</span></span>

|<span data-ttu-id="ae149-113">**Para configurar ou recuperar o...**</span><span class="sxs-lookup"><span data-stu-id="ae149-113">**To configure or retrieve the…**</span></span>|<span data-ttu-id="ae149-114">**Na API gerenciada do EWS, use...**</span><span class="sxs-lookup"><span data-stu-id="ae149-114">**In the EWS Managed API, use…**</span></span>|<span data-ttu-id="ae149-115">**Em EWS, use...**</span><span class="sxs-lookup"><span data-stu-id="ae149-115">**In EWS, use…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ae149-116">Número máximo de itens ou pastas em uma resposta</span><span class="sxs-lookup"><span data-stu-id="ae149-116">Maximum number of items or folders in a response</span></span>  <br/> |<span data-ttu-id="ae149-117">O parâmetro **PageSize** para o [Construtor de AllViews](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) ou o [Construtor folderview](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ae149-117">The **pageSize** parameter to the [ItemView constructor](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) or the [FolderView constructor](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx)</span></span> <br/> <span data-ttu-id="ae149-118">Ou</span><span class="sxs-lookup"><span data-stu-id="ae149-118">Or</span></span>  <br/> <span data-ttu-id="ae149-119">A propriedade [PagedView. PageSize](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ae149-119">The [PagedView.PageSize](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="ae149-120">O atributo **MaxEntriesReturned** no elemento [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou no elemento [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ae149-120">The **MaxEntriesReturned** attribute on the [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element or the [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="ae149-121">Ponto de partida na lista de itens ou pastas</span><span class="sxs-lookup"><span data-stu-id="ae149-121">Starting point in the list of items or folders</span></span>  <br/> |<span data-ttu-id="ae149-122">O parâmetro **offsetBasePoint** para o construtor **AllViews** ou o construtor **folderview**</span><span class="sxs-lookup"><span data-stu-id="ae149-122">The **offsetBasePoint** parameter to the **ItemView** constructor or the **FolderView** constructor</span></span>  <br/> <span data-ttu-id="ae149-123">Ou</span><span class="sxs-lookup"><span data-stu-id="ae149-123">Or</span></span>  <br/> <span data-ttu-id="ae149-124">A propriedade [PagedView. OffsetBasePoint](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ae149-124">The [PagedView.OffsetBasePoint](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="ae149-125">O atributo **BasePoint** no elemento **IndexedPageItemView** ou no elemento **IndexedPageFolderView**</span><span class="sxs-lookup"><span data-stu-id="ae149-125">The **BasePoint** attribute on the **IndexedPageItemView** element or the **IndexedPageFolderView** element</span></span>  <br/> |
|<span data-ttu-id="ae149-126">Deslocamento a partir do ponto de partida</span><span class="sxs-lookup"><span data-stu-id="ae149-126">Offset from the starting point</span></span>  <br/> |<span data-ttu-id="ae149-127">O parâmetro **offset** para o construtor de **AllViews** ou o construtor **folderview**</span><span class="sxs-lookup"><span data-stu-id="ae149-127">The **offset** parameter to the **ItemView** constructor or the **FolderView** constructor</span></span>  <br/> <span data-ttu-id="ae149-128">Ou</span><span class="sxs-lookup"><span data-stu-id="ae149-128">Or</span></span>  <br/> <span data-ttu-id="ae149-129">A propriedade [PagedView. Offset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ae149-129">The [PagedView.Offset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="ae149-130">O atributo **offset** no elemento **IndexedPageItemView** ou o elemento **IndexedPageFolderView**</span><span class="sxs-lookup"><span data-stu-id="ae149-130">The **Offset** attribute on the **IndexedPageItemView** element or the **IndexedPageFolderView** element</span></span>  <br/> |
|<span data-ttu-id="ae149-131">Número total de resultados no servidor</span><span class="sxs-lookup"><span data-stu-id="ae149-131">Total number of results on the server</span></span>  <br/> |<span data-ttu-id="ae149-132">A propriedade [FindItemsResults. TotalCount](https://msdn.microsoft.com/library/dd635348%28v=exchg.80%29.aspx) ou a propriedade [FindFoldersResults. TotalCount](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ae149-132">The [FindItemsResults.TotalCount](https://msdn.microsoft.com/library/dd635348%28v=exchg.80%29.aspx) property or the [FindFoldersResults.TotalCount](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="ae149-133">O atributo **TotalItemsInView** no elemento [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) ou no elemento [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ae149-133">The **TotalItemsInView** attribute on the [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) element or the [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="ae149-134">Deslocamento do primeiro item ou pasta não incluído na resposta atual</span><span class="sxs-lookup"><span data-stu-id="ae149-134">Offset of first item or folder not included in current response</span></span>  <br/> |<span data-ttu-id="ae149-135">A propriedade [FindItemsResults. NextPageOffset](https://msdn.microsoft.com/library/ee693014%28v=exchg.80%29.aspx) ou a propriedade [FindFoldersResults. NextPageOffset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ae149-135">The [FindItemsResults.NextPageOffset](https://msdn.microsoft.com/library/ee693014%28v=exchg.80%29.aspx) property or the [FindFoldersResults.NextPageOffset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="ae149-136">O atributo **IndexedPagingOffset** no elemento **RootFolder**</span><span class="sxs-lookup"><span data-stu-id="ae149-136">The **IndexedPagingOffset** attribute on the **RootFolder** element</span></span>  <br/> |
|<span data-ttu-id="ae149-137">Indicador de que a resposta inclui o último item ou pasta na lista</span><span class="sxs-lookup"><span data-stu-id="ae149-137">Indicator that response includes the last item or folder in the list</span></span>  <br/> |<span data-ttu-id="ae149-138">A propriedade [FindItemsResults. MoreAvailable](https://msdn.microsoft.com/library/dd635477%28v=exchg.80%29.aspx) ou a propriedade [FindFoldersResults. MoreAvailable](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="ae149-138">The [FindItemsResults.MoreAvailable](https://msdn.microsoft.com/library/dd635477%28v=exchg.80%29.aspx) property or the [FindFoldersResults.MoreAvailable](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="ae149-139">O atributo **IncludesLastItemInRange** no elemento **RootFolder**</span><span class="sxs-lookup"><span data-stu-id="ae149-139">The **IncludesLastItemInRange** attribute on the **RootFolder** element</span></span>  <br/> |
   
## <a name="how-paging-works"></a><span data-ttu-id="ae149-140">Como a paginação funciona</span><span class="sxs-lookup"><span data-stu-id="ae149-140">How paging works</span></span>
<span data-ttu-id="ae149-141"><a name="bk_HowPagingWorks"> </a></span><span class="sxs-lookup"><span data-stu-id="ae149-141"><a name="bk_HowPagingWorks"> </a></span></span>

<span data-ttu-id="ae149-142">Para entender como a paginação funciona, é útil visualizar as mensagens em uma pasta como os murals alinhados lado a lado em um campo fora da sua casa.</span><span class="sxs-lookup"><span data-stu-id="ae149-142">To understand how paging works, it's helpful to visualize the messages in a folder as billboards lined up side by side in a field outside your house.</span></span> <span data-ttu-id="ae149-143">Você pode ver algumas dessas mensagems por meio de uma janela do Magical.</span><span class="sxs-lookup"><span data-stu-id="ae149-143">You can see some of these billboards through a magical window.</span></span> <span data-ttu-id="ae149-144">Você pode alterar o tamanho da janela (para ver mais ou menos mensagens de uma vez) e mover a janela (para controlar quais mensagens você pode ver).</span><span class="sxs-lookup"><span data-stu-id="ae149-144">You have the ability to change the size of the window (to see more or fewer billboards at once) and to move the window (to control which billboards you can see).</span></span> <span data-ttu-id="ae149-145">Essa manipulação da janela é paginação.</span><span class="sxs-lookup"><span data-stu-id="ae149-145">This manipulation of the window is paging.</span></span> 
  
<span data-ttu-id="ae149-146">Ao enviar sua solicitação para o servidor do Exchange, você especifica o tamanho da janela em termos de quantos itens serão retornados.</span><span class="sxs-lookup"><span data-stu-id="ae149-146">When you send your request to the Exchange server, you specify the size of your window in terms of how many items to return.</span></span> <span data-ttu-id="ae149-147">Você define a posição da janela especificando um ponto de partida (o início da linha ou o final da linha) e um deslocamento a partir desse ponto inicial, expresso em um número de itens.</span><span class="sxs-lookup"><span data-stu-id="ae149-147">You set the position of the window by specifying a starting point (either the beginning of the line or the end of the line) and an offset from that starting point, expressed in a number of items.</span></span> <span data-ttu-id="ae149-148">O início da janela é o número de itens especificados pelo deslocamento a partir do ponto inicial.</span><span class="sxs-lookup"><span data-stu-id="ae149-148">The beginning of the window is the number of items specified by the offset from the starting point.</span></span>
  
<span data-ttu-id="ae149-149">Onde a paginação fica um pouco mais interessante é na resposta do servidor e como seu aplicativo pode usar essa resposta para forma sua próxima solicitação.</span><span class="sxs-lookup"><span data-stu-id="ae149-149">Where paging gets a bit more interesting is in the server's response, and how your application can use that response to shape its next request.</span></span> <span data-ttu-id="ae149-150">O servidor fornece três informações que você pode usar para determinar como configurar sua "janela" para sua próxima solicitação:</span><span class="sxs-lookup"><span data-stu-id="ae149-150">The server gives you three pieces of information that you can use to determine how to configure your "window" for your next request:</span></span> 
  
- <span data-ttu-id="ae149-151">Se os resultados na resposta incluem o último item no conjunto de resultados geral no servidor.</span><span class="sxs-lookup"><span data-stu-id="ae149-151">Whether the results in the response include the last item in the overall result set on the server.</span></span>
    
- <span data-ttu-id="ae149-152">O número total de itens no conjunto de resultados no servidor.</span><span class="sxs-lookup"><span data-stu-id="ae149-152">The total number of items in the result set on the server.</span></span>
    
- <span data-ttu-id="ae149-153">Qual será o próximo valor de deslocamento, se você quiser avançar a janela para o próximo item no conjunto de resultados que não está incluído na resposta atual.</span><span class="sxs-lookup"><span data-stu-id="ae149-153">What the next offset value should be, if you want to advance your window to the next item in the result set that isn't included in the current response.</span></span>
    
<span data-ttu-id="ae149-154">Vamos dar uma olhada em um exemplo simples.</span><span class="sxs-lookup"><span data-stu-id="ae149-154">Let's look at a simple example.</span></span> <span data-ttu-id="ae149-155">Imagine uma caixa de entrada com 15 mensagens.</span><span class="sxs-lookup"><span data-stu-id="ae149-155">Imagine an Inbox with 15 messages in it.</span></span> <span data-ttu-id="ae149-156">O aplicativo envia uma solicitação inicial para recuperar um máximo de 10 itens, começando no início da lista de mensagens (de modo que o deslocamento seja zero).</span><span class="sxs-lookup"><span data-stu-id="ae149-156">Your application sends an initial request to retrieve a maximum of 10 items, starting at the beginning of the list of messages (so the offset is zero).</span></span> <span data-ttu-id="ae149-157">O servidor responde com as 10 primeiras mensagens e indica que a resposta não inclui o último item, que há um total de 15 itens e que o próximo deslocamento deve ser 10.</span><span class="sxs-lookup"><span data-stu-id="ae149-157">The server responds with the first 10 messages, and indicates that the response does not include the last item, that there are a total of 15 items, and that the next offset should be 10.</span></span>
  
<span data-ttu-id="ae149-158">**Figura 1. Solicitar 10 itens no deslocamento 0 do início de uma lista de 15 itens**</span><span class="sxs-lookup"><span data-stu-id="ae149-158">**Figure 1. Requesting 10 items at offset 0 from the beginning of a list of 15 items**</span></span>

![A diagram showing the results of requesting 10 items at offset 0 from the beginning of a list of 15 items.](media/Ex15_PagedSearch_FirstPage.png)
  
<span data-ttu-id="ae149-160">Em seguida, o aplicativo reenvia a mesma solicitação para o servidor, com a única alteração que o deslocamento agora é 10.</span><span class="sxs-lookup"><span data-stu-id="ae149-160">Your application then resends the same request to the server, with the only change being that the offset is now 10.</span></span> <span data-ttu-id="ae149-161">O servidor retorna os últimos cinco itens e indica que a resposta inclui o último item, que há um total de 15 itens e que o próximo deslocamento deve ser 15 (porém, você chegou ao fim, portanto, não haverá um deslocamento próximo).</span><span class="sxs-lookup"><span data-stu-id="ae149-161">The server returns the last five items, and indicates that the response does include the last item, that there are a total of 15 items, and that the next offset should be 15 (though of course, you've reached the end, so there won't be a next offset.)</span></span>
  
<span data-ttu-id="ae149-162">**Figura 2. Solicitar 10 itens no deslocamento 10 do início de uma lista de 15 itens**</span><span class="sxs-lookup"><span data-stu-id="ae149-162">**Figure 2. Requesting 10 items at offset 10 from the beginning of a list of 15 items**</span></span>

![A diagram showing the results of requesting 10 items at offset 10 from the beginning of a list of 15 items.](media/Ex15_PagedSearch_SecondPage.png)
  
## <a name="design-considerations-for-paging"></a><span data-ttu-id="ae149-164">Considerações de design para paginação</span><span class="sxs-lookup"><span data-stu-id="ae149-164">Design considerations for paging</span></span>
<span data-ttu-id="ae149-165"><a name="bk_DesignConsiderations"> </a></span><span class="sxs-lookup"><span data-stu-id="ae149-165"><a name="bk_DesignConsiderations"> </a></span></span>

<span data-ttu-id="ae149-166">Tornar o máximo da paginação em seu aplicativo exige alguma consideração.</span><span class="sxs-lookup"><span data-stu-id="ae149-166">Making the most out of paging in your application does require some consideration.</span></span> <span data-ttu-id="ae149-167">Por exemplo, qual é o tamanho da "janela"?</span><span class="sxs-lookup"><span data-stu-id="ae149-167">For example, how large do you make your "window"?</span></span> <span data-ttu-id="ae149-168">O que fazer se os resultados no servidor mudarem enquanto você estiver movendo sua "janela"?</span><span class="sxs-lookup"><span data-stu-id="ae149-168">What do you do if the results on the server change while you're moving your "window"?</span></span>
  
### <a name="determine-the-size-of-your-window"></a><span data-ttu-id="ae149-169">Determinar o tamanho da janela</span><span class="sxs-lookup"><span data-stu-id="ae149-169">Determine the size of your window</span></span>

<span data-ttu-id="ae149-170">Não há um número máximo de entradas de "um tamanho para tudo" que todos os aplicativos devem usar.</span><span class="sxs-lookup"><span data-stu-id="ae149-170">There is no "one-size-fits-all" maximum number of entries that all applications should use.</span></span> <span data-ttu-id="ae149-171">Determinar o número certo para seu aplicativo depende de vários fatores diferentes.</span><span class="sxs-lookup"><span data-stu-id="ae149-171">Determining the number that's right for your application depends on several different factors.</span></span> <span data-ttu-id="ae149-172">No entanto, é útil manter as seguintes diretrizes em mente:</span><span class="sxs-lookup"><span data-stu-id="ae149-172">However, it's helpful to keep the following guidelines in mind:</span></span>
  
- <span data-ttu-id="ae149-173">Por padrão, o Exchange limita o número máximo de itens que podem ser retornados em uma única solicitação para 1000.</span><span class="sxs-lookup"><span data-stu-id="ae149-173">By default, Exchange limits the maximum number of items that can be returned in a single request to 1000.</span></span>
    
- <span data-ttu-id="ae149-174">Definir o número máximo de entradas para um número maior resulta em ter que enviar menos solicitações para obter todos os itens, ao custo de esperar mais por respostas.</span><span class="sxs-lookup"><span data-stu-id="ae149-174">Setting the maximum number of entries to a larger number results in having to send fewer requests to get all items, at the cost of having to wait longer for responses.</span></span>
    
- <span data-ttu-id="ae149-175">Definir o número máximo de entradas para um número menor resulta em tempos de resposta mais rápidos, ao custo de ter que enviar mais solicitações para obter todos os itens.</span><span class="sxs-lookup"><span data-stu-id="ae149-175">Setting the maximum number of entries to a smaller number results in quicker response times, at the cost of having to send more requests to get all items.</span></span>
    
### <a name="handling-changes-to-the-result-set"></a><span data-ttu-id="ae149-176">Gerenciar alterações no conjunto de resultados</span><span class="sxs-lookup"><span data-stu-id="ae149-176">Handling changes to the result set</span></span>

<span data-ttu-id="ae149-177">No exemplo simples, anteriormente neste artigo, o número de itens na caixa de entrada do usuário permaneceu constante.</span><span class="sxs-lookup"><span data-stu-id="ae149-177">In the simple example earlier in this article, the number of items in the user's Inbox remained constant.</span></span> <span data-ttu-id="ae149-178">No entanto, na realidade, o número de itens em uma caixa de entrada pode ser alterado com frequência.</span><span class="sxs-lookup"><span data-stu-id="ae149-178">However, in reality, the number of items in an Inbox can change frequently.</span></span> <span data-ttu-id="ae149-179">Novas mensagens podem chegar e os itens podem ser excluídos ou movidos a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="ae149-179">New messages can arrive and items can be deleted or moved at any time.</span></span> <span data-ttu-id="ae149-180">Mas como isso afeta a paginação?</span><span class="sxs-lookup"><span data-stu-id="ae149-180">But how does this impact paging?</span></span> <span data-ttu-id="ae149-181">Vamos modificar o cenário de exemplo anterior para descobrir.</span><span class="sxs-lookup"><span data-stu-id="ae149-181">Let's modify the earlier example scenario to find out.</span></span>
  
<span data-ttu-id="ae149-182">Vamos começar novamente com os 15 itens na caixa de entrada do usuário e enviar a mesma solicitação inicial.</span><span class="sxs-lookup"><span data-stu-id="ae149-182">We'll start again with the 15 items in the user's Inbox, and send the same initial request.</span></span> <span data-ttu-id="ae149-183">Como antes, o servidor responde com as 10 primeiras mensagens e indica que a resposta não inclui o último item, que há um total de 15 itens e que o próximo deslocamento deve ser 10, conforme mostrado na Figura 1.</span><span class="sxs-lookup"><span data-stu-id="ae149-183">As before, the server responds with the first 10 messages, and indicates that the response does not include the last item, that there are a total of 15 items, and that the next offset should be 10, as shown in Figure 1.</span></span>
  
<span data-ttu-id="ae149-184">Agora, enquanto o aplicativo está processando esses 10 itens, uma nova mensagem chega na caixa de entrada e é adicionada ao conjunto de resultados no servidor.</span><span class="sxs-lookup"><span data-stu-id="ae149-184">Now, while your application is processing those 10 items, a new message arrives in the Inbox and is added to the result set on the server.</span></span> <span data-ttu-id="ae149-185">O aplicativo reenvia a mesma solicitação para o servidor (somente com o deslocamento definido como 10).</span><span class="sxs-lookup"><span data-stu-id="ae149-185">Your application resends the same request to the server (only with the offset set to 10).</span></span> <span data-ttu-id="ae149-186">Desta vez, o servidor recebe o retorno de seis itens e indica que há um total de 16 itens no conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="ae149-186">This time the server gets back six items, and indicates that there are a total of 16 items in the result set.</span></span>
  
<span data-ttu-id="ae149-187">Neste ponto, você pode estar se perguntando se isso é um problema.</span><span class="sxs-lookup"><span data-stu-id="ae149-187">At this point you might be wondering if this is even a problem.</span></span> <span data-ttu-id="ae149-188">Afinal, você tem 16 itens de volta nas duas respostas, então por que todas as complicações?</span><span class="sxs-lookup"><span data-stu-id="ae149-188">After all, you got 16 items back over the two responses, so why all the fuss?</span></span> <span data-ttu-id="ae149-189">A resposta depende de onde o novo item é colocado na lista.</span><span class="sxs-lookup"><span data-stu-id="ae149-189">The answer depends on where in the list the new item is placed.</span></span> <span data-ttu-id="ae149-190">Se a lista for classificada de forma que os itens mais antigos (por data/hora de recebimento) sejam os primeiros, não há nenhuma causa de preocupação neste cenário.</span><span class="sxs-lookup"><span data-stu-id="ae149-190">If the list is sorted so that the oldest items (by received date/time) are first, there's no cause for concern in this scenario.</span></span> <span data-ttu-id="ae149-191">O novo item será colocado no final da lista e será incluído na segunda resposta.</span><span class="sxs-lookup"><span data-stu-id="ae149-191">The new item will be placed at the end of the list, and will be included in the second response.</span></span>
  
<span data-ttu-id="ae149-192">**Figura 3. Solicitar 10 itens no deslocamento 10 do início de uma lista de 16 itens, com o 16º item na lista sendo novo**</span><span class="sxs-lookup"><span data-stu-id="ae149-192">**Figure 3. Requesting 10 items at offset 10 from the beginning of a list of 16 items, with the 16th item in the list being new**</span></span>

![A diagram showing the results of requesting 10 items at offset 10 from the beginning of a list of 16 items when the 16th item was added to the end of the list.](media/Ex15_PagedSearch_SecondPage_NewItemEnd.png)
  
<span data-ttu-id="ae149-194">Se a lista for classificada de forma que os itens mais recentes sejam primeiro, ele será um texto diferente.</span><span class="sxs-lookup"><span data-stu-id="ae149-194">If the list is sorted so that the newest items are first, it's a different story.</span></span> <span data-ttu-id="ae149-195">Nesse caso, o primeiro item da segunda solicitação seria o último item da solicitação anterior mais os cinco itens restantes do original 15.</span><span class="sxs-lookup"><span data-stu-id="ae149-195">In this case, the first item in the second request would be the last item from the previous request plus the remaining five items from the original 15.</span></span> <span data-ttu-id="ae149-196">Para colocá-lo em termos de nossa janela imaginária Magical, você moveu a posição da sua janela por 10, mas os próprios murals também foram deslocados por 1.</span><span class="sxs-lookup"><span data-stu-id="ae149-196">To put it in terms of our imaginary magical window, you shifted your window's position by 10, but the billboards themselves also shifted by 1.</span></span>
  
<span data-ttu-id="ae149-197">**Figura 4. Solicitar 10 itens no deslocamento 10 do início de uma lista de 16 itens, com o primeiro item da lista sendo novo**</span><span class="sxs-lookup"><span data-stu-id="ae149-197">**Figure 4. Requesting 10 items at offset 10 from the beginning of a list of 16 items, with the first item in the list being new**</span></span>

![A diagram showing the results of asking for 10 items at offset 10 from the beginning of a list of 16 items when the 16th item was added to the beginning of the list.](media/Ex15_PagedSearch_SecondPage_NewItemBeginning.png)
  
<span data-ttu-id="ae149-199">Uma maneira de detectar uma alteração nos resultados no servidor é usar o conceito de um item de âncora.</span><span class="sxs-lookup"><span data-stu-id="ae149-199">One way to detect a change to the results on the server is to use the concept of an anchor item.</span></span> <span data-ttu-id="ae149-200">Um item de âncora é um item adicional em sua resposta que não é processado junto com o restante dos resultados, mas é usado para comparar com os próximos resultados para ver se os itens em si foram deslocados.</span><span class="sxs-lookup"><span data-stu-id="ae149-200">An anchor item is an additional item in your response that is not processed along with the rest of the results, but is used to compare with the next results to see if the items themselves have shifted.</span></span> <span data-ttu-id="ae149-201">Criando novamente em nosso exemplo simples, se o aplicativo estiver usando um tamanho de "janela" de 10, você realmente definirá o número máximo de itens para retornar a 11.</span><span class="sxs-lookup"><span data-stu-id="ae149-201">Building again on our simple example, if your application is using a "window" size of 10, you actually set the maximum number of items to return to 11.</span></span> <span data-ttu-id="ae149-202">Seu aplicativo processa os primeiros 10 itens na resposta como de costume.</span><span class="sxs-lookup"><span data-stu-id="ae149-202">Your application processes the first 10 items in the response as usual.</span></span> <span data-ttu-id="ae149-203">Para o último item, você salva o identificador do item como uma âncora e, em seguida, emite a próxima solicitação com um deslocamento de 10.</span><span class="sxs-lookup"><span data-stu-id="ae149-203">For the last item, you save the item's identifier as an anchor, then issue the next request with an offset of 10.</span></span> <span data-ttu-id="ae149-204">Se os dados não tiverem sido alterados, o primeiro item da segunda resposta deverá ter um identificador de item que corresponda à âncora.</span><span class="sxs-lookup"><span data-stu-id="ae149-204">If the data has not changed, the first item in the second response should have an item identifier that matches the anchor.</span></span> <span data-ttu-id="ae149-205">Se os identificadores de item não forem correspondentes, você saberá que os dados foram removidos ou inseridos nas partes da lista que você já "pausou".</span><span class="sxs-lookup"><span data-stu-id="ae149-205">If the item identifiers don't match, you know that the data has been removed or inserted in the parts of the list you have already "paged" over.</span></span>
  
<span data-ttu-id="ae149-206">Mesmo quando você sabe que os dados foram alterados, ainda precisa decidir como reagir.</span><span class="sxs-lookup"><span data-stu-id="ae149-206">Even when you know that the data has changed, you still need to decide how to react.</span></span> <span data-ttu-id="ae149-207">Não há uma resposta de tamanho único para essa pergunta.</span><span class="sxs-lookup"><span data-stu-id="ae149-207">There isn't a one-size-fits-all answer for this question either.</span></span> <span data-ttu-id="ae149-208">Suas ações dependerão da natureza do seu aplicativo e de como é essencial capturar todos os itens.</span><span class="sxs-lookup"><span data-stu-id="ae149-208">Your actions will depend on the nature of your application and how critical it is to capture all items.</span></span> <span data-ttu-id="ae149-209">Você pode ignorá-lo, reiniciar o processo do início ou do controle de volta e tentar detectar onde a alteração ocorreu.</span><span class="sxs-lookup"><span data-stu-id="ae149-209">You might ignore it altogether, restart the process from the beginning, or back track and try to detect where the change happened.</span></span>
  
## <a name="example-perform-a-paged-search-by-using-the-ews-managed-api"></a><span data-ttu-id="ae149-210">Exemplo: executar uma pesquisa paginada usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="ae149-210">Example: Perform a paged search by using the EWS Managed API</span></span>
<span data-ttu-id="ae149-211"><a name="bk_PagedSearchEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="ae149-211"><a name="bk_PagedSearchEWSMA"> </a></span></span>

<span data-ttu-id="ae149-212">A paginação é suportada pelos seguintes métodos da API gerenciada do EWS:</span><span class="sxs-lookup"><span data-stu-id="ae149-212">Paging is supported by the following EWS Managed API methods:</span></span>
  
- [<span data-ttu-id="ae149-213">ExchangeService. FindFolders</span><span class="sxs-lookup"><span data-stu-id="ae149-213">ExchangeService.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="ae149-214">ExchangeService. FindItems</span><span class="sxs-lookup"><span data-stu-id="ae149-214">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="ae149-215">Folder. FindFolders</span><span class="sxs-lookup"><span data-stu-id="ae149-215">Folder.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="ae149-216">Folder. FindFolders</span><span class="sxs-lookup"><span data-stu-id="ae149-216">Folder.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
<span data-ttu-id="ae149-217">Se você estiver usando a API gerenciada do EWS, seu aplicativo configurará a paginação com o [DefaultView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) ou a classe [folderview](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) e receberá informações do servidor referente à paginação na classe [FindItemsResults](https://msdn.microsoft.com/library/dd635381%28v=exchg.80%29.aspx) ou [FindFoldersResults](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ae149-217">If you are using the EWS Managed API, your application configures paging with the [ItemView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) or [FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) class and receives information from the server regarding paging from the [FindItemsResults](https://msdn.microsoft.com/library/dd635381%28v=exchg.80%29.aspx) or [FindFoldersResults](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx) class.</span></span> 
  
<span data-ttu-id="ae149-218">O exemplo a seguir recupera todos os itens em uma pasta usando uma pesquisa paginada que retorna cinco itens em cada resposta.</span><span class="sxs-lookup"><span data-stu-id="ae149-218">The following example retrieves all the items in a folder using a paged search that returns five items in each response.</span></span> <span data-ttu-id="ae149-219">Ele também recupera um item adicional para servir como uma âncora para detectar alterações nos resultados no servidor.</span><span class="sxs-lookup"><span data-stu-id="ae149-219">It also retrieves an additional item to serve as an anchor to detect changes to the results on the server.</span></span> 
  
<span data-ttu-id="ae149-220">Este exemplo pressupõe que o objeto **ExchangeService** tenha sido inicializado com valores válidos nas propriedades de [credenciais](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) e [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ae149-220">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
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
            if (moreItems &amp;&amp; anchorId != null)
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
            int displayCount = results.Items.Count > pageSize ? pageSize : results.Items.Count;
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

## <a name="example-perform-a-paged-search-by-using-ews"></a><span data-ttu-id="ae149-221">Exemplo: executar uma pesquisa paginada usando o EWS</span><span class="sxs-lookup"><span data-stu-id="ae149-221">Example: Perform a paged search by using EWS</span></span>
<span data-ttu-id="ae149-222"><a name="bk_PagedSearchEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="ae149-222"><a name="bk_PagedSearchEWS"> </a></span></span>

<span data-ttu-id="ae149-223">A paginação é suportada pelas seguintes operações do EWS:</span><span class="sxs-lookup"><span data-stu-id="ae149-223">Paging is supported by the following EWS operations:</span></span>
  
- [<span data-ttu-id="ae149-224">FindFolder</span><span class="sxs-lookup"><span data-stu-id="ae149-224">FindFolder</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [<span data-ttu-id="ae149-225">FindItem</span><span class="sxs-lookup"><span data-stu-id="ae149-225">FindItem</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
<span data-ttu-id="ae149-226">Se você estiver usando o EWS, o aplicativo configurará a paginação com o elemento [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou o elemento [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) e receberá informações do servidor em relação à paginação a partir do elemento [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) ou do elemento [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ae149-226">If you're using EWS, your application configures paging with the [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element or the [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) element and receives information from the server regarding paging from the [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) element or the [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) element.</span></span> 
  
<span data-ttu-id="ae149-227">Neste exemplo de solicitação, uma solicitação **FindItem** é enviada para um máximo de seis itens, começando em um deslocamento de zero do início da lista de itens na caixa de entrada do usuário.</span><span class="sxs-lookup"><span data-stu-id="ae149-227">In this request example, a **FindItem** request is sent for a maximum of six items, starting at an offset of zero from the beginning of the list of items in the user's Inbox.</span></span> 
  
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

<span data-ttu-id="ae149-228">O servidor retorna a seguinte resposta, que contém seis itens.</span><span class="sxs-lookup"><span data-stu-id="ae149-228">The server returns the following response, which contains six items.</span></span> <span data-ttu-id="ae149-229">A resposta também indica que há um total de oito itens nos resultados no servidor e que o último item na lista de resultados não está presente nesta resposta.</span><span class="sxs-lookup"><span data-stu-id="ae149-229">The response also indicates that there are a total of eight items in the results on the server, and that the last item in the results list is not present in this response.</span></span>
  
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

<span data-ttu-id="ae149-230">Neste exemplo, a mesma solicitação é enviada, mas desta vez, o atributo **offset** é alterado para cinco, o que indica que o servidor deve retornar no máximo seis itens começando no deslocamento cinco do início.</span><span class="sxs-lookup"><span data-stu-id="ae149-230">In this example, the same request is sent, but this time, the **Offset** attribute is changed to five, which indicates that the server should return at most six items starting at offset five from the beginning.</span></span> 
  
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

<span data-ttu-id="ae149-231">O servidor envia a seguinte resposta, que contém três itens.</span><span class="sxs-lookup"><span data-stu-id="ae149-231">The server sends the following response, which contains three items.</span></span> <span data-ttu-id="ae149-232">A resposta também indica que o número total de itens nos resultados no servidor ainda é oito e que o último item na lista de resultados está incluído nesta resposta.</span><span class="sxs-lookup"><span data-stu-id="ae149-232">The response also indicates that the total number of items in the results on the server is still eight, and that the last item in the results list is included in this response.</span></span>
  
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

## <a name="see-also"></a><span data-ttu-id="ae149-233">Confira também</span><span class="sxs-lookup"><span data-stu-id="ae149-233">See also</span></span>


- [<span data-ttu-id="ae149-234">Pesquisar e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ae149-234">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)
    
- [<span data-ttu-id="ae149-235">Método ExchangeService. FindFolders</span><span class="sxs-lookup"><span data-stu-id="ae149-235">ExchangeService.FindFolders method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="ae149-236">Método ExchangeService. FindItems</span><span class="sxs-lookup"><span data-stu-id="ae149-236">ExchangeService.FindItems method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="ae149-237">Método Folder. FindFolders</span><span class="sxs-lookup"><span data-stu-id="ae149-237">Folder.FindFolders method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="ae149-238">Método Folder. FindFolders</span><span class="sxs-lookup"><span data-stu-id="ae149-238">Folder.FindFolders method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="ae149-239">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="ae149-239">FindFolder operation</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [<span data-ttu-id="ae149-240">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="ae149-240">FindItem operation</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- [<span data-ttu-id="ae149-241">Limitação do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ae149-241">EWS throttling in Exchange</span></span>](ews-throttling-in-exchange.md)
    

