---
title: ContactsFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContactsFolder
api_type:
- schema
ms.assetid: 6c299de8-2087-4aeb-8e66-2bc7586509a6
description: O elemento ContactsFolder representa uma pasta de contatos que está contida em uma caixa de correio.
ms.openlocfilehash: 997b4f603198e6d05a011c4ef6bac7fe4dfbfe52
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529431"
---
# <a name="contactsfolder"></a><span data-ttu-id="bf97b-103">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="bf97b-103">ContactsFolder</span></span>

<span data-ttu-id="bf97b-104">O elemento **ContactsFolder** representa uma pasta de contatos que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="bf97b-104">The **ContactsFolder** element represents a contacts folder that is contained in a mailbox.</span></span> 
  
```xml
<ContactsFolder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <EffectiveRights/>
   <SharingEffectiveRights/>
   <PermissionSet/>
</ContactsFolder>
```

 <span data-ttu-id="bf97b-105">**ContactsFolderType**</span><span class="sxs-lookup"><span data-stu-id="bf97b-105">**ContactsFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bf97b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="bf97b-106">Attributes and elements</span></span>

<span data-ttu-id="bf97b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="bf97b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bf97b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="bf97b-108">Attributes</span></span>

<span data-ttu-id="bf97b-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bf97b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bf97b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="bf97b-110">Child elements</span></span>

|<span data-ttu-id="bf97b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bf97b-111">**Element**</span></span>|<span data-ttu-id="bf97b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bf97b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bf97b-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="bf97b-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="bf97b-114">Contém o identificador e a chave de alteração de uma pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="bf97b-114">Contains the identifier and change key of a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="bf97b-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="bf97b-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="bf97b-116">Representa o identificador da pasta pai que contém a pasta contatos.</span><span class="sxs-lookup"><span data-stu-id="bf97b-116">Represents the identifier of the parent folder that contains the contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="bf97b-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="bf97b-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="bf97b-118">Representa a classe Folder de uma pasta contatos.</span><span class="sxs-lookup"><span data-stu-id="bf97b-118">Represents the folder class for a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="bf97b-119">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="bf97b-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="bf97b-120">Contém o nome de exibição de uma pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="bf97b-120">Contains the display name of a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="bf97b-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="bf97b-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="bf97b-122">Representa a contagem total de itens em uma pasta contatos.</span><span class="sxs-lookup"><span data-stu-id="bf97b-122">Represents the total count of items within a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="bf97b-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="bf97b-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="bf97b-124">Representa o número de pastas filhas que estão contidas em uma pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="bf97b-124">Represents the number of child folders that are contained within a contacts folder.</span></span> <span data-ttu-id="bf97b-125">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bf97b-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="bf97b-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="bf97b-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="bf97b-127">Identifica as propriedades estendidas nas pastas de contatos.</span><span class="sxs-lookup"><span data-stu-id="bf97b-127">Identifies extended properties on contacts folders.</span></span>  <br/> |
|[<span data-ttu-id="bf97b-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="bf97b-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="bf97b-129">Contém informações sobre uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="bf97b-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="bf97b-130">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="bf97b-130">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="bf97b-131">Contém os direitos do cliente com base nas configurações de permissão para o item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="bf97b-131">Contains the client's rights based on the permission settings for the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="bf97b-132">SharingEffectiveRights (PermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="bf97b-132">SharingEffectiveRights (PermissionReadAccessType)</span></span>](sharingeffectiverights-permissionreadaccesstype.md) <br/> |<span data-ttu-id="bf97b-133">Indica as permissões que o usuário tem para os dados de contato que estão sendo compartilhados.</span><span class="sxs-lookup"><span data-stu-id="bf97b-133">Indicates the permissions that the user has for the contact data that is being shared.</span></span>  <br/> |
|[<span data-ttu-id="bf97b-134">PermissionSet (PermissionSettype)</span><span class="sxs-lookup"><span data-stu-id="bf97b-134">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="bf97b-135">Contém todas as permissões configuradas para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="bf97b-135">Contains all the configured permissions for a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bf97b-136">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="bf97b-136">Parent elements</span></span>

|<span data-ttu-id="bf97b-137">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="bf97b-137">**Element**</span></span>|<span data-ttu-id="bf97b-138">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="bf97b-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bf97b-139">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="bf97b-139">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="bf97b-140">Especifica os dados a serem acrescentados a uma propriedade de pasta durante uma [operação UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="bf97b-140">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="bf97b-141">Criar (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="bf97b-141">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="bf97b-142">Identifica uma única pasta a ser criada no armazenamento do cliente local.</span><span class="sxs-lookup"><span data-stu-id="bf97b-142">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="bf97b-143">Setfolderfield</span><span class="sxs-lookup"><span data-stu-id="bf97b-143">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="bf97b-144">Representa uma atualização de uma única propriedade em uma pasta em uma [operação UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="bf97b-144">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="bf97b-145">Atualização (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="bf97b-145">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="bf97b-146">Identifica uma única pasta a ser atualizada no repositório do cliente local.</span><span class="sxs-lookup"><span data-stu-id="bf97b-146">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="bf97b-147">Pastas</span><span class="sxs-lookup"><span data-stu-id="bf97b-147">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="bf97b-148">Contém uma matriz de pastas que são usadas em operações de pasta.</span><span class="sxs-lookup"><span data-stu-id="bf97b-148">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bf97b-149">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="bf97b-149">Text value</span></span>

<span data-ttu-id="bf97b-150">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="bf97b-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bf97b-151">Comentários</span><span class="sxs-lookup"><span data-stu-id="bf97b-151">Remarks</span></span>

<span data-ttu-id="bf97b-152">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="bf97b-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bf97b-153">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="bf97b-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bf97b-154">Namespace</span><span class="sxs-lookup"><span data-stu-id="bf97b-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bf97b-155">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="bf97b-155">Schema Name</span></span>  <br/> |<span data-ttu-id="bf97b-156">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="bf97b-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="bf97b-157">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="bf97b-157">Validation File</span></span>  <br/> |<span data-ttu-id="bf97b-158">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="bf97b-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bf97b-159">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="bf97b-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="bf97b-160">False</span><span class="sxs-lookup"><span data-stu-id="bf97b-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bf97b-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="bf97b-161">See also</span></span>



- [<span data-ttu-id="bf97b-162">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="bf97b-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

