---
title: Folder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Folder
api_type:
- schema
ms.assetid: 812948d8-c7db-45ce-bb3a-77233a53a974
description: O elemento Folder define uma pasta para criar, obter, localizar, sincronizar ou atualizar.
ms.openlocfilehash: 156813b3f7ecc6a2e1437f473ae1daa76b138e6e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457246"
---
# <a name="folder"></a><span data-ttu-id="392e1-103">Folder</span><span class="sxs-lookup"><span data-stu-id="392e1-103">Folder</span></span>

<span data-ttu-id="392e1-104">O elemento **Folder** define uma pasta para criar, obter, localizar, sincronizar ou atualizar.</span><span class="sxs-lookup"><span data-stu-id="392e1-104">The **Folder** element defines a folder to create, get, find, synchronize, or update.</span></span> 
  
```xml
<Folder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <UnreadCount/>
   <PermissionSet/>
   <EffectiveRights/>
</Folder>
```

 <span data-ttu-id="392e1-105">**FolderType**</span><span class="sxs-lookup"><span data-stu-id="392e1-105">**FolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="392e1-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="392e1-106">Attributes and elements</span></span>

<span data-ttu-id="392e1-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="392e1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="392e1-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="392e1-108">Attributes</span></span>

<span data-ttu-id="392e1-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="392e1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="392e1-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="392e1-110">Child elements</span></span>

|<span data-ttu-id="392e1-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="392e1-111">**Element**</span></span>|<span data-ttu-id="392e1-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="392e1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="392e1-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="392e1-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="392e1-114">Contém o identificador e a chave de alteração de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="392e1-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="392e1-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="392e1-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="392e1-116">Representa o identificador da pasta pai que contém a pasta.</span><span class="sxs-lookup"><span data-stu-id="392e1-116">Represents the identifier of the parent folder that contains the folder.</span></span>  <br/> |
|[<span data-ttu-id="392e1-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="392e1-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="392e1-118">Representa a classe Folder de uma determinada pasta.</span><span class="sxs-lookup"><span data-stu-id="392e1-118">Represents the folder class for a given folder.</span></span>  <br/> |
|[<span data-ttu-id="392e1-119">DisplayName (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="392e1-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="392e1-120">Contém o nome de exibição de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="392e1-120">Contains the display name of a folder.</span></span>  <br/> |
|[<span data-ttu-id="392e1-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="392e1-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="392e1-122">Representa a contagem total de itens em uma determinada pasta.</span><span class="sxs-lookup"><span data-stu-id="392e1-122">Represents the total count of items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="392e1-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="392e1-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="392e1-124">Representa o número de pastas filhas que estão contidas em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="392e1-124">Represents the number of child folders that are contained within a folder.</span></span> <span data-ttu-id="392e1-125">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="392e1-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="392e1-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="392e1-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="392e1-127">Identifica as propriedades estendidas em pastas.</span><span class="sxs-lookup"><span data-stu-id="392e1-127">Identifies extended properties on folders.</span></span>  <br/> |
|[<span data-ttu-id="392e1-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="392e1-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="392e1-129">Contém informações sobre uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="392e1-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="392e1-130">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="392e1-130">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="392e1-131">Representa a contagem de itens não lidos em uma determinada pasta.</span><span class="sxs-lookup"><span data-stu-id="392e1-131">Represents the count of unread items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="392e1-132">PermissionSet (PermissionSettype)</span><span class="sxs-lookup"><span data-stu-id="392e1-132">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="392e1-133">Contém todas as permissões configuradas para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="392e1-133">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="392e1-134">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="392e1-134">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="392e1-135">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="392e1-135">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="392e1-136">Contém os direitos do cliente com base nas configurações de permissão para o item ou pasta.</span><span class="sxs-lookup"><span data-stu-id="392e1-136">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="392e1-137">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="392e1-137">This element is read-only.</span></span> <span data-ttu-id="392e1-138">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="392e1-138">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="392e1-139">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="392e1-139">Parent elements</span></span>

|<span data-ttu-id="392e1-140">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="392e1-140">**Element**</span></span>|<span data-ttu-id="392e1-141">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="392e1-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="392e1-142">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="392e1-142">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="392e1-143">Especifica os dados a serem acrescentados a uma propriedade de pasta durante uma [operação UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="392e1-143">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="392e1-144">Criar (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="392e1-144">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="392e1-145">Identifica uma única pasta a ser criada no armazenamento do cliente local.</span><span class="sxs-lookup"><span data-stu-id="392e1-145">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="392e1-146">Setfolderfield</span><span class="sxs-lookup"><span data-stu-id="392e1-146">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="392e1-147">Representa uma atualização de uma única propriedade em uma pasta em uma [operação UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="392e1-147">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="392e1-148">Atualização (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="392e1-148">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="392e1-149">Identifica uma única pasta a ser atualizada no repositório do cliente local.</span><span class="sxs-lookup"><span data-stu-id="392e1-149">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="392e1-150">Pastas</span><span class="sxs-lookup"><span data-stu-id="392e1-150">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="392e1-151">Contém uma matriz de pastas que são usadas em operações de pasta.</span><span class="sxs-lookup"><span data-stu-id="392e1-151">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="392e1-152">Comentários</span><span class="sxs-lookup"><span data-stu-id="392e1-152">Remarks</span></span>

<span data-ttu-id="392e1-153">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Exchange 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="392e1-153">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="392e1-154">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="392e1-154">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="392e1-155">Namespace</span><span class="sxs-lookup"><span data-stu-id="392e1-155">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="392e1-156">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="392e1-156">Schema Name</span></span>  <br/> |<span data-ttu-id="392e1-157">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="392e1-157">Types schema</span></span>  <br/> |
|<span data-ttu-id="392e1-158">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="392e1-158">Validation File</span></span>  <br/> |<span data-ttu-id="392e1-159">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="392e1-159">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="392e1-160">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="392e1-160">Can be Empty</span></span>  <br/> |<span data-ttu-id="392e1-161">False</span><span class="sxs-lookup"><span data-stu-id="392e1-161">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="392e1-162">Confira também</span><span class="sxs-lookup"><span data-stu-id="392e1-162">See also</span></span>



[<span data-ttu-id="392e1-163">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="392e1-163">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="392e1-164">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="392e1-164">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

