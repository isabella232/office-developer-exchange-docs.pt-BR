---
title: Operação MoveFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveFolder
api_type:
- schema
ms.assetid: c7233966-6c87-4a14-8156-b1610760176d
description: A operação MoveFolder move as pastas de uma pasta especificada e as coloca em outra pasta.
ms.openlocfilehash: dc572130ca3b2f2b152abbb4a8b68cc6f67790e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460579"
---
# <a name="movefolder-operation"></a><span data-ttu-id="bf91f-103">Operação MoveFolder</span><span class="sxs-lookup"><span data-stu-id="bf91f-103">MoveFolder operation</span></span>

<span data-ttu-id="bf91f-104">A operação MoveFolder move as pastas de uma pasta especificada e as coloca em outra pasta.</span><span class="sxs-lookup"><span data-stu-id="bf91f-104">The MoveFolder operation moves folders from a specified folder and puts them in another folder.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bf91f-105">Comentários</span><span class="sxs-lookup"><span data-stu-id="bf91f-105">Remarks</span></span>

<span data-ttu-id="bf91f-106">A operação MoveFolder é semelhante à operação CopyFolder.</span><span class="sxs-lookup"><span data-stu-id="bf91f-106">The MoveFolder operation is similar to the CopyFolder operation.</span></span> <span data-ttu-id="bf91f-107">Não é possível mover pastas diferenciadas.</span><span class="sxs-lookup"><span data-stu-id="bf91f-107">You cannot move distinguished folders.</span></span> <span data-ttu-id="bf91f-108">Você pode mover várias pastas de uma só vez para a pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="bf91f-108">You can move multiple folders at one time to the destination folder.</span></span>
  
## <a name="movefolder-request-example"></a><span data-ttu-id="bf91f-109">Exemplo de solicitação MoveFolder</span><span class="sxs-lookup"><span data-stu-id="bf91f-109">MoveFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="bf91f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf91f-110">Description</span></span>

<span data-ttu-id="bf91f-111">O exemplo a seguir de uma solicitação MoveFolder mostra como formar uma solicitação para mover uma pasta identificada por [FolderId](folderid.md) e colocar a pasta na pasta diferenciada de lixo eletrônico.</span><span class="sxs-lookup"><span data-stu-id="bf91f-111">The following example of a MoveFolder request shows how to form a request to move a folder identified by the [FolderId](folderid.md) and put the folder in the Junk E-mail distinguished folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="bf91f-112">Código</span><span class="sxs-lookup"><span data-stu-id="bf91f-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <MoveFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="junkemail"/>
      </ToFolderId>
      <FolderIds>
        <t:FolderId Id="AScAc"/>
      </FolderIds>
    </MoveFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="bf91f-113">Comentários</span><span class="sxs-lookup"><span data-stu-id="bf91f-113">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="bf91f-114">O valor do atributo ID do elemento [FolderId](folderid.md) foi reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bf91f-114">The value of the ID attribute of the [FolderId](folderid.md) element has been shortened for readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="bf91f-115">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="bf91f-115">Request elements</span></span>

<span data-ttu-id="bf91f-116">Essa solicitação de MoveFolder inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="bf91f-116">This MoveFolder request includes the following elements:</span></span>
  
- [<span data-ttu-id="bf91f-117">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="bf91f-117">MoveFolder</span></span>](movefolder.md)
    
- [<span data-ttu-id="bf91f-118">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="bf91f-118">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="bf91f-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="bf91f-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="bf91f-120">FolderIds</span><span class="sxs-lookup"><span data-stu-id="bf91f-120">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="bf91f-121">FolderId</span><span class="sxs-lookup"><span data-stu-id="bf91f-121">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="bf91f-122">Confira o esquema para elementos adicionais que você pode usar para formar uma solicitação de MoveFolder.</span><span class="sxs-lookup"><span data-stu-id="bf91f-122">See the schema for additional elements that you can use to form a MoveFolder request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="bf91f-123">O local padrão do esquema está no diretório virtual EWS no computador em que a função de servidor de acesso para cliente está instalada.</span><span class="sxs-lookup"><span data-stu-id="bf91f-123">The default location of the schema is in the EWS virtual directory on the computer that has the Client Access server role installed.</span></span> 
  
## <a name="successful-movefolder-response-example"></a><span data-ttu-id="bf91f-124">Exemplo de resposta MoveFolder bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="bf91f-124">Successful MoveFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="bf91f-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf91f-125">Description</span></span>

<span data-ttu-id="bf91f-126">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação MoveFolder.</span><span class="sxs-lookup"><span data-stu-id="bf91f-126">The following example shows a successful response to the MoveFolder request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="bf91f-127">Código</span><span class="sxs-lookup"><span data-stu-id="bf91f-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <MoveFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:MoveFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AAAlAFV" ChangeKey="AQAAAB" />
            </t:Folder>
          </m:Folders>
        </m:MoveFolderResponseMessage>
      </m:ResponseMessages>
    </MoveFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="bf91f-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="bf91f-128">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="bf91f-129">A ID da pasta e a chave de alteração foram reduzidas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bf91f-129">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="bf91f-130">O FolderId retornado na resposta representa a pasta que foi movida para o novo local da pasta.</span><span class="sxs-lookup"><span data-stu-id="bf91f-130">The FolderId that is returned in the response represents the folder that was moved to the new the folder location.</span></span>
  
### <a name="response-elements"></a><span data-ttu-id="bf91f-131">Elementos de resposta</span><span class="sxs-lookup"><span data-stu-id="bf91f-131">Response elements</span></span>

<span data-ttu-id="bf91f-132">A resposta MoveFolder inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="bf91f-132">The MoveFolder response includes the following elements:</span></span>
  
- [<span data-ttu-id="bf91f-133">MoveFolderResponse</span><span class="sxs-lookup"><span data-stu-id="bf91f-133">MoveFolderResponse</span></span>](movefolderresponse.md)
    
- [<span data-ttu-id="bf91f-134">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bf91f-134">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="bf91f-135">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bf91f-135">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
    
- [<span data-ttu-id="bf91f-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="bf91f-136">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="bf91f-137">Pastas</span><span class="sxs-lookup"><span data-stu-id="bf91f-137">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="bf91f-138">Folder</span><span class="sxs-lookup"><span data-stu-id="bf91f-138">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="bf91f-139">FolderId</span><span class="sxs-lookup"><span data-stu-id="bf91f-139">FolderId</span></span>](folderid.md)
    
## <a name="movefolder-error-response-example"></a><span data-ttu-id="bf91f-140">Exemplo de resposta de erro MoveFolder</span><span class="sxs-lookup"><span data-stu-id="bf91f-140">MoveFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="bf91f-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf91f-141">Description</span></span>

<span data-ttu-id="bf91f-142">O exemplo a seguir mostra uma resposta de erro que ocorre quando você tenta mover uma pasta distinta.</span><span class="sxs-lookup"><span data-stu-id="bf91f-142">The following example shows an error response that occurs when you try to move a distinguished folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="bf91f-143">Código</span><span class="sxs-lookup"><span data-stu-id="bf91f-143">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <MoveFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:MoveFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Cannot move distinguished folder.</m:MessageText>
          <m:ResponseCode>ErrorMoveDistinguishedFolder</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:MoveFolderResponseMessage>
      </m:ResponseMessages>
    </MoveFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="bf91f-144">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="bf91f-144">Error response elements</span></span>

<span data-ttu-id="bf91f-145">A resposta de erro MoveFolder inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="bf91f-145">The MoveFolder error response includes the following elements:</span></span>
  
- [<span data-ttu-id="bf91f-146">MoveFolderResponse</span><span class="sxs-lookup"><span data-stu-id="bf91f-146">MoveFolderResponse</span></span>](movefolderresponse.md)
    
- [<span data-ttu-id="bf91f-147">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bf91f-147">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="bf91f-148">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bf91f-148">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
    
- [<span data-ttu-id="bf91f-149">MessageText</span><span class="sxs-lookup"><span data-stu-id="bf91f-149">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="bf91f-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="bf91f-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="bf91f-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="bf91f-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="bf91f-152">Pastas</span><span class="sxs-lookup"><span data-stu-id="bf91f-152">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="bf91f-153">Também consulte</span><span class="sxs-lookup"><span data-stu-id="bf91f-153">See also</span></span>



[<span data-ttu-id="bf91f-154">Operação CopyFolder</span><span class="sxs-lookup"><span data-stu-id="bf91f-154">CopyFolder operation</span></span>](copyfolder-operation.md)

