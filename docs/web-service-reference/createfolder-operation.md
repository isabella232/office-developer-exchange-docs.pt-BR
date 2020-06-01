---
title: Operação CreateFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateFolder
api_type:
- schema
ms.assetid: 6f6c334c-b190-4e55-8f0a-38f2a018d1b3
description: A operação CreateFolder cria pastas, pastas de calendário, pastas de contatos, pastas de tarefas e pastas de pesquisa.
ms.openlocfilehash: 125a6d212e5eaf85ace71c048de809f3a05ba9b6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457547"
---
# <a name="createfolder-operation"></a><span data-ttu-id="f75a9-103">Operação CreateFolder</span><span class="sxs-lookup"><span data-stu-id="f75a9-103">CreateFolder operation</span></span>

<span data-ttu-id="f75a9-104">A operação CreateFolder cria pastas, pastas de calendário, pastas de contatos, pastas de tarefas e pastas de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="f75a9-104">The CreateFolder operation creates folders, calendar folders, contacts folders, tasks folders, and search folders.</span></span>
  
## <a name="createfolder-request-example"></a><span data-ttu-id="f75a9-105">Exemplo de solicitação CreateFolder</span><span class="sxs-lookup"><span data-stu-id="f75a9-105">CreateFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="f75a9-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="f75a9-106">Description</span></span>

<span data-ttu-id="f75a9-107">O exemplo a seguir de uma solicitação CreateFolder mostra como formar uma solicitação para criar duas novas pastas na raiz da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f75a9-107">The following example of a CreateFolder request shows how to form a request to create two new folders in the mailbox root.</span></span>
  
### <a name="code"></a><span data-ttu-id="f75a9-108">Código</span><span class="sxs-lookup"><span data-stu-id="f75a9-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ParentFolderId>
        <t:DistinguishedFolderId Id="msgfolderroot"/>
      </ParentFolderId>
      <Folders>
        <t:Folder>
          <t:DisplayName>Folder1</t:DisplayName>
        </t:Folder>
        <t:Folder>
          <t:DisplayName>Folder2</t:DisplayName>
        </t:Folder>
      </Folders>
    </CreateFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="f75a9-109">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="f75a9-109">Request elements</span></span>

<span data-ttu-id="f75a9-110">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="f75a9-110">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="f75a9-111">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="f75a9-111">CreateFolder</span></span>](createfolder.md)
    
- [<span data-ttu-id="f75a9-112">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="f75a9-112">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)
    
- [<span data-ttu-id="f75a9-113">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="f75a9-113">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="f75a9-114">Pastas</span><span class="sxs-lookup"><span data-stu-id="f75a9-114">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="f75a9-115">Folder</span><span class="sxs-lookup"><span data-stu-id="f75a9-115">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="f75a9-116">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="f75a9-116">DisplayName (string)</span></span>](displayname-string.md)
    
> [!NOTE]
> <span data-ttu-id="f75a9-117">O esquema que descreve esses elementos está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f75a9-117">The schema that describes these elements is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="f75a9-118">Para encontrar outras opções para a mensagem de solicitação da operação CreateFolder, explore a hierarquia do esquema.</span><span class="sxs-lookup"><span data-stu-id="f75a9-118">To find other options for the request message of the CreateFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="f75a9-119">Inicie no elemento [CreateFolder](createfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="f75a9-119">Start at the [CreateFolder](createfolder.md) element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="f75a9-120">Se você criar uma pasta de pesquisa com uma restrição usando a propriedade **calendário: organizador** , uma chamada de pasta Get subsequente retornará a restrição com a propriedade **Message: from** em seu lugar.</span><span class="sxs-lookup"><span data-stu-id="f75a9-120">If you create a search folder with a restriction by using the **calendar:Organizer** property, a subsequent get folder call will return the restriction with the **message:from** property in its place.</span></span> <span data-ttu-id="f75a9-121">Essas duas propriedades são mapeadas para a mesma propriedade MAPI subjacente.</span><span class="sxs-lookup"><span data-stu-id="f75a9-121">These two properties map to the same underlying MAPI property.</span></span> 
  
<span data-ttu-id="f75a9-122">A operação CreateFolder oferece suporte à criação de uma classe de pasta personalizada somente quando você cria a pasta usando um elemento de tipo de pasta genérico e define o elemento **FolderClass** .</span><span class="sxs-lookup"><span data-stu-id="f75a9-122">The CreateFolder operation supports the creation of a custom folder class only when you create the folder by using a generic folder type element and set the **FolderClass** element.</span></span> 
  
## <a name="successful-createfolder-response-example"></a><span data-ttu-id="f75a9-123">Exemplo de resposta CreateFolder bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="f75a9-123">Successful CreateFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="f75a9-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f75a9-124">Description</span></span>

<span data-ttu-id="f75a9-125">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação CreateFolder.</span><span class="sxs-lookup"><span data-stu-id="f75a9-125">The following example shows a successful response to the CreateFolder request.</span></span> <span data-ttu-id="f75a9-126">Neste exemplo, a resposta retorna os identificadores das novas pastas.</span><span class="sxs-lookup"><span data-stu-id="f75a9-126">In this example, the response returns the identifiers of the new folders.</span></span>
  
> [!NOTE]
> <span data-ttu-id="f75a9-127">A ID da pasta e a chave de alteração foram reduzidas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f75a9-127">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f75a9-128">Código</span><span class="sxs-lookup"><span data-stu-id="f75a9-128">Code</span></span>

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
    <CreateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS4AUn==" />
            </t:Folder>
          </m:Folders>
        </m:CreateFolderResponseMessage>
        <m:CreateFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS4AUn==" />
            </t:Folder>
          </m:Folders>
        </m:CreateFolderResponseMessage>
      </m:ResponseMessages>
    </CreateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="f75a9-129">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="f75a9-129">Successful response elements</span></span>

<span data-ttu-id="f75a9-130">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="f75a9-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="f75a9-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f75a9-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="f75a9-132">CreateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="f75a9-132">CreateFolderResponse</span></span>](createfolderresponse.md)
    
- [<span data-ttu-id="f75a9-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f75a9-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="f75a9-134">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f75a9-134">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md)
    
- [<span data-ttu-id="f75a9-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f75a9-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f75a9-136">Pastas</span><span class="sxs-lookup"><span data-stu-id="f75a9-136">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="f75a9-137">Folder</span><span class="sxs-lookup"><span data-stu-id="f75a9-137">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="f75a9-138">FolderId</span><span class="sxs-lookup"><span data-stu-id="f75a9-138">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="f75a9-139">Para encontrar outras opções para a mensagem de resposta da operação CreateFolder, explore a hierarquia do esquema.</span><span class="sxs-lookup"><span data-stu-id="f75a9-139">To find other options for the response message of the CreateFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="f75a9-140">Inicie no elemento [CreateFolderResponse](createfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="f75a9-140">Start at the [CreateFolderResponse](createfolderresponse.md) element.</span></span> 
  
## <a name="createfolder-error-response"></a><span data-ttu-id="f75a9-141">Resposta de erro CreateFolder</span><span class="sxs-lookup"><span data-stu-id="f75a9-141">CreateFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="f75a9-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="f75a9-142">Description</span></span>

<span data-ttu-id="f75a9-143">O exemplo a seguir mostra uma resposta de erro a uma solicitação CreateFolder.</span><span class="sxs-lookup"><span data-stu-id="f75a9-143">The following example shows an error response to a CreateFolder request.</span></span>
  
### <a name="code"></a><span data-ttu-id="f75a9-144">Código</span><span class="sxs-lookup"><span data-stu-id="f75a9-144">Code</span></span>

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
    <CreateFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateFolderResponseMessage ResponseClass="Error">
          <m:MessageText>A folder with the specified name already exists.</m:MessageText>
          <m:ResponseCode>ErrorFolderExists</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:CreateFolderResponseMessage>
      </m:ResponseMessages>
    </CreateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="f75a9-145">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="f75a9-145">Error response elements</span></span>

<span data-ttu-id="f75a9-146">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="f75a9-146">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="f75a9-147">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f75a9-147">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="f75a9-148">CreateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="f75a9-148">CreateFolderResponse</span></span>](createfolderresponse.md)
    
- [<span data-ttu-id="f75a9-149">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f75a9-149">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="f75a9-150">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f75a9-150">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md)
    
- [<span data-ttu-id="f75a9-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="f75a9-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="f75a9-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f75a9-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f75a9-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f75a9-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="f75a9-154">Pastas</span><span class="sxs-lookup"><span data-stu-id="f75a9-154">Folders</span></span>](folders-ex15websvcsotherref.md)
    
<span data-ttu-id="f75a9-155">Para encontrar outras opções para a mensagem de resposta de erro da operação CreateFolder, explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="f75a9-155">To find other options for the error response message of the CreateFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="f75a9-156">Inicie no elemento [CreateFolderResponse](createfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="f75a9-156">Start at the [CreateFolderResponse](createfolderresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="f75a9-157">Também consulte</span><span class="sxs-lookup"><span data-stu-id="f75a9-157">See also</span></span>



[<span data-ttu-id="f75a9-158">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="f75a9-158">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="f75a9-159">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="f75a9-159">FindFolder operation</span></span>](findfolder-operation.md)
  
 <span data-ttu-id="f75a9-160">**CreateFolderType**</span><span class="sxs-lookup"><span data-stu-id="f75a9-160">**CreateFolderType**</span></span>


- [<span data-ttu-id="f75a9-161">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f75a9-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="f75a9-162">Criando pastas (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="f75a9-162">Creating Folders (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

