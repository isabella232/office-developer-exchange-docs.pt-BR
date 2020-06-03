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
ms.openlocfilehash: 1f9a7a3f3ede2d3cf8f9d41677d8ce0487266f17
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468891"
---
# <a name="copyfolder-operation"></a><span data-ttu-id="d7792-103">Operação CopyFolder</span><span class="sxs-lookup"><span data-stu-id="d7792-103">CopyFolder operation</span></span>

<span data-ttu-id="d7792-104">A operação CopyFolder copia pastas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d7792-104">The CopyFolder operation copies folders in a mailbox.</span></span>
  
## <a name="using-the-copyfolder-operation"></a><span data-ttu-id="d7792-105">Usando a operação CopyFolder</span><span class="sxs-lookup"><span data-stu-id="d7792-105">Using the CopyFolder operation</span></span>

<span data-ttu-id="d7792-106">A operação CopyFolder é semelhante à [operação MoveFolder](movefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="d7792-106">The CopyFolder operation is similar to the [MoveFolder operation](movefolder-operation.md).</span></span> <span data-ttu-id="d7792-107">Ele copia pastas identificadas e retorna a **ID** e **ChangeKey** das pastas copiadas.</span><span class="sxs-lookup"><span data-stu-id="d7792-107">It copies identified folders and returns the **Id** and **ChangeKey** of the copied folders.</span></span> 
  
## <a name="copyfolder-request-example"></a><span data-ttu-id="d7792-108">Exemplo de solicitação CopyFolder</span><span class="sxs-lookup"><span data-stu-id="d7792-108">CopyFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="d7792-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7792-109">Description</span></span>

<span data-ttu-id="d7792-110">O exemplo a seguir de uma solicitação CopyFolder mostra como copiar pastas para a pasta caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="d7792-110">The following example of a CopyFolder request shows how to copy folders into the Inbox folder.</span></span>
  
> [!NOTE]
> <span data-ttu-id="d7792-111">O valor do atributo **ID** do elemento [FolderId](folderid.md) foi reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d7792-111">The value of the **Id** attribute of the [FolderId](folderid.md) element has been shortened for readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d7792-112">Código</span><span class="sxs-lookup"><span data-stu-id="d7792-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CopyFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="d7792-113">Comentários</span><span class="sxs-lookup"><span data-stu-id="d7792-113">Comments</span></span>

<span data-ttu-id="d7792-114">As pastas podem ser identificadas pelo elemento [DistinguishedFolderId](distinguishedfolderid.md) ou o elemento [FolderId](folderid.md) para uso nos elementos [ToFolderId](tofolderid.md) ou [FolderIds](folderids.md) .</span><span class="sxs-lookup"><span data-stu-id="d7792-114">Folders can be identified by either the [DistinguishedFolderId](distinguishedfolderid.md) element or the [FolderId](folderid.md) element for use in either the [ToFolderId](tofolderid.md) or the [FolderIds](folderids.md) elements.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="d7792-115">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="d7792-115">Request elements</span></span>

<span data-ttu-id="d7792-116">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="d7792-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="d7792-117">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="d7792-117">CopyFolder</span></span>](copyfolder.md)
    
- [<span data-ttu-id="d7792-118">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="d7792-118">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="d7792-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="d7792-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="d7792-120">FolderIds</span><span class="sxs-lookup"><span data-stu-id="d7792-120">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="d7792-121">FolderId</span><span class="sxs-lookup"><span data-stu-id="d7792-121">FolderId</span></span>](folderid.md)
    
> [!NOTE]
> <span data-ttu-id="d7792-122">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="d7792-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="d7792-123">Para encontrar outras opções para a mensagem de solicitação da operação CopyFolder, explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="d7792-123">To find other options for the request message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="d7792-124">Inicie no elemento [CopyFolder](copyfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="d7792-124">Start at the [CopyFolder](copyfolder.md) element.</span></span> 
  
## <a name="successful-copyfolder-response"></a><span data-ttu-id="d7792-125">Resposta CopyFolder bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="d7792-125">Successful CopyFolder response</span></span>

### <a name="description"></a><span data-ttu-id="d7792-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7792-126">Description</span></span>

<span data-ttu-id="d7792-127">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação CopyFolder.</span><span class="sxs-lookup"><span data-stu-id="d7792-127">The following example shows a successful response to the CopyFolder request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="d7792-128">A ID da pasta e a chave de alteração foram reduzidas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d7792-128">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d7792-129">Código</span><span class="sxs-lookup"><span data-stu-id="d7792-129">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comment"></a><span data-ttu-id="d7792-130">Comentário</span><span class="sxs-lookup"><span data-stu-id="d7792-130">Comment</span></span>

<span data-ttu-id="d7792-131">O elemento [FolderId](folderid.md) retornado na resposta representa a pasta que foi copiada no novo local da pasta.</span><span class="sxs-lookup"><span data-stu-id="d7792-131">The [FolderId](folderid.md) element that is returned in the response represents the folder that was copied in the new folder location.</span></span> 
  
### <a name="response-elements"></a><span data-ttu-id="d7792-132">Elementos de resposta</span><span class="sxs-lookup"><span data-stu-id="d7792-132">Response elements</span></span>

<span data-ttu-id="d7792-133">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="d7792-133">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="d7792-134">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d7792-134">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="d7792-135">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="d7792-135">CopyFolderResponse</span></span>](copyfolderresponse.md)
    
- [<span data-ttu-id="d7792-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d7792-136">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="d7792-137">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d7792-137">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md)
    
- [<span data-ttu-id="d7792-138">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d7792-138">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d7792-139">Pastas</span><span class="sxs-lookup"><span data-stu-id="d7792-139">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="d7792-140">Folder</span><span class="sxs-lookup"><span data-stu-id="d7792-140">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="d7792-141">FolderId</span><span class="sxs-lookup"><span data-stu-id="d7792-141">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="d7792-142">Para encontrar outras opções para a mensagem de resposta da operação CopyFolder, explore a hierarquia do esquema.</span><span class="sxs-lookup"><span data-stu-id="d7792-142">To find other options for the response message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="d7792-143">Inicie no elemento [CopyFolderResponse](copyfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="d7792-143">Start at the [CopyFolderResponse](copyfolderresponse.md) element.</span></span> 
  
## <a name="copyfolder-error-response"></a><span data-ttu-id="d7792-144">Resposta de erro CopyFolder</span><span class="sxs-lookup"><span data-stu-id="d7792-144">CopyFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="d7792-145">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7792-145">Description</span></span>

<span data-ttu-id="d7792-146">O exemplo a seguir mostra uma resposta de erro a uma solicitação CopyFolder.</span><span class="sxs-lookup"><span data-stu-id="d7792-146">The following example shows an error response to a CopyFolder request.</span></span> <span data-ttu-id="d7792-147">O erro ocorreu porque já existe uma pasta com o mesmo nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="d7792-147">The error occurred because a folder with the same display name already exists.</span></span>
  
### <a name="code"></a><span data-ttu-id="d7792-148">Código</span><span class="sxs-lookup"><span data-stu-id="d7792-148">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="d7792-149">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="d7792-149">Error response elements</span></span>

<span data-ttu-id="d7792-150">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="d7792-150">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="d7792-151">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="d7792-151">CopyFolderResponse</span></span>](copyfolderresponse.md)
    
- [<span data-ttu-id="d7792-152">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d7792-152">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="d7792-153">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d7792-153">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md)
    
- [<span data-ttu-id="d7792-154">MessageText</span><span class="sxs-lookup"><span data-stu-id="d7792-154">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="d7792-155">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d7792-155">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d7792-156">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d7792-156">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="d7792-157">Pastas</span><span class="sxs-lookup"><span data-stu-id="d7792-157">Folders</span></span>](folders-ex15websvcsotherref.md)
    
<span data-ttu-id="d7792-158">Para encontrar outras opções para a mensagem de resposta de erro da operação CopyFolder, explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="d7792-158">To find other options for the error response message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="d7792-159">Inicie no elemento [CopyFolderResponse](copyfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="d7792-159">Start at the [CopyFolderResponse](copyfolderresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="d7792-160">Confira também</span><span class="sxs-lookup"><span data-stu-id="d7792-160">See also</span></span>

- [<span data-ttu-id="d7792-161">Operação MoveFolder</span><span class="sxs-lookup"><span data-stu-id="d7792-161">MoveFolder operation</span></span>](movefolder-operation.md)
- [<span data-ttu-id="d7792-162">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d7792-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

