---
title: FolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderId
api_type:
- schema
ms.assetid: 00d14e3e-4365-4f21-8f88-eaeea73b9bf7
description: O elemento FolderId contém o identificador e a chave de alteração de uma pasta.
ms.openlocfilehash: 7aa5070fa7a2c51303c7159de04fe277f909a874
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461384"
---
# <a name="folderid"></a><span data-ttu-id="6f9cb-103">FolderId</span><span class="sxs-lookup"><span data-stu-id="6f9cb-103">FolderId</span></span>

<span data-ttu-id="6f9cb-104">O elemento **FolderId** contém o identificador e a chave de alteração de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-104">The **FolderId** element contains the identifier and change key of a folder.</span></span> 
  
```XML
<FolderId Id="" ChangeKey="" />
```

 <span data-ttu-id="6f9cb-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="6f9cb-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6f9cb-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6f9cb-106">Attributes and elements</span></span>

<span data-ttu-id="6f9cb-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6f9cb-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6f9cb-108">Attributes</span></span>

|<span data-ttu-id="6f9cb-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="6f9cb-109">**Attribute**</span></span>|<span data-ttu-id="6f9cb-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6f9cb-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6f9cb-111">Id</span><span class="sxs-lookup"><span data-stu-id="6f9cb-111">Id</span></span>  <br/> |<span data-ttu-id="6f9cb-112">Contém uma cadeia de caracteres que identifica uma pasta no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="6f9cb-113">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="6f9cb-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="6f9cb-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="6f9cb-115">Contém uma cadeia de caracteres que identifica uma versão de uma pasta identificada pelo atributo ID.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="6f9cb-116">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-116">This attribute is optional.</span></span> <span data-ttu-id="6f9cb-117">Use este atributo para certificar-se de que a versão correta de uma pasta é usada.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6f9cb-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6f9cb-118">Child elements</span></span>

<span data-ttu-id="6f9cb-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6f9cb-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6f9cb-120">Parent elements</span></span>

|<span data-ttu-id="6f9cb-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6f9cb-121">**Element**</span></span>|<span data-ttu-id="6f9cb-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6f9cb-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f9cb-123">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="6f9cb-123">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="6f9cb-124">Indica a pasta que é direcionada para ações que usam pastas.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-124">Indicates the folder that is targeted for actions that use folders.</span></span>  <br/> |
|[<span data-ttu-id="6f9cb-125">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="6f9cb-125">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="6f9cb-126">Representa um evento no qual um item ou pasta é copiado.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-126">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="6f9cb-127">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="6f9cb-127">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="6f9cb-128">Indica a pasta de destino para ações de copiar e mover.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-128">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="6f9cb-129">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="6f9cb-129">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> | <span data-ttu-id="6f9cb-130">Identifica a pasta onde uma nova pasta ou item é criado.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-130">Identifies the folder where a new folder or item is created.</span></span>  <br/><br/>  <span data-ttu-id="6f9cb-131">A seguir estão as expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="6f9cb-131">The following are the XPath expressions to this element:</span></span><br/>  <br/> `/CreateItem/ParentFolderId` <br/><br/>  `/CreateFolder/ParentFolderId` <br/> |
|[<span data-ttu-id="6f9cb-132">BaseFolderIds</span><span class="sxs-lookup"><span data-stu-id="6f9cb-132">BaseFolderIds</span></span>](basefolderids.md) <br/> |<span data-ttu-id="6f9cb-133">Representa a coleção de pastas que será minada para determinar o conteúdo de uma pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-133">Represents the collection of folders that will be mined to determine the contents of a search folder.</span></span>  <br/> |
|[<span data-ttu-id="6f9cb-134">Excluir (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="6f9cb-134">Delete (FolderSync)</span></span>](delete-foldersync.md) <br/> |<span data-ttu-id="6f9cb-135">Identifica uma única pasta a ser excluída no repositório do cliente local.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-135">Identifies a single folder to delete in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="6f9cb-136">Folder</span><span class="sxs-lookup"><span data-stu-id="6f9cb-136">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="6f9cb-137">Representa uma pasta em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-137">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6f9cb-138">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="6f9cb-138">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="6f9cb-139">Representa uma pasta de calendário em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-139">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6f9cb-140">FolderChange</span><span class="sxs-lookup"><span data-stu-id="6f9cb-140">FolderChange</span></span>](folderchange.md) <br/> |<span data-ttu-id="6f9cb-141">Representa uma coleção de alterações a serem realizadas em uma única pasta.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-141">Represents a collection of changes to be performed on a single folder.</span></span>  <br/> <span data-ttu-id="6f9cb-142">A seguir está a expressão XPath para este elemento:`/UpdateFolder/FolderChanges/FolderChange`</span><span class="sxs-lookup"><span data-stu-id="6f9cb-142">The following is the XPath expression to this element:  `/UpdateFolder/FolderChanges/FolderChange`</span></span> <br/> |
|[<span data-ttu-id="6f9cb-143">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="6f9cb-143">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="6f9cb-144">Representa uma pasta de contatos em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-144">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6f9cb-145">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="6f9cb-145">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="6f9cb-146">Representa uma pasta de pesquisa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-146">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6f9cb-147">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="6f9cb-147">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="6f9cb-148">Representa uma pasta de tarefas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-148">Represents a task folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6f9cb-149">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="6f9cb-149">ToFolderId</span></span>](tofolderid.md) <br/> | <span data-ttu-id="6f9cb-150">Representa a pasta de destino para uma pasta ou item copiado ou movido.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-150">Represents the destination folder for a copied or moved item or folder.</span></span> <br/> <br/>  <span data-ttu-id="6f9cb-151">A seguir estão as expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="6f9cb-151">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/MoveFolder/ToFolderId` <br/> <br/> `/CopyFolder/ToFolderId` <br/> <br/> `/MoveItem/ToFolderId`<br/> <br/>  `/CopyItem/ToFolderId` <br/> |
|[<span data-ttu-id="6f9cb-152">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="6f9cb-152">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> | <span data-ttu-id="6f9cb-153">Identifica a pasta de destino para operações que atualizam, enviam e criam itens no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-153">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/><br/>  <span data-ttu-id="6f9cb-154">A seguir estão as expressões XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="6f9cb-154">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/CreateItem/SavedItemFolderId` <br/><br/>  `/UpdateItem/SavedItemFolderId` <br/><br/>  `/SendItem/SavedItemFolderId` <br/> |
|[<span data-ttu-id="6f9cb-155">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="6f9cb-155">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="6f9cb-156">Representa a pasta que contém os itens a serem sincronizados.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-156">Represents the folder that contains the items to synchronize.</span></span>  <br/> |
|[<span data-ttu-id="6f9cb-157">Userconfigurationname</span><span class="sxs-lookup"><span data-stu-id="6f9cb-157">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="6f9cb-158">Representa o nome de um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-158">Represents the name of a user configuration object.</span></span> <span data-ttu-id="6f9cb-159">O nome do objeto de configuração do usuário é o identificador de um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-159">The user configuration object name is the identifier for a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="6f9cb-160">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="6f9cb-160">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="6f9cb-161">Identifica a ID da pasta para a qual os itens de email serão copiados.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-161">Identifies the ID of the folder that e-mail items will be copied to.</span></span>  <br/> |
|[<span data-ttu-id="6f9cb-162">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="6f9cb-162">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="6f9cb-163">Identifica a ID da pasta para a qual os itens de email serão movidos.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-163">Identifies the ID of the folder that e-mail items will be moved to.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6f9cb-164">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="6f9cb-164">Text value</span></span>

<span data-ttu-id="6f9cb-165">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6f9cb-166">Comentários</span><span class="sxs-lookup"><span data-stu-id="6f9cb-166">Remarks</span></span>

<span data-ttu-id="6f9cb-167">Todos os elementos **FolderId** são do tipo **FolderIdType** .</span><span class="sxs-lookup"><span data-stu-id="6f9cb-167">All **FolderId** elements are of the **FolderIdType** type.</span></span> <span data-ttu-id="6f9cb-168">O elemento **FolderId** é necessário em todos os casos, exceto nos elementos cujo tipo estende o **BaseFolderType** ou onde o elemento **FolderId** faz parte de uma opção.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-168">The **FolderId** element is required in every case except in elements whose type extends the **BaseFolderType** or where the **FolderId** element is a part of a choice.</span></span> <span data-ttu-id="6f9cb-169">Revise o esquema para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-169">Review the schema for more information.</span></span> 
  
<span data-ttu-id="6f9cb-170">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6f9cb-170">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6f9cb-171">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6f9cb-171">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6f9cb-172">Namespace</span><span class="sxs-lookup"><span data-stu-id="6f9cb-172">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6f9cb-173">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6f9cb-173">Schema Name</span></span>  <br/> |<span data-ttu-id="6f9cb-174">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="6f9cb-174">Types schema</span></span>  <br/> |
|<span data-ttu-id="6f9cb-175">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6f9cb-175">Validation File</span></span>  <br/> |<span data-ttu-id="6f9cb-176">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6f9cb-176">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6f9cb-177">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6f9cb-177">Can be Empty</span></span>  <br/> |<span data-ttu-id="6f9cb-178">False</span><span class="sxs-lookup"><span data-stu-id="6f9cb-178">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6f9cb-179">Confira também</span><span class="sxs-lookup"><span data-stu-id="6f9cb-179">See also</span></span>

- [<span data-ttu-id="6f9cb-180">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6f9cb-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="6f9cb-181">Criando pastas (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="6f9cb-181">Creating Folders (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

