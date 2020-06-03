---
title: Operação CreateManagedFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateManagedFolder
api_type:
- schema
ms.assetid: 60a668a2-b4e9-4db9-ac76-9b181e47b302
description: A operação CreateManagedFolder cria uma pasta gerenciada no repositório do Exchange.
ms.openlocfilehash: 779c730b55b9b441644108a6837f9e22d39cc2f4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44444590"
---
# <a name="createmanagedfolder-operation"></a><span data-ttu-id="53846-103">Operação CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="53846-103">CreateManagedFolder operation</span></span>

<span data-ttu-id="53846-104">A operação CreateManagedFolder cria uma pasta gerenciada no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="53846-104">The CreateManagedFolder operation creates a managed folder in the Exchange store.</span></span>
  
## <a name="using-the-createmanagedfolder-operation"></a><span data-ttu-id="53846-105">Usando a operação CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="53846-105">Using the CreateManagedFolder Operation</span></span>

<span data-ttu-id="53846-106">A operação CreateManagedFolder adiciona uma pasta personalizada gerenciada à caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="53846-106">The CreateManagedFolder operation adds a managed custom folder to a user's mailbox.</span></span> <span data-ttu-id="53846-107">Você pode usar o cmdlet **Get-ManagedFolder** do Shell de gerenciamento do Exchange para localizar pastas gerenciadas disponíveis para adicionar.</span><span class="sxs-lookup"><span data-stu-id="53846-107">You can use the Exchange Management Shell **Get-ManagedFolder** cmdlet to find available managed folders to add.</span></span> <span data-ttu-id="53846-108">Embora este cmdlet retorne pastas personalizadas gerenciadas e pastas padrão gerenciadas, somente pastas personalizadas gerenciadas podem ser adicionadas.</span><span class="sxs-lookup"><span data-stu-id="53846-108">Although this cmdlet returns both managed custom folders and managed default folders, only managed custom folders can be added.</span></span> <span data-ttu-id="53846-109">Pastas personalizadas gerenciadas são identificadas pelo tipo de pasta ManagedCustomFolder.</span><span class="sxs-lookup"><span data-stu-id="53846-109">Managed custom folders are identified by the ManagedCustomFolder folder type.</span></span> <span data-ttu-id="53846-110">O namespace System. DirectoryServices também inclui tipos que podem ser usados para descobrir os nomes das pastas gerenciadas disponíveis.</span><span class="sxs-lookup"><span data-stu-id="53846-110">The System.DirectoryServices namespace also includes types that can be used to discover the names of available managed folders.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="53846-111">Você não pode usar os serviços Web do Exchange para localizar os nomes das pastas gerenciadas disponíveis para adicionar a uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="53846-111">You cannot use Exchange Web Services to find the names of available managed folders to add to a mailbox.</span></span> 
  
<span data-ttu-id="53846-112">Você pode usar as operações FindFolder e GetFolder para acessar pastas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="53846-112">You can use the FindFolder and GetFolder operations to access managed folders.</span></span> <span data-ttu-id="53846-113">FindFolder é usado para pesquisar pastas em uma pasta pai especificada.</span><span class="sxs-lookup"><span data-stu-id="53846-113">FindFolder is used to search for folders in a specified parent folder.</span></span> <span data-ttu-id="53846-114">Isso pode ser usado para que pastas gerenciadas possam ser descobertas em uma pasta antes de tentar adicionar uma pasta personalizada gerenciada duplicada no mesmo diretório.</span><span class="sxs-lookup"><span data-stu-id="53846-114">This can be used so that managed folders can be discovered in a folder before trying to add a duplicate managed custom folder to the same directory.</span></span> <span data-ttu-id="53846-115">GetFolder é usado após a operação FindFolder para obter mais informações sobre uma pasta personalizada gerenciada.</span><span class="sxs-lookup"><span data-stu-id="53846-115">GetFolder is used after the FindFolder operation to get more information about a managed custom folder.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="53846-116">Comentários</span><span class="sxs-lookup"><span data-stu-id="53846-116">Remarks</span></span>

<span data-ttu-id="53846-117">Para obter informações sobre como configurar a política de gerenciamento de registros de mensagens (MRM), consulte [como criar uma política de caixa de correio de pasta gerenciada](https://go.microsoft.com/fwlink/?LinkId=100975).</span><span class="sxs-lookup"><span data-stu-id="53846-117">For information about how to set up messaging records management (MRM) policy, see [How to Create a Managed Folder Mailbox Policy](https://go.microsoft.com/fwlink/?LinkId=100975).</span></span>
  
<span data-ttu-id="53846-118">Para obter informações sobre como remover pastas personalizadas gerenciadas de uma caixa de correio, consulte [Remove-ManagedFolder](https://go.microsoft.com/fwlink/?LinkId=100976).</span><span class="sxs-lookup"><span data-stu-id="53846-118">For information about how to remove managed custom folders from a mailbox, see [Remove-ManagedFolder](https://go.microsoft.com/fwlink/?LinkId=100976).</span></span>
  
## <a name="createmanagedfolder-request-example"></a><span data-ttu-id="53846-119">Exemplo de solicitação CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="53846-119">CreateManagedFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="53846-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="53846-120">Description</span></span>

<span data-ttu-id="53846-121">O exemplo a seguir de uma solicitação CreateManagedFolder mostra como adicionar uma pasta gerenciada chamada testar pasta gerenciada a uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="53846-121">The following example of a CreateManagedFolder request shows how to add a managed folder named Test Managed Folder to a mailbox.</span></span>
  
> [!NOTE]
> <span data-ttu-id="53846-122">Você também pode usar o acesso de representante para adicionar pastas personalizadas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="53846-122">You can also use delegate access to add managed custom folders.</span></span> 
  
### <a name="code"></a><span data-ttu-id="53846-123">Código</span><span class="sxs-lookup"><span data-stu-id="53846-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateManagedFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderNames>
        <t:FolderName>Test Managed Folder</t:FolderName>
      </FolderNames>
    </CreateManagedFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="53846-124">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="53846-124">Request elements</span></span>

<span data-ttu-id="53846-125">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="53846-125">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="53846-126">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="53846-126">CreateManagedFolder</span></span>](createmanagedfolder.md)
    
- [<span data-ttu-id="53846-127">FolderNames</span><span class="sxs-lookup"><span data-stu-id="53846-127">FolderNames</span></span>](foldernames.md)
    
- [<span data-ttu-id="53846-128">FolderName</span><span class="sxs-lookup"><span data-stu-id="53846-128">FolderName</span></span>](foldername.md)
    
<span data-ttu-id="53846-129">Para encontrar outras opções para a mensagem de solicitação da operação CreateManagedFolder, explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="53846-129">To find other options for the request message of the CreateManagedFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="53846-130">Inicie no elemento [CreateManagedFolder](createmanagedfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="53846-130">Start at the [CreateManagedFolder](createmanagedfolder.md) element.</span></span> 
  
## <a name="successful-createmanagedfolder-response"></a><span data-ttu-id="53846-131">Resposta CreateManagedFolder bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="53846-131">Successful CreateManagedFolder Response</span></span>

### <a name="description"></a><span data-ttu-id="53846-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="53846-132">Description</span></span>

<span data-ttu-id="53846-133">O exemplo de código a seguir mostra uma resposta bem-sucedida a uma solicitação CreateManagedFolder.</span><span class="sxs-lookup"><span data-stu-id="53846-133">The following code example shows a successful response to a CreateManagedFolder request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="53846-134">Os valores de atributo **ID** e **ChangeKey** foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="53846-134">The **Id** and **ChangeKey** attribute values have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="53846-135">Código</span><span class="sxs-lookup"><span data-stu-id="53846-135">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateManagedFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS0AdX=" ChangeKey="AACADA=="/>
            </t:Folder>
          </m:Folders>
        </m:CreateManagedFolderResponseMessage>
      </m:ResponseMessages>
    </CreateManagedFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="53846-136">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="53846-136">Successful response elements</span></span>

<span data-ttu-id="53846-137">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="53846-137">The following elements are used in the response:</span></span> 
  
- [<span data-ttu-id="53846-138">CreateManagedFolderResponse</span><span class="sxs-lookup"><span data-stu-id="53846-138">CreateManagedFolderResponse</span></span>](createmanagedfolderresponse.md)
    
- [<span data-ttu-id="53846-139">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="53846-139">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="53846-140">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="53846-140">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md)
    
- [<span data-ttu-id="53846-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="53846-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="53846-142">Pastas</span><span class="sxs-lookup"><span data-stu-id="53846-142">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="53846-143">Folder</span><span class="sxs-lookup"><span data-stu-id="53846-143">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="53846-144">FolderId</span><span class="sxs-lookup"><span data-stu-id="53846-144">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="53846-145">Para encontrar outras opções para as mensagens de resposta da operação CreateManagedFolder, explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="53846-145">To find other options for the response messages of the CreateManagedFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="53846-146">Inicie no elemento [CreateManagedFolderResponse](createmanagedfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="53846-146">Start at the [CreateManagedFolderResponse](createmanagedfolderresponse.md) element.</span></span> 
  
## <a name="createmanagedfolder-error-response"></a><span data-ttu-id="53846-147">Resposta de erro CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="53846-147">CreateManagedFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="53846-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="53846-148">Description</span></span>

<span data-ttu-id="53846-149">O exemplo de código a seguir mostra uma resposta de erro a uma solicitação CreateManagedFolder.</span><span class="sxs-lookup"><span data-stu-id="53846-149">The following code example shows an error response to a CreateManagedFolder request.</span></span>
  
### <a name="code"></a><span data-ttu-id="53846-150">Código</span><span class="sxs-lookup"><span data-stu-id="53846-150">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateManagedFolderResponseMessage ResponseClass="Error">
          <m:MessageText>A specified managed folder already exists in the mailbox.</m:MessageText>
          <m:ResponseCode>ErrorManagedFolderAlreadyExists</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders/>
        </m:CreateManagedFolderResponseMessage>
      </m:ResponseMessages>
    </CreateManagedFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="53846-151">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="53846-151">Error response elements</span></span>

<span data-ttu-id="53846-152">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="53846-152">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="53846-153">CreateManagedFolderResponse</span><span class="sxs-lookup"><span data-stu-id="53846-153">CreateManagedFolderResponse</span></span>](createmanagedfolderresponse.md)
    
- [<span data-ttu-id="53846-154">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="53846-154">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="53846-155">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="53846-155">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md)
    
- [<span data-ttu-id="53846-156">MessageText</span><span class="sxs-lookup"><span data-stu-id="53846-156">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="53846-157">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="53846-157">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="53846-158">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="53846-158">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="53846-159">Pastas</span><span class="sxs-lookup"><span data-stu-id="53846-159">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="53846-160">Confira também</span><span class="sxs-lookup"><span data-stu-id="53846-160">See also</span></span>



[<span data-ttu-id="53846-161">Operação GetFolder</span><span class="sxs-lookup"><span data-stu-id="53846-161">GetFolder operation</span></span>](getfolder-operation.md)
  
[<span data-ttu-id="53846-162">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="53846-162">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="53846-163">Localizando pastas</span><span class="sxs-lookup"><span data-stu-id="53846-163">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="53846-164">Adicionando pastas gerenciadas</span><span class="sxs-lookup"><span data-stu-id="53846-164">Adding Managed Folders</span></span>](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

