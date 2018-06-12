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
description: O elemento de FolderId contém o identificador e alterar a chave de uma pasta.
ms.openlocfilehash: 5764a164d5af183b8f313955ace5274dc6023a6a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752335"
---
# <a name="folderid"></a><span data-ttu-id="56b22-103">FolderId</span><span class="sxs-lookup"><span data-stu-id="56b22-103">FolderId</span></span>

<span data-ttu-id="56b22-104">O elemento de **FolderId** contém o identificador e alterar a chave de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="56b22-104">The **FolderId** element contains the identifier and change key of a folder.</span></span> 
  
```XML
<FolderId Id="" ChangeKey="" />
```

 <span data-ttu-id="56b22-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="56b22-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="56b22-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="56b22-106">Attributes and elements</span></span>

<span data-ttu-id="56b22-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="56b22-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="56b22-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="56b22-108">Attributes</span></span>

|<span data-ttu-id="56b22-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="56b22-109">**Attribute**</span></span>|<span data-ttu-id="56b22-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="56b22-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="56b22-111">Id</span><span class="sxs-lookup"><span data-stu-id="56b22-111">Id</span></span>  <br/> |<span data-ttu-id="56b22-112">Contém uma cadeia de caracteres que identifica uma pasta no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="56b22-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="56b22-113">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="56b22-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="56b22-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="56b22-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="56b22-115">Contém uma cadeia de caracteres que identifica uma versão de uma pasta que é identificada pelo atributo Id.</span><span class="sxs-lookup"><span data-stu-id="56b22-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="56b22-116">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="56b22-116">This attribute is optional.</span></span> <span data-ttu-id="56b22-117">Use este atributo para certificar-se de que a versão correta de uma pasta é usada.</span><span class="sxs-lookup"><span data-stu-id="56b22-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="56b22-118">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="56b22-118">Child elements</span></span>

<span data-ttu-id="56b22-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="56b22-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="56b22-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="56b22-120">Parent elements</span></span>

|<span data-ttu-id="56b22-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="56b22-121">**Element**</span></span>|<span data-ttu-id="56b22-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="56b22-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="56b22-123">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="56b22-123">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="56b22-124">Indica a pasta que está programada para ações que usam pastas.</span><span class="sxs-lookup"><span data-stu-id="56b22-124">Indicates the folder that is targeted for actions that use folders.</span></span>  <br/> |
|[<span data-ttu-id="56b22-125">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="56b22-125">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="56b22-126">Representa um evento no qual uma pasta ou um item é copiada.</span><span class="sxs-lookup"><span data-stu-id="56b22-126">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="56b22-127">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="56b22-127">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="56b22-128">Indica a pasta de destino para cópia e mover ações.</span><span class="sxs-lookup"><span data-stu-id="56b22-128">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="56b22-129">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="56b22-129">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> | <span data-ttu-id="56b22-130">Identifica a pasta onde uma nova pasta ou um item é criado.</span><span class="sxs-lookup"><span data-stu-id="56b22-130">Identifies the folder where a new folder or item is created.</span></span>  <br/><br/>  <span data-ttu-id="56b22-131">A seguir estão as expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="56b22-131">The following are the XPath expressions to this element:</span></span><br/>  <br/> `/CreateItem/ParentFolderId` <br/><br/>  `/CreateFolder/ParentFolderId` <br/> |
|[<span data-ttu-id="56b22-132">BaseFolderIds</span><span class="sxs-lookup"><span data-stu-id="56b22-132">BaseFolderIds</span></span>](basefolderids.md) <br/> |<span data-ttu-id="56b22-133">Representa a coleção das pastas que serão extraídos para determinar o conteúdo de uma pasta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="56b22-133">Represents the collection of folders that will be mined to determine the contents of a search folder.</span></span>  <br/> |
|[<span data-ttu-id="56b22-134">Excluir (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="56b22-134">Delete (FolderSync)</span></span>](delete-foldersync.md) <br/> |<span data-ttu-id="56b22-135">Identifica uma única pasta a ser excluído no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="56b22-135">Identifies a single folder to delete in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="56b22-136">Folder</span><span class="sxs-lookup"><span data-stu-id="56b22-136">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="56b22-137">Representa uma pasta em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="56b22-137">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="56b22-138">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="56b22-138">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="56b22-139">Representa uma pasta de calendário em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="56b22-139">Represents a calendar folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="56b22-140">FolderChange</span><span class="sxs-lookup"><span data-stu-id="56b22-140">FolderChange</span></span>](folderchange.md) <br/> |<span data-ttu-id="56b22-141">Representa uma coleção de alterações a serem realizadas em uma única pasta.</span><span class="sxs-lookup"><span data-stu-id="56b22-141">Represents a collection of changes to be performed on a single folder.</span></span>  <br/> <span data-ttu-id="56b22-142">Este é a expressão XPath para esse elemento:`/UpdateFolder/FolderChanges/FolderChange`</span><span class="sxs-lookup"><span data-stu-id="56b22-142">The following is the XPath expression to this element:  `/UpdateFolder/FolderChanges/FolderChange`</span></span> <br/> |
|[<span data-ttu-id="56b22-143">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="56b22-143">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="56b22-144">Representa uma pasta de contato em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="56b22-144">Represents a contact folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="56b22-145">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="56b22-145">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="56b22-146">Representa uma pasta de pesquisa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="56b22-146">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="56b22-147">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="56b22-147">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="56b22-148">Representa uma pasta de tarefa em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="56b22-148">Represents a task folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="56b22-149">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="56b22-149">ToFolderId</span></span>](tofolderid.md) <br/> | <span data-ttu-id="56b22-150">Representa a pasta de destino para um item movido ou copiada ou uma pasta.</span><span class="sxs-lookup"><span data-stu-id="56b22-150">Represents the destination folder for a copied or moved item or folder.</span></span> <br/> <br/>  <span data-ttu-id="56b22-151">A seguir estão as expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="56b22-151">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/MoveFolder/ToFolderId` <br/> <br/> `/CopyFolder/ToFolderId` <br/> <br/> `/MoveItem/ToFolderId`<br/> <br/>  `/CopyItem/ToFolderId` <br/> |
|[<span data-ttu-id="56b22-152">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="56b22-152">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> | <span data-ttu-id="56b22-153">Identifica a pasta de destino para operações de atualização, enviar e crie itens no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="56b22-153">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/><br/>  <span data-ttu-id="56b22-154">A seguir estão as expressões XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="56b22-154">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/CreateItem/SavedItemFolderId` <br/><br/>  `/UpdateItem/SavedItemFolderId` <br/><br/>  `/SendItem/SavedItemFolderId` <br/> |
|[<span data-ttu-id="56b22-155">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="56b22-155">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="56b22-156">Representa a pasta que contém os itens a serem sincronizados.</span><span class="sxs-lookup"><span data-stu-id="56b22-156">Represents the folder that contains the items to synchronize.</span></span>  <br/> |
|[<span data-ttu-id="56b22-157">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="56b22-157">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="56b22-158">Representa o nome de um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="56b22-158">Represents the name of a user configuration object.</span></span> <span data-ttu-id="56b22-159">O nome de objeto de configuração do usuário é o identificador de um objeto de configuração do usuário.</span><span class="sxs-lookup"><span data-stu-id="56b22-159">The user configuration object name is the identifier for a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="56b22-160">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="56b22-160">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="56b22-161">Identifica a ID da pasta que serão copiados para itens de email.</span><span class="sxs-lookup"><span data-stu-id="56b22-161">Identifies the ID of the folder that e-mail items will be copied to.</span></span>  <br/> |
|[<span data-ttu-id="56b22-162">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="56b22-162">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="56b22-163">Identifica a ID da pasta que serão movidos para itens de email.</span><span class="sxs-lookup"><span data-stu-id="56b22-163">Identifies the ID of the folder that e-mail items will be moved to.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="56b22-164">Text value</span><span class="sxs-lookup"><span data-stu-id="56b22-164">Text value</span></span>

<span data-ttu-id="56b22-165">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="56b22-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="56b22-166">Comentários</span><span class="sxs-lookup"><span data-stu-id="56b22-166">Remarks</span></span>

<span data-ttu-id="56b22-167">Todos os elementos de **FolderId** são do tipo **FolderIdType** .</span><span class="sxs-lookup"><span data-stu-id="56b22-167">All **FolderId** elements are of the **FolderIdType** type.</span></span> <span data-ttu-id="56b22-168">O elemento **FolderId** é necessário em cada caso, exceto nos elementos cujo tipo estende o **BaseFolderType** ou onde o elemento **FolderId** é uma parte de uma opção.</span><span class="sxs-lookup"><span data-stu-id="56b22-168">The **FolderId** element is required in every case except in elements whose type extends the **BaseFolderType** or where the **FolderId** element is a part of a choice.</span></span> <span data-ttu-id="56b22-169">Revise o esquema para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="56b22-169">Review the schema for more information.</span></span> 
  
<span data-ttu-id="56b22-170">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="56b22-170">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="56b22-171">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="56b22-171">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="56b22-172">Namespace</span><span class="sxs-lookup"><span data-stu-id="56b22-172">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="56b22-173">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="56b22-173">Schema Name</span></span>  <br/> |<span data-ttu-id="56b22-174">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="56b22-174">Types schema</span></span>  <br/> |
|<span data-ttu-id="56b22-175">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="56b22-175">Validation File</span></span>  <br/> |<span data-ttu-id="56b22-176">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="56b22-176">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="56b22-177">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="56b22-177">Can be Empty</span></span>  <br/> |<span data-ttu-id="56b22-178">False</span><span class="sxs-lookup"><span data-stu-id="56b22-178">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="56b22-179">Ver também</span><span class="sxs-lookup"><span data-stu-id="56b22-179">See also</span></span>

- [<span data-ttu-id="56b22-180">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="56b22-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="56b22-181">Criação de pastas (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="56b22-181">Creating Folders (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

