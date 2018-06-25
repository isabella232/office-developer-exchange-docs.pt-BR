---
title: Trabalhar com pastas usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 4b3eb746-74c4-42a0-aa2c-742c147f1871
description: Saiba como criar, obter, atualizar e excluir pastas usando a API gerenciada de EWS ou EWS no Exchange.
ms.openlocfilehash: a9a9e5974b2751268f37a1c9faacce43a333bcdb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750859"
---
# <a name="work-with-folders-by-using-ews-in-exchange"></a><span data-ttu-id="d9ea7-103">Trabalhar com pastas usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d9ea7-103">Work with folders by using EWS in Exchange</span></span>

<span data-ttu-id="d9ea7-104">Saiba como criar, obter, atualizar e excluir pastas usando a API gerenciada de EWS ou EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-104">Learn how to create, get, update, and delete folders by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="d9ea7-105">EWS no Exchange usa pastas para estruturar e organizar as caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-105">EWS in Exchange uses folders to structure and organize mailboxes.</span></span> <span data-ttu-id="d9ea7-106">Você pode criar novos, obter, atualizar e excluir pastas usando a API gerenciada de EWS ou o EWS.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-106">You can create new, get, update, and delete folders by using the EWS Managed API or EWS.</span></span> <span data-ttu-id="d9ea7-107">Cada um dos métodos ou operações listadas na tabela a seguir é executada em um objeto [Folder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) , um tipo de [pasta](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) ou [uma das classes derivadas de pasta ou tipos](folders-and-items-in-ews-in-exchange.md#bk_folders).</span><span class="sxs-lookup"><span data-stu-id="d9ea7-107">Each of the methods or operations listed in the following table is performed on a [Folder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) object, a [Folder](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) type, or [one of the derived folder classes or types](folders-and-items-in-ews-in-exchange.md#bk_folders).</span></span>
  
<span data-ttu-id="d9ea7-108">**Tabela 1. Métodos e as operações para criar, obter, atualizando e excluindo pastas**</span><span class="sxs-lookup"><span data-stu-id="d9ea7-108">**Table 1. Methods and operations for creating, getting, updating and deleting folders**</span></span>

|<span data-ttu-id="d9ea7-109">**Para...**</span><span class="sxs-lookup"><span data-stu-id="d9ea7-109">**In order to…**</span></span>|<span data-ttu-id="d9ea7-110">**Método API gerenciada de EWS**</span><span class="sxs-lookup"><span data-stu-id="d9ea7-110">**EWS Managed API method**</span></span>|<span data-ttu-id="d9ea7-111">**Operação do EWS**</span><span class="sxs-lookup"><span data-stu-id="d9ea7-111">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d9ea7-112">Crie uma pasta</span><span class="sxs-lookup"><span data-stu-id="d9ea7-112">Create a folder</span></span>  <br/> |[<span data-ttu-id="d9ea7-113">Folder.Save</span><span class="sxs-lookup"><span data-stu-id="d9ea7-113">Folder.Save</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d9ea7-114">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="d9ea7-114">CreateFolder</span></span>](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="d9ea7-115">Criar uma hierarquia de pastas</span><span class="sxs-lookup"><span data-stu-id="d9ea7-115">Create a folder hierarchy</span></span>  <br/> |<span data-ttu-id="d9ea7-116">Não disponível</span><span class="sxs-lookup"><span data-stu-id="d9ea7-116">Not available</span></span>  <br/> |[<span data-ttu-id="d9ea7-117">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="d9ea7-117">CreateFolderPath</span></span>](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="d9ea7-118">Obtenha uma pasta</span><span class="sxs-lookup"><span data-stu-id="d9ea7-118">Get a folder</span></span>  <br/> |[<span data-ttu-id="d9ea7-119">Folder.Bind</span><span class="sxs-lookup"><span data-stu-id="d9ea7-119">Folder.Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d9ea7-120">GetFolder</span><span class="sxs-lookup"><span data-stu-id="d9ea7-120">GetFolder</span></span>](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="d9ea7-121">Obtenha uma hierarquia de pastas</span><span class="sxs-lookup"><span data-stu-id="d9ea7-121">Get a folder hierarchy</span></span>  <br/> |[<span data-ttu-id="d9ea7-122">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="d9ea7-122">Folder.FindFolders</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d9ea7-123">FindFolder</span><span class="sxs-lookup"><span data-stu-id="d9ea7-123">FindFolder</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="d9ea7-124">Atualizar uma pasta</span><span class="sxs-lookup"><span data-stu-id="d9ea7-124">Update a folder</span></span>  <br/> |[<span data-ttu-id="d9ea7-125">Folder.Update</span><span class="sxs-lookup"><span data-stu-id="d9ea7-125">Folder.Update</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d9ea7-126">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="d9ea7-126">UpdateFolder</span></span>](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="d9ea7-127">Excluir uma pasta</span><span class="sxs-lookup"><span data-stu-id="d9ea7-127">Delete a folder</span></span>  <br/> |[<span data-ttu-id="d9ea7-128">Folder.Delete</span><span class="sxs-lookup"><span data-stu-id="d9ea7-128">Folder.Delete</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="d9ea7-129">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="d9ea7-129">DeleteFolder</span></span>](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |

<span data-ttu-id="d9ea7-130"><a name="bk_createfolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="d9ea7-130"></span></span>

## <a name="create-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="d9ea7-131">Crie uma pasta usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="d9ea7-131">Create a folder by using the EWS Managed API</span></span>

<span data-ttu-id="d9ea7-132">O exemplo de código a seguir mostra como usar a classe de [pasta](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) para criar uma nova pasta genérica com um [DisplayName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) de "Custom pasta" e um valor da propriedade [FolderClass](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.folderclass%28v=exchg.80%29.aspx) de falha de página inválida. Nota.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-132">The following code example shows how to use the [Folder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) class to create a new generic folder with a [DisplayName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) of "Custom Folder" and a [FolderClass](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.folderclass%28v=exchg.80%29.aspx) property value of IPF.Note.</span></span> <span data-ttu-id="d9ea7-133">O método [Folder.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) salva a pasta como uma pasta filho da pasta caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-133">The [Folder.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) method saves the folder as a child folder of the Inbox folder.</span></span> 
  
<span data-ttu-id="d9ea7-134">Estes exemplos pressupõem esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-134">These examples assume that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// Create a custom folder.
Folder folder = new Folder(service);
folder.DisplayName = "Custom Folder";
folder.FolderClass = "IPF.Note";
// Save the folder as a child folder of the Inbox.
folder.Save(WellKnownFolderName.Inbox);
```

<span data-ttu-id="d9ea7-135">Para criar um tipo diferente de pasta, como um [CalendarFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx), [ContactsFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx), [SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)ou [TasksFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx), criar uma nova instância da classe específica (em vez da classe genérica da **pasta** ) e não definir a Propriedade **FolderClass** .</span><span class="sxs-lookup"><span data-stu-id="d9ea7-135">To create a different type of folder, such as a [CalendarFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx), [ContactsFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx), [SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx), or [TasksFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx), create a new instance of the specific class (instead of the generic **Folder** class) and do not set the **FolderClass** property.</span></span> <span data-ttu-id="d9ea7-136">Por exemplo, o exemplo de código a seguir mostra como criar um novo [TasksFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="d9ea7-136">For example, the following code example shows how to create a new [TasksFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx).</span></span>
  
```cs
// Create a custom Tasks folder.
TasksFolder folder = new TasksFolder(service);
folder.DisplayName = "Custom Tasks";
// Save the folder as a child folder in the Inbox folder.
// This method call results in a CreateFolder call to EWS.
folder.Save(WellKnownFolderName.Inbox);
```

<span data-ttu-id="d9ea7-137">Se você tentar criar uma instância de uma classe específica e também definir a propriedade **FolderClass** , o erro [ErrorNoFolderClassOverride](http://msdn.microsoft.com/en-us/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) é disparado.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-137">If you try to create an instance of a specific class and also set the **FolderClass** property, the [ErrorNoFolderClassOverride](http://msdn.microsoft.com/en-us/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) error is thrown.</span></span> 
  
<span data-ttu-id="d9ea7-138">Observe que você não pode lote a criação de várias pastas em uma única chamada de método usando a API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-138">Note that you cannot batch the creation of multiple folders in a single method call by using the EWS Managed API.</span></span>
  
## <a name="create-a-folder-by-using-ews"></a><span data-ttu-id="d9ea7-139">Criar uma pasta usando o EWS</span><span class="sxs-lookup"><span data-stu-id="d9ea7-139">Create a folder by using EWS</span></span>
<span data-ttu-id="d9ea7-140"><a name="bk_createfolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="d9ea7-140"></span></span>

<span data-ttu-id="d9ea7-141">Você pode criar uma única pasta ou múltiplo de pastas usando o EWS.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-141">You can create a single folder or multiple of folders by using EWS.</span></span>
  
<span data-ttu-id="d9ea7-142">Para criar uma única pasta, envie uma mensagem de solicitação de operação [CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d9ea7-142">To create a single folder, send a [CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) operation request message.</span></span> <span data-ttu-id="d9ea7-143">A solicitação de operação **CreateFolder** indica que a pasta pai é a caixa de entrada, o [DisplayName](http://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx) é "Custom pasta" e o valor do elemento [FolderClass](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) é IPF. Nota.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-143">The **CreateFolder** operation request indicates that the parent folder is the Inbox, the [DisplayName](http://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx) is "Custom Folder", and the [FolderClass](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) element value is IPF.Note.</span></span> 
  
<span data-ttu-id="d9ea7-144">Isso também é a solicitação XML que o EWS Managed API envia quando você cria uma nova pasta e chame o método [Folder.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d9ea7-144">This is also the XML request that the EWS Managed API sends when you create a new folder and call the [Folder.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateFolder>
      <m:ParentFolderId>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderId>
      <m:Folders>
        <t:Folder>
          <t:FolderClass>IPF.Note</t:FolderClass>
          <t:DisplayName>Custom Folder</t:DisplayName>
        </t:Folder>
      </m:Folders>
    </m:CreateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="d9ea7-145">O servidor responde à solicitação **CreateFolder** com uma mensagem de [CreateFolderResponse](http://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) que inclui um valor de [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) de **NoError**, que indica se a pasta foi criada com êxito e o [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) de a mensagem recém-criado.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-145">The server responds to the **CreateFolder** request with a [CreateFolderResponse](http://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the folder was created successfully, and the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the newly created message.</span></span> 
  
<span data-ttu-id="d9ea7-146">Para criar várias pastas, inclua vários elementos de [pasta](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) na mensagem de solicitação de operação **CreateFolder** .</span><span class="sxs-lookup"><span data-stu-id="d9ea7-146">To create multiple folders, include multiple [Folder](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) elements in the **CreateFolder** operation request message.</span></span> <span data-ttu-id="d9ea7-147">Todas as novas pastas devem ser na mesma pasta pai.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-147">All the new folders must be in the same parent folder.</span></span> 
  
## <a name="create-a-folder-hierarchy-by-using-ews"></a><span data-ttu-id="d9ea7-148">Criar uma hierarquia de pastas usando o EWS</span><span class="sxs-lookup"><span data-stu-id="d9ea7-148">Create a folder hierarchy by using EWS</span></span>
<span data-ttu-id="d9ea7-149"><a name="bk_createfolderhierarchy"> </a></span><span class="sxs-lookup"><span data-stu-id="d9ea7-149"></span></span>

<span data-ttu-id="d9ea7-150">Você pode criar uma hierarquia de pastas em uma única chamada usando a operação de EWS [CreateFolderPath](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d9ea7-150">You can create a folder hierarchy in a single call by using the EWS [CreateFolderPath](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="d9ea7-151">A mesma funcionalidade não está disponível na API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-151">The same functionality is not available in the EWS Managed API.</span></span> <span data-ttu-id="d9ea7-152">Em vez disso, se você estiver usando o EWS Managed API, você pode criar uma das pastas, conforme mostrado em [criar uma pasta usando o EWS](#bk_createfolderews).</span><span class="sxs-lookup"><span data-stu-id="d9ea7-152">Instead, if you are using the EWS Managed API, you can create folders one by one, as shown in [Create a folder by using EWS](#bk_createfolderews).</span></span>
  
> [!NOTE]
> <span data-ttu-id="d9ea7-153">A API gerenciada EWS não implementa essa funcionalidade.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-153">The EWS Managed API does not implement this functionality.</span></span> 
  
## <a name="get-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="d9ea7-154">Obtenha uma pasta usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="d9ea7-154">Get a folder by using the EWS Managed API</span></span>
<span data-ttu-id="d9ea7-155"><a name="bk_getfolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="d9ea7-155"></span></span>

<span data-ttu-id="d9ea7-156">O exemplo de código a seguir mostra como usar o método [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) para obter a pasta de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-156">The following code example shows how to use the [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method to get the Inbox folder.</span></span> <span data-ttu-id="d9ea7-157">Como prática recomendada, limite as propriedades retornadas somente àqueles necessários para seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-157">As a best practice, limit the properties returned to only those required for your application.</span></span> <span data-ttu-id="d9ea7-158">Este exemplo limita as propriedades de retorno para incluir apenas a propriedade [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) criando um objeto [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) e aplicando o valor de [IdOnly](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) à propriedade [BasePropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset.basepropertyset%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d9ea7-158">This example limits the return properties to only include the [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) property by creating a [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) object and applying the [IdOnly](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) value to the [BasePropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset.basepropertyset%28v=exchg.80%29.aspx) property.</span></span> 
  
<span data-ttu-id="d9ea7-159">Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-159">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// As a best practice, limit the properties returned to only those that are required.
// In this scenario, you only need the FolderId.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly);
// Bind to an existing folder and get only the properties specified in the PropertySet.
// This method call results in a GetFolder call to EWS.
Folder rootfolder = Folder.Bind(service, WellKnownFolderName.Inbox, propSet);
```

<span data-ttu-id="d9ea7-160">Se você precisar retornar propriedades adicionais, adicionar propriedades da classe [FolderSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderschema%28v=exchg.80%29.aspx) para o **PropertySet**ou use um dos sobrecarregados métodos [vincular](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) retorna todas as propriedades de primeira classe.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-160">If you need to return additional properties, add properties from the [FolderSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderschema%28v=exchg.80%29.aspx) class to the **PropertySet**, or use one of the overloaded [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) methods that returns all first class properties.</span></span> 
  
<span data-ttu-id="d9ea7-161">Observe que você não pode obter várias pastas de uma só vez usando a API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-161">Note that you cannot get multiple folders at one time by using the EWS Managed API.</span></span> <span data-ttu-id="d9ea7-162">Você precisará chamar o método **associar** cada pasta separadamente.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-162">You have to call the **Bind** method on each folder separately.</span></span> 
  
## <a name="get-a-folder-by-using-ews"></a><span data-ttu-id="d9ea7-163">Obter uma pasta usando o EWS</span><span class="sxs-lookup"><span data-stu-id="d9ea7-163">Get a folder by using EWS</span></span>
<span data-ttu-id="d9ea7-164"><a name="bk_getfolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="d9ea7-164"></span></span>

<span data-ttu-id="d9ea7-165">Você pode obter uma única pasta ou várias pastas usando o EWS.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-165">You can get a single folder or multiple folders by using EWS.</span></span>
  
<span data-ttu-id="d9ea7-166">Para obter uma única pasta, envie uma mensagem de solicitação de operação [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) para o servidor.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-166">To get a single folder, send a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request message to the server.</span></span> <span data-ttu-id="d9ea7-167">No exemplo a seguir, o [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) é definido para **IdOnly**, para que apenas o [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) da pasta especificada será retornado.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-167">In the following example, the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) is set to **IdOnly**, so only the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the specified folder is returned.</span></span> <span data-ttu-id="d9ea7-168">O elemento [FolderIds](http://msdn.microsoft.com/library/3ff9d15a-7220-4785-ae6b-583a7eb82005%28Office.15%29.aspx) indica que a pasta para recuperar a pasta de caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-168">The [FolderIds](http://msdn.microsoft.com/library/3ff9d15a-7220-4785-ae6b-583a7eb82005%28Office.15%29.aspx) element indicates that the folder to retrieve is the Inbox folder.</span></span> 
  
<span data-ttu-id="d9ea7-169">Isso também é a solicitação XML que o EWS Managed API envia ao vincular a uma pasta usando o método [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d9ea7-169">This is also the XML request that the EWS Managed API sends when you bind to a folder by using the [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="d9ea7-170">Para obter várias pastas, inclua vários elementos de [FolderIds](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) na mensagem de solicitação de operação **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="d9ea7-170">To get multiple folders, include multiple [FolderIds](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) elements in the **GetFolder** operation request message.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="d9ea7-171">O exemplo XML a seguir mostra a mensagem de [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) é enviada do servidor para o cliente em resposta à solicitação de operação **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="d9ea7-171">The following XML example shows the [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) message that is sent from the server to the client in response to the **GetFolder** operation request.</span></span> <span data-ttu-id="d9ea7-172">Ele contém apenas o valor de [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) da pasta caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-172">It only contains the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) value of the Inbox folder.</span></span> <span data-ttu-id="d9ea7-173">Os valores de alguns atributos e elementos foram diminuídos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-173">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="800"
                         MinorBuildNumber="16"
                         Version="V2_6"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AAAENAAA=" ChangeKey="AQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAEkbCr"/>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

## <a name="get-a-folder-hierarchy-by-using-the-ews-managed-api"></a><span data-ttu-id="d9ea7-174">Obtenha uma hierarquia de pastas usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="d9ea7-174">Get a folder hierarchy by using the EWS Managed API</span></span>
<span data-ttu-id="d9ea7-175"><a name="bk_getfolderhierarchyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="d9ea7-175"></span></span>

<span data-ttu-id="d9ea7-176">O exemplo de código a seguir mostra como recuperar as subpastas de uma pasta raiz especificada.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-176">The following code example shows how to retrieve the subfolders for a specified root folder.</span></span> <span data-ttu-id="d9ea7-177">Este exemplo recupera as subpastas da pasta **MsgFolderRoot** , que é a raiz da subárvore IPM (onde suas pastas de caixa de correio e os itens são armazenados).</span><span class="sxs-lookup"><span data-stu-id="d9ea7-177">This example retrieves the subfolders of the **MsgFolderRoot** folder, which is the root of the IPM Subtree (where your mailbox folders and items are stored).</span></span> 
  
<span data-ttu-id="d9ea7-178">Neste exemplo, um objeto de classe [FolderView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) é criado para limitar os resultados da resposta [Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) método.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-178">In this example, a [FolderView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) class object is created to limit the results of the [Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) method response.</span></span> <span data-ttu-id="d9ea7-179">Este cenário limita as propriedades para retornar o seguinte: [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx), [DisplayName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx)e a propriedade estendida que indica se a pasta é uma pasta oculta.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-179">This scenario limits the properties to return to the following: [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx), [DisplayName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx), and the extended property that indicates whether the folder is a hidden folder.</span></span> <span data-ttu-id="d9ea7-180">Defina o valor de [FolderView.Traversal](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview.traversal%28v=EXCHG.80%29.aspx) para profunda para executar uma pesquisa recursiva para que o servidor recupera as subpastas e defina a pasta raiz para **MsgFolderRoot**, para que o servidor retorna todas as pastas do usuário (e o servidor não retorna pastas do sistema na subárvore Non-IPM).</span><span class="sxs-lookup"><span data-stu-id="d9ea7-180">Set the [FolderView.Traversal](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview.traversal%28v=EXCHG.80%29.aspx) value to Deep to perform a recursive search so that the server retrieves the subfolders, and set the root folder to **MsgFolderRoot**, so that the server returns all the user's folders (and the server does not return system folders in the Non-IPM Subtree).</span></span>
  
<span data-ttu-id="d9ea7-181">Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-181">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```XML
// Create a new folder view, and pass in the maximum number of folders to return.
FolderView view = new FolderView(folderViewSize);
// Create an extended property definition for the PR_ATTR_HIDDEN property,
// so that your results will indicate whether the folder is a hidden folder.
ExtendedPropertyDefinition isHiddenProp = new ExtendedPropertyDefinition(0x10f4, MapiPropertyType.Boolean);
// As a best practice, limit the properties returned to only those required.
// In this case, return the folder ID, DisplayName, and the value of the isHiddenProp
// extended property.
view.PropertySet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.DisplayName, isHiddenProp);
// Indicate a Traversal value of Deep, so that all subfolders are retrieved.
view.Traversal = FolderTraversal.Deep;
// Call FindFolders to retrieve the folder hierarchy, starting with the MsgFolderRoot folder.
// This method call results in a FindFolder call to EWS.
FindFoldersResults findFolderResults = service.FindFolders(WellKnownFolderName.MsgFolderRoot, view);
```

## <a name="get-a-folder-hierarchy-by-using-ews"></a><span data-ttu-id="d9ea7-182">Obtenha uma hierarquia de pastas usando o EWS</span><span class="sxs-lookup"><span data-stu-id="d9ea7-182">Get a folder hierarchy by using EWS</span></span>
<span data-ttu-id="d9ea7-183"><a name="bk_getfolderhierarchyews"> </a></span><span class="sxs-lookup"><span data-stu-id="d9ea7-183"></span></span>

<span data-ttu-id="d9ea7-184">Os exemplos XML a seguir mostram como usar a operação [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) para recuperar uma hierarquia de pastas usando o EWS.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-184">The following XML examples show how to use the [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) operation to retrieve a folder hierarchy by using EWS.</span></span> <span data-ttu-id="d9ea7-185">Este exemplo recupera a pasta de **msgfolderroot** , que é a raiz da subárvore IPM e todas as suas subpastas.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-185">This example retrieves the **msgfolderroot** folder, which is the root of the IPM Subtree, and all its subfolders.</span></span> <span data-ttu-id="d9ea7-186">O atributo de **passagem** é definido como **minuciosa** para que o servidor executa uma pesquisa recursiva da hierarquia de pastas e retorna apenas as pastas e subpastas sob a raiz especificada na resposta.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-186">The **Traversal** attribute is set to **Deep** so that the server performs a recursive search of the folder hierarchy and only returns folders and subfolders under the specified root in the response.</span></span> <span data-ttu-id="d9ea7-187">Neste exemplo, o elemento [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) é definido como **IdOnly** para que o servidor retorna apenas o elemento [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d9ea7-187">In this example, the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element is set to **IdOnly** so that the server only returns the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="d9ea7-188">Para facilitar a saída entender, inclua o elemento **DisplayName** em seus resultados incluindo-o no elemento [AdditionalProperties](http://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) na solicitação, juntamente com o valor de **ExtendedFieldURI** para o **PR_ATTR_HIDDEN** propriedade, para que você saiba se as pastas são pastas ocultas.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-188">To make the output easier to understand, include the **DisplayName** element in your results by including it in the [AdditionalProperties](http://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) element in the request, along with the **ExtendedFieldURI** value for the **PR_ATTR_HIDDEN** property, so that you know whether the folders are hidden folders.</span></span> 
  
<span data-ttu-id="d9ea7-189">Isso também é a solicitação XML que o EWS Managed API envia ao chamar o método [FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d9ea7-189">This is also the XML request that the EWS Managed API sends when you call the [FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Deep">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="100"
                               Offset="0"
                               BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="msgfolderroot" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="d9ea7-190">O exemplo XML a seguir mostra a mensagem de [FindFolderResponse](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) é enviada do servidor para o cliente em resposta à solicitação de operação **FindFolder** .</span><span class="sxs-lookup"><span data-stu-id="d9ea7-190">The following XML example shows the [FindFolderResponse](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) message that is sent from the server to the client in response to the **FindFolder** operation request.</span></span> <span data-ttu-id="d9ea7-191">Ele contém apenas a [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx), [DisplayName](http://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx), e o valor do **PR_ATTR_HIDDEN** estendido de propriedade para todas as subpastas sob a pasta **msgrootfolder** .</span><span class="sxs-lookup"><span data-stu-id="d9ea7-191">It contains only the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx), the [DisplayName](http://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx), and the value of the **PR_ATTR_HIDDEN** extended property for all the subfolders under the **msgrootfolder** folder.</span></span> <span data-ttu-id="d9ea7-192">Se o elemento de [valor](http://msdn.microsoft.com/library/9a30cadd-909e-41b1-b4e9-291643dd89c6%28Office.15%29.aspx) for definido como true, a pasta deve estar ocultos em modo de exibição de cliente.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-192">If the [Value](http://msdn.microsoft.com/library/9a30cadd-909e-41b1-b4e9-291643dd89c6%28Office.15%29.aspx) element is set to true, the folder should be hidden in the client view.</span></span> 
  
<span data-ttu-id="d9ea7-193">Isso também é a resposta XML que o EWS Managed API envia quando você obtiver várias pastas usando o método [FindFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d9ea7-193">This is also the XML response that the EWS Managed API sends when you get multiple folders by using the [FindFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="d9ea7-194">Os valores de alguns atributos e elementos foram diminuídos para facilitar a leitura e algumas pastas não foram incluídas para fins de concisão.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-194">The values of some attributes and elements have been shortened for readability, and some folders have not been included for brevity.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="815"
                         MinorBuildNumber="6"
                         Version="V2_7"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="16"
                        TotalItemsInView="16"
                        IncludesLastItemInRange="true">
            <t:Folders>
              <t:CalendarFolder>
                <t:FolderId Id="AAAEOAAA="
                            ChangeKey="AgAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAA3"/>
                <t:DisplayName>Calendar</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>false</t:Value>
                </t:ExtendedProperty>
              </t:CalendarFolder>
              <t:ContactsFolder>
                <t:FolderId Id="AAAEPAAA="
                            ChangeKey="AwAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAA4"/>
                <t:DisplayName>Contacts</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>false</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="AAAUKAAA="
                            ChangeKey="AwAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAS5"/>
                <t:DisplayName>Recipient Cache</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:Folder>
                <t:FolderId Id="AAAUJAAA="
                            ChangeKey="AQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAASx"/>
                <t:DisplayName>Conversation Action Settings</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
…
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

## <a name="update-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="d9ea7-195">Atualizar uma pasta usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="d9ea7-195">Update a folder by using the EWS Managed API</span></span>
<span data-ttu-id="d9ea7-196"><a name="bk_updatefolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="d9ea7-196"></span></span>

<span data-ttu-id="d9ea7-197">O exemplo de código a seguir mostra como atualizar o nome de exibição de uma pasta usando a API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-197">The following code example shows how to update the display name of a folder by using the EWS Managed API.</span></span>
  
<span data-ttu-id="d9ea7-198">Primeiro, crie um [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) para limitar o número de propriedades que o servidor retorna na resposta [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d9ea7-198">First, create a [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) to limit the number of properties that the server returns in the [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) response.</span></span> <span data-ttu-id="d9ea7-199">Recomendamos que você use o **IdOnly** **BasePropertySet** para reduzir chamadas para o banco de dados do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-199">We recommend that you use the **IdOnly** **BasePropertySet** to reduce calls to the Exchange database.</span></span> <span data-ttu-id="d9ea7-200">Em seguida, use o método **vincular** para vincular para a pasta ao atualizar.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-200">Next, use the **Bind** method to bind to the folder to update.</span></span> <span data-ttu-id="d9ea7-201">Em seguida, atualize a propriedade [DisplayName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) e use o método [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) para salvar as alterações.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-201">Then, update the [DisplayName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) property, and use the [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method to save the changes.</span></span> 
  
<span data-ttu-id="d9ea7-202">Neste exemplo, vamos pressupor que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-202">In this example, we assume that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="d9ea7-203">A variável local *folderId* é a [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) da pasta para atualizar.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-203">The local variable  *folderId*  is the [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) of the folder to update.</span></span> 
  
```cs
// As a best practice, only include the ID value in the PropertySet.
PropertySet propertySet = new PropertySet(BasePropertySet.IdOnly);
// Bind to an existing folder and get the FolderId.
// This method call results in a GetFolder call to EWS.
Folder folder = Folder.Bind(service, folderId, propertySet);
// Update the display name of the folder.
folder.DisplayName = "Updated folder name";
// Save the updates.
// This method call results in an UpdateFolder call to EWS.
folder.Update();

```

## <a name="update-a-folder-by-using-ews"></a><span data-ttu-id="d9ea7-204">Atualizar uma pasta usando o EWS</span><span class="sxs-lookup"><span data-stu-id="d9ea7-204">Update a folder by using EWS</span></span>
<span data-ttu-id="d9ea7-205"><a name="bk_updatefolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="d9ea7-205"></span></span>

<span data-ttu-id="d9ea7-206">Os exemplos XML a seguir mostram como atualizar o nome de exibição de uma pasta usando o EWS.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-206">The following XML examples show how to update the display name of a folder by using EWS.</span></span>
  
<span data-ttu-id="d9ea7-207">Primeiro, envie uma mensagem de solicitação de operação [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) para obter a pasta para atualizar, conforme mostrado na [obter uma hierarquia de pastas usando o EWS](#bk_getfolderhierarchyews).</span><span class="sxs-lookup"><span data-stu-id="d9ea7-207">First, send a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request message to get the folder to update, as shown in [Get a folder hierarchy by using EWS](#bk_getfolderhierarchyews).</span></span>
  
<span data-ttu-id="d9ea7-208">Em seguida, envie uma mensagem de solicitação de operação [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) para o servidor para atualizar uma pasta.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-208">Next, send an [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) operation request message to the server to update a folder.</span></span> <span data-ttu-id="d9ea7-209">A solicitação de operação **UpdateFolder** atualiza o [DisplayName](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) "Atualizado o sinalizador pasta".</span><span class="sxs-lookup"><span data-stu-id="d9ea7-209">The **UpdateFolder** operation request updates the [DisplayName](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) to "Updated Custom Folder".</span></span> 
  
<span data-ttu-id="d9ea7-210">Isso também é a solicitação XML que o EWS Managed API envia ao atualizar uma pasta usando o método [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d9ea7-210">This is also the XML request that the EWS Managed API sends when you update a folder by using the [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="d9ea7-211">Os valores de alguns atributos e elementos foram diminuídos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-211">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="OrV9ZAAA=" ChangeKey="AQAAABYAAABVzRdyy/cHS4XTC9itCRdUAAAOrXWb" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:DisplayName" />
              <t:Folder>
                <t:DisplayName>Updated Custom Folder</t:DisplayName>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="d9ea7-212">O servidor responde à solicitação **UpdateFolder** com uma mensagem de [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) que inclui o valor [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**e ao [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) da pasta que foi atualizada com uma **atualizado ChangeKey** valor do atributo.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-212">The server responds to the **UpdateFolder** request with a [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes the a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, and the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the folder that was updated with an updated **ChangeKey** attribute value.</span></span> 
  
## <a name="delete-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="d9ea7-213">Excluir uma pasta usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="d9ea7-213">Delete a folder by using the EWS Managed API</span></span>
<span data-ttu-id="d9ea7-214"><a name="bk_deletefolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="d9ea7-214"></span></span>

<span data-ttu-id="d9ea7-215">Este artigo fornece um exemplo básico que mostra como excluir uma pasta usando a API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-215">This article provides a basic example that shows you how to delete a folder by using the EWS Managed API.</span></span> <span data-ttu-id="d9ea7-216">Para obter mais detalhes sobre a exclusão de pastas, consulte [Excluindo itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="d9ea7-216">For more details about deleting folders, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="d9ea7-217">Para excluir uma pasta usando a API gerenciada de EWS, primeiro, use o método de [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) para ligar para o objeto de serviço para a pasta para excluir.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-217">To delete a folder by using the EWS Managed API, first, use the [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method to bind to the service object to the folder to delete.</span></span> <span data-ttu-id="d9ea7-218">Em seguida, use o método [Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) para excluir a pasta usando o modo de exclusão de [HardDelete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d9ea7-218">Next, use the [Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) method to delete the folder by using the [HardDelete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx) deletion mode.</span></span> 
  
<span data-ttu-id="d9ea7-219">Este exemplo supõe que esse **serviço** é um objeto válido do [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) e que o usuário foi autenticado com um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-219">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="d9ea7-220">A variável local *folderId* é a [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) da pasta para excluir.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-220">The local variable  *folderId*  is the [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) of the folder to delete.</span></span> 
  
```cs
// Bind to an existing folder and get all its properties.
// This method call results in a GetFolder call to EWS.
Folder folder = Folder.Bind(service, folderId);
// HardDelete the folder.
// This method call results in a DeleteFolder call to EWS.
folder.Delete(DeleteMode.HardDelete);
```

## <a name="delete-a-folder-by-using-ews"></a><span data-ttu-id="d9ea7-221">Excluir uma pasta usando o EWS</span><span class="sxs-lookup"><span data-stu-id="d9ea7-221">Delete a folder by using EWS</span></span>
<span data-ttu-id="d9ea7-222"><a name="bk_deletefolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="d9ea7-222"></span></span>

<span data-ttu-id="d9ea7-223">Este artigo fornece um exemplo básico de XML que mostra como excluir uma pasta usando o EWS.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-223">This article provides a basic XML example that shows you how to delete a folder by using EWS.</span></span> <span data-ttu-id="d9ea7-224">Para obter mais detalhes sobre a exclusão de pastas, consulte [Excluindo itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="d9ea7-224">For more details about deleting folders, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="d9ea7-225">Para excluir uma pasta usando o EWS, primeiro, envie uma mensagem de solicitação de operação [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) para obter a pasta para atualizar, conforme mostrado na [obter uma pasta usando o EWS](#bk_getfolderews).</span><span class="sxs-lookup"><span data-stu-id="d9ea7-225">To delete a folder by using EWS, first, send a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request message to get the folder to update as shown in [Get a folder by using EWS](#bk_getfolderews).</span></span> 
  
<span data-ttu-id="d9ea7-226">Em seguida, envie uma mensagem de solicitação de operação [DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) para o servidor para excluir a pasta.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-226">Next, send a [DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) operation request message to the server to delete the folder.</span></span> <span data-ttu-id="d9ea7-227">A solicitação de operação **DeleteFolder** indica que o **DeleteType** é **HardDelete** e inclui o [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) da pasta para excluir.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-227">The **DeleteFolder** operation request indicates that the **DeleteType** is **HardDelete** and it includes the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the folder to delete.</span></span> 
  
<span data-ttu-id="d9ea7-228">Isso também é a solicitação XML que o EWS Managed API envia quando você exclui uma pasta usando o método [Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="d9ea7-228">This is also the XML request that the EWS Managed API sends when you delete a folder by using the [Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="d9ea7-229">Os valores de alguns atributos e elementos foram diminuídos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-229">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:DeleteFolder DeleteType="HardDelete">
      <m:FolderIds>
        <t:FolderId Id="OrV9ZAAA=" ChangeKey="AQAAABYAAABVzRdyy/cHS4XTC9itCRdUAAAOrXWf" />
      </m:FolderIds>
    </m:DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="d9ea7-230">O servidor responde à solicitação **DeleteFolder** com uma mensagem de [DeleteFolderResponse](http://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) que inclui o valor [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, que indica que a exclusão de pasta foi bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-230">The server responds to the **DeleteFolder** request with a [DeleteFolderResponse](http://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) message that includes the a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the folder deletion was successful.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="d9ea7-231">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="d9ea7-231">Next steps</span></span>
<span data-ttu-id="d9ea7-232"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="d9ea7-232"></span></span>

<span data-ttu-id="d9ea7-233">Depois que você tiver recuperado as pastas no servidor ou fazer alterações às pastas, convém [sincronizar sua hierarquia de pastas](how-to-synchronize-folders-by-using-ews-in-exchange.md) ou [assinar notificações sobre alterações de pasta](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) no servidor.</span><span class="sxs-lookup"><span data-stu-id="d9ea7-233">After you have retrieved the folders on the server, or made changes to folders, you might want to [synchronize your folder hierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md) or [subscribe to notifications about folder changes](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) on the server.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="d9ea7-234">Confira também</span><span class="sxs-lookup"><span data-stu-id="d9ea7-234">See also</span></span>

- [<span data-ttu-id="d9ea7-235">Pastas e itens no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d9ea7-235">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)   
- [<span data-ttu-id="d9ea7-236">Trabalhar com itens de caixa de correio do Exchange usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d9ea7-236">Work with Exchange mailbox items by using EWS in Exchange</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="d9ea7-237">Excluindo itens usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d9ea7-237">Deleting items by using EWS in Exchange</span></span>](deleting-items-by-using-ews-in-exchange.md)   
- [<span data-ttu-id="d9ea7-238">Develop web service clients for Exchange</span><span class="sxs-lookup"><span data-stu-id="d9ea7-238">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

