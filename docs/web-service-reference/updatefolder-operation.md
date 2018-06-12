---
title: Operação UpdateFolder
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateFolder
api_type:
- schema
ms.assetid: 3494c996-b834-4813-b1ca-d99642d8b4e7
description: 'A operação UpdateFolder é usada para modificar as propriedades de um item existente no armazenamento do Exchange. Cada operação UpdateFolder consiste no seguinte:'
ms.openlocfilehash: b33937bb09f0dcbe3d3ed61bbf5233423f320d9c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837884"
---
# <a name="updatefolder-operation"></a><span data-ttu-id="21bbd-104">Operação UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="21bbd-104">UpdateFolder operation</span></span>

<span data-ttu-id="21bbd-105">A operação UpdateFolder é usada para modificar as propriedades de um item existente no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="21bbd-105">The UpdateFolder operation is used to modify properties of an existing item in the Exchange store.</span></span> <span data-ttu-id="21bbd-106">Cada operação UpdateFolder consiste no seguinte:</span><span class="sxs-lookup"><span data-stu-id="21bbd-106">Each UpdateFolder operation consists of the following:</span></span>
  
- <span data-ttu-id="21bbd-107">Um elemento de [FolderId](folderid.md) que especifica uma pasta a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="21bbd-107">A [FolderId](folderid.md) element that specifies a folder to update.</span></span> 
    
- <span data-ttu-id="21bbd-108">Um caminho interno de um elemento na pasta, conforme especificado pela forma pasta, que especifica os dados para atualizar.</span><span class="sxs-lookup"><span data-stu-id="21bbd-108">An internal path of an element in the folder, as specified by the folder shape, which specifies the data to update.</span></span>
    
- <span data-ttu-id="21bbd-109">Uma pasta que contém o novo valor do campo atualizado, se a atualização não for uma exclusão.</span><span class="sxs-lookup"><span data-stu-id="21bbd-109">A folder that contains the new value of the updated field, if the update is not a deletion.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="21bbd-110">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="21bbd-110">Remarks</span></span>

<span data-ttu-id="21bbd-111">Três ações de atualização básica podem ser executadas em um item.</span><span class="sxs-lookup"><span data-stu-id="21bbd-111">Three basic update actions can be performed on an item.</span></span> <span data-ttu-id="21bbd-112">Essas ações são listadas na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="21bbd-112">These actions are listed in the following table.</span></span>
  
|<span data-ttu-id="21bbd-113">**Action**</span><span class="sxs-lookup"><span data-stu-id="21bbd-113">**Action**</span></span>|<span data-ttu-id="21bbd-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="21bbd-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="21bbd-115">Acréscimo</span><span class="sxs-lookup"><span data-stu-id="21bbd-115">Append</span></span>  <br/> |<span data-ttu-id="21bbd-116">A ação append adiciona dados a uma propriedade existente.</span><span class="sxs-lookup"><span data-stu-id="21bbd-116">The append action adds data to an existing property.</span></span> <span data-ttu-id="21bbd-117">Preserva os dados que está atualmente lá.</span><span class="sxs-lookup"><span data-stu-id="21bbd-117">It preserves the data that is currently there.</span></span> <span data-ttu-id="21bbd-118">Acrescentar não é aplicável a todas as propriedades.</span><span class="sxs-lookup"><span data-stu-id="21bbd-118">Append is not applicable to all properties.</span></span>  <br/> |
|<span data-ttu-id="21bbd-119">Conjunto</span><span class="sxs-lookup"><span data-stu-id="21bbd-119">Set</span></span>  <br/> |<span data-ttu-id="21bbd-120">A ação set substitui os dados de uma propriedade se ele contém dados, ou cria a propriedade e define seu valor, se não existir.</span><span class="sxs-lookup"><span data-stu-id="21bbd-120">The set action replaces data for a property if it contains data, or creates the property and sets its value if it does not exist.</span></span> <span data-ttu-id="21bbd-121">A ação set só é aplicável às propriedades graváveis.</span><span class="sxs-lookup"><span data-stu-id="21bbd-121">The set action is only applicable to writable properties.</span></span>  <br/> |
|<span data-ttu-id="21bbd-122">Excluir</span><span class="sxs-lookup"><span data-stu-id="21bbd-122">Delete</span></span>  <br/> |<span data-ttu-id="21bbd-123">A ação Excluir remove uma propriedade de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="21bbd-123">The delete action removes a property from a folder.</span></span> <span data-ttu-id="21bbd-124">Isso é diferente de defini-la como um valor vazio.</span><span class="sxs-lookup"><span data-stu-id="21bbd-124">This is different than setting it to an empty value.</span></span> <span data-ttu-id="21bbd-125">Quando concluir, a propriedade não existe para a pasta.</span><span class="sxs-lookup"><span data-stu-id="21bbd-125">When complete, the property does not exist for the folder.</span></span> <span data-ttu-id="21bbd-126">Excluir só é aplicável às propriedades graváveis.</span><span class="sxs-lookup"><span data-stu-id="21bbd-126">Delete is only applicable to writable properties.</span></span>  <br/> |
   
## <a name="updatefolder-request-example"></a><span data-ttu-id="21bbd-127">Exemplo de solicitação UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="21bbd-127">UpdateFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="21bbd-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="21bbd-128">Description</span></span>

<span data-ttu-id="21bbd-129">O exemplo a seguir de uma solicitação de UpdateFolder mostra como atualizar um nome de exibição da pasta.</span><span class="sxs-lookup"><span data-stu-id="21bbd-129">The following example of an UpdateFolder request shows how to update a folder display name.</span></span> 
  
### <a name="code"></a><span data-ttu-id="21bbd-130">Código</span><span class="sxs-lookup"><span data-stu-id="21bbd-130">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="AScA" ChangeKey="GO3u/"/>
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:DisplayName"/>
              <t:Folder>
                <t:DisplayName>NewFolderName</t:DisplayName>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </FolderChanges>
    </UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="21bbd-131">Comments</span><span class="sxs-lookup"><span data-stu-id="21bbd-131">Comments</span></span>

<span data-ttu-id="21bbd-132">Este exemplo altera o nome de exibição da pasta para novonomedepasta.</span><span class="sxs-lookup"><span data-stu-id="21bbd-132">This example changes the display name of the folder to NewFolderName.</span></span>
  
> [!NOTE]
> <span data-ttu-id="21bbd-133">Os valores de **Id** e **ChangeKey** atributos do elemento [FolderId](folderid.md) foram diminuídos para melhorar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="21bbd-133">The values of the **Id** and **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened for readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="21bbd-134">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="21bbd-134">Request elements</span></span>

<span data-ttu-id="21bbd-135">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="21bbd-135">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="21bbd-136">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="21bbd-136">UpdateFolder</span></span>](updatefolder.md)
    
- [<span data-ttu-id="21bbd-137">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="21bbd-137">FolderChanges</span></span>](folderchanges.md)
    
- [<span data-ttu-id="21bbd-138">FolderChange</span><span class="sxs-lookup"><span data-stu-id="21bbd-138">FolderChange</span></span>](folderchange.md)
    
- [<span data-ttu-id="21bbd-139">FolderId</span><span class="sxs-lookup"><span data-stu-id="21bbd-139">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="21bbd-140">Atualizações (Item)</span><span class="sxs-lookup"><span data-stu-id="21bbd-140">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="21bbd-141">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="21bbd-141">SetFolderField</span></span>](setfolderfield.md)
    
- [<span data-ttu-id="21bbd-142">FieldURI</span><span class="sxs-lookup"><span data-stu-id="21bbd-142">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="21bbd-143">Folder</span><span class="sxs-lookup"><span data-stu-id="21bbd-143">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="21bbd-144">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="21bbd-144">DisplayName (string)</span></span>](displayname-string.md)
    
<span data-ttu-id="21bbd-145">Consulte o esquema de elementos adicionais que você pode usar para formar uma solicitação UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="21bbd-145">See the schema for additional elements that you can use to form an UpdateFolder request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="21bbd-146">O local padrão do esquema está no diretório virtual EWS no computador que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="21bbd-146">The default location of the schema is in the EWS virtual directory on the computer that has the Client Access server role installed.</span></span> 
  
## <a name="updatefolder-response-example"></a><span data-ttu-id="21bbd-147">Exemplo de resposta UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="21bbd-147">UpdateFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="21bbd-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="21bbd-148">Description</span></span>

<span data-ttu-id="21bbd-149">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="21bbd-149">The following example shows a successful response to the UpdateFolder request.</span></span> <span data-ttu-id="21bbd-150">Neste exemplo, a nova chave de alteração é retornada para refletir o status atualizado da pasta.</span><span class="sxs-lookup"><span data-stu-id="21bbd-150">In this example, the new change key is returned to reflect the updated status of the folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="21bbd-151">Código</span><span class="sxs-lookup"><span data-stu-id="21bbd-151">Code</span></span>

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
    <UpdateFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AAAlAFVz" ChangeKey="AQAAAB" />
            </t:Folder>
          </m:Folders>
        </m:UpdateFolderResponseMessage>
      </m:ResponseMessages>
    </UpdateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="21bbd-152">Comments</span><span class="sxs-lookup"><span data-stu-id="21bbd-152">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="21bbd-153">A ID de pasta e a chave de alteração tem sido reduzidas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="21bbd-153">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="21bbd-154">O ID da pasta que é retornado na resposta representa a pasta atualizada.</span><span class="sxs-lookup"><span data-stu-id="21bbd-154">The folder ID that is returned in the response represents the updated folder.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="21bbd-155">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="21bbd-155">Successful response elements</span></span>

<span data-ttu-id="21bbd-156">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="21bbd-156">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="21bbd-157">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="21bbd-157">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="21bbd-158">UpdateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="21bbd-158">UpdateFolderResponse</span></span>](updatefolderresponse.md)
    
- [<span data-ttu-id="21bbd-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="21bbd-159">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="21bbd-160">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="21bbd-160">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md)
    
- [<span data-ttu-id="21bbd-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="21bbd-161">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="21bbd-162">Pastas</span><span class="sxs-lookup"><span data-stu-id="21bbd-162">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="21bbd-163">Folder</span><span class="sxs-lookup"><span data-stu-id="21bbd-163">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="21bbd-164">FolderId</span><span class="sxs-lookup"><span data-stu-id="21bbd-164">FolderId</span></span>](folderid.md)
    
## <a name="updatefolder-error-response-example"></a><span data-ttu-id="21bbd-165">Exemplo de resposta de erro UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="21bbd-165">UpdateFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="21bbd-166">Descrição</span><span class="sxs-lookup"><span data-stu-id="21bbd-166">Description</span></span>

<span data-ttu-id="21bbd-167">O exemplo a seguir mostra uma resposta de erro a uma solicitação de UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="21bbd-167">The following example shows an error response to an UpdateFolder request.</span></span>
  
### <a name="code"></a><span data-ttu-id="21bbd-168">Código</span><span class="sxs-lookup"><span data-stu-id="21bbd-168">Code</span></span>

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
    <UpdateFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The change key is invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidChangeKey</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:UpdateFolderResponseMessage>
      </m:ResponseMessages>
    </UpdateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="21bbd-169">Comments</span><span class="sxs-lookup"><span data-stu-id="21bbd-169">Comments</span></span>

<span data-ttu-id="21bbd-170">Este exemplo mostra uma resposta de erro é gerada por um atributo **ChangeKey** inválido na solicitação.</span><span class="sxs-lookup"><span data-stu-id="21bbd-170">This example shows an error response that is caused by an invalid **ChangeKey** attribute in the request.</span></span> 
  
### <a name="error-response-elements"></a><span data-ttu-id="21bbd-171">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="21bbd-171">Error response elements</span></span>

<span data-ttu-id="21bbd-172">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="21bbd-172">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="21bbd-173">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="21bbd-173">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="21bbd-174">UpdateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="21bbd-174">UpdateFolderResponse</span></span>](updatefolderresponse.md)
    
- [<span data-ttu-id="21bbd-175">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="21bbd-175">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="21bbd-176">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="21bbd-176">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md)
    
- [<span data-ttu-id="21bbd-177">MessageText</span><span class="sxs-lookup"><span data-stu-id="21bbd-177">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="21bbd-178">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="21bbd-178">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="21bbd-179">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="21bbd-179">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="21bbd-180">Pastas</span><span class="sxs-lookup"><span data-stu-id="21bbd-180">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="21bbd-181">Confira também</span><span class="sxs-lookup"><span data-stu-id="21bbd-181">See also</span></span>



- [<span data-ttu-id="21bbd-182">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="21bbd-182">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

