---
title: TasksFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TasksFolder
api_type:
- schema
ms.assetid: 5a9a4612-8064-4986-b467-c44f268c64df
description: O elemento TasksFolder representa uma pasta de tarefas que está contida em uma caixa de correio.
ms.openlocfilehash: b2151c68519a6ff15fbc74b48fc93a7e06af9e76
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837698"
---
# <a name="tasksfolder"></a><span data-ttu-id="97d92-103">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="97d92-103">TasksFolder</span></span>

<span data-ttu-id="97d92-104">O elemento **TasksFolder** representa uma pasta de tarefas que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="97d92-104">The **TasksFolder** element represents a Tasks folder that is contained in a mailbox.</span></span> 
  
```xml
<TasksFolder>
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
</TasksFolder>
```

<span data-ttu-id="97d92-105">**TasksFolderType**</span><span class="sxs-lookup"><span data-stu-id="97d92-105">**TasksFolderType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="97d92-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="97d92-106">Attributes and elements</span></span>

<span data-ttu-id="97d92-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="97d92-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97d92-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="97d92-108">Attributes</span></span>

<span data-ttu-id="97d92-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="97d92-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="97d92-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="97d92-110">Child elements</span></span>

|<span data-ttu-id="97d92-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="97d92-111">**Element**</span></span>|<span data-ttu-id="97d92-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="97d92-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97d92-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="97d92-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="97d92-114">Contém o identificador e alterar a chave de uma pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="97d92-114">Contains the identifier and change key of a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="97d92-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="97d92-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="97d92-116">Representa o identificador da pasta pai que contém a pasta tarefas.</span><span class="sxs-lookup"><span data-stu-id="97d92-116">Represents the identifier of the parent folder that contains the Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="97d92-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="97d92-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="97d92-118">Representa a classe de pasta para uma pasta tarefas.</span><span class="sxs-lookup"><span data-stu-id="97d92-118">Represents the folder class for a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="97d92-119">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="97d92-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="97d92-120">Contém o nome de exibição de uma pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="97d92-120">Contains the display name of a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="97d92-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="97d92-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="97d92-122">Representa a contagem total de itens dentro de uma pasta tarefas.</span><span class="sxs-lookup"><span data-stu-id="97d92-122">Represents the total count of items within a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="97d92-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="97d92-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="97d92-124">Representa o número de pastas filho que está contido dentro de uma pasta tarefas.</span><span class="sxs-lookup"><span data-stu-id="97d92-124">Represents the number of child folders that are contained within a Tasks folder.</span></span> <span data-ttu-id="97d92-125">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="97d92-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="97d92-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="97d92-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="97d92-127">Identifica as propriedades estendidas em uma pasta tarefas.</span><span class="sxs-lookup"><span data-stu-id="97d92-127">Identifies extended properties on a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="97d92-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="97d92-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="97d92-129">Contém informações sobre uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="97d92-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="97d92-130">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="97d92-130">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="97d92-131">Representa a contagem de itens não lidos dentro de uma pasta de tarefas.</span><span class="sxs-lookup"><span data-stu-id="97d92-131">Represents the count of unread items within a Tasks folder.</span></span>  <br/> |
|[<span data-ttu-id="97d92-132">PermissionSet (PermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="97d92-132">PermissionSet (PermissionSetType)</span></span>](permissionset-permissionsettype.md) <br/> |<span data-ttu-id="97d92-133">Contém todas as permissões configuradas para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="97d92-133">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="97d92-134">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="97d92-134">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="97d92-135">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="97d92-135">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="97d92-136">Contém os direitos do cliente com base nas configurações de permissão para o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="97d92-136">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="97d92-137">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="97d92-137">This element is read-only.</span></span> <span data-ttu-id="97d92-138">Este elemento foi introduzido no Microsoft Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="97d92-138">This element was introduced in Microsoft Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="97d92-139">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="97d92-139">Parent elements</span></span>

|<span data-ttu-id="97d92-140">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="97d92-140">**Element**</span></span>|<span data-ttu-id="97d92-141">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="97d92-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97d92-142">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="97d92-142">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="97d92-143">Especifica os dados a serem acrescentados a uma propriedade de pasta durante uma [operação UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="97d92-143">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="97d92-144">Criar (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="97d92-144">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="97d92-145">Identifica uma única pasta para criar no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="97d92-145">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="97d92-146">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="97d92-146">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="97d92-147">Representa uma atualização para uma única propriedade em uma pasta em uma [operação UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="97d92-147">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="97d92-148">Atualização (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="97d92-148">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="97d92-149">Identifica uma única pasta ao atualizar no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="97d92-149">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="97d92-150">Pastas</span><span class="sxs-lookup"><span data-stu-id="97d92-150">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="97d92-151">Contém uma matriz das pastas que são usadas nas operações da pasta.</span><span class="sxs-lookup"><span data-stu-id="97d92-151">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="97d92-152">Comentários</span><span class="sxs-lookup"><span data-stu-id="97d92-152">Remarks</span></span>

<span data-ttu-id="97d92-153">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="97d92-153">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97d92-154">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="97d92-154">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97d92-155">Namespace</span><span class="sxs-lookup"><span data-stu-id="97d92-155">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="97d92-156">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="97d92-156">Schema Name</span></span>  <br/> |<span data-ttu-id="97d92-157">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="97d92-157">Types schema</span></span>  <br/> |
|<span data-ttu-id="97d92-158">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="97d92-158">Validation File</span></span>  <br/> |<span data-ttu-id="97d92-159">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="97d92-159">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="97d92-160">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="97d92-160">Can be Empty</span></span>  <br/> |<span data-ttu-id="97d92-161">False</span><span class="sxs-lookup"><span data-stu-id="97d92-161">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="97d92-162">Ver também</span><span class="sxs-lookup"><span data-stu-id="97d92-162">See also</span></span>

- [<span data-ttu-id="97d92-163">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="97d92-163">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

