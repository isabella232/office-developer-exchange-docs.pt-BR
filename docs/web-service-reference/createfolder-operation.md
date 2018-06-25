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
description: A operação CreateFolder cria pastas, as pastas de calendário, pastas de contatos, tarefas de pastas e pesquisa pastas.
ms.openlocfilehash: 97156d4a3747cacbdcf9563d21d93a0aa44c3358
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751584"
---
# <a name="createfolder-operation"></a><span data-ttu-id="13ce6-103">Operação CreateFolder</span><span class="sxs-lookup"><span data-stu-id="13ce6-103">CreateFolder operation</span></span>

<span data-ttu-id="13ce6-104">A operação CreateFolder cria pastas, as pastas de calendário, pastas de contatos, tarefas de pastas e pesquisa pastas.</span><span class="sxs-lookup"><span data-stu-id="13ce6-104">The CreateFolder operation creates folders, calendar folders, contacts folders, tasks folders, and search folders.</span></span>
  
## <a name="createfolder-request-example"></a><span data-ttu-id="13ce6-105">Exemplo de solicitação CreateFolder</span><span class="sxs-lookup"><span data-stu-id="13ce6-105">CreateFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="13ce6-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="13ce6-106">Description</span></span>

<span data-ttu-id="13ce6-107">O exemplo a seguir de uma solicitação de CreateFolder mostra como uma solicitação para criar duas novas pastas na raiz da caixa de correio de formulário.</span><span class="sxs-lookup"><span data-stu-id="13ce6-107">The following example of a CreateFolder request shows how to form a request to create two new folders in the mailbox root.</span></span>
  
### <a name="code"></a><span data-ttu-id="13ce6-108">Código</span><span class="sxs-lookup"><span data-stu-id="13ce6-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="request-elements"></a><span data-ttu-id="13ce6-109">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="13ce6-109">Request elements</span></span>

<span data-ttu-id="13ce6-110">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="13ce6-110">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="13ce6-111">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="13ce6-111">CreateFolder</span></span>](createfolder.md)
    
- [<span data-ttu-id="13ce6-112">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="13ce6-112">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)
    
- [<span data-ttu-id="13ce6-113">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="13ce6-113">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="13ce6-114">Pastas</span><span class="sxs-lookup"><span data-stu-id="13ce6-114">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="13ce6-115">Folder</span><span class="sxs-lookup"><span data-stu-id="13ce6-115">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="13ce6-116">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="13ce6-116">DisplayName (string)</span></span>](displayname-string.md)
    
> [!NOTE]
> <span data-ttu-id="13ce6-117">O esquema que descreve esses elementos está localizado no diretório virtual EWS do computador que está executando o MicrosoftExchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="13ce6-117">The schema that describes these elements is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="13ce6-118">Para localizar outras opções para a mensagem de solicitação da operação CreateFolder, explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="13ce6-118">To find other options for the request message of the CreateFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="13ce6-119">Inicie o elemento [CreateFolder](createfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="13ce6-119">Start at the [CreateFolder](createfolder.md) element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="13ce6-120">Se você criar uma pasta de pesquisa com uma restrição usando a propriedade de **Calendário: organizador** , uma chamada de pasta get subsequentes retornará a restrição com o **mensagem: do** propriedade em seu lugar.</span><span class="sxs-lookup"><span data-stu-id="13ce6-120">If you create a search folder with a restriction by using the **calendar:Organizer** property, a subsequent get folder call will return the restriction with the **message:from** property in its place.</span></span> <span data-ttu-id="13ce6-121">Essas duas propriedades mapeiam para a mesma propriedade MAPI subjacente.</span><span class="sxs-lookup"><span data-stu-id="13ce6-121">These two properties map to the same underlying MAPI property.</span></span> 
  
<span data-ttu-id="13ce6-122">A operação CreateFolder suporta a criação de uma classe de pasta personalizada somente quando você cria a pasta usando um elemento de tipo de pasta genérico e defina o elemento **FolderClass** .</span><span class="sxs-lookup"><span data-stu-id="13ce6-122">The CreateFolder operation supports the creation of a custom folder class only when you create the folder by using a generic folder type element and set the **FolderClass** element.</span></span> 
  
## <a name="successful-createfolder-response-example"></a><span data-ttu-id="13ce6-123">Exemplo de resposta bem-sucedida CreateFolder</span><span class="sxs-lookup"><span data-stu-id="13ce6-123">Successful CreateFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="13ce6-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="13ce6-124">Description</span></span>

<span data-ttu-id="13ce6-125">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação CreateFolder.</span><span class="sxs-lookup"><span data-stu-id="13ce6-125">The following example shows a successful response to the CreateFolder request.</span></span> <span data-ttu-id="13ce6-126">Neste exemplo, a resposta retorna os identificadores das novas pastas.</span><span class="sxs-lookup"><span data-stu-id="13ce6-126">In this example, the response returns the identifiers of the new folders.</span></span>
  
> [!NOTE]
> <span data-ttu-id="13ce6-127">A ID de pasta e a chave de alteração tem sido reduzidas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="13ce6-127">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="13ce6-128">Código</span><span class="sxs-lookup"><span data-stu-id="13ce6-128">Code</span></span>

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
    <CreateFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a><span data-ttu-id="13ce6-129">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="13ce6-129">Successful response elements</span></span>

<span data-ttu-id="13ce6-130">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="13ce6-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="13ce6-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="13ce6-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="13ce6-132">CreateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="13ce6-132">CreateFolderResponse</span></span>](createfolderresponse.md)
    
- [<span data-ttu-id="13ce6-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="13ce6-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="13ce6-134">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="13ce6-134">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md)
    
- [<span data-ttu-id="13ce6-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="13ce6-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="13ce6-136">Pastas</span><span class="sxs-lookup"><span data-stu-id="13ce6-136">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="13ce6-137">Folder</span><span class="sxs-lookup"><span data-stu-id="13ce6-137">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="13ce6-138">FolderId</span><span class="sxs-lookup"><span data-stu-id="13ce6-138">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="13ce6-139">Para localizar outras opções para a mensagem de resposta da operação CreateFolder, explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="13ce6-139">To find other options for the response message of the CreateFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="13ce6-140">Inicie o elemento [CreateFolderResponse](createfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="13ce6-140">Start at the [CreateFolderResponse](createfolderresponse.md) element.</span></span> 
  
## <a name="createfolder-error-response"></a><span data-ttu-id="13ce6-141">Resposta de erro CreateFolder</span><span class="sxs-lookup"><span data-stu-id="13ce6-141">CreateFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="13ce6-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="13ce6-142">Description</span></span>

<span data-ttu-id="13ce6-143">O exemplo a seguir mostra uma resposta de erro a uma solicitação de CreateFolder.</span><span class="sxs-lookup"><span data-stu-id="13ce6-143">The following example shows an error response to a CreateFolder request.</span></span>
  
### <a name="code"></a><span data-ttu-id="13ce6-144">Código</span><span class="sxs-lookup"><span data-stu-id="13ce6-144">Code</span></span>

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
    <CreateFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="13ce6-145">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="13ce6-145">Error response elements</span></span>

<span data-ttu-id="13ce6-146">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="13ce6-146">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="13ce6-147">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="13ce6-147">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="13ce6-148">CreateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="13ce6-148">CreateFolderResponse</span></span>](createfolderresponse.md)
    
- [<span data-ttu-id="13ce6-149">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="13ce6-149">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="13ce6-150">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="13ce6-150">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md)
    
- [<span data-ttu-id="13ce6-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="13ce6-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="13ce6-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="13ce6-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="13ce6-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="13ce6-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="13ce6-154">Pastas</span><span class="sxs-lookup"><span data-stu-id="13ce6-154">Folders</span></span>](folders-ex15websvcsotherref.md)
    
<span data-ttu-id="13ce6-155">Para localizar outras opções para a mensagem de resposta de erro da operação CreateFolder, explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="13ce6-155">To find other options for the error response message of the CreateFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="13ce6-156">Inicie o elemento [CreateFolderResponse](createfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="13ce6-156">Start at the [CreateFolderResponse](createfolderresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="13ce6-157">Confira também</span><span class="sxs-lookup"><span data-stu-id="13ce6-157">See also</span></span>



[<span data-ttu-id="13ce6-158">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="13ce6-158">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="13ce6-159">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="13ce6-159">FindFolder operation</span></span>](findfolder-operation.md)
  
 <span data-ttu-id="13ce6-160">**CreateFolderType**</span><span class="sxs-lookup"><span data-stu-id="13ce6-160">**CreateFolderType**</span></span>


- [<span data-ttu-id="13ce6-161">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="13ce6-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="13ce6-162">Criação de pastas (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="13ce6-162">Creating Folders (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

