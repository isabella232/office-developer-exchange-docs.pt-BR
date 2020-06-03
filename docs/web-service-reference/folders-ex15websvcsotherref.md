---
title: Folders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Folders
api_type:
- schema
ms.assetid: 8e71cb44-1df6-444a-add7-0c1363863f65
description: O elemento Folders contém uma matriz de pastas que são usadas em operações de pasta.
ms.openlocfilehash: b087be0501f04390b80458458e7e7ccc24bf27bd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530976"
---
# <a name="folders"></a><span data-ttu-id="6f258-103">Folders</span><span class="sxs-lookup"><span data-stu-id="6f258-103">Folders</span></span>

<span data-ttu-id="6f258-104">O elemento **Folders** contém uma matriz de pastas que são usadas em operações de pasta.</span><span class="sxs-lookup"><span data-stu-id="6f258-104">The **Folders** element contains an array of folders that are used in folder operations.</span></span> 
  
```xml
<Folders>
   <Folder/>
</Folders>
```

```xml
<Folders>
   <ContactsFolder/> 
</Folders>
```

```xml
<Folders>
   <TasksFolder/>
</Folders>
```

```xml
<Folders>
   <CalendarFolder/>
</Folders>
```

```xml
<Folders>
   <SearchFolder/> 
</Folders>
```

<span data-ttu-id="6f258-105">**ArrayOfFoldersType** ou **NonEmptyArrayOfFoldersType**</span><span class="sxs-lookup"><span data-stu-id="6f258-105">**ArrayOfFoldersType** or **NonEmptyArrayOfFoldersType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6f258-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6f258-106">Attributes and elements</span></span>

<span data-ttu-id="6f258-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6f258-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6f258-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="6f258-108">Attributes</span></span>

<span data-ttu-id="6f258-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6f258-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6f258-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6f258-110">Child elements</span></span>

|<span data-ttu-id="6f258-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6f258-111">**Element**</span></span>|<span data-ttu-id="6f258-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6f258-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f258-113">Folder</span><span class="sxs-lookup"><span data-stu-id="6f258-113">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="6f258-114">Identifica uma pasta para criar, obter, localizar, sincronizar ou atualizar.</span><span class="sxs-lookup"><span data-stu-id="6f258-114">Identifies a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="6f258-115">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="6f258-115">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="6f258-116">Representa uma pasta que contém principalmente itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="6f258-116">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="6f258-117">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="6f258-117">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="6f258-118">Representa uma pasta contatos em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6f258-118">Represents a Contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6f258-119">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="6f258-119">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="6f258-120">Representa uma pasta de pesquisa contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6f258-120">Represents a Search folder contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="6f258-121">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="6f258-121">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="6f258-122">Representa uma pasta tarefas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="6f258-122">Represents a Tasks folder in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6f258-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6f258-123">Parent elements</span></span>

|<span data-ttu-id="6f258-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6f258-124">**Element**</span></span>|<span data-ttu-id="6f258-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6f258-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f258-126">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6f258-126">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md) <br/> |<span data-ttu-id="6f258-127">Contém o status e o resultado de uma única solicitação de [operação CopyFolder](copyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6f258-127">Contains the status and result of a single [CopyFolder operation](copyfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="6f258-128">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="6f258-128">CreateFolder</span></span>](createfolder.md) <br/> |<span data-ttu-id="6f258-129">Define uma solicitação para criar uma pasta no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="6f258-129">Defines a request to create a folder in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6f258-130">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6f258-130">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md) <br/> |<span data-ttu-id="6f258-131">Contém o status e o resultado de uma única solicitação de [operação CreateFolder](createfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6f258-131">Contains the status and result of a single [CreateFolder operation](createfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="6f258-132">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6f258-132">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md) <br/> |<span data-ttu-id="6f258-133">Contém o status e o resultado de uma única solicitação de [operação CreateManagedFolder](createmanagedfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6f258-133">Contains the status and result of a single [CreateManagedFolder operation](createmanagedfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="6f258-134">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6f258-134">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md) <br/> |<span data-ttu-id="6f258-135">Contém o status e o resultado de uma solicitação de [operação GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6f258-135">Contains the status and result of a [GetFolder operation](getfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="6f258-136">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6f258-136">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md) <br/> |<span data-ttu-id="6f258-137">Contém o status e o resultado de uma solicitação de [operação MoveFolder](movefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6f258-137">Contains the status and result of a [MoveFolder operation](movefolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="6f258-138">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="6f258-138">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="6f258-139">Identifica a pasta na qual uma nova pasta é criada.</span><span class="sxs-lookup"><span data-stu-id="6f258-139">Identifies the folder where a new folder is created.</span></span>  <br/> |
|[<span data-ttu-id="6f258-140">RootFolder (FindFolderResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="6f258-140">RootFolder (FindFolderResponseMessage)</span></span>](rootfolder-findfolderresponsemessage.md) <br/> |<span data-ttu-id="6f258-141">Contém os resultados da pesquisa de uma única pasta raiz durante uma [operação FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="6f258-141">Contains the results from searching a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="6f258-142">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6f258-142">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md) <br/> |<span data-ttu-id="6f258-143">Contém o status e o resultado de uma única solicitação de [operação UpdateFolder](updatefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="6f258-143">Contains the status and result of a single [UpdateFolder operation](updatefolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6f258-144">Comentários</span><span class="sxs-lookup"><span data-stu-id="6f258-144">Remarks</span></span>

<span data-ttu-id="6f258-145">Este elemento é um elemento filho obrigatório do elemento [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="6f258-145">This element is a required child element of the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span> 
  
<span data-ttu-id="6f258-146">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="6f258-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6f258-147">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6f258-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6f258-148">Namespace</span><span class="sxs-lookup"><span data-stu-id="6f258-148">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6f258-149">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6f258-149">Schema Name</span></span>  <br/> |<span data-ttu-id="6f258-150">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="6f258-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="6f258-151">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6f258-151">Validation File</span></span>  <br/> |<span data-ttu-id="6f258-152">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6f258-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6f258-153">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6f258-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="6f258-154">False</span><span class="sxs-lookup"><span data-stu-id="6f258-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6f258-155">Confira também</span><span class="sxs-lookup"><span data-stu-id="6f258-155">See also</span></span>

- [<span data-ttu-id="6f258-156">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="6f258-156">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)

