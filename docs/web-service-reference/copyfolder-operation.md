---
title: Operação CopyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolder
api_type:
- schema
ms.assetid: c7ea0d68-9793-4144-b378-d99536776db9
description: A operação CopyFolder copia pastas em uma caixa de correio.
ms.openlocfilehash: a83444ff0927a3c8fe075c79d44d02357a737773
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751545"
---
# <a name="copyfolder-operation"></a><span data-ttu-id="c5d63-103">Operação CopyFolder</span><span class="sxs-lookup"><span data-stu-id="c5d63-103">CopyFolder operation</span></span>

<span data-ttu-id="c5d63-104">A operação CopyFolder copia pastas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c5d63-104">The CopyFolder operation copies folders in a mailbox.</span></span>
  
## <a name="using-the-copyfolder-operation"></a><span data-ttu-id="c5d63-105">Usando a operação CopyFolder</span><span class="sxs-lookup"><span data-stu-id="c5d63-105">Using the CopyFolder operation</span></span>

<span data-ttu-id="c5d63-106">A operação CopyFolder é semelhante à [operação MoveFolder](movefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="c5d63-106">The CopyFolder operation is similar to the [MoveFolder operation](movefolder-operation.md).</span></span> <span data-ttu-id="c5d63-107">Ele copia pastas identificadas e retorna a **Id** e a **ChangeKey** das pastas copiadas.</span><span class="sxs-lookup"><span data-stu-id="c5d63-107">It copies identified folders and returns the **Id** and **ChangeKey** of the copied folders.</span></span> 
  
## <a name="copyfolder-request-example"></a><span data-ttu-id="c5d63-108">Exemplo de solicitação CopyFolder</span><span class="sxs-lookup"><span data-stu-id="c5d63-108">CopyFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="c5d63-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5d63-109">Description</span></span>

<span data-ttu-id="c5d63-110">O exemplo a seguir de uma solicitação de CopyFolder mostra como copie as pastas na pasta caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="c5d63-110">The following example of a CopyFolder request shows how to copy folders into the Inbox folder.</span></span>
  
> [!NOTE]
> <span data-ttu-id="c5d63-111">O valor do atributo **Id** do elemento [FolderId](folderid.md) foi reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c5d63-111">The value of the **Id** attribute of the [FolderId](folderid.md) element has been shortened for readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c5d63-112">Código</span><span class="sxs-lookup"><span data-stu-id="c5d63-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CopyFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </ToFolderId>
      <FolderIds>
        <t:FolderId Id="AS4A=" ChangeKey="fsVU4=="/>
        <t:FolderId Id="AS4AU=" ChangeKey="fsVU4o=="/>
      </FolderIds>
    </CopyFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="c5d63-113">Comments</span><span class="sxs-lookup"><span data-stu-id="c5d63-113">Comments</span></span>

<span data-ttu-id="c5d63-114">Pastas podem ser identificadas por elemento [DistinguishedFolderId](distinguishedfolderid.md) ou o elemento [FolderId](folderid.md) para uso em tanto o [ToFolderId](tofolderid.md) ou os elementos de [FolderIds](folderids.md) .</span><span class="sxs-lookup"><span data-stu-id="c5d63-114">Folders can be identified by either the [DistinguishedFolderId](distinguishedfolderid.md) element or the [FolderId](folderid.md) element for use in either the [ToFolderId](tofolderid.md) or the [FolderIds](folderids.md) elements.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="c5d63-115">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c5d63-115">Request elements</span></span>

<span data-ttu-id="c5d63-116">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="c5d63-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="c5d63-117">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="c5d63-117">CopyFolder</span></span>](copyfolder.md)
    
- [<span data-ttu-id="c5d63-118">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="c5d63-118">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="c5d63-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="c5d63-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="c5d63-120">FolderIds</span><span class="sxs-lookup"><span data-stu-id="c5d63-120">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="c5d63-121">FolderId</span><span class="sxs-lookup"><span data-stu-id="c5d63-121">FolderId</span></span>](folderid.md)
    
> [!NOTE]
> <span data-ttu-id="c5d63-122">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="c5d63-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="c5d63-123">Para localizar outras opções para a mensagem de solicitação da operação CopyFolder, explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="c5d63-123">To find other options for the request message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="c5d63-124">Inicie o elemento [CopyFolder](copyfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="c5d63-124">Start at the [CopyFolder](copyfolder.md) element.</span></span> 
  
## <a name="successful-copyfolder-response"></a><span data-ttu-id="c5d63-125">Resposta de CopyFolder bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="c5d63-125">Successful CopyFolder response</span></span>

### <a name="description"></a><span data-ttu-id="c5d63-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5d63-126">Description</span></span>

<span data-ttu-id="c5d63-127">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação CopyFolder.</span><span class="sxs-lookup"><span data-stu-id="c5d63-127">The following example shows a successful response to the CopyFolder request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="c5d63-128">A ID de pasta e a chave de alteração tem sido reduzidas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c5d63-128">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c5d63-129">Código</span><span class="sxs-lookup"><span data-stu-id="c5d63-129">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS4AUn=" ChangeKey="fsVU4o==" />
            </t:Folder>
          </m:Folders>
        </m:CopyFolderResponseMessage>
      </m:ResponseMessages>
    </CopyFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="c5d63-130">Comment</span><span class="sxs-lookup"><span data-stu-id="c5d63-130">Comment</span></span>

<span data-ttu-id="c5d63-131">O elemento [FolderId](folderid.md) retornado na resposta representa a pasta que foi copiada no novo local de pasta.</span><span class="sxs-lookup"><span data-stu-id="c5d63-131">The [FolderId](folderid.md) element that is returned in the response represents the folder that was copied in the new folder location.</span></span> 
  
### <a name="response-elements"></a><span data-ttu-id="c5d63-132">Elementos de resposta</span><span class="sxs-lookup"><span data-stu-id="c5d63-132">Response elements</span></span>

<span data-ttu-id="c5d63-133">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="c5d63-133">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="c5d63-134">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c5d63-134">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="c5d63-135">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="c5d63-135">CopyFolderResponse</span></span>](copyfolderresponse.md)
    
- [<span data-ttu-id="c5d63-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c5d63-136">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c5d63-137">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c5d63-137">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md)
    
- [<span data-ttu-id="c5d63-138">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c5d63-138">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c5d63-139">Pastas</span><span class="sxs-lookup"><span data-stu-id="c5d63-139">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="c5d63-140">Folder</span><span class="sxs-lookup"><span data-stu-id="c5d63-140">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="c5d63-141">FolderId</span><span class="sxs-lookup"><span data-stu-id="c5d63-141">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="c5d63-142">Para localizar outras opções para a mensagem de resposta da operação CopyFolder, explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="c5d63-142">To find other options for the response message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="c5d63-143">Inicie o elemento [CopyFolderResponse](copyfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="c5d63-143">Start at the [CopyFolderResponse](copyfolderresponse.md) element.</span></span> 
  
## <a name="copyfolder-error-response"></a><span data-ttu-id="c5d63-144">Resposta de erro CopyFolder</span><span class="sxs-lookup"><span data-stu-id="c5d63-144">CopyFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="c5d63-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="c5d63-145">Description</span></span>

<span data-ttu-id="c5d63-146">O exemplo a seguir mostra uma resposta de erro a uma solicitação de CopyFolder.</span><span class="sxs-lookup"><span data-stu-id="c5d63-146">The following example shows an error response to a CopyFolder request.</span></span> <span data-ttu-id="c5d63-147">O erro ocorreu porque já existe uma pasta com o mesmo nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="c5d63-147">The error occurred because a folder with the same display name already exists.</span></span>
  
### <a name="code"></a><span data-ttu-id="c5d63-148">Código</span><span class="sxs-lookup"><span data-stu-id="c5d63-148">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The move or copy operation failed.</m:MessageText>
          <m:ResponseCode>ErrorMoveCopyFailed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:CopyFolderResponseMessage>
      </m:ResponseMessages>
    </CopyFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="c5d63-149">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="c5d63-149">Error response elements</span></span>

<span data-ttu-id="c5d63-150">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="c5d63-150">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="c5d63-151">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="c5d63-151">CopyFolderResponse</span></span>](copyfolderresponse.md)
    
- [<span data-ttu-id="c5d63-152">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c5d63-152">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c5d63-153">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c5d63-153">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md)
    
- [<span data-ttu-id="c5d63-154">MessageText</span><span class="sxs-lookup"><span data-stu-id="c5d63-154">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="c5d63-155">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c5d63-155">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c5d63-156">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c5d63-156">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="c5d63-157">Pastas</span><span class="sxs-lookup"><span data-stu-id="c5d63-157">Folders</span></span>](folders-ex15websvcsotherref.md)
    
<span data-ttu-id="c5d63-158">Para localizar outras opções para a mensagem de resposta de erro da operação CopyFolder, explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="c5d63-158">To find other options for the error response message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="c5d63-159">Inicie o elemento [CopyFolderResponse](copyfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="c5d63-159">Start at the [CopyFolderResponse](copyfolderresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="c5d63-160">Confira também</span><span class="sxs-lookup"><span data-stu-id="c5d63-160">See also</span></span>

- [<span data-ttu-id="c5d63-161">Operação MoveFolder</span><span class="sxs-lookup"><span data-stu-id="c5d63-161">MoveFolder operation</span></span>](movefolder-operation.md)
- [<span data-ttu-id="c5d63-162">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c5d63-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

