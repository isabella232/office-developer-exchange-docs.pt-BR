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
ms.openlocfilehash: 01302f00d84cfff9713e3b188b7799c537fc0629
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751449"
---
# <a name="contactsfolder"></a><span data-ttu-id="e3150-103">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="e3150-103">ContactsFolder</span></span>

<span data-ttu-id="e3150-104">O elemento **ContactsFolder** representa uma pasta de contatos que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e3150-104">The **ContactsFolder** element represents a contacts folder that is contained in a mailbox.</span></span> 
  
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

 <span data-ttu-id="e3150-105">**ContactsFolderType**</span><span class="sxs-lookup"><span data-stu-id="e3150-105">**ContactsFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e3150-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e3150-106">Attributes and elements</span></span>

<span data-ttu-id="e3150-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e3150-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e3150-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e3150-108">Attributes</span></span>

<span data-ttu-id="e3150-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e3150-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e3150-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e3150-110">Child elements</span></span>

|<span data-ttu-id="e3150-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e3150-111">**Element**</span></span>|<span data-ttu-id="e3150-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e3150-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3150-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="e3150-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="e3150-114">Contém o identificador e alterar a chave de uma pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="e3150-114">Contains the identifier and change key of a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="e3150-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="e3150-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="e3150-116">Representa o identificador da pasta pai que contém a pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="e3150-116">Represents the identifier of the parent folder that contains the contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="e3150-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="e3150-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="e3150-118">Representa a classe de pasta para uma pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="e3150-118">Represents the folder class for a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="e3150-119">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="e3150-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="e3150-120">Contém o nome de exibição de uma pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="e3150-120">Contains the display name of a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="e3150-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="e3150-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="e3150-122">Representa a contagem total de itens dentro de uma pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="e3150-122">Represents the total count of items within a contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="e3150-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="e3150-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="e3150-124">Representa o número de pastas filho que está contido dentro de uma pasta de contatos.</span><span class="sxs-lookup"><span data-stu-id="e3150-124">Represents the number of child folders that are contained within a contacts folder.</span></span> <span data-ttu-id="e3150-125">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e3150-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="e3150-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="e3150-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="e3150-127">Identifica as propriedades estendidas em pastas de contatos.</span><span class="sxs-lookup"><span data-stu-id="e3150-127">Identifies extended properties on contacts folders.</span></span>  <br/> |
|[<span data-ttu-id="e3150-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="e3150-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="e3150-129">Contém informações sobre uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="e3150-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="e3150-130">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="e3150-130">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="e3150-131">Contém os direitos do cliente com base nas configurações de permissão para o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="e3150-131">Contains the client's rights based on the permission settings for the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="e3150-132">SharingEffectiveRights (PermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="e3150-132">SharingEffectiveRights (PermissionReadAccessType)</span></span>](sharingeffectiverights-permissionreadaccesstype.md) <br/> |<span data-ttu-id="e3150-133">Indica as permissões que o usuário tem para os dados de contato que está sendo compartilhados.</span><span class="sxs-lookup"><span data-stu-id="e3150-133">Indicates the permissions that the user has for the contact data that is being shared.</span></span>  <br/> |
|[<span data-ttu-id="e3150-134">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="e3150-134">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="e3150-135">Contém todas as permissões configuradas para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="e3150-135">Contains all the configured permissions for a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e3150-136">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e3150-136">Parent elements</span></span>

|<span data-ttu-id="e3150-137">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e3150-137">**Element**</span></span>|<span data-ttu-id="e3150-138">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e3150-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3150-139">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="e3150-139">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="e3150-140">Especifica os dados a serem acrescentados a uma propriedade de pasta durante uma [operação UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="e3150-140">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="e3150-141">Criar (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="e3150-141">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="e3150-142">Identifica uma única pasta para criar no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="e3150-142">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="e3150-143">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="e3150-143">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="e3150-144">Representa uma atualização para uma única propriedade em uma pasta em uma [operação UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="e3150-144">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="e3150-145">Atualização (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="e3150-145">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="e3150-146">Identifica uma única pasta ao atualizar no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="e3150-146">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="e3150-147">Pastas</span><span class="sxs-lookup"><span data-stu-id="e3150-147">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="e3150-148">Contém uma matriz das pastas que são usadas nas operações da pasta.</span><span class="sxs-lookup"><span data-stu-id="e3150-148">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e3150-149">Text value</span><span class="sxs-lookup"><span data-stu-id="e3150-149">Text value</span></span>

<span data-ttu-id="e3150-150">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e3150-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e3150-151">Comentários</span><span class="sxs-lookup"><span data-stu-id="e3150-151">Remarks</span></span>

<span data-ttu-id="e3150-152">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e3150-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e3150-153">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e3150-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e3150-154">Namespace</span><span class="sxs-lookup"><span data-stu-id="e3150-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e3150-155">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e3150-155">Schema Name</span></span>  <br/> |<span data-ttu-id="e3150-156">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="e3150-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="e3150-157">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e3150-157">Validation File</span></span>  <br/> |<span data-ttu-id="e3150-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e3150-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e3150-159">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e3150-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="e3150-160">False</span><span class="sxs-lookup"><span data-stu-id="e3150-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e3150-161">Ver também</span><span class="sxs-lookup"><span data-stu-id="e3150-161">See also</span></span>



- [<span data-ttu-id="e3150-162">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e3150-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

