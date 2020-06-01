---
title: Trabalhar com pastas de pesquisa usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: abe703c5-6d85-46d9-bf20-230c34782a9f
description: Descubra como criar, obter, atualizar e excluir pastas de pesquisa usando a API gerenciada do EWS ou o EWS no Exchange.
ms.openlocfilehash: 880c14bc99c4f6c674d4f7566036c4b8f5f19e55
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456364"
---
# <a name="work-with-search-folders-by-using-ews-in-exchange"></a><span data-ttu-id="4a77e-103">Trabalhar com pastas de pesquisa usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4a77e-103">Work with search folders by using EWS in Exchange</span></span>

<span data-ttu-id="4a77e-104">Descubra como criar, obter, atualizar e excluir pastas de pesquisa usando a API gerenciada do EWS ou o EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="4a77e-104">Find out how to create, get, update, and delete search folders by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="4a77e-105">Uma pasta de pesquisa representa uma pesquisa persistente "sempre ativada" na caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="4a77e-105">A search folder represents a persistent "always-on" search in a user's mailbox.</span></span> <span data-ttu-id="4a77e-106">Uma pasta de pesquisa se assemelha e age como uma pasta de caixa de correio normal.</span><span class="sxs-lookup"><span data-stu-id="4a77e-106">A search folder looks and acts like a regular mailbox folder.</span></span> <span data-ttu-id="4a77e-107">No entanto, em vez de conter itens, ele contém uma cópia "virtual" dos itens de qualquer pasta em seu escopo de pesquisa que corresponde aos critérios de pesquisa definidos na pasta.</span><span class="sxs-lookup"><span data-stu-id="4a77e-107">However, instead of containing items, it contains a "virtual" copy of items from any folders in its search scope that match the search criteria set on the folder.</span></span> <span data-ttu-id="4a77e-108">Os aplicativos e os usuários finais podem usar pastas de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4a77e-108">Both applications and end-users can use search folders.</span></span> <span data-ttu-id="4a77e-109">O aplicativo precisa realizar a mesma pesquisa através de e para mais?</span><span class="sxs-lookup"><span data-stu-id="4a77e-109">Does your application need to perform the same search over and over?</span></span> <span data-ttu-id="4a77e-110">As pastas de pesquisa são uma ótima ferramenta para essa tarefa.</span><span class="sxs-lookup"><span data-stu-id="4a77e-110">Search folders are a great tool for this task.</span></span> <span data-ttu-id="4a77e-111">Ou talvez você queira apenas dar aos usuários a capacidade de acessar e gerenciar pastas de pesquisa no cliente.</span><span class="sxs-lookup"><span data-stu-id="4a77e-111">Or maybe you just want to give your users the ability to access and manage search folders in your client.</span></span> <span data-ttu-id="4a77e-112">Seja qual for o seu cenário, a API gerenciada do EWS e o EWS permitem que o aplicativo interaja completamente com as pastas de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4a77e-112">Whatever your scenario, the EWS Managed API and EWS enable your application to fully interact with search folders.</span></span>

> [!NOTE] 
> <span data-ttu-id="4a77e-113">Este artigo aplica-se somente ao uso do Outlook no modo online.</span><span class="sxs-lookup"><span data-stu-id="4a77e-113">This article applies only when using Outlook in online mode.</span></span> <span data-ttu-id="4a77e-114">As pastas de pesquisa não são sincronizadas; Portanto, as pastas de pesquisa criadas no modo online não aparecerão no modo cache.</span><span class="sxs-lookup"><span data-stu-id="4a77e-114">Search folders do not sync; therefore, search folders created in online mode will not appear in cached mode.</span></span>
  
<span data-ttu-id="4a77e-115">**Tabela 1. Métodos da API gerenciada do EWS e operações do EWS para trabalhar com pastas de pesquisa**</span><span class="sxs-lookup"><span data-stu-id="4a77e-115">**Table 1. EWS Managed API methods and EWS operations for working with search folders**</span></span>

|<span data-ttu-id="4a77e-116">Se você quiser...</span><span class="sxs-lookup"><span data-stu-id="4a77e-116">If you want to…</span></span>|<span data-ttu-id="4a77e-117">Na API gerenciada do EWS, use...</span><span class="sxs-lookup"><span data-stu-id="4a77e-117">In the EWS Managed API, use…</span></span>|<span data-ttu-id="4a77e-118">Em EWS, use...</span><span class="sxs-lookup"><span data-stu-id="4a77e-118">In EWS, use…</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4a77e-119">Criar uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="4a77e-119">Create a search folder</span></span>  <br/> |[<span data-ttu-id="4a77e-120">SearchFolder. Save</span><span class="sxs-lookup"><span data-stu-id="4a77e-120">SearchFolder.Save</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="4a77e-121">Operação CreateFolder</span><span class="sxs-lookup"><span data-stu-id="4a77e-121">CreateFolder operation</span></span>](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="4a77e-122">Obter uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="4a77e-122">Get a search folder</span></span>  <br/> |[<span data-ttu-id="4a77e-123">SearchFolder. bind</span><span class="sxs-lookup"><span data-stu-id="4a77e-123">SearchFolder.Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="4a77e-124">Operação GetFolder</span><span class="sxs-lookup"><span data-stu-id="4a77e-124">GetFolder operation</span></span>](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="4a77e-125">Atualizar uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="4a77e-125">Update a search folder</span></span>  <br/> |[<span data-ttu-id="4a77e-126">SearchFolder. Update</span><span class="sxs-lookup"><span data-stu-id="4a77e-126">SearchFolder.Update</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="4a77e-127">Operação UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="4a77e-127">UpdateFolder operation</span></span>](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="4a77e-128">Excluir uma pasta de pesquisa</span><span class="sxs-lookup"><span data-stu-id="4a77e-128">Delete a search folder</span></span>  <br/> |[<span data-ttu-id="4a77e-129">SearchFolder. Delete</span><span class="sxs-lookup"><span data-stu-id="4a77e-129">SearchFolder.Delete</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="4a77e-130">Operação DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="4a77e-130">DeleteFolder operation</span></span>](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |
   
## <a name="core-concepts-to-know-for-working-with-search-folders"></a><span data-ttu-id="4a77e-131">Principais conceitos que você deve saber para trabalhar com pastas de pesquisa</span><span class="sxs-lookup"><span data-stu-id="4a77e-131">Core concepts to know for working with search folders</span></span>
<span data-ttu-id="4a77e-132"><a name="bk_CoreConcepts"> </a></span><span class="sxs-lookup"><span data-stu-id="4a77e-132"><a name="bk_CoreConcepts"> </a></span></span>

<span data-ttu-id="4a77e-133">Antes de começar a trabalhar com pastas de pesquisa, você deve estar familiarizado com a forma como os filtros de pesquisa funcionam.</span><span class="sxs-lookup"><span data-stu-id="4a77e-133">Before you start working with search folders, you'll want to be familiar with how search filters work.</span></span> <span data-ttu-id="4a77e-134">As pastas de pesquisa dependem de filtros de pesquisa para expressar seus critérios.</span><span class="sxs-lookup"><span data-stu-id="4a77e-134">Search folders rely on search filters to express their criteria.</span></span> <span data-ttu-id="4a77e-135">Os filtros de pesquisa para pastas de pesquisa são construídos da mesma forma que os [filtros de pesquisa para operações de pesquisa](how-to-use-search-filters-with-ews-in-exchange.md) são construídos.</span><span class="sxs-lookup"><span data-stu-id="4a77e-135">Search filters for search folders are constructed in the same way that [search filters for search operations](how-to-use-search-filters-with-ews-in-exchange.md) are constructed.</span></span> 
  
## <a name="create-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="4a77e-136">Criar uma pasta de pesquisa usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="4a77e-136">Create a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="4a77e-137"><a name="bk_CreateEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="4a77e-137"><a name="bk_CreateEWSMA"> </a></span></span>

<span data-ttu-id="4a77e-138">Basicamente, você cria uma pasta de pesquisa usando a API gerenciada do EWS da mesma maneira que você cria uma pasta normal.</span><span class="sxs-lookup"><span data-stu-id="4a77e-138">Basically, you create a search folder using the EWS Managed API in the same way that you create a regular folder.</span></span> <span data-ttu-id="4a77e-139">No entanto, em vez de usar a [classe Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx), você usa a [classe SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)e define a [Propriedade SearchParameters](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.searchparameters%28v=exchg.80%29.aspx) para configurar os critérios de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4a77e-139">However, instead of using the [Folder class](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx), you use the [SearchFolder class](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx), and set the [SearchParameters property](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.searchparameters%28v=exchg.80%29.aspx) to configure the search criteria.</span></span> 
  
<span data-ttu-id="4a77e-140">No exemplo a seguir, uma pasta de pesquisa é criada para localizar todas as mensagens na caixa de entrada e suas subpastas que foram enviadas pelo gerente do usuário, sadie@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="4a77e-140">In the following example, a search folder is created to find all messages in the Inbox and its subfolders that were sent by the user's manager, sadie@contoso.com.</span></span> <span data-ttu-id="4a77e-141">A pasta é criada como um filho da pasta de pastas de pesquisa na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="4a77e-141">The folder is created as a child of the Search Folders folder in the user's mailbox.</span></span>
  
> [!NOTE]
> <span data-ttu-id="4a77e-142">Você pode criar uma pasta de pesquisa como um filho de qualquer pasta na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="4a77e-142">You can create a search folder as a child of any folder in the user's mailbox.</span></span> <span data-ttu-id="4a77e-143">No entanto, se você deseja que a pasta recém-criada seja mostrada em pastas de pesquisa no Outlook, crie-a na pasta de pesquisa pastas bem conhecidas, usando o valor de **SearchFolders** da [Enumeração WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="4a77e-143">However, if you want the newly created folder to show up under Search Folders in Outlook, create it under the Search Folders well-known folder, using the **SearchFolders** value of the [WellKnownFolderName enumeration](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx).</span></span> 
  
<span data-ttu-id="4a77e-144">Este exemplo pressupõe que o objeto **ExchangeService** tenha sido inicializado com valores válidos nas propriedades de [credenciais](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) e [URL](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4a77e-144">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void CreateSearchFolder(ExchangeService service)
{
    // Create the folder.
    SearchFolder searchFolder = new SearchFolder(service);
    searchFolder.DisplayName = "From Manager";
    // Create a search filter to express the criteria
    // for the folder.
    EmailAddress manager = new EmailAddress("sadie@contoso.com");
    SearchFilter.IsEqualTo fromManagerFilter =
        new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
    // Set the search filter.
    searchFolder.SearchParameters.SearchFilter = fromManagerFilter;
    // Set the folder to search.
    searchFolder.SearchParameters.RootFolderIds.Add(WellKnownFolderName.Inbox);
    // Set the search traversal. Deep will search all subfolders.
    searchFolder.SearchParameters.Traversal = SearchFolderTraversal.Deep;
    // Call Save to make the EWS call to create the folder.
    searchFolder.Save(WellKnownFolderName.SearchFolders);
}
```

## <a name="create-a-search-folder-by-using-ews"></a><span data-ttu-id="4a77e-145">Criar uma pasta de pesquisa usando o EWS</span><span class="sxs-lookup"><span data-stu-id="4a77e-145">Create a search folder by using EWS</span></span>
<span data-ttu-id="4a77e-146"><a name="bk_CreateEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="4a77e-146"><a name="bk_CreateEWS"> </a></span></span>

<span data-ttu-id="4a77e-147">Se você estiver usando o EWS, use a [operação CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) com um elemento [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) para criar uma pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4a77e-147">If you are using EWS, use the [CreateFolder operation](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) with a [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) element to create a search folder.</span></span> <span data-ttu-id="4a77e-148">No exemplo de solicitação a seguir, uma pasta de pesquisa é criada para localizar todas as mensagens na caixa de entrada e suas subpastas que foram enviadas pelo gerente do usuário, sadie@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="4a77e-148">In the following request example, a search folder is created to find all messages in the Inbox and its subfolders that were sent by the user's manager, sadie@contoso.com.</span></span> <span data-ttu-id="4a77e-149">A pasta é criada na pasta pastas de pesquisa na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="4a77e-149">The folder is created in the Search Folders folder in the user's mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="4a77e-150">Você pode criar uma pasta de pesquisa como um filho de qualquer pasta na caixa de correio do usuário.</span><span class="sxs-lookup"><span data-stu-id="4a77e-150">You can create a search folder as a child of any folder in the user's mailbox.</span></span> <span data-ttu-id="4a77e-151">No entanto, se você deseja que a pasta recém-criada seja mostrada em pastas de pesquisa no Outlook, crie-a na pasta de pesquisa pastas bem conhecidas, usando o valor **SearchFolders** no atributo **ID** do elemento [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4a77e-151">However, if you want the newly created folder to show up under Search Folders in Outlook, create it under the Search Folders well-known folder, using the **searchfolders** value in the **Id** attribute of the [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) element.</span></span> 
  
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
    <m:CreateFolder>
      <m:ParentFolderId>
        <t:DistinguishedFolderId Id="searchfolders" />
      </m:ParentFolderId>
      <m:Folders>
        <t:SearchFolder>
          <t:DisplayName>From Manager</t:DisplayName>
          <t:SearchParameters Traversal="Deep">
            <t:Restriction>
              <t:IsEqualTo>
                <t:FieldURI FieldURI="message:Sender" />
                <t:FieldURIOrConstant>
                  <t:Constant Value="sadie@contoso.com" />
                </t:FieldURIOrConstant>
              </t:IsEqualTo>
            </t:Restriction>
            <t:BaseFolderIds>
              <t:DistinguishedFolderId Id="inbox" />
            </t:BaseFolderIds>
          </t:SearchParameters>
        </t:SearchFolder>
      </m:Folders>
    </m:CreateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="4a77e-152">O servidor responde com uma mensagem [CreateFolderResponse](https://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) que inclui um valor [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica êxito.</span><span class="sxs-lookup"><span data-stu-id="4a77e-152">The server responds with a [CreateFolderResponse](https://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates success.</span></span>
  
## <a name="get-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="4a77e-153">Obter uma pasta de pesquisa usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="4a77e-153">Get a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="4a77e-154"><a name="bk_RetrieveEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="4a77e-154"><a name="bk_RetrieveEWSMA"> </a></span></span>

<span data-ttu-id="4a77e-155">Use o método de API gerenciada do EWS [ExchangeService. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) para localizar pastas de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4a77e-155">Use the [ExchangeService.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) EWS Managed API method to find search folders.</span></span> <span data-ttu-id="4a77e-156">Observe, no entanto, que você não pode limitar seus resultados para incluir apenas pastas de pesquisa; Você deve ter isso em mente ao processar os resultados.</span><span class="sxs-lookup"><span data-stu-id="4a77e-156">Note, however, that you can't limit your results to only include search folders; you'll want to keep that in mind when you process the results.</span></span> <span data-ttu-id="4a77e-157">Use o método [SearchFolder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.bind%28v=exchg.80%29.aspx) para obter pastas de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4a77e-157">Use the [SearchFolder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder.bind%28v=exchg.80%29.aspx) method to get search folders.</span></span> 
  
<span data-ttu-id="4a77e-158">O exemplo a seguir localiza as primeiras 10 pastas na pasta de pastas de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4a77e-158">The following example finds the first 10 folders in the Search Folders folder.</span></span> <span data-ttu-id="4a77e-159">Ele verifica para determinar se cada um é uma pasta de pesquisa e, em caso afirmativo, obtém a pasta de pesquisa e exibe quantas pastas de destino ele pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4a77e-159">It checks to determine whether each one is a search folder, and if so, it gets the search folder and displays how many target folders it searches.</span></span>
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void GetSearchFolders(ExchangeService service)
{
    FolderView folderView = new FolderView(10);
    folderView.PropertySet = new PropertySet(FolderSchema.DisplayName);
    try
    {
        FindFoldersResults findResults = service.FindFolders(WellKnownFolderName.SearchFolders, folderView);
        foreach (Folder folder in findResults.Folders)
        {
            // You can't request only search folders in 
            // a FindFolders request, so other search folders might also be present.
            if (folder is SearchFolder)
            {
                Console.WriteLine("{0} is a search folder.", folder.DisplayName);
                // In order to access the SearchParameters property,
                // you have to bind to the folder. SearchParameters are not
                // returned in FindFolders results.
                SearchFolder searchFolder = SearchFolder.Bind(service, folder.Id);
                Console.WriteLine("Number of folders searched: {0}.",
                    searchFolder.SearchParameters.RootFolderIds.Count);
            }
            else
            {
                Console.WriteLine("{0} is NOT a search folder.", folder.DisplayName);
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

## <a name="get-a-search-folder-by-using-ews"></a><span data-ttu-id="4a77e-160">Obter uma pasta de pesquisa usando o EWS</span><span class="sxs-lookup"><span data-stu-id="4a77e-160">Get a search folder by using EWS</span></span>
<span data-ttu-id="4a77e-161"><a name="bk_RetrieveEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="4a77e-161"><a name="bk_RetrieveEWS"> </a></span></span>

<span data-ttu-id="4a77e-162">Se você estiver usando o EWS, use a [operação FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) para encontrar pastas de pesquisa e a [operação GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) para obter pastas de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4a77e-162">If you're using EWS, use the [FindFolder operation](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) to find search folders, and the [GetFolder operation](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) to get search folders.</span></span> <span data-ttu-id="4a77e-163">Uma resposta **GetFolder** bem-sucedida para uma pasta de pesquisa conterá um elemento [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4a77e-163">A successful **GetFolder** response for a search folder will contain a [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="4a77e-164">O exemplo de solicitação a seguir localiza as primeiras 10 pastas na pasta de pastas de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4a77e-164">The following request example finds the first 10 folders in the Search Folders folder.</span></span> 
  
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
    <m:FindFolder Traversal="Shallow">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:DisplayName" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="searchfolders" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="4a77e-165">O servidor retorna a seguinte resposta, que mostra uma pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4a77e-165">The server returns the following response, which shows one search folder.</span></span>
  
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
    <m:FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="3" TotalItemsInView="3" IncludesLastItemInRange="true">
            <t:Folders>
              <t:SearchFolder>
                <t:FolderId Id="AAMkAGM2..." ChangeKey="CAAAABYA..." />
                <t:DisplayName>From Manager</t:DisplayName>
              </t:SearchFolder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="4a77e-166">O exemplo a seguir usa o valor do elemento [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) da resposta anterior em uma solicitação de operação **GetFolder** para obter a pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4a77e-166">The following example of a request uses the value of the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) element from the previous response in a **GetFolder** operation request to get the search folder.</span></span> 
  
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
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:FolderIds>
        <t:FolderId Id="AAMkAGM2..." ChangeKey="CAAAABYA..." />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="4a77e-167">O servidor retorna a seguinte resposta com todas as propriedades de primeira classe da pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4a77e-167">The server returns the following response with all the first-class properties for the search folder.</span></span>
  
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
    <m:GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:SearchFolder>
              <t:FolderId Id="AAMkAGM2..." ChangeKey="CAAAABYA..." />
              <t:ParentFolderId Id="AQMkAGM2..." ChangeKey="AQAAAA==" />
              <t:FolderClass>IPF.Note</t:FolderClass>
              <t:DisplayName>From Manager</t:DisplayName>
              <t:TotalCount>8</t:TotalCount>
              <t:ChildFolderCount>0</t:ChildFolderCount>
              <t:EffectiveRights>
                <t:CreateAssociated>true</t:CreateAssociated>
                <t:CreateContents>true</t:CreateContents>
                <t:CreateHierarchy>true</t:CreateHierarchy>
                <t:Delete>true</t:Delete>
                <t:Modify>true</t:Modify>
                <t:Read>true</t:Read>
                <t:ViewPrivateItems>true</t:ViewPrivateItems>
              </t:EffectiveRights>
              <t:UnreadCount>0</t:UnreadCount>
              <t:SearchParameters Traversal="Deep">
                <t:Restriction>
                  <t:IsEqualTo>
                    <t:FieldURI FieldURI="message:Sender" />
                    <t:FieldURIOrConstant>
                      <t:Constant Value="/o=First Organization/ou=Exchange Administrative Group (FYDIBOHF23SPDLT)/cn=Recipients/cn=8d84a3f4cbb34d48838a3aecf99795c0-Sadie" />
                    </t:FieldURIOrConstant>
                  </t:IsEqualTo>
                </t:Restriction>
                <t:BaseFolderIds>
                  <t:FolderId Id="AQMkAGM2..." ChangeKey="AQAAAA==" />
                </t:BaseFolderIds>
              </t:SearchParameters>
            </t:SearchFolder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

## <a name="update-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="4a77e-168">Atualizar uma pasta de pesquisa usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="4a77e-168">Update a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="4a77e-169"><a name="bk_UpdateEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="4a77e-169"><a name="bk_UpdateEWSMA"> </a></span></span>

<span data-ttu-id="4a77e-170">Use o método [Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) EWS Managed API em um objeto **SearchFolder** para atualizar uma pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4a77e-170">Use the [Folder.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) EWS Managed API method on a **SearchFolder** object to update a search folder.</span></span> <span data-ttu-id="4a77e-171">O exemplo a seguir atualiza os critérios de pesquisa em uma pasta de pesquisa com o nome de exibição "de gerente".</span><span class="sxs-lookup"><span data-stu-id="4a77e-171">The following example updates the search criteria on a search folder with the display name "From Manager".</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void UpdateSearchFolder(ExchangeService service)
{
    FolderView folderView = new FolderView(10);
    folderView.PropertySet = new PropertySet(FolderSchema.DisplayName);
    try
    {
        FindFoldersResults findResults = service.FindFolders(WellKnownFolderName.SearchFolders, folderView);
        foreach (Folder folder in findResults.Folders)
        {
            // You cannot request only search folders in 
            // a FindFolders request, so other search folders might also be present.
            if (folder is SearchFolder &amp;&amp; folder.DisplayName.Equals("From Manager"))
            {
                Console.WriteLine("\"{0}\" folder found.", folder.DisplayName);
                SearchFolder searchFolder = folder as SearchFolder;
                EmailAddress newManager = new EmailAddress("hope@contoso.com");
                SearchFilter.IsEqualTo newManagerFilter =
                    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, newManager);
                searchFolder.SearchParameters.SearchFilter = newManagerFilter;
                searchFolder.SearchParameters.RootFolderIds.Add(WellKnownFolderName.Inbox);
                searchFolder.SearchParameters.Traversal = SearchFolderTraversal.Deep;
                searchFolder.Update();
                Console.WriteLine("\"{0}\" folder updated.", folder.DisplayName);
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

## <a name="update-a-search-folder-by-using-ews"></a><span data-ttu-id="4a77e-172">Atualizar uma pasta de pesquisa usando o EWS</span><span class="sxs-lookup"><span data-stu-id="4a77e-172">Update a search folder by using EWS</span></span>
<span data-ttu-id="4a77e-173"><a name="bk_UpdateEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="4a77e-173"><a name="bk_UpdateEWS"> </a></span></span>

<span data-ttu-id="4a77e-174">Se você estiver usando o EWS, use a [operação UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) com um elemento [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) para atualizar uma pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4a77e-174">If you're using EWS, use the [UpdateFolder operation](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) with a [SearchFolder](https://msdn.microsoft.com/library/1a7d408b-2e98-4391-8834-085ed6d5757c%28Office.15%29.aspx) element to update a search folder.</span></span> <span data-ttu-id="4a77e-175">O exemplo de solicitação a seguir atualiza os critérios de pesquisa na pasta de pesquisa "do gerente".</span><span class="sxs-lookup"><span data-stu-id="4a77e-175">The following request example updates the search criteria on the "From Manager" search folder.</span></span> 
  
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
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="AAMkAGM2..." ChangeKey="CAAAABYA..." />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:SearchParameters" />
              <t:SearchFolder>
                <t:SearchParameters Traversal="Deep">
                  <t:Restriction>
                    <t:IsEqualTo>
                      <t:FieldURI FieldURI="message:Sender" />
                      <t:FieldURIOrConstant>
                        <t:Constant Value="hope@contoso.com" />
                      </t:FieldURIOrConstant>
                    </t:IsEqualTo>
                  </t:Restriction>
                  <t:BaseFolderIds>
                    <t:DistinguishedFolderId Id="inbox" />
                  </t:BaseFolderIds>
                </t:SearchParameters>
              </t:SearchFolder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="4a77e-176">O servidor responde com uma mensagem [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) que inclui um valor [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica êxito.</span><span class="sxs-lookup"><span data-stu-id="4a77e-176">The server responds with an [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates success.</span></span>
  
## <a name="delete-a-search-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="4a77e-177">Excluir uma pasta de pesquisa usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="4a77e-177">Delete a search folder by using the EWS Managed API</span></span>
<span data-ttu-id="4a77e-178"><a name="bk_DeleteEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="4a77e-178"><a name="bk_DeleteEWSMA"> </a></span></span>

<span data-ttu-id="4a77e-179">Use o método [Folder. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) EWS Managed API em um objeto **SearchFolder** para excluir uma pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4a77e-179">Use the [Folder.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) EWS Managed API method on a **SearchFolder** object to delete a search folder.</span></span> <span data-ttu-id="4a77e-180">O exemplo a seguir exclui uma pasta de pesquisa com o nome de exibição "de gerente".</span><span class="sxs-lookup"><span data-stu-id="4a77e-180">The following example deletes a search folder with the display name "From Manager".</span></span> <span data-ttu-id="4a77e-181">A pasta de pesquisa excluída é movida para a pasta itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="4a77e-181">The deleted search folder is moved to the Deleted Items folder.</span></span> 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void DeleteSearchFolder(ExchangeService service)
{
    FolderView folderView = new FolderView(10);
    folderView.PropertySet = new PropertySet(FolderSchema.DisplayName);
    try
    {
        FindFoldersResults findResults = service.FindFolders(WellKnownFolderName.SearchFolders, folderView);
        foreach (Folder folder in findResults.Folders)
        {
            // You cannot request only search folders in 
            // a FindFolders request, so other folders might also be present.
            if (folder is SearchFolder &amp;&amp; folder.DisplayName.Equals("From Manager"))
            {
                Console.WriteLine("\"{0}\" folder found.", folder.DisplayName);
                folder.Delete(DeleteMode.MoveToDeletedItems);
                Console.WriteLine("\"{0}\" folder deleted.", folder.DisplayName);
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

## <a name="delete-a-search-folder-by-using-ews"></a><span data-ttu-id="4a77e-182">Excluir uma pasta de pesquisa usando o EWS</span><span class="sxs-lookup"><span data-stu-id="4a77e-182">Delete a search folder by using EWS</span></span>
<span data-ttu-id="4a77e-183"><a name="bk_DeleteEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="4a77e-183"><a name="bk_DeleteEWS"> </a></span></span>

<span data-ttu-id="4a77e-184">Se você estiver usando o EWS, use a [operação DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) para excluir uma pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4a77e-184">If you're using EWS, use the [DeleteFolder operation](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) to delete a search folder.</span></span> <span data-ttu-id="4a77e-185">O exemplo a seguir exclui uma pasta de pesquisa e a move para a pasta itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="4a77e-185">The following example deletes a search folder and moves it to the Deleted Items folder.</span></span> 
  
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
    <m:DeleteFolder DeleteType="MoveToDeletedItems">
      <m:FolderIds>
        <t:FolderId Id="AAMkAGM2..." ChangeKey="CAAAABYA..." />
      </m:FolderIds>
    </m:DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="4a77e-186">O servidor responde com uma mensagem [DeleteFolderResponse](https://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) que inclui um valor [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) de **NOERROR**, que indica êxito.</span><span class="sxs-lookup"><span data-stu-id="4a77e-186">The server responds with a [DeleteFolderResponse](https://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates success.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="4a77e-187">Também consulte</span><span class="sxs-lookup"><span data-stu-id="4a77e-187">See also</span></span>

- [<span data-ttu-id="4a77e-188">Pesquisar e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4a77e-188">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)   
- [<span data-ttu-id="4a77e-189">Usar filtros de pesquisa com o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4a77e-189">Use search filters with EWS in Exchange</span></span>](how-to-use-search-filters-with-ews-in-exchange.md)    
- [<span data-ttu-id="4a77e-190">Classe SearchFolder</span><span class="sxs-lookup"><span data-stu-id="4a77e-190">SearchFolder class</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="4a77e-191">Operação CreateFolder</span><span class="sxs-lookup"><span data-stu-id="4a77e-191">CreateFolder operation</span></span>](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx)    
- [<span data-ttu-id="4a77e-192">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="4a77e-192">FindFolder operation</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)   
- [<span data-ttu-id="4a77e-193">Operação GetFolder</span><span class="sxs-lookup"><span data-stu-id="4a77e-193">GetFolder operation</span></span>](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)    
- [<span data-ttu-id="4a77e-194">Operação UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="4a77e-194">UpdateFolder operation</span></span>](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)    
- [<span data-ttu-id="4a77e-195">Operação DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="4a77e-195">DeleteFolder operation</span></span>](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx)
    

