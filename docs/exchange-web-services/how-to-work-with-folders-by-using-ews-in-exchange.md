---
title: Trabalhar com pastas usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 4b3eb746-74c4-42a0-aa2c-742c147f1871
description: Saiba como criar, obter, atualizar e excluir pastas usando a API gerenciada do EWS ou o EWS no Exchange.
localization_priority: Priority
ms.openlocfilehash: a184d8da4d6949f01f47afc6a9fb7ed30729fd3b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456378"
---
# <a name="work-with-folders-by-using-ews-in-exchange"></a><span data-ttu-id="fb46c-103">Trabalhar com pastas usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fb46c-103">Work with folders by using EWS in Exchange</span></span>

<span data-ttu-id="fb46c-104">Saiba como criar, obter, atualizar e excluir pastas usando a API gerenciada do EWS ou o EWS no Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb46c-104">Learn how to create, get, update, and delete folders by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="fb46c-105">O EWS no Exchange usa pastas para estruturar e organizar caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="fb46c-105">EWS in Exchange uses folders to structure and organize mailboxes.</span></span> <span data-ttu-id="fb46c-106">Você pode criar novas pastas, obter, atualizar e excluir pastas usando a API gerenciada do EWS ou o EWS.</span><span class="sxs-lookup"><span data-stu-id="fb46c-106">You can create new, get, update, and delete folders by using the EWS Managed API or EWS.</span></span> <span data-ttu-id="fb46c-107">Cada um dos métodos ou operações listados na tabela a seguir é executado em um objeto [Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) , um tipo de [pasta](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) ou [um dos tipos ou classes de pasta derivadas](folders-and-items-in-ews-in-exchange.md#bk_folders).</span><span class="sxs-lookup"><span data-stu-id="fb46c-107">Each of the methods or operations listed in the following table is performed on a [Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) object, a [Folder](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) type, or [one of the derived folder classes or types](folders-and-items-in-ews-in-exchange.md#bk_folders).</span></span>
  
<span data-ttu-id="fb46c-108">**Tabela 1. Métodos e operações para criar, obter, atualizar e excluir pastas**</span><span class="sxs-lookup"><span data-stu-id="fb46c-108">**Table 1. Methods and operations for creating, getting, updating and deleting folders**</span></span>

|<span data-ttu-id="fb46c-109">**Para...**</span><span class="sxs-lookup"><span data-stu-id="fb46c-109">**In order to…**</span></span>|<span data-ttu-id="fb46c-110">**Método de API gerenciada do EWS**</span><span class="sxs-lookup"><span data-stu-id="fb46c-110">**EWS Managed API method**</span></span>|<span data-ttu-id="fb46c-111">**Operação do EWS**</span><span class="sxs-lookup"><span data-stu-id="fb46c-111">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="fb46c-112">Criar uma pasta</span><span class="sxs-lookup"><span data-stu-id="fb46c-112">Create a folder</span></span>  <br/> |[<span data-ttu-id="fb46c-113">Folder. Save</span><span class="sxs-lookup"><span data-stu-id="fb46c-113">Folder.Save</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="fb46c-114">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="fb46c-114">CreateFolder</span></span>](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="fb46c-115">Criar uma hierarquia de pastas</span><span class="sxs-lookup"><span data-stu-id="fb46c-115">Create a folder hierarchy</span></span>  <br/> |<span data-ttu-id="fb46c-116">Não disponível</span><span class="sxs-lookup"><span data-stu-id="fb46c-116">Not available</span></span>  <br/> |[<span data-ttu-id="fb46c-117">Createfolderpath</span><span class="sxs-lookup"><span data-stu-id="fb46c-117">CreateFolderPath</span></span>](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="fb46c-118">Obter uma pasta</span><span class="sxs-lookup"><span data-stu-id="fb46c-118">Get a folder</span></span>  <br/> |[<span data-ttu-id="fb46c-119">Folder. bind</span><span class="sxs-lookup"><span data-stu-id="fb46c-119">Folder.Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="fb46c-120">GetFolder</span><span class="sxs-lookup"><span data-stu-id="fb46c-120">GetFolder</span></span>](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="fb46c-121">Obter uma hierarquia de pastas</span><span class="sxs-lookup"><span data-stu-id="fb46c-121">Get a folder hierarchy</span></span>  <br/> |[<span data-ttu-id="fb46c-122">Folder. FindFolders</span><span class="sxs-lookup"><span data-stu-id="fb46c-122">Folder.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="fb46c-123">FindFolder</span><span class="sxs-lookup"><span data-stu-id="fb46c-123">FindFolder</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="fb46c-124">Atualizar uma pasta</span><span class="sxs-lookup"><span data-stu-id="fb46c-124">Update a folder</span></span>  <br/> |[<span data-ttu-id="fb46c-125">Pasta. Update</span><span class="sxs-lookup"><span data-stu-id="fb46c-125">Folder.Update</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="fb46c-126">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="fb46c-126">UpdateFolder</span></span>](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="fb46c-127">Excluir uma pasta</span><span class="sxs-lookup"><span data-stu-id="fb46c-127">Delete a folder</span></span>  <br/> |[<span data-ttu-id="fb46c-128">Pasta. Delete</span><span class="sxs-lookup"><span data-stu-id="fb46c-128">Folder.Delete</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="fb46c-129">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="fb46c-129">DeleteFolder</span></span>](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |

<span data-ttu-id="fb46c-130"><a name="bk_createfolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="fb46c-130"><a name="bk_createfolderewsma"> </a></span></span>

## <a name="create-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="fb46c-131">Criar uma pasta usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="fb46c-131">Create a folder by using the EWS Managed API</span></span>

<span data-ttu-id="fb46c-132">O exemplo de código a seguir mostra como usar a classe [Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) para criar uma nova pasta genérica com um [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) de "pasta personalizada" e um valor de propriedade [FolderClass](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.folderclass%28v=exchg.80%29.aspx) de IPF. Observação.</span><span class="sxs-lookup"><span data-stu-id="fb46c-132">The following code example shows how to use the [Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) class to create a new generic folder with a [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) of "Custom Folder" and a [FolderClass](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.folderclass%28v=exchg.80%29.aspx) property value of IPF.Note.</span></span> <span data-ttu-id="fb46c-133">O método [Folder. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) salva a pasta como uma pasta filho da pasta caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="fb46c-133">The [Folder.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) method saves the folder as a child folder of the Inbox folder.</span></span> 
  
<span data-ttu-id="fb46c-134">Estes exemplos pressupõem que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb46c-134">These examples assume that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// Create a custom folder.
Folder folder = new Folder(service);
folder.DisplayName = "Custom Folder";
folder.FolderClass = "IPF.Note";
// Save the folder as a child folder of the Inbox.
folder.Save(WellKnownFolderName.Inbox);
```

<span data-ttu-id="fb46c-135">Para criar um tipo diferente de pasta, como [CalendarFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx), [ContactsFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx), [SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)ou [TasksFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx), crie uma nova instância da classe específica (em vez da classe de **pasta** genérica) e não defina a propriedade **FolderClass** .</span><span class="sxs-lookup"><span data-stu-id="fb46c-135">To create a different type of folder, such as a [CalendarFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx), [ContactsFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx), [SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx), or [TasksFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx), create a new instance of the specific class (instead of the generic **Folder** class) and do not set the **FolderClass** property.</span></span> <span data-ttu-id="fb46c-136">Por exemplo, o exemplo de código a seguir mostra como criar um novo [TasksFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="fb46c-136">For example, the following code example shows how to create a new [TasksFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx).</span></span>
  
```cs
// Create a custom Tasks folder.
TasksFolder folder = new TasksFolder(service);
folder.DisplayName = "Custom Tasks";
// Save the folder as a child folder in the Inbox folder.
// This method call results in a CreateFolder call to EWS.
folder.Save(WellKnownFolderName.Inbox);
```

<span data-ttu-id="fb46c-137">Se você tentar criar uma instância de uma classe específica e também definir a propriedade **FolderClass** , o erro [ErrorNoFolderClassOverride](https://msdn.microsoft.com/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) será gerado.</span><span class="sxs-lookup"><span data-stu-id="fb46c-137">If you try to create an instance of a specific class and also set the **FolderClass** property, the [ErrorNoFolderClassOverride](https://msdn.microsoft.com/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) error is thrown.</span></span> 
  
<span data-ttu-id="fb46c-138">Observe que você não pode criar um lote para a criação de várias pastas em uma única chamada de método usando a API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="fb46c-138">Note that you cannot batch the creation of multiple folders in a single method call by using the EWS Managed API.</span></span>
  
## <a name="create-a-folder-by-using-ews"></a><span data-ttu-id="fb46c-139">Criar uma pasta usando o EWS</span><span class="sxs-lookup"><span data-stu-id="fb46c-139">Create a folder by using EWS</span></span>
<span data-ttu-id="fb46c-140"><a name="bk_createfolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="fb46c-140"><a name="bk_createfolderews"> </a></span></span>

<span data-ttu-id="fb46c-141">Você pode criar uma única pasta ou várias pastas usando o EWS.</span><span class="sxs-lookup"><span data-stu-id="fb46c-141">You can create a single folder or multiple of folders by using EWS.</span></span>
  
<span data-ttu-id="fb46c-142">Para criar uma única pasta, envie uma mensagem de solicitação de operação [CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="fb46c-142">To create a single folder, send a [CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) operation request message.</span></span> <span data-ttu-id="fb46c-143">A solicitação de operação **CreateFolder** indica que a pasta pai é a caixa de entrada, o [DisplayName](https://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx) é "Custom Folder" e o valor do elemento [FolderClass](https://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) é IPF. Observação.</span><span class="sxs-lookup"><span data-stu-id="fb46c-143">The **CreateFolder** operation request indicates that the parent folder is the Inbox, the [DisplayName](https://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx) is "Custom Folder", and the [FolderClass](https://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) element value is IPF.Note.</span></span> 
  
<span data-ttu-id="fb46c-144">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você cria uma nova pasta e chama o método [Folder. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="fb46c-144">This is also the XML request that the EWS Managed API sends when you create a new folder and call the [Folder.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="fb46c-145">O servidor responde à solicitação **CreateFolder** com uma mensagem [CreateFolderResponse](https://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) que inclui um valor [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) de **NOERROR**, que indica que a pasta foi criada com êxito e o [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) da mensagem recém-criada.</span><span class="sxs-lookup"><span data-stu-id="fb46c-145">The server responds to the **CreateFolder** request with a [CreateFolderResponse](https://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the folder was created successfully, and the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the newly created message.</span></span> 
  
<span data-ttu-id="fb46c-146">Para criar várias pastas, inclua vários elementos de [pasta](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) na mensagem de solicitação de operação **CreateFolder** .</span><span class="sxs-lookup"><span data-stu-id="fb46c-146">To create multiple folders, include multiple [Folder](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) elements in the **CreateFolder** operation request message.</span></span> <span data-ttu-id="fb46c-147">Todas as novas pastas devem estar na mesma pasta pai.</span><span class="sxs-lookup"><span data-stu-id="fb46c-147">All the new folders must be in the same parent folder.</span></span> 
  
## <a name="create-a-folder-hierarchy-by-using-ews"></a><span data-ttu-id="fb46c-148">Criar uma hierarquia de pastas usando o EWS</span><span class="sxs-lookup"><span data-stu-id="fb46c-148">Create a folder hierarchy by using EWS</span></span>
<span data-ttu-id="fb46c-149"><a name="bk_createfolderhierarchy"> </a></span><span class="sxs-lookup"><span data-stu-id="fb46c-149"><a name="bk_createfolderhierarchy"> </a></span></span>

<span data-ttu-id="fb46c-150">Você pode criar uma hierarquia de pastas em uma única chamada usando a operação EWS [createfolderpath](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="fb46c-150">You can create a folder hierarchy in a single call by using the EWS [CreateFolderPath](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="fb46c-151">A mesma funcionalidade não está disponível na API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="fb46c-151">The same functionality is not available in the EWS Managed API.</span></span> <span data-ttu-id="fb46c-152">Em vez disso, se você estiver usando a API gerenciada do EWS, você pode criar pastas um por um, conforme mostrado em [criar uma pasta usando o EWS](#bk_createfolderews).</span><span class="sxs-lookup"><span data-stu-id="fb46c-152">Instead, if you are using the EWS Managed API, you can create folders one by one, as shown in [Create a folder by using EWS](#bk_createfolderews).</span></span>
  
> [!NOTE]
> <span data-ttu-id="fb46c-153">A API gerenciada EWS não implementa essa funcionalidade.</span><span class="sxs-lookup"><span data-stu-id="fb46c-153">The EWS Managed API does not implement this functionality.</span></span> 
  
## <a name="get-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="fb46c-154">Obter uma pasta usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="fb46c-154">Get a folder by using the EWS Managed API</span></span>
<span data-ttu-id="fb46c-155"><a name="bk_getfolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="fb46c-155"><a name="bk_getfolderewsma"> </a></span></span>

<span data-ttu-id="fb46c-156">O exemplo de código a seguir mostra como usar o método [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) para obter a pasta caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="fb46c-156">The following code example shows how to use the [Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method to get the Inbox folder.</span></span> <span data-ttu-id="fb46c-157">Como prática recomendada, limite as propriedades retornadas somente para as necessárias para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb46c-157">As a best practice, limit the properties returned to only those required for your application.</span></span> <span data-ttu-id="fb46c-158">Este exemplo limita as propriedades de retorno para incluir apenas a propriedade [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) , criando um objeto [PropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) e aplicando o valor [IdOnly](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) à propriedade [BasePropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset.basepropertyset%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="fb46c-158">This example limits the return properties to only include the [Id](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) property by creating a [PropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) object and applying the [IdOnly](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) value to the [BasePropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset.basepropertyset%28v=exchg.80%29.aspx) property.</span></span> 
  
<span data-ttu-id="fb46c-159">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb46c-159">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// As a best practice, limit the properties returned to only those that are required.
// In this scenario, you only need the FolderId.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly);
// Bind to an existing folder and get only the properties specified in the PropertySet.
// This method call results in a GetFolder call to EWS.
Folder rootfolder = Folder.Bind(service, WellKnownFolderName.Inbox, propSet);
```

<span data-ttu-id="fb46c-160">Se você precisar retornar propriedades adicionais, adicione as propriedades da classe [FolderSchema](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderschema%28v=exchg.80%29.aspx) ao **PropertySet**ou use um dos métodos [BIND](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) sobrecarregado que retorna todas as propriedades de primeira classe.</span><span class="sxs-lookup"><span data-stu-id="fb46c-160">If you need to return additional properties, add properties from the [FolderSchema](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderschema%28v=exchg.80%29.aspx) class to the **PropertySet**, or use one of the overloaded [Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) methods that returns all first class properties.</span></span> 
  
<span data-ttu-id="fb46c-161">Observe que você não pode obter várias pastas ao mesmo tempo usando a API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="fb46c-161">Note that you cannot get multiple folders at one time by using the EWS Managed API.</span></span> <span data-ttu-id="fb46c-162">Você precisa chamar o método **BIND** em cada pasta separadamente.</span><span class="sxs-lookup"><span data-stu-id="fb46c-162">You have to call the **Bind** method on each folder separately.</span></span> 
  
## <a name="get-a-folder-by-using-ews"></a><span data-ttu-id="fb46c-163">Obter uma pasta usando o EWS</span><span class="sxs-lookup"><span data-stu-id="fb46c-163">Get a folder by using EWS</span></span>
<span data-ttu-id="fb46c-164"><a name="bk_getfolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="fb46c-164"><a name="bk_getfolderews"> </a></span></span>

<span data-ttu-id="fb46c-165">Você pode obter uma única pasta ou várias pastas usando o EWS.</span><span class="sxs-lookup"><span data-stu-id="fb46c-165">You can get a single folder or multiple folders by using EWS.</span></span>
  
<span data-ttu-id="fb46c-166">Para obter uma única pasta, envie uma mensagem de solicitação de operação [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) para o servidor.</span><span class="sxs-lookup"><span data-stu-id="fb46c-166">To get a single folder, send a [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request message to the server.</span></span> <span data-ttu-id="fb46c-167">No exemplo a seguir, o [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) é definido como **IdOnly**, de modo que somente [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) da pasta especificada é retornado.</span><span class="sxs-lookup"><span data-stu-id="fb46c-167">In the following example, the [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) is set to **IdOnly**, so only the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the specified folder is returned.</span></span> <span data-ttu-id="fb46c-168">O elemento [FolderIds](https://msdn.microsoft.com/library/3ff9d15a-7220-4785-ae6b-583a7eb82005%28Office.15%29.aspx) indica que a pasta a ser recuperada é a pasta caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="fb46c-168">The [FolderIds](https://msdn.microsoft.com/library/3ff9d15a-7220-4785-ae6b-583a7eb82005%28Office.15%29.aspx) element indicates that the folder to retrieve is the Inbox folder.</span></span> 
  
<span data-ttu-id="fb46c-169">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você associa a uma pasta usando o método [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="fb46c-169">This is also the XML request that the EWS Managed API sends when you bind to a folder by using the [Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="fb46c-170">Para obter várias pastas, inclua vários elementos [FolderIds](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) na mensagem de solicitação de operação **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="fb46c-170">To get multiple folders, include multiple [FolderIds](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) elements in the **GetFolder** operation request message.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="fb46c-171">O exemplo de XML a seguir mostra a mensagem [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) que é enviada do servidor para o cliente em resposta à solicitação de operação **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="fb46c-171">The following XML example shows the [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) message that is sent from the server to the client in response to the **GetFolder** operation request.</span></span> <span data-ttu-id="fb46c-172">Ele contém apenas o valor [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) da pasta caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="fb46c-172">It only contains the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) value of the Inbox folder.</span></span> <span data-ttu-id="fb46c-173">Os valores de alguns atributos e elementos foram reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="fb46c-173">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="800"
                         MinorBuildNumber="16"
                         Version="V2_6"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="get-a-folder-hierarchy-by-using-the-ews-managed-api"></a><span data-ttu-id="fb46c-174">Obter uma hierarquia de pastas usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="fb46c-174">Get a folder hierarchy by using the EWS Managed API</span></span>
<span data-ttu-id="fb46c-175"><a name="bk_getfolderhierarchyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="fb46c-175"><a name="bk_getfolderhierarchyewsma"> </a></span></span>

<span data-ttu-id="fb46c-176">O exemplo de código a seguir mostra como recuperar as subpastas de uma pasta raiz especificada.</span><span class="sxs-lookup"><span data-stu-id="fb46c-176">The following code example shows how to retrieve the subfolders for a specified root folder.</span></span> <span data-ttu-id="fb46c-177">Este exemplo recupera as subpastas da pasta **MsgFolderRoot** , que é a raiz da sub-árvore IPM (onde as pastas e os itens da caixa de correio são armazenados).</span><span class="sxs-lookup"><span data-stu-id="fb46c-177">This example retrieves the subfolders of the **MsgFolderRoot** folder, which is the root of the IPM Subtree (where your mailbox folders and items are stored).</span></span> 
  
<span data-ttu-id="fb46c-178">Neste exemplo, um objeto de classe [folderview](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) é criado para limitar os resultados da resposta do método [Folder. FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="fb46c-178">In this example, a [FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) class object is created to limit the results of the [Folder.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) method response.</span></span> <span data-ttu-id="fb46c-179">Este cenário limita as propriedades para retornar ao seguinte: [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx), [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx)e a propriedade estendida que indica se a pasta é uma pasta oculta.</span><span class="sxs-lookup"><span data-stu-id="fb46c-179">This scenario limits the properties to return to the following: [Id](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx), [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx), and the extended property that indicates whether the folder is a hidden folder.</span></span> <span data-ttu-id="fb46c-180">Defina o valor [folderview. Traversal](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.traversal%28v=EXCHG.80%29.aspx) como profundo para executar uma pesquisa recursiva para que o servidor recupere as subpastas e defina a pasta raiz para **MsgFolderRoot**, de modo que o servidor retorne todas as pastas do usuário (e o servidor não retorne pastas de sistema na subárvore não-IPM).</span><span class="sxs-lookup"><span data-stu-id="fb46c-180">Set the [FolderView.Traversal](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.traversal%28v=EXCHG.80%29.aspx) value to Deep to perform a recursive search so that the server retrieves the subfolders, and set the root folder to **MsgFolderRoot**, so that the server returns all the user's folders (and the server does not return system folders in the Non-IPM Subtree).</span></span>
  
<span data-ttu-id="fb46c-181">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb46c-181">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="get-a-folder-hierarchy-by-using-ews"></a><span data-ttu-id="fb46c-182">Obter uma hierarquia de pastas usando o EWS</span><span class="sxs-lookup"><span data-stu-id="fb46c-182">Get a folder hierarchy by using EWS</span></span>
<span data-ttu-id="fb46c-183"><a name="bk_getfolderhierarchyews"> </a></span><span class="sxs-lookup"><span data-stu-id="fb46c-183"><a name="bk_getfolderhierarchyews"> </a></span></span>

<span data-ttu-id="fb46c-184">Os exemplos de XML a seguir mostram como usar a operação [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) para recuperar uma hierarquia de pastas usando o EWS.</span><span class="sxs-lookup"><span data-stu-id="fb46c-184">The following XML examples show how to use the [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) operation to retrieve a folder hierarchy by using EWS.</span></span> <span data-ttu-id="fb46c-185">Este exemplo recupera a pasta **msgfolderroot** , que é a raiz da sub-árvore IPM e todas as suas subpastas.</span><span class="sxs-lookup"><span data-stu-id="fb46c-185">This example retrieves the **msgfolderroot** folder, which is the root of the IPM Subtree, and all its subfolders.</span></span> <span data-ttu-id="fb46c-186">O atributo de **passagem** é definido como **profundo** para que o servidor execute uma pesquisa recursiva da hierarquia de pastas e só retorne pastas e subpastas na raiz especificada na resposta.</span><span class="sxs-lookup"><span data-stu-id="fb46c-186">The **Traversal** attribute is set to **Deep** so that the server performs a recursive search of the folder hierarchy and only returns folders and subfolders under the specified root in the response.</span></span> <span data-ttu-id="fb46c-187">Neste exemplo, o elemento [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) é definido como **IdOnly** para que o servidor retorne apenas o elemento [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="fb46c-187">In this example, the [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element is set to **IdOnly** so that the server only returns the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="fb46c-188">Para facilitar a compreensão da saída, inclua o elemento **DisplayName** nos resultados, incluindo-o no elemento [AdditionalProperties](https://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) na solicitação, junto com o valor **ExtendedFieldURI** para a propriedade **PR_ATTR_HIDDEN** , para que você saiba se as pastas estão ocultas.</span><span class="sxs-lookup"><span data-stu-id="fb46c-188">To make the output easier to understand, include the **DisplayName** element in your results by including it in the [AdditionalProperties](https://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) element in the request, along with the **ExtendedFieldURI** value for the **PR_ATTR_HIDDEN** property, so that you know whether the folders are hidden folders.</span></span> 
  
<span data-ttu-id="fb46c-189">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você chama o método [FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="fb46c-189">This is also the XML request that the EWS Managed API sends when you call the [FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="fb46c-190">O exemplo de XML a seguir mostra a mensagem [FindFolderResponse](https://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) que é enviada do servidor para o cliente em resposta à solicitação de operação **FindFolder** .</span><span class="sxs-lookup"><span data-stu-id="fb46c-190">The following XML example shows the [FindFolderResponse](https://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) message that is sent from the server to the client in response to the **FindFolder** operation request.</span></span> <span data-ttu-id="fb46c-191">Ele contém apenas [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx), [DisplayName](https://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx)e o valor da propriedade estendida **PR_ATTR_HIDDEN** para todas as subpastas na pasta **msgrootfolder**</span><span class="sxs-lookup"><span data-stu-id="fb46c-191">It contains only the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx), the [DisplayName](https://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx), and the value of the **PR_ATTR_HIDDEN** extended property for all the subfolders under the **msgrootfolder** folder.</span></span> <span data-ttu-id="fb46c-192">Se o elemento [Value](https://msdn.microsoft.com/library/9a30cadd-909e-41b1-b4e9-291643dd89c6%28Office.15%29.aspx) for definido como true, a pasta deverá estar oculta no modo de exibição do cliente.</span><span class="sxs-lookup"><span data-stu-id="fb46c-192">If the [Value](https://msdn.microsoft.com/library/9a30cadd-909e-41b1-b4e9-291643dd89c6%28Office.15%29.aspx) element is set to true, the folder should be hidden in the client view.</span></span> 
  
<span data-ttu-id="fb46c-193">Essa é também a resposta XML que a API gerenciada do EWS envia quando você obtém várias pastas usando o método [FindFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="fb46c-193">This is also the XML response that the EWS Managed API sends when you get multiple folders by using the [FindFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="fb46c-194">Os valores de alguns atributos e elementos foram reduzidos para legibilidade, e algumas pastas não foram incluídas por brevidade.</span><span class="sxs-lookup"><span data-stu-id="fb46c-194">The values of some attributes and elements have been shortened for readability, and some folders have not been included for brevity.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="815"
                         MinorBuildNumber="6"
                         Version="V2_7"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="update-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="fb46c-195">Atualizar uma pasta usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="fb46c-195">Update a folder by using the EWS Managed API</span></span>
<span data-ttu-id="fb46c-196"><a name="bk_updatefolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="fb46c-196"><a name="bk_updatefolderewsma"> </a></span></span>

<span data-ttu-id="fb46c-197">O exemplo de código a seguir mostra como atualizar o nome de exibição de uma pasta usando a API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="fb46c-197">The following code example shows how to update the display name of a folder by using the EWS Managed API.</span></span>
  
<span data-ttu-id="fb46c-198">Primeiro, crie um [PropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) para limitar o número de propriedades que o servidor retorna na resposta [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="fb46c-198">First, create a [PropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) to limit the number of properties that the server returns in the [Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) response.</span></span> <span data-ttu-id="fb46c-199">Recomendamos que você use o **IdOnly** **BasePropertySet** do IdOnly para reduzir as chamadas para o banco de dados do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb46c-199">We recommend that you use the **IdOnly** **BasePropertySet** to reduce calls to the Exchange database.</span></span> <span data-ttu-id="fb46c-200">Em seguida, use o método **BIND** para vincular à pasta a ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="fb46c-200">Next, use the **Bind** method to bind to the folder to update.</span></span> <span data-ttu-id="fb46c-201">Em seguida, atualize a propriedade [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) e use o método [Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) para salvar as alterações.</span><span class="sxs-lookup"><span data-stu-id="fb46c-201">Then, update the [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) property, and use the [Folder.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method to save the changes.</span></span> 
  
<span data-ttu-id="fb46c-202">Neste exemplo, presumimos que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb46c-202">In this example, we assume that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="fb46c-203">A variável local *FolderId* é a [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) da pasta a ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="fb46c-203">The local variable  *folderId*  is the [Id](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) of the folder to update.</span></span> 
  
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

## <a name="update-a-folder-by-using-ews"></a><span data-ttu-id="fb46c-204">Atualizar uma pasta usando o EWS</span><span class="sxs-lookup"><span data-stu-id="fb46c-204">Update a folder by using EWS</span></span>
<span data-ttu-id="fb46c-205"><a name="bk_updatefolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="fb46c-205"><a name="bk_updatefolderews"> </a></span></span>

<span data-ttu-id="fb46c-206">Os exemplos de XML a seguir mostram como atualizar o nome de exibição de uma pasta usando o EWS.</span><span class="sxs-lookup"><span data-stu-id="fb46c-206">The following XML examples show how to update the display name of a folder by using EWS.</span></span>
  
<span data-ttu-id="fb46c-207">Primeiro, envie uma mensagem de solicitação de operação [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) para obter a pasta a ser atualizada, conforme mostrado em [obter uma hierarquia de pastas usando o EWS](#bk_getfolderhierarchyews).</span><span class="sxs-lookup"><span data-stu-id="fb46c-207">First, send a [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request message to get the folder to update, as shown in [Get a folder hierarchy by using EWS](#bk_getfolderhierarchyews).</span></span>
  
<span data-ttu-id="fb46c-208">Em seguida, envie uma mensagem de solicitação de operação do [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) para o servidor para atualizar uma pasta.</span><span class="sxs-lookup"><span data-stu-id="fb46c-208">Next, send an [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) operation request message to the server to update a folder.</span></span> <span data-ttu-id="fb46c-209">A solicitação de operação **UpdateFolder** atualiza o [DisplayName](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) para "pasta personalizada atualizada".</span><span class="sxs-lookup"><span data-stu-id="fb46c-209">The **UpdateFolder** operation request updates the [DisplayName](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) to "Updated Custom Folder".</span></span> 
  
<span data-ttu-id="fb46c-210">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você atualiza uma pasta usando o método [Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="fb46c-210">This is also the XML request that the EWS Managed API sends when you update a folder by using the [Folder.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="fb46c-211">Os valores de alguns atributos e elementos foram reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="fb46c-211">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="fb46c-212">O servidor responde à solicitação **UpdateFolder** com uma mensagem [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) que inclui o valor de [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) de **NOERROR**e [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) da pasta que foi atualizada com um valor de atributo **ChangeKey** atualizado.</span><span class="sxs-lookup"><span data-stu-id="fb46c-212">The server responds to the **UpdateFolder** request with a [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes the a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, and the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the folder that was updated with an updated **ChangeKey** attribute value.</span></span> 
  
## <a name="delete-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="fb46c-213">Excluir uma pasta usando a API gerenciada do EWS</span><span class="sxs-lookup"><span data-stu-id="fb46c-213">Delete a folder by using the EWS Managed API</span></span>
<span data-ttu-id="fb46c-214"><a name="bk_deletefolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="fb46c-214"><a name="bk_deletefolderewsma"> </a></span></span>

<span data-ttu-id="fb46c-215">Este artigo fornece um exemplo básico que mostra como excluir uma pasta usando a API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="fb46c-215">This article provides a basic example that shows you how to delete a folder by using the EWS Managed API.</span></span> <span data-ttu-id="fb46c-216">Para obter mais detalhes sobre como excluir pastas, consulte [excluindo itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="fb46c-216">For more details about deleting folders, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="fb46c-217">Para excluir uma pasta usando a API gerenciada do EWS, primeiro use o método [Folder. bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) para vincular o objeto Service à pasta a ser excluída.</span><span class="sxs-lookup"><span data-stu-id="fb46c-217">To delete a folder by using the EWS Managed API, first, use the [Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method to bind to the service object to the folder to delete.</span></span> <span data-ttu-id="fb46c-218">Em seguida, use o método [Folder. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) para excluir a pasta usando o modo de exclusão [HardDelete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="fb46c-218">Next, use the [Folder.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) method to delete the folder by using the [HardDelete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx) deletion mode.</span></span> 
  
<span data-ttu-id="fb46c-219">Este exemplo pressupõe que o **serviço** é um objeto [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) válido e que o usuário foi autenticado em um servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb46c-219">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="fb46c-220">A variável local *FolderId* é a [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) da pasta a ser excluída.</span><span class="sxs-lookup"><span data-stu-id="fb46c-220">The local variable  *folderId*  is the [Id](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) of the folder to delete.</span></span> 
  
```cs
// Bind to an existing folder and get all its properties.
// This method call results in a GetFolder call to EWS.
Folder folder = Folder.Bind(service, folderId);
// HardDelete the folder.
// This method call results in a DeleteFolder call to EWS.
folder.Delete(DeleteMode.HardDelete);
```

## <a name="delete-a-folder-by-using-ews"></a><span data-ttu-id="fb46c-221">Excluir uma pasta usando o EWS</span><span class="sxs-lookup"><span data-stu-id="fb46c-221">Delete a folder by using EWS</span></span>
<span data-ttu-id="fb46c-222"><a name="bk_deletefolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="fb46c-222"><a name="bk_deletefolderews"> </a></span></span>

<span data-ttu-id="fb46c-223">Este artigo fornece um exemplo de XML básico que mostra como excluir uma pasta usando o EWS.</span><span class="sxs-lookup"><span data-stu-id="fb46c-223">This article provides a basic XML example that shows you how to delete a folder by using EWS.</span></span> <span data-ttu-id="fb46c-224">Para obter mais detalhes sobre como excluir pastas, consulte [excluindo itens usando o EWS no Exchange](deleting-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="fb46c-224">For more details about deleting folders, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="fb46c-225">Para excluir uma pasta usando o EWS, primeiro, envie uma mensagem de solicitação de operação [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) para obter a pasta a ser atualizada, conforme mostrado em [obter uma pasta usando o EWS](#bk_getfolderews).</span><span class="sxs-lookup"><span data-stu-id="fb46c-225">To delete a folder by using EWS, first, send a [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request message to get the folder to update as shown in [Get a folder by using EWS](#bk_getfolderews).</span></span> 
  
<span data-ttu-id="fb46c-226">Em seguida, envie uma mensagem de solicitação de operação do [DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) para o servidor para excluir a pasta.</span><span class="sxs-lookup"><span data-stu-id="fb46c-226">Next, send a [DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) operation request message to the server to delete the folder.</span></span> <span data-ttu-id="fb46c-227">A solicitação de operação **DeleteFolder** indica que o **DeleteType** é **HardDelete** e inclui o [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) da pasta a ser excluída.</span><span class="sxs-lookup"><span data-stu-id="fb46c-227">The **DeleteFolder** operation request indicates that the **DeleteType** is **HardDelete** and it includes the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the folder to delete.</span></span> 
  
<span data-ttu-id="fb46c-228">Essa é também a solicitação XML que a API gerenciada do EWS envia quando você exclui uma pasta usando o método [Folder. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="fb46c-228">This is also the XML request that the EWS Managed API sends when you delete a folder by using the [Folder.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="fb46c-229">Os valores de alguns atributos e elementos foram reduzidos para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="fb46c-229">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="fb46c-230">O servidor responde à solicitação **DeleteFolder** com uma mensagem [DeleteFolderResponse](https://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) que inclui o valor de [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) de **NOERROR**, que indica que a exclusão da pasta foi bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="fb46c-230">The server responds to the **DeleteFolder** request with a [DeleteFolderResponse](https://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) message that includes the a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the folder deletion was successful.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="fb46c-231">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="fb46c-231">Next steps</span></span>
<span data-ttu-id="fb46c-232"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="fb46c-232"><a name="bk_nextsteps"> </a></span></span>

<span data-ttu-id="fb46c-233">Após recuperar as pastas no servidor ou fazer alterações em pastas, talvez você queira [sincronizar sua hierarquia de pastas](how-to-synchronize-folders-by-using-ews-in-exchange.md) ou [assinar notificações sobre alterações de pasta](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) no servidor.</span><span class="sxs-lookup"><span data-stu-id="fb46c-233">After you have retrieved the folders on the server, or made changes to folders, you might want to [synchronize your folder hierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md) or [subscribe to notifications about folder changes](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) on the server.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="fb46c-234">Confira também</span><span class="sxs-lookup"><span data-stu-id="fb46c-234">See also</span></span>

- [<span data-ttu-id="fb46c-235">Pastas e itens no EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fb46c-235">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)   
- [<span data-ttu-id="fb46c-236">Trabalhar com itens de caixa de correio do Exchange usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fb46c-236">Work with Exchange mailbox items by using EWS in Exchange</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="fb46c-237">Excluir itens usando o EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fb46c-237">Deleting items by using EWS in Exchange</span></span>](deleting-items-by-using-ews-in-exchange.md)   
- [<span data-ttu-id="fb46c-238">Develop web service clients for Exchange</span><span class="sxs-lookup"><span data-stu-id="fb46c-238">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

