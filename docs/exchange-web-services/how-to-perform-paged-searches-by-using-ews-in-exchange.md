---
title: Realizar pesquisas paginadas utilizando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 64ed70e4-32eb-4c25-bfc4-43d1477296e5
description: Descubra como realizar pesquisas paginadas em sua API gerenciada de EWS ou aplicativos do EWS que tem como destino o Exchange.
ms.openlocfilehash: 3f82f46d0582b0b7ff8be63de8a7054b5f3cacab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750806"
---
# <a name="perform-paged-searches-by-using-ews-in-exchange"></a><span data-ttu-id="623c8-103">Realizar pesquisas paginadas utilizando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="623c8-103">Perform paged searches by using EWS in Exchange</span></span>

<span data-ttu-id="623c8-104">Descubra como realizar pesquisas paginadas em sua API gerenciada de EWS ou aplicativos do EWS que tem como destino o Exchange.</span><span class="sxs-lookup"><span data-stu-id="623c8-104">Find out how to perform paged searches in your EWS Managed API or EWS application that targets Exchange.</span></span>
  
<span data-ttu-id="623c8-105">Paginação é um recurso do EWS que permite controlar o tamanho dos resultados de uma pesquisa.</span><span class="sxs-lookup"><span data-stu-id="623c8-105">Paging is a feature in EWS that enables you to control the size of the results of a search.</span></span> <span data-ttu-id="623c8-106">Em vez de recuperar o conjunto em uma resposta EWS de resultados inteiro, é possível recuperar conjuntos menores em várias respostas do EWS.</span><span class="sxs-lookup"><span data-stu-id="623c8-106">Rather than retrieve the entire result set in one EWS response, you can retrieve smaller sets in multiple EWS responses.</span></span> <span data-ttu-id="623c8-107">Por exemplo, considere um usuário com 10.000 mensagens de email na sua caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="623c8-107">For example, consider a user with 10,000 email messages in their Inbox.</span></span> <span data-ttu-id="623c8-108">Hipoteticamente, você pode recuperar todos os emails de 10.000 em uma resposta muito grande, mas talvez você queira que divida em partes mais gerenciáveis por motivos de desempenho ou a largura de banda.</span><span class="sxs-lookup"><span data-stu-id="623c8-108">Hypothetically, you could retrieve all 10,000 emails in one very large response, but you might want to break that up into more manageable chunks for bandwidth or performance reasons.</span></span> <span data-ttu-id="623c8-109">Paginação oferece as ferramentas necessárias para fazer isso.</span><span class="sxs-lookup"><span data-stu-id="623c8-109">Paging gives you the tools to do just that.</span></span>
  
> [!NOTE]
> <span data-ttu-id="623c8-110">Hipoteticamente, é possível recuperar 10.000 itens em uma solicitação, na verdade, isso é improvável devido à limitação EWS.</span><span class="sxs-lookup"><span data-stu-id="623c8-110">While you can hypothetically retrieve 10,000 items in one request, in reality, this is unlikely due to EWS throttling.</span></span> <span data-ttu-id="623c8-111">Para obter mais informações, consulte a [limitação do EWS no Exchange](ews-throttling-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="623c8-111">To find out more, see [EWS throttling in Exchange](ews-throttling-in-exchange.md).</span></span> 
  
<span data-ttu-id="623c8-112">**Tabela 1. Parâmetros de paginação na API gerenciada de EWS e EWS**</span><span class="sxs-lookup"><span data-stu-id="623c8-112">**Table 1. Paging parameters in the EWS Managed API and EWS**</span></span>

|<span data-ttu-id="623c8-113">**Para definir ou recuperar o …**</span><span class="sxs-lookup"><span data-stu-id="623c8-113">**To configure or retrieve the…**</span></span>|<span data-ttu-id="623c8-114">**Na API gerenciada do EWS, use …**</span><span class="sxs-lookup"><span data-stu-id="623c8-114">**In the EWS Managed API, use…**</span></span>|<span data-ttu-id="623c8-115">**No EWS, use …**</span><span class="sxs-lookup"><span data-stu-id="623c8-115">**In EWS, use…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="623c8-116">Número máximo de itens ou pastas em uma resposta</span><span class="sxs-lookup"><span data-stu-id="623c8-116">Maximum number of items or folders in a response</span></span>  <br/> |<span data-ttu-id="623c8-117">O parâmetro **pageSize** para o [Construtor de ItemView](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) ou o [Construtor de FolderView](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="623c8-117">The **pageSize** parameter to the [ItemView constructor](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) or the [FolderView constructor](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx)</span></span> <br/> <span data-ttu-id="623c8-118">Or</span><span class="sxs-lookup"><span data-stu-id="623c8-118">Or</span></span>  <br/> <span data-ttu-id="623c8-119">A propriedade [PagedView.PageSize](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="623c8-119">The [PagedView.PageSize](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="623c8-120">O atributo **MaxEntriesReturned** no elemento [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou o elemento [IndexedPageFolderView](http://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="623c8-120">The **MaxEntriesReturned** attribute on the [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element or the [IndexedPageFolderView](http://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="623c8-121">Ponto de partida na lista de itens ou pastas</span><span class="sxs-lookup"><span data-stu-id="623c8-121">Starting point in the list of items or folders</span></span>  <br/> |<span data-ttu-id="623c8-122">O parâmetro **offsetBasePoint** para o construtor de **ItemView** ou o construtor de **FolderView**</span><span class="sxs-lookup"><span data-stu-id="623c8-122">The **offsetBasePoint** parameter to the **ItemView** constructor or the **FolderView** constructor</span></span>  <br/> <span data-ttu-id="623c8-123">Or</span><span class="sxs-lookup"><span data-stu-id="623c8-123">Or</span></span>  <br/> <span data-ttu-id="623c8-124">A propriedade [PagedView.OffsetBasePoint](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="623c8-124">The [PagedView.OffsetBasePoint](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="623c8-125">O atributo de **ponto de base** no elemento **IndexedPageItemView** ou o elemento **IndexedPageFolderView**</span><span class="sxs-lookup"><span data-stu-id="623c8-125">The **BasePoint** attribute on the **IndexedPageItemView** element or the **IndexedPageFolderView** element</span></span>  <br/> |
|<span data-ttu-id="623c8-126">Deslocamento a partir do ponto de partida</span><span class="sxs-lookup"><span data-stu-id="623c8-126">Offset from the starting point</span></span>  <br/> |<span data-ttu-id="623c8-127">O parâmetro de **deslocamento** para o construtor de **ItemView** ou o construtor de **FolderView**</span><span class="sxs-lookup"><span data-stu-id="623c8-127">The **offset** parameter to the **ItemView** constructor or the **FolderView** constructor</span></span>  <br/> <span data-ttu-id="623c8-128">Or</span><span class="sxs-lookup"><span data-stu-id="623c8-128">Or</span></span>  <br/> <span data-ttu-id="623c8-129">A propriedade [PagedView.Offset](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="623c8-129">The [PagedView.Offset](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="623c8-130">O atributo **deslocamento** no elemento **IndexedPageItemView** ou o elemento **IndexedPageFolderView**</span><span class="sxs-lookup"><span data-stu-id="623c8-130">The **Offset** attribute on the **IndexedPageItemView** element or the **IndexedPageFolderView** element</span></span>  <br/> |
|<span data-ttu-id="623c8-131">Número total de resultados no servidor</span><span class="sxs-lookup"><span data-stu-id="623c8-131">Total number of results on the server</span></span>  <br/> |<span data-ttu-id="623c8-132">A propriedade [FindItemsResults.TotalCount](http://msdn.microsoft.com/pt-br/library/dd635348%28v=exchg.80%29.aspx) ou a propriedade [FindFoldersResults.TotalCount](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="623c8-132">The [FindItemsResults.TotalCount](http://msdn.microsoft.com/pt-br/library/dd635348%28v=exchg.80%29.aspx) property or the [FindFoldersResults.TotalCount](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="623c8-133">O atributo **TotalItemsInView** no elemento [RootFolder (FindItemResponseMessage)](http://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) ou o elemento [RootFolder (FindFolderResponseMessage)](http://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="623c8-133">The **TotalItemsInView** attribute on the [RootFolder (FindItemResponseMessage)](http://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) element or the [RootFolder (FindFolderResponseMessage)](http://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="623c8-134">Deslocamento do primeiro item ou pasta não incluído na resposta atual</span><span class="sxs-lookup"><span data-stu-id="623c8-134">Offset of first item or folder not included in current response</span></span>  <br/> |<span data-ttu-id="623c8-135">A propriedade [FindItemsResults.NextPageOffset](http://msdn.microsoft.com/pt-br/library/ee693014%28v=exchg.80%29.aspx) ou a propriedade [FindFoldersResults.NextPageOffset](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="623c8-135">The [FindItemsResults.NextPageOffset](http://msdn.microsoft.com/pt-br/library/ee693014%28v=exchg.80%29.aspx) property or the [FindFoldersResults.NextPageOffset](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="623c8-136">O atributo **IndexedPagingOffset** no elemento **RootFolder**</span><span class="sxs-lookup"><span data-stu-id="623c8-136">The **IndexedPagingOffset** attribute on the **RootFolder** element</span></span>  <br/> |
|<span data-ttu-id="623c8-137">Indicador que a resposta inclui o último item ou a pasta na lista</span><span class="sxs-lookup"><span data-stu-id="623c8-137">Indicator that response includes the last item or folder in the list</span></span>  <br/> |<span data-ttu-id="623c8-138">A propriedade [FindItemsResults.MoreAvailable](http://msdn.microsoft.com/pt-br/library/dd635477%28v=exchg.80%29.aspx) ou a propriedade [FindFoldersResults.MoreAvailable](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="623c8-138">The [FindItemsResults.MoreAvailable](http://msdn.microsoft.com/pt-br/library/dd635477%28v=exchg.80%29.aspx) property or the [FindFoldersResults.MoreAvailable](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="623c8-139">O atributo **IncludesLastItemInRange** no elemento **RootFolder**</span><span class="sxs-lookup"><span data-stu-id="623c8-139">The **IncludesLastItemInRange** attribute on the **RootFolder** element</span></span>  <br/> |
   
## <a name="how-paging-works"></a><span data-ttu-id="623c8-140">Como funciona a paginação</span><span class="sxs-lookup"><span data-stu-id="623c8-140">How paging works</span></span>
<span data-ttu-id="623c8-141"><a name="bk_HowPagingWorks"> </a></span><span class="sxs-lookup"><span data-stu-id="623c8-141"></span></span>

<span data-ttu-id="623c8-142">Para entender como funciona a paginação, é útil visualizar as mensagens em uma pasta como cartazes alinhados lado a lado em um campo fora de sua casa.</span><span class="sxs-lookup"><span data-stu-id="623c8-142">To understand how paging works, it's helpful to visualize the messages in a folder as billboards lined up side by side in a field outside your house.</span></span> <span data-ttu-id="623c8-143">Você pode ver alguns desses cartazes é através de uma janela de mágica.</span><span class="sxs-lookup"><span data-stu-id="623c8-143">You can see some of these billboards through a magical window.</span></span> <span data-ttu-id="623c8-144">Você tem a capacidade de alterar o tamanho da janela (para ver cartazes é mais ou menos de uma vez) e para mover a janela (para controlar quais cartazes, você pode ver).</span><span class="sxs-lookup"><span data-stu-id="623c8-144">You have the ability to change the size of the window (to see more or fewer billboards at once) and to move the window (to control which billboards you can see).</span></span> <span data-ttu-id="623c8-145">Este manipulação da janela é paginação.</span><span class="sxs-lookup"><span data-stu-id="623c8-145">This manipulation of the window is paging.</span></span> 
  
<span data-ttu-id="623c8-146">Quando você enviar sua solicitação para o Exchange server, você pode especificar o tamanho da sua janela em termos de quantos itens para retornar.</span><span class="sxs-lookup"><span data-stu-id="623c8-146">When you send your request to the Exchange server, you specify the size of your window in terms of how many items to return.</span></span> <span data-ttu-id="623c8-147">Você pode definir a posição da janela, especificando um ponto de partida um (o início da linha) ou o final da linha e um deslocamento a partir desse ponto inicial, expressado em um número de itens.</span><span class="sxs-lookup"><span data-stu-id="623c8-147">You set the position of the window by specifying a starting point (either the beginning of the line or the end of the line) and an offset from that starting point, expressed in a number of items.</span></span> <span data-ttu-id="623c8-148">O início da janela é o número de itens especificada pelo deslocamento, desde o ponto de partida.</span><span class="sxs-lookup"><span data-stu-id="623c8-148">The beginning of the window is the number of items specified by the offset from the starting point.</span></span>
  
<span data-ttu-id="623c8-149">Onde paginação obtém um pouco mais interessante está na resposta do servidor, e como o seu aplicativo pode usar essa resposta para sua próxima solicitação de forma.</span><span class="sxs-lookup"><span data-stu-id="623c8-149">Where paging gets a bit more interesting is in the server's response, and how your application can use that response to shape its next request.</span></span> <span data-ttu-id="623c8-150">O servidor fornece três partes de informações que você pode usar para determinar como configurar seu "janela" para sua próxima solicitação:</span><span class="sxs-lookup"><span data-stu-id="623c8-150">The server gives you three pieces of information that you can use to determine how to configure your "window" for your next request:</span></span> 
  
- <span data-ttu-id="623c8-151">Se os resultados na resposta incluir o último item geral conjunto de resultados no servidor.</span><span class="sxs-lookup"><span data-stu-id="623c8-151">Whether the results in the response include the last item in the overall result set on the server.</span></span>
    
- <span data-ttu-id="623c8-152">O número total de itens no resultado definido no servidor.</span><span class="sxs-lookup"><span data-stu-id="623c8-152">The total number of items in the result set on the server.</span></span>
    
- <span data-ttu-id="623c8-153">O que o valor de deslocamento próximo deve ser, se você deseja avançar sua janela para o próximo item no conjunto de resultados que não esteja incluído na resposta atual.</span><span class="sxs-lookup"><span data-stu-id="623c8-153">What the next offset value should be, if you want to advance your window to the next item in the result set that isn't included in the current response.</span></span>
    
<span data-ttu-id="623c8-154">Vamos ver um exemplo simples.</span><span class="sxs-lookup"><span data-stu-id="623c8-154">Let's look at a simple example.</span></span> <span data-ttu-id="623c8-155">Imagine uma caixa de entrada com 15 mensagens dela.</span><span class="sxs-lookup"><span data-stu-id="623c8-155">Imagine an Inbox with 15 messages in it.</span></span> <span data-ttu-id="623c8-156">Seu aplicativo envia uma solicitação inicial para recuperar um máximo de 10 itens, desde o início da lista de mensagens (para que o deslocamento for zero).</span><span class="sxs-lookup"><span data-stu-id="623c8-156">Your application sends an initial request to retrieve a maximum of 10 items, starting at the beginning of the list of messages (so the offset is zero).</span></span> <span data-ttu-id="623c8-157">O servidor responde com as mensagens de 10 primeiros e indica que a resposta não incluir o último item, que não há um total de 15 itens e que o próximo deslocamento deve ser 10.</span><span class="sxs-lookup"><span data-stu-id="623c8-157">The server responds with the first 10 messages, and indicates that the response does not include the last item, that there are a total of 15 items, and that the next offset should be 10.</span></span>
  
<span data-ttu-id="623c8-158">**Figura 1. Solicitando 10 itens em deslocamento 0 desde o início de uma lista de 15 itens**</span><span class="sxs-lookup"><span data-stu-id="623c8-158">**Figure 1. Requesting 10 items at offset 0 from the beginning of a list of 15 items**</span></span>

![A diagram showing the results of requesting 10 items at offset 0 from the beginning of a list of 15 items.](media/Ex15_PagedSearch_FirstPage.png)
  
<span data-ttu-id="623c8-160">Seu aplicativo, em seguida, reenvia a mesma solicitação ao servidor, com a única alteração de que o deslocamento agora é 10.</span><span class="sxs-lookup"><span data-stu-id="623c8-160">Your application then resends the same request to the server, with the only change being that the offset is now 10.</span></span> <span data-ttu-id="623c8-161">O servidor retorna os últimos cinco itens e indica que a resposta incluir o último item, que não há um total de 15 itens e que o próximo deslocamento deve ser 15 (embora obviamente, você chegou final, portanto, não haverá um deslocamento próximo.)</span><span class="sxs-lookup"><span data-stu-id="623c8-161">The server returns the last five items, and indicates that the response does include the last item, that there are a total of 15 items, and that the next offset should be 15 (though of course, you've reached the end, so there won't be a next offset.)</span></span>
  
<span data-ttu-id="623c8-162">**Figura 2. Solicitando 10 itens em deslocamento 10 desde o início de uma lista de 15 itens**</span><span class="sxs-lookup"><span data-stu-id="623c8-162">**Figure 2. Requesting 10 items at offset 10 from the beginning of a list of 15 items**</span></span>

![A diagram showing the results of requesting 10 items at offset 10 from the beginning of a list of 15 items.](media/Ex15_PagedSearch_SecondPage.png)
  
## <a name="design-considerations-for-paging"></a><span data-ttu-id="623c8-164">Considerações de design para paginação</span><span class="sxs-lookup"><span data-stu-id="623c8-164">Design considerations for paging</span></span>
<span data-ttu-id="623c8-165"><a name="bk_DesignConsiderations"> </a></span><span class="sxs-lookup"><span data-stu-id="623c8-165"></span></span>

<span data-ttu-id="623c8-166">Tornar o máximo da paginação em seu aplicativo requerem alguns consideração.</span><span class="sxs-lookup"><span data-stu-id="623c8-166">Making the most out of paging in your application does require some consideration.</span></span> <span data-ttu-id="623c8-167">Por exemplo, como grandes ter sua janela""?</span><span class="sxs-lookup"><span data-stu-id="623c8-167">For example, how large do you make your "window"?</span></span> <span data-ttu-id="623c8-168">O que fazer se os resultados no servidor alterar enquanto você estiver movendo sua janela""?</span><span class="sxs-lookup"><span data-stu-id="623c8-168">What do you do if the results on the server change while you're moving your "window"?</span></span>
  
### <a name="determine-the-size-of-your-window"></a><span data-ttu-id="623c8-169">Determinar o tamanho da sua janela</span><span class="sxs-lookup"><span data-stu-id="623c8-169">Determine the size of your window</span></span>

<span data-ttu-id="623c8-170">Não há nenhum "única" número máximo de entradas que todos os aplicativos devem usar.</span><span class="sxs-lookup"><span data-stu-id="623c8-170">There is no "one-size-fits-all" maximum number of entries that all applications should use.</span></span> <span data-ttu-id="623c8-171">Determinando o número correto para seu aplicativo depende de vários fatores diferentes.</span><span class="sxs-lookup"><span data-stu-id="623c8-171">Determining the number that's right for your application depends on several different factors.</span></span> <span data-ttu-id="623c8-172">No entanto, é útil ter as seguintes diretrizes em mente:</span><span class="sxs-lookup"><span data-stu-id="623c8-172">However, it's helpful to keep the following guidelines in mind:</span></span>
  
- <span data-ttu-id="623c8-173">Por padrão, o Exchange limita o número máximo de itens que podem ser retornadas em uma única solicitação a 1000.</span><span class="sxs-lookup"><span data-stu-id="623c8-173">By default, Exchange limits the maximum number of items that can be returned in a single request to 1000.</span></span>
    
- <span data-ttu-id="623c8-174">Definindo o número máximo de entradas para um maior resulta de número em precisar enviar solicitações menos para obter todos os itens ao custo da necessidade de aguardar mais respostas.</span><span class="sxs-lookup"><span data-stu-id="623c8-174">Setting the maximum number of entries to a larger number results in having to send fewer requests to get all items, at the cost of having to wait longer for responses.</span></span>
    
- <span data-ttu-id="623c8-175">Definindo o número máximo de entradas para um menor número os resultados nos tempos de resposta mais rápidos, ao custo de enviar mais solicitações para obter todos os itens.</span><span class="sxs-lookup"><span data-stu-id="623c8-175">Setting the maximum number of entries to a smaller number results in quicker response times, at the cost of having to send more requests to get all items.</span></span>
    
### <a name="handling-changes-to-the-result-set"></a><span data-ttu-id="623c8-176">Tratamento de alterações ao conjunto de resultados</span><span class="sxs-lookup"><span data-stu-id="623c8-176">Handling changes to the result set</span></span>

<span data-ttu-id="623c8-177">No exemplo simple neste artigo, o número de itens na caixa de entrada do usuário permaneceu constante.</span><span class="sxs-lookup"><span data-stu-id="623c8-177">In the simple example earlier in this article, the number of items in the user's Inbox remained constant.</span></span> <span data-ttu-id="623c8-178">No entanto, na realidade, o número de itens em uma caixa de entrada pode alterar com frequência.</span><span class="sxs-lookup"><span data-stu-id="623c8-178">However, in reality, the number of items in an Inbox can change frequently.</span></span> <span data-ttu-id="623c8-179">Novas mensagens podem chegar e itens podem ser excluídos ou movidos a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="623c8-179">New messages can arrive and items can be deleted or moved at any time.</span></span> <span data-ttu-id="623c8-180">Mas como funciona a paginação este impacto?</span><span class="sxs-lookup"><span data-stu-id="623c8-180">But how does this impact paging?</span></span> <span data-ttu-id="623c8-181">Vamos modificar o cenário de exemplo anterior para descobrir.</span><span class="sxs-lookup"><span data-stu-id="623c8-181">Let's modify the earlier example scenario to find out.</span></span>
  
<span data-ttu-id="623c8-182">Começaremos novamente com os 15 itens na caixa de entrada do usuário e enviar a solicitação inicial mesma.</span><span class="sxs-lookup"><span data-stu-id="623c8-182">We'll start again with the 15 items in the user's Inbox, and send the same initial request.</span></span> <span data-ttu-id="623c8-183">Como antes, o servidor responde com as mensagens de 10 primeiros e indica que a resposta não incluir o último item, que não há um total de 15 itens e que o próximo deslocamento deve ser 10, conforme mostrado na Figura 1.</span><span class="sxs-lookup"><span data-stu-id="623c8-183">As before, the server responds with the first 10 messages, and indicates that the response does not include the last item, that there are a total of 15 items, and that the next offset should be 10, as shown in Figure 1.</span></span>
  
<span data-ttu-id="623c8-184">Agora, enquanto o seu aplicativo está processando esses 10 itens, uma nova mensagem chega na caixa de entrada e é adicionada ao resultado definido no servidor.</span><span class="sxs-lookup"><span data-stu-id="623c8-184">Now, while your application is processing those 10 items, a new message arrives in the Inbox and is added to the result set on the server.</span></span> <span data-ttu-id="623c8-185">Seu aplicativo reenvia a mesma solicitação ao servidor (somente com o deslocamento definido como 10).</span><span class="sxs-lookup"><span data-stu-id="623c8-185">Your application resends the same request to the server (only with the offset set to 10).</span></span> <span data-ttu-id="623c8-186">Neste momento o servidor obtém volta seis itens e indica que há um total de 16 itens no conjunto de resultados.</span><span class="sxs-lookup"><span data-stu-id="623c8-186">This time the server gets back six items, and indicates that there are a total of 16 items in the result set.</span></span>
  
<span data-ttu-id="623c8-187">Nesse momento você deve estar se perguntando se isso ainda é um problema.</span><span class="sxs-lookup"><span data-stu-id="623c8-187">At this point you might be wondering if this is even a problem.</span></span> <span data-ttu-id="623c8-188">Afinal, você obteve 16 itens novamente sobre as duas respostas, então, por que tudo isso?</span><span class="sxs-lookup"><span data-stu-id="623c8-188">After all, you got 16 items back over the two responses, so why all the fuss?</span></span> <span data-ttu-id="623c8-189">A resposta depende de onde colocado o novo item na lista.</span><span class="sxs-lookup"><span data-stu-id="623c8-189">The answer depends on where in the list the new item is placed.</span></span> <span data-ttu-id="623c8-190">Se a lista é classificada para que os itens mais antigos (por data/hora recebido) sejam primeiro, não há nenhum motivo de preocupação neste cenário.</span><span class="sxs-lookup"><span data-stu-id="623c8-190">If the list is sorted so that the oldest items (by received date/time) are first, there's no cause for concern in this scenario.</span></span> <span data-ttu-id="623c8-191">O novo item será colocado no final da lista e será incluído na segunda resposta.</span><span class="sxs-lookup"><span data-stu-id="623c8-191">The new item will be placed at the end of the list, and will be included in the second response.</span></span>
  
<span data-ttu-id="623c8-192">**Figura 3. Solicitando 10 itens em deslocamento 10 desde o início de uma lista de itens de 16, com o item 16 na lista sendo novo**</span><span class="sxs-lookup"><span data-stu-id="623c8-192">**Figure 3. Requesting 10 items at offset 10 from the beginning of a list of 16 items, with the 16th item in the list being new**</span></span>

![A diagram showing the results of requesting 10 items at offset 10 from the beginning of a list of 16 items when the 16th item was added to the end of the list.](media/Ex15_PagedSearch_SecondPage_NewItemEnd.png)
  
<span data-ttu-id="623c8-194">Se a lista é classificada para que os itens mais novos são primeiro, é uma história diferente.</span><span class="sxs-lookup"><span data-stu-id="623c8-194">If the list is sorted so that the newest items are first, it's a different story.</span></span> <span data-ttu-id="623c8-195">Nesse caso, o primeiro item na segunda solicitação seria o último item da solicitação anterior plus os cinco itens restantes de 15 a original.</span><span class="sxs-lookup"><span data-stu-id="623c8-195">In this case, the first item in the second request would be the last item from the previous request plus the remaining five items from the original 15.</span></span> <span data-ttu-id="623c8-196">Para colocar em termos de nossa janela mágica imaginária, você deslocados posição da sua janela em 10, mas os cartazes sozinhos também deslocadas por 1.</span><span class="sxs-lookup"><span data-stu-id="623c8-196">To put it in terms of our imaginary magical window, you shifted your window's position by 10, but the billboards themselves also shifted by 1.</span></span>
  
<span data-ttu-id="623c8-197">**Figura 4. Solicitando 10 itens em deslocamento 10 desde o início de uma lista de itens de 16, com o primeiro item na lista que está sendo novo**</span><span class="sxs-lookup"><span data-stu-id="623c8-197">**Figure 4. Requesting 10 items at offset 10 from the beginning of a list of 16 items, with the first item in the list being new**</span></span>

![A diagram showing the results of asking for 10 items at offset 10 from the beginning of a list of 16 items when the 16th item was added to the beginning of the list.](media/Ex15_PagedSearch_SecondPage_NewItemBeginning.png)
  
<span data-ttu-id="623c8-199">Uma maneira para detectar uma alteração para os resultados no servidor é usar o conceito de um item de âncora.</span><span class="sxs-lookup"><span data-stu-id="623c8-199">One way to detect a change to the results on the server is to use the concept of an anchor item.</span></span> <span data-ttu-id="623c8-200">Um item de âncora é um item adicional em sua resposta que não é processado com o restante dos resultados, mas é usada para comparação com os próximos resultados para ver se alteraram próprios itens.</span><span class="sxs-lookup"><span data-stu-id="623c8-200">An anchor item is an additional item in your response that is not processed along with the rest of the results, but is used to compare with the next results to see if the items themselves have shifted.</span></span> <span data-ttu-id="623c8-201">Criando novamente no nosso exemplo simple, se o seu aplicativo está usando um tamanho de "janela" 10, realmente definir o número máximo de itens para retornar à 11.</span><span class="sxs-lookup"><span data-stu-id="623c8-201">Building again on our simple example, if your application is using a "window" size of 10, you actually set the maximum number of items to return to 11.</span></span> <span data-ttu-id="623c8-202">Seu aplicativo processa os 10 primeiros itens na resposta como de costume.</span><span class="sxs-lookup"><span data-stu-id="623c8-202">Your application processes the first 10 items in the response as usual.</span></span> <span data-ttu-id="623c8-203">Para o último item, você salvar o identificador do item como âncora e emita a próxima solicitação com um deslocamento de 10.</span><span class="sxs-lookup"><span data-stu-id="623c8-203">For the last item, you save the item's identifier as an anchor, then issue the next request with an offset of 10.</span></span> <span data-ttu-id="623c8-204">Se os dados não tem sido alterado, o primeiro item na segunda resposta deve ter um identificador de item que corresponda à âncora.</span><span class="sxs-lookup"><span data-stu-id="623c8-204">If the data has not changed, the first item in the second response should have an item identifier that matches the anchor.</span></span> <span data-ttu-id="623c8-205">Se os identificadores de item não coincidirem, você saberá que os dados foi removidos ou inseridos na lista partes da lista de você ter já "paginados" sobre.</span><span class="sxs-lookup"><span data-stu-id="623c8-205">If the item identifiers don't match, you know that the data has been removed or inserted in the parts of the list you have already "paged" over.</span></span>
  
<span data-ttu-id="623c8-206">Mesmo quando você souber que os dados foram alterados, você ainda precisará decidir como reagir.</span><span class="sxs-lookup"><span data-stu-id="623c8-206">Even when you know that the data has changed, you still need to decide how to react.</span></span> <span data-ttu-id="623c8-207">Há não uma única resposta para essa pergunta.</span><span class="sxs-lookup"><span data-stu-id="623c8-207">There isn't a one-size-fits-all answer for this question either.</span></span> <span data-ttu-id="623c8-208">Suas ações dependerá da natureza do seu aplicativo e como é essencial capturar todos os itens.</span><span class="sxs-lookup"><span data-stu-id="623c8-208">Your actions will depend on the nature of your application and how critical it is to capture all items.</span></span> <span data-ttu-id="623c8-209">Você pode ignorá-la completamente, reinicie o processo desde o início, ou fazer track e tente detectar onde a alteração aconteceu.</span><span class="sxs-lookup"><span data-stu-id="623c8-209">You might ignore it altogether, restart the process from the beginning, or back track and try to detect where the change happened.</span></span>
  
## <a name="example-perform-a-paged-search-by-using-the-ews-managed-api"></a><span data-ttu-id="623c8-210">Exemplo: Executar uma pesquisa paginada usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="623c8-210">Example: Perform a paged search by using the EWS Managed API</span></span>
<span data-ttu-id="623c8-211"><a name="bk_PagedSearchEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="623c8-211"></span></span>

<span data-ttu-id="623c8-212">Paginação é suportada pelos seguintes métodos API gerenciada de EWS:</span><span class="sxs-lookup"><span data-stu-id="623c8-212">Paging is supported by the following EWS Managed API methods:</span></span>
  
- [<span data-ttu-id="623c8-213">ExchangeService.FindFolders</span><span class="sxs-lookup"><span data-stu-id="623c8-213">ExchangeService.FindFolders</span></span>](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="623c8-214">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="623c8-214">ExchangeService.FindItems</span></span>](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="623c8-215">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="623c8-215">Folder.FindFolders</span></span>](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="623c8-216">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="623c8-216">Folder.FindFolders</span></span>](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
<span data-ttu-id="623c8-217">Se você estiver usando a API gerenciada de EWS, seu aplicativo configura paginação com a classe [ItemView](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) ou [FolderView](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) e recebe informações do servidor referente a paginação do [FindItemsResults](http://msdn.microsoft.com/pt-br/library/dd635381%28v=exchg.80%29.aspx) ou [FindFoldersResults](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx) classe.</span><span class="sxs-lookup"><span data-stu-id="623c8-217">If you are using the EWS Managed API, your application configures paging with the [ItemView](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) or [FolderView](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) class and receives information from the server regarding paging from the [FindItemsResults](http://msdn.microsoft.com/pt-br/library/dd635381%28v=exchg.80%29.aspx) or [FindFoldersResults](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx) class.</span></span> 
  
<span data-ttu-id="623c8-218">O exemplo a seguir recupera todos os itens em uma pasta usando uma pesquisa paginada que retorne cinco itens em cada resposta.</span><span class="sxs-lookup"><span data-stu-id="623c8-218">The following example retrieves all the items in a folder using a paged search that returns five items in each response.</span></span> <span data-ttu-id="623c8-219">Ele também recupera um item adicional para servir como uma âncora para detectar alterações aos resultados no servidor.</span><span class="sxs-lookup"><span data-stu-id="623c8-219">It also retrieves an additional item to serve as an anchor to detect changes to the results on the server.</span></span> 
  
<span data-ttu-id="623c8-220">Este exemplo pressupõe que o objeto **ExchangeService** foi inicializado com valores válidos nas propriedades [credenciais](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) e [Url](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="623c8-220">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
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

## <a name="example-perform-a-paged-search-by-using-ews"></a><span data-ttu-id="623c8-221">Exemplo: Executar uma pesquisa paginada usando o EWS</span><span class="sxs-lookup"><span data-stu-id="623c8-221">Example: Perform a paged search by using EWS</span></span>
<span data-ttu-id="623c8-222"><a name="bk_PagedSearchEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="623c8-222"></span></span>

<span data-ttu-id="623c8-223">Paginação é suportada pelos seguintes operações EWS:</span><span class="sxs-lookup"><span data-stu-id="623c8-223">Paging is supported by the following EWS operations:</span></span>
  
- [<span data-ttu-id="623c8-224">FindFolder</span><span class="sxs-lookup"><span data-stu-id="623c8-224">FindFolder</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [<span data-ttu-id="623c8-225">FindItem</span><span class="sxs-lookup"><span data-stu-id="623c8-225">FindItem</span></span>](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
<span data-ttu-id="623c8-226">Se você estiver usando o EWS, seu aplicativo configura paginação com o elemento [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) ou o elemento [IndexedPageFolderView](http://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) e recebe informações do servidor referente a paginação do [(RootFolder FindItemResponseMessage)](http://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) elemento ou o elemento [RootFolder (FindFolderResponseMessage)](http://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="623c8-226">If you're using EWS, your application configures paging with the [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element or the [IndexedPageFolderView](http://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) element and receives information from the server regarding paging from the [RootFolder (FindItemResponseMessage)](http://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) element or the [RootFolder (FindFolderResponseMessage)](http://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) element.</span></span> 
  
<span data-ttu-id="623c8-227">Neste exemplo de solicitação, uma solicitação de **FindItem** é enviada para um máximo de seis itens, começando em um deslocamento de zero desde o início da lista de itens na caixa de entrada do usuário.</span><span class="sxs-lookup"><span data-stu-id="623c8-227">In this request example, a **FindItem** request is sent for a maximum of six items, starting at an offset of zero from the beginning of the list of items in the user's Inbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="623c8-228">O servidor retorna a seguinte resposta, que contém seis itens.</span><span class="sxs-lookup"><span data-stu-id="623c8-228">The server returns the following response, which contains six items.</span></span> <span data-ttu-id="623c8-229">A resposta também indica que não há um total de oito itens nos resultados no servidor e que o último item na lista de resultados não está presente nesta resposta.</span><span class="sxs-lookup"><span data-stu-id="623c8-229">The response also indicates that there are a total of eight items in the results on the server, and that the last item in the results list is not present in this response.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
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

<span data-ttu-id="623c8-230">Neste exemplo, a mesma solicitação é enviada, mas desta vez, o atributo de **deslocamento** é alterado para cinco, que indica que o servidor deve retornar no máximo seis itens, começando com offset cinco desde o início.</span><span class="sxs-lookup"><span data-stu-id="623c8-230">In this example, the same request is sent, but this time, the **Offset** attribute is changed to five, which indicates that the server should return at most six items starting at offset five from the beginning.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="623c8-231">O servidor envia a seguinte resposta, que contém três itens.</span><span class="sxs-lookup"><span data-stu-id="623c8-231">The server sends the following response, which contains three items.</span></span> <span data-ttu-id="623c8-232">A resposta também indica que o número total de itens nos resultados no servidor ainda oito e que o último item nos resultados da lista está incluída nesta resposta.</span><span class="sxs-lookup"><span data-stu-id="623c8-232">The response also indicates that the total number of items in the results on the server is still eight, and that the last item in the results list is included in this response.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
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

## <a name="see-also"></a><span data-ttu-id="623c8-233">Confira também</span><span class="sxs-lookup"><span data-stu-id="623c8-233">See also</span></span>


- [<span data-ttu-id="623c8-234">Pesquisa e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="623c8-234">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)
    
- [<span data-ttu-id="623c8-235">Método ExchangeService.FindFolders</span><span class="sxs-lookup"><span data-stu-id="623c8-235">ExchangeService.FindFolders method</span></span>](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="623c8-236">Método ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="623c8-236">ExchangeService.FindItems method</span></span>](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="623c8-237">Método Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="623c8-237">Folder.FindFolders method</span></span>](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="623c8-238">Método Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="623c8-238">Folder.FindFolders method</span></span>](http://msdn.microsoft.com/pt-br/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="623c8-239">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="623c8-239">FindFolder operation</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [<span data-ttu-id="623c8-240">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="623c8-240">FindItem operation</span></span>](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- [<span data-ttu-id="623c8-241">EWS limitação no Exchange</span><span class="sxs-lookup"><span data-stu-id="623c8-241">EWS throttling in Exchange</span></span>](ews-throttling-in-exchange.md)
    

