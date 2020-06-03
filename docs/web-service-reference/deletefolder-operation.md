---
title: Operação DeleteFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolder
api_type:
- schema
ms.assetid: b0f92682-4895-4bcf-a4a1-e4c2e8403979
description: A operação DeleteFolder exclui pastas de uma caixa de correio.
ms.openlocfilehash: e9bb9199027c2af2cbbb664ef7ad4fa70b7ef718
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455741"
---
# <a name="deletefolder-operation"></a><span data-ttu-id="f3679-103">Operação DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="f3679-103">DeleteFolder operation</span></span>

<span data-ttu-id="f3679-104">A operação **DeleteFolder** exclui pastas de uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f3679-104">The **DeleteFolder** operation deletes folders from a mailbox.</span></span> 
  
## <a name="deletefolder-request-example"></a><span data-ttu-id="f3679-105">Exemplo de solicitação DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="f3679-105">DeleteFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="f3679-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3679-106">Description</span></span>

<span data-ttu-id="f3679-107">O exemplo a seguir de uma solicitação **DeleteFolder** mostra como formar uma solicitação para excluir uma pasta.</span><span class="sxs-lookup"><span data-stu-id="f3679-107">This following example of a **DeleteFolder** request shows how to form a request to delete a folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f3679-108">Código</span><span class="sxs-lookup"><span data-stu-id="f3679-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                  DeleteType="HardDelete" >
      <FolderIds>
        <t:FolderId Id="AS4AUnVz=" />
      </FolderIds>
    </DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="f3679-109">Comentários</span><span class="sxs-lookup"><span data-stu-id="f3679-109">Comments</span></span>

<span data-ttu-id="f3679-110">Este exemplo executa uma exclusão de disco rígido na pasta.</span><span class="sxs-lookup"><span data-stu-id="f3679-110">This example performs a hard delete on the folder.</span></span>
  
> [!NOTE]
> <span data-ttu-id="f3679-111">A ID da pasta foi reduzida para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f3679-111">The folder ID has been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="f3679-112">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="f3679-112">Request elements</span></span>

<span data-ttu-id="f3679-113">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="f3679-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="f3679-114">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="f3679-114">DeleteFolder</span></span>](deletefolder.md)
    
- [<span data-ttu-id="f3679-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="f3679-115">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="f3679-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="f3679-116">FolderId</span></span>](folderid.md)
    
> [!NOTE]
> <span data-ttu-id="f3679-117">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f3679-117">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="f3679-118">Para encontrar outras opções para a mensagem de solicitação da operação **DeleteFolder** , explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="f3679-118">To find other options for the request message of the **DeleteFolder** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="f3679-119">Inicie no elemento [DeleteFolder](deletefolder.md) .</span><span class="sxs-lookup"><span data-stu-id="f3679-119">Start at the [DeleteFolder](deletefolder.md) element.</span></span> 
  
## <a name="successful-deletefolder-response"></a><span data-ttu-id="f3679-120">Resposta DeleteFolder bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="f3679-120">Successful DeleteFolder response</span></span>

### <a name="description"></a><span data-ttu-id="f3679-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3679-121">Description</span></span>

<span data-ttu-id="f3679-122">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação **DeleteFolder** .</span><span class="sxs-lookup"><span data-stu-id="f3679-122">The following example shows a successful response to the **DeleteFolder** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f3679-123">Código</span><span class="sxs-lookup"><span data-stu-id="f3679-123">Code</span></span>

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
    <DeleteFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteFolderResponseMessage>
      </m:ResponseMessages>
    </DeleteFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="f3679-124">Elementos de resposta</span><span class="sxs-lookup"><span data-stu-id="f3679-124">Response elements</span></span>

<span data-ttu-id="f3679-125">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="f3679-125">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="f3679-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f3679-126">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="f3679-127">DeleteFolderResponse</span><span class="sxs-lookup"><span data-stu-id="f3679-127">DeleteFolderResponse</span></span>](deletefolderresponse.md)
    
- [<span data-ttu-id="f3679-128">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f3679-128">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="f3679-129">DeleteFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f3679-129">DeleteFolderResponseMessage</span></span>](deletefolderresponsemessage.md)
    
- [<span data-ttu-id="f3679-130">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f3679-130">ResponseCode</span></span>](responsecode.md)
    
<span data-ttu-id="f3679-131">Para encontrar outras opções para a mensagem de resposta da operação **DeleteFolder** , explore a hierarquia do esquema.</span><span class="sxs-lookup"><span data-stu-id="f3679-131">To find other options for the response message of the **DeleteFolder** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="f3679-132">Inicie no elemento [DeleteFolderResponse](deletefolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="f3679-132">Start at the [DeleteFolderResponse](deletefolderresponse.md) element.</span></span> 
  
## <a name="deletefolder-error-response"></a><span data-ttu-id="f3679-133">Resposta de erro DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="f3679-133">DeleteFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="f3679-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3679-134">Description</span></span>

<span data-ttu-id="f3679-135">O exemplo a seguir mostra uma resposta de erro a uma solicitação **DeleteFolder** .</span><span class="sxs-lookup"><span data-stu-id="f3679-135">The following example shows an error response to a **DeleteFolder** request.</span></span> <span data-ttu-id="f3679-136">O erro foi causado por uma solicitação para excluir uma pasta que não estava presente na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f3679-136">The error was caused by a request to delete a folder that was not present in the mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f3679-137">Código</span><span class="sxs-lookup"><span data-stu-id="f3679-137">Code</span></span>

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
    <DeleteFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DeleteFolderResponseMessage>
      </m:ResponseMessages>
    </DeleteFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="f3679-138">Comentários</span><span class="sxs-lookup"><span data-stu-id="f3679-138">Comments</span></span>

<span data-ttu-id="f3679-139">A operação **DeleteFolder** não pode ser usada em pastas diferenciadas.</span><span class="sxs-lookup"><span data-stu-id="f3679-139">The **DeleteFolder** operation cannot be used on distinguished folders.</span></span> 
  
### <a name="error-response-elements"></a><span data-ttu-id="f3679-140">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="f3679-140">Error response elements</span></span>

<span data-ttu-id="f3679-141">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="f3679-141">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="f3679-142">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f3679-142">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="f3679-143">DeleteFolderResponse</span><span class="sxs-lookup"><span data-stu-id="f3679-143">DeleteFolderResponse</span></span>](deletefolderresponse.md)
    
- [<span data-ttu-id="f3679-144">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f3679-144">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="f3679-145">DeleteFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f3679-145">DeleteFolderResponseMessage</span></span>](deletefolderresponsemessage.md)
    
- [<span data-ttu-id="f3679-146">MessageText</span><span class="sxs-lookup"><span data-stu-id="f3679-146">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="f3679-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f3679-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f3679-148">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f3679-148">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="f3679-149">Para encontrar outras opções para a mensagem de resposta de erro da operação **DeleteFolder** , explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="f3679-149">To find other options for the error response message of the **DeleteFolder** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="f3679-150">Inicie no elemento [DeleteFolderResponse](deletefolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="f3679-150">Start at the [DeleteFolderResponse](deletefolderresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="f3679-151">Confira também</span><span class="sxs-lookup"><span data-stu-id="f3679-151">See also</span></span>

- [<span data-ttu-id="f3679-152">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f3679-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="f3679-153">Excluindo pastas</span><span class="sxs-lookup"><span data-stu-id="f3679-153">Deleting Folders</span></span>](https://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

