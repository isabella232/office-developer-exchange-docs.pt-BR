---
title: SearchFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SearchFolder
api_type:
- schema
ms.assetid: 1a7d408b-2e98-4391-8834-085ed6d5757c
description: O elemento SearchFolder representa uma pasta de pesquisa que está contida em uma caixa de correio.
ms.openlocfilehash: e1d5893e00f3b199451622061785e2566c6f32e5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464004"
---
# <a name="searchfolder"></a><span data-ttu-id="ca074-103">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="ca074-103">SearchFolder</span></span>

<span data-ttu-id="ca074-104">O elemento **SearchFolder** representa uma pasta de pesquisa que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ca074-104">The **SearchFolder** element represents a search folder that is contained in a mailbox.</span></span> 
  
```xml
<SearchFolder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <UnreadCount/>
   <SearchParameters/>
   <PermissionSet/>
      <EffectiveRights/>
</SearchFolder>
```

 <span data-ttu-id="ca074-105">**SearchFolderType**</span><span class="sxs-lookup"><span data-stu-id="ca074-105">**SearchFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ca074-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ca074-106">Attributes and elements</span></span>

<span data-ttu-id="ca074-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ca074-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ca074-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ca074-108">Attributes</span></span>

<span data-ttu-id="ca074-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ca074-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ca074-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ca074-110">Child elements</span></span>

|<span data-ttu-id="ca074-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ca074-111">**Element**</span></span>|<span data-ttu-id="ca074-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ca074-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ca074-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="ca074-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="ca074-114">Contém o identificador e a chave de alteração de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="ca074-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="ca074-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="ca074-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="ca074-116">Representa o identificador da pasta pai que contém a pasta.</span><span class="sxs-lookup"><span data-stu-id="ca074-116">Represents the identifier of the parent folder that contains the folder.</span></span>  <br/> |
|[<span data-ttu-id="ca074-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="ca074-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="ca074-118">Representa a classe Folder de uma determinada pasta.</span><span class="sxs-lookup"><span data-stu-id="ca074-118">Represents the folder class for a given folder.</span></span>  <br/> |
|[<span data-ttu-id="ca074-119">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="ca074-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="ca074-120">Contém o nome de exibição de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="ca074-120">Contains the display name of a folder.</span></span>  <br/> |
|[<span data-ttu-id="ca074-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="ca074-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="ca074-122">Representa a contagem total de itens em uma determinada pasta.</span><span class="sxs-lookup"><span data-stu-id="ca074-122">Represents the total count of items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="ca074-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="ca074-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="ca074-124">Representa o número de pastas filhas contidas em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="ca074-124">Represents the number of child folders contained within a folder.</span></span> <span data-ttu-id="ca074-125">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca074-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="ca074-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="ca074-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="ca074-127">Identifica as propriedades estendidas em pastas.</span><span class="sxs-lookup"><span data-stu-id="ca074-127">Identifies extended properties on folders.</span></span>  <br/> |
|[<span data-ttu-id="ca074-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="ca074-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="ca074-129">Contém informações sobre uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="ca074-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="ca074-130">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="ca074-130">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="ca074-131">Representa a contagem de itens não lidos em uma determinada pasta.</span><span class="sxs-lookup"><span data-stu-id="ca074-131">Represents the count of unread items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="ca074-132">SearchParameters</span><span class="sxs-lookup"><span data-stu-id="ca074-132">SearchParameters</span></span>](searchparameters.md) <br/> |<span data-ttu-id="ca074-133">Contém os parâmetros que definem uma pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="ca074-133">Contains the parameters that define a search folder.</span></span>  <br/> |
|[<span data-ttu-id="ca074-134">PermissionSet (PermissionSettype)</span><span class="sxs-lookup"><span data-stu-id="ca074-134">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="ca074-135">Contém todas as permissões configuradas para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="ca074-135">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="ca074-136">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ca074-136">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="ca074-137">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="ca074-137">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="ca074-138">Contém os direitos do cliente com base nas configurações de permissão para o item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="ca074-138">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="ca074-139">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ca074-139">This element is read-only.</span></span> <span data-ttu-id="ca074-140">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="ca074-140">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ca074-141">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ca074-141">Parent elements</span></span>

|<span data-ttu-id="ca074-142">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ca074-142">**Element**</span></span>|<span data-ttu-id="ca074-143">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ca074-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ca074-144">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="ca074-144">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="ca074-145">Especifica os dados a serem acrescentados a uma propriedade de pasta durante uma [operação UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ca074-145">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="ca074-146">Criar (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="ca074-146">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="ca074-147">Identifica uma única pasta a ser criada no armazenamento do cliente local.</span><span class="sxs-lookup"><span data-stu-id="ca074-147">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="ca074-148">Setfolderfield</span><span class="sxs-lookup"><span data-stu-id="ca074-148">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="ca074-149">Representa uma atualização de uma única propriedade em uma pasta em uma [operação UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ca074-149">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="ca074-150">Atualização (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="ca074-150">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="ca074-151">Identifica uma única pasta a ser atualizada no repositório do cliente local.</span><span class="sxs-lookup"><span data-stu-id="ca074-151">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="ca074-152">Pastas</span><span class="sxs-lookup"><span data-stu-id="ca074-152">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ca074-153">Contém uma matriz de pastas usadas em operações de pasta.</span><span class="sxs-lookup"><span data-stu-id="ca074-153">Contains an array of folders used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ca074-154">Comentários</span><span class="sxs-lookup"><span data-stu-id="ca074-154">Remarks</span></span>

 <span data-ttu-id="ca074-155">**SearchFolder** é usado para pastas de pesquisa regulares e pastas de pesquisa visíveis do MicrosoftOfficeOutlook e do Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="ca074-155">**SearchFolder** is used for both regular search folders and MicrosoftOfficeOutlook and Outlook Web Access visible search folders.</span></span> <span data-ttu-id="ca074-156">Para que uma pasta de pesquisa fique visível para o Outlook e o Outlook Web Access, a pasta deve ser criada na pasta distinta do SearchFolders.</span><span class="sxs-lookup"><span data-stu-id="ca074-156">For a search folder to be visible to Outlook and Outlook Web Access, the folder must be created under the SearchFolders distinguished folder.</span></span> 
  
<span data-ttu-id="ca074-157">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="ca074-157">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ca074-158">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ca074-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ca074-159">Namespace</span><span class="sxs-lookup"><span data-stu-id="ca074-159">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ca074-160">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ca074-160">Schema Name</span></span>  <br/> |<span data-ttu-id="ca074-161">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ca074-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="ca074-162">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ca074-162">Validation File</span></span>  <br/> |<span data-ttu-id="ca074-163">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ca074-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ca074-164">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ca074-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="ca074-165">False</span><span class="sxs-lookup"><span data-stu-id="ca074-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ca074-166">Confira também</span><span class="sxs-lookup"><span data-stu-id="ca074-166">See also</span></span>



- [<span data-ttu-id="ca074-167">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ca074-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

