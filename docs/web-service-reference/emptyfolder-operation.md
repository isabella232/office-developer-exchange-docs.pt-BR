---
title: Operação EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 98161486-e2f2-480f-8d5d-708ba81b208a
description: A operação EmptyFolder esvazia pastas em uma caixa de correio. Opcionalmente, essa operação permite que você exclua as subpastas da pasta especificada. Quando uma subpasta é excluída, a subpasta e as mensagens dentro da subpasta são excluídas.
ms.openlocfilehash: 1913db74d33f1e6750cd158df5870f257d0e7839
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530681"
---
# <a name="emptyfolder-operation"></a><span data-ttu-id="88d0d-105">Operação EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="88d0d-105">EmptyFolder operation</span></span>

<span data-ttu-id="88d0d-106">A operação **EmptyFolder** esvazia pastas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="88d0d-106">The **EmptyFolder** operation empties folders in a mailbox.</span></span> <span data-ttu-id="88d0d-107">Opcionalmente, essa operação permite que você exclua as subpastas da pasta especificada.</span><span class="sxs-lookup"><span data-stu-id="88d0d-107">Optionally, this operation enables you to delete the subfolders of the specified folder.</span></span> <span data-ttu-id="88d0d-108">Quando uma subpasta é excluída, a subpasta e as mensagens dentro da subpasta são excluídas.</span><span class="sxs-lookup"><span data-stu-id="88d0d-108">When a subfolder is deleted, the subfolder and the messages within the subfolder are deleted.</span></span> 
  
## <a name="emptyfolder-request-example"></a><span data-ttu-id="88d0d-109">Exemplo de solicitação EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="88d0d-109">EmptyFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="88d0d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="88d0d-110">Description</span></span>

<span data-ttu-id="88d0d-111">O exemplo a seguir de uma solicitação **EmptyFolder** mostra como formar uma solicitação para esvaziar uma pasta.</span><span class="sxs-lookup"><span data-stu-id="88d0d-111">This following example of an **EmptyFolder** request shows how to form a request to empty a folder.</span></span> <span data-ttu-id="88d0d-112">Este exemplo exclui todas as subpastas da pasta identificada.</span><span class="sxs-lookup"><span data-stu-id="88d0d-112">This example deletes all subfolders of the identified folder.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="88d0d-113">Os valores dos atributos **ID** e **ChangeKey** do elemento [FolderId](folderid.md) foram reduzidos para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="88d0d-113">The values of the **Id** and the **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened for readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="88d0d-114">Código</span><span class="sxs-lookup"><span data-stu-id="88d0d-114">Code</span></span>

```XML
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
    </soap:Header>
    <soap:Body>
      <m:EmptyFolder DeleteType="HardDelete" DeleteSubFolders="true">
        <m:FolderIds>
          <t:FolderId Id="AQMkADhhOGU0"  ChangeKey="AQAAABYAAABsMB" />
        </m:FolderIds>
      </m:EmptyFolder>
    </soap:Body>
</soap:Envelope>

```

### <a name="comments"></a><span data-ttu-id="88d0d-115">Comentários</span><span class="sxs-lookup"><span data-stu-id="88d0d-115">Comments</span></span>

<span data-ttu-id="88d0d-116">Este exemplo executa uma exclusão de disco rígido na pasta.</span><span class="sxs-lookup"><span data-stu-id="88d0d-116">This example performs a hard delete on the folder.</span></span>
  
<span data-ttu-id="88d0d-117">As pastas podem ser identificadas pelo elemento [DistinguishedFolderId](distinguishedfolderid.md) ou o elemento [FolderId](folderid.md) para uso no elemento [FolderIds](folderids.md) .</span><span class="sxs-lookup"><span data-stu-id="88d0d-117">Folders can be identified by either the [DistinguishedFolderId](distinguishedfolderid.md) element or the [FolderId](folderid.md) element for use in the [FolderIds](folderids.md) element.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="88d0d-118">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="88d0d-118">Request elements</span></span>

<span data-ttu-id="88d0d-119">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="88d0d-119">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="88d0d-120">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="88d0d-120">EmptyFolder</span></span>](emptyfolder.md)
    
- [<span data-ttu-id="88d0d-121">FolderIds</span><span class="sxs-lookup"><span data-stu-id="88d0d-121">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="88d0d-122">FolderId</span><span class="sxs-lookup"><span data-stu-id="88d0d-122">FolderId</span></span>](folderid.md)
    
## <a name="successful-emptyfolder-response"></a><span data-ttu-id="88d0d-123">Resposta EmptyFolder bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="88d0d-123">Successful EmptyFolder response</span></span>

### <a name="description"></a><span data-ttu-id="88d0d-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="88d0d-124">Description</span></span>

<span data-ttu-id="88d0d-125">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação **EmptyFolder** .</span><span class="sxs-lookup"><span data-stu-id="88d0d-125">The following example shows a successful response to the **EmptyFolder** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="88d0d-126">Código</span><span class="sxs-lookup"><span data-stu-id="88d0d-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="164" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:EmptyFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                           xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:EmptyFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:EmptyFolderResponseMessage>
      </m:ResponseMessages>
    </m:EmptyFolderResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="88d0d-127">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="88d0d-127">Successful response elements</span></span>

<span data-ttu-id="88d0d-128">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="88d0d-128">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="88d0d-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="88d0d-129">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="88d0d-130">EmptyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="88d0d-130">EmptyFolderResponse</span></span>](emptyfolderresponse.md)
    
- [<span data-ttu-id="88d0d-131">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="88d0d-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="88d0d-132">EmptyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="88d0d-132">EmptyFolderResponseMessage</span></span>](emptyfolderresponsemessage.md)
    
- [<span data-ttu-id="88d0d-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="88d0d-133">ResponseCode</span></span>](responsecode.md)
    
## <a name="emptyfolder-error-response"></a><span data-ttu-id="88d0d-134">Resposta de erro EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="88d0d-134">EmptyFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="88d0d-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="88d0d-135">Description</span></span>

<span data-ttu-id="88d0d-136">O exemplo a seguir mostra uma resposta de erro a uma solicitação **EmptyFolder** .</span><span class="sxs-lookup"><span data-stu-id="88d0d-136">The following example shows an error response to an **Emptyfolder** request.</span></span> <span data-ttu-id="88d0d-137">O erro foi criado porque a operação tentou esvaziar uma pasta que não foi encontrada no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="88d0d-137">The error was created because the operation tried to empty a folder that was not found in the Exchange store.</span></span> 
  
### <a name="code"></a><span data-ttu-id="88d0d-138">Código</span><span class="sxs-lookup"><span data-stu-id="88d0d-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
            MinorVersion="1" 
            MajorBuildNumber="164" 
            MinorBuildNumber="0" 
            Version="Exchange2010_SP1" 
            xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
            xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
            xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse 
          xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="88d0d-139">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="88d0d-139">Error response elements</span></span>

<span data-ttu-id="88d0d-140">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="88d0d-140">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="88d0d-141">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="88d0d-141">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="88d0d-142">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="88d0d-142">GetFolderResponse</span></span>](getfolderresponse.md)
    
- [<span data-ttu-id="88d0d-143">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="88d0d-143">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="88d0d-144">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="88d0d-144">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
    
- [<span data-ttu-id="88d0d-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="88d0d-145">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="88d0d-146">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="88d0d-146">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="88d0d-147">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="88d0d-147">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="88d0d-148">Pastas</span><span class="sxs-lookup"><span data-stu-id="88d0d-148">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="88d0d-149">Confira também</span><span class="sxs-lookup"><span data-stu-id="88d0d-149">See also</span></span>

- [<span data-ttu-id="88d0d-150">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="88d0d-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

