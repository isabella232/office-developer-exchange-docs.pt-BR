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
description: A operação MoveFolder move pastas de uma pasta especificada e os coloca em outra pasta.
ms.openlocfilehash: 5da6929f11ce9ba74db190db6d799f25974d2192
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824490"
---
# <a name="movefolder-operation"></a><span data-ttu-id="29276-103">Operação MoveFolder</span><span class="sxs-lookup"><span data-stu-id="29276-103">MoveFolder operation</span></span>

<span data-ttu-id="29276-104">A operação MoveFolder move pastas de uma pasta especificada e os coloca em outra pasta.</span><span class="sxs-lookup"><span data-stu-id="29276-104">The MoveFolder operation moves folders from a specified folder and puts them in another folder.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="29276-105">Comentários</span><span class="sxs-lookup"><span data-stu-id="29276-105">Remarks</span></span>

<span data-ttu-id="29276-106">A operação MoveFolder é semelhante à operação CopyFolder.</span><span class="sxs-lookup"><span data-stu-id="29276-106">The MoveFolder operation is similar to the CopyFolder operation.</span></span> <span data-ttu-id="29276-107">Você não pode mover pastas diferenciadas.</span><span class="sxs-lookup"><span data-stu-id="29276-107">You cannot move distinguished folders.</span></span> <span data-ttu-id="29276-108">Você pode mover várias pastas de uma vez para a pasta de destino.</span><span class="sxs-lookup"><span data-stu-id="29276-108">You can move multiple folders at one time to the destination folder.</span></span>
  
## <a name="movefolder-request-example"></a><span data-ttu-id="29276-109">Exemplo de solicitação MoveFolder</span><span class="sxs-lookup"><span data-stu-id="29276-109">MoveFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="29276-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="29276-110">Description</span></span>

<span data-ttu-id="29276-111">O exemplo a seguir de uma solicitação de MoveFolder mostra como uma solicitação para mover uma pasta identificada ao [FolderId](folderid.md) e colocar a pasta na pasta Lixo eletrônico distinto de formulário.</span><span class="sxs-lookup"><span data-stu-id="29276-111">The following example of a MoveFolder request shows how to form a request to move a folder identified by the [FolderId](folderid.md) and put the folder in the Junk E-mail distinguished folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="29276-112">Código</span><span class="sxs-lookup"><span data-stu-id="29276-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <MoveFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="29276-113">Comments</span><span class="sxs-lookup"><span data-stu-id="29276-113">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="29276-114">O valor do atributo ID do elemento [FolderId](folderid.md) foi reduzido para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="29276-114">The value of the ID attribute of the [FolderId](folderid.md) element has been shortened for readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="29276-115">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29276-115">Request elements</span></span>

<span data-ttu-id="29276-116">Essa solicitação MoveFolder inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="29276-116">This MoveFolder request includes the following elements:</span></span>
  
- [<span data-ttu-id="29276-117">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="29276-117">MoveFolder</span></span>](movefolder.md)
    
- [<span data-ttu-id="29276-118">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="29276-118">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="29276-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="29276-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="29276-120">FolderIds</span><span class="sxs-lookup"><span data-stu-id="29276-120">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="29276-121">FolderId</span><span class="sxs-lookup"><span data-stu-id="29276-121">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="29276-122">Consulte o esquema de elementos adicionais que você pode usar para formar uma solicitação MoveFolder.</span><span class="sxs-lookup"><span data-stu-id="29276-122">See the schema for additional elements that you can use to form a MoveFolder request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="29276-123">O local padrão do esquema está no diretório virtual EWS no computador que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="29276-123">The default location of the schema is in the EWS virtual directory on the computer that has the Client Access server role installed.</span></span> 
  
## <a name="successful-movefolder-response-example"></a><span data-ttu-id="29276-124">Exemplo de resposta bem-sucedida MoveFolder</span><span class="sxs-lookup"><span data-stu-id="29276-124">Successful MoveFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="29276-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="29276-125">Description</span></span>

<span data-ttu-id="29276-126">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação MoveFolder.</span><span class="sxs-lookup"><span data-stu-id="29276-126">The following example shows a successful response to the MoveFolder request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="29276-127">Código</span><span class="sxs-lookup"><span data-stu-id="29276-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <MoveFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="29276-128">Comments</span><span class="sxs-lookup"><span data-stu-id="29276-128">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="29276-129">A ID de pasta e a chave de alteração tem sido reduzidas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="29276-129">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="29276-130">O que é retornado na resposta FolderId representa a pasta que foi movido para o novo local da pasta.</span><span class="sxs-lookup"><span data-stu-id="29276-130">The FolderId that is returned in the response represents the folder that was moved to the new the folder location.</span></span>
  
### <a name="response-elements"></a><span data-ttu-id="29276-131">Elementos de resposta</span><span class="sxs-lookup"><span data-stu-id="29276-131">Response elements</span></span>

<span data-ttu-id="29276-132">A resposta MoveFolder inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="29276-132">The MoveFolder response includes the following elements:</span></span>
  
- [<span data-ttu-id="29276-133">MoveFolderResponse</span><span class="sxs-lookup"><span data-stu-id="29276-133">MoveFolderResponse</span></span>](movefolderresponse.md)
    
- [<span data-ttu-id="29276-134">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="29276-134">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="29276-135">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="29276-135">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
    
- [<span data-ttu-id="29276-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="29276-136">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="29276-137">Pastas</span><span class="sxs-lookup"><span data-stu-id="29276-137">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="29276-138">Folder</span><span class="sxs-lookup"><span data-stu-id="29276-138">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="29276-139">FolderId</span><span class="sxs-lookup"><span data-stu-id="29276-139">FolderId</span></span>](folderid.md)
    
## <a name="movefolder-error-response-example"></a><span data-ttu-id="29276-140">Exemplo de resposta de erro MoveFolder</span><span class="sxs-lookup"><span data-stu-id="29276-140">MoveFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="29276-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="29276-141">Description</span></span>

<span data-ttu-id="29276-142">O exemplo a seguir mostra uma resposta de erro que ocorre quando você tenta mover uma pasta distinta.</span><span class="sxs-lookup"><span data-stu-id="29276-142">The following example shows an error response that occurs when you try to move a distinguished folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="29276-143">Código</span><span class="sxs-lookup"><span data-stu-id="29276-143">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <MoveFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="29276-144">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="29276-144">Error response elements</span></span>

<span data-ttu-id="29276-145">A resposta de erro MoveFolder inclui os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="29276-145">The MoveFolder error response includes the following elements:</span></span>
  
- [<span data-ttu-id="29276-146">MoveFolderResponse</span><span class="sxs-lookup"><span data-stu-id="29276-146">MoveFolderResponse</span></span>](movefolderresponse.md)
    
- [<span data-ttu-id="29276-147">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="29276-147">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="29276-148">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="29276-148">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
    
- [<span data-ttu-id="29276-149">MessageText</span><span class="sxs-lookup"><span data-stu-id="29276-149">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="29276-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="29276-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="29276-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="29276-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="29276-152">Pastas</span><span class="sxs-lookup"><span data-stu-id="29276-152">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="29276-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="29276-153">See also</span></span>



[<span data-ttu-id="29276-154">Operação CopyFolder</span><span class="sxs-lookup"><span data-stu-id="29276-154">CopyFolder operation</span></span>](copyfolder-operation.md)

