---
title: Pastas
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
description: O elemento de pastas contém uma matriz das pastas que são usadas nas operações da pasta.
ms.openlocfilehash: e1b9e337f633dbf6fda159c28725d3fb8dcd55a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752338"
---
# <a name="folders"></a><span data-ttu-id="30d02-103">Pastas</span><span class="sxs-lookup"><span data-stu-id="30d02-103">Folders</span></span>

<span data-ttu-id="30d02-104">O elemento de **pastas** contém uma matriz das pastas que são usadas nas operações da pasta.</span><span class="sxs-lookup"><span data-stu-id="30d02-104">The **Folders** element contains an array of folders that are used in folder operations.</span></span> 
  
```xml
<Folders>
   <Folder/>
</Folders>
```

 <span data-ttu-id="30d02-105">**ArrayOfFoldersType** ou **NonEmptyArrayOfFoldersType**</span><span class="sxs-lookup"><span data-stu-id="30d02-105">**ArrayOfFoldersType** or **NonEmptyArrayOfFoldersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="30d02-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="30d02-106">Attributes and elements</span></span>

<span data-ttu-id="30d02-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="30d02-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="30d02-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="30d02-108">Attributes</span></span>

<span data-ttu-id="30d02-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="30d02-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="30d02-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="30d02-110">Child elements</span></span>

|<span data-ttu-id="30d02-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="30d02-111">**Element**</span></span>|<span data-ttu-id="30d02-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="30d02-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30d02-113">Folder</span><span class="sxs-lookup"><span data-stu-id="30d02-113">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="30d02-114">Identifica uma pasta para criar, obter, encontre, sincronizar ou atualizar.</span><span class="sxs-lookup"><span data-stu-id="30d02-114">Identifies a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="30d02-115">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="30d02-115">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="30d02-116">Representa uma pasta que contém principalmente itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="30d02-116">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="30d02-117">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="30d02-117">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="30d02-118">Representa uma pasta de contatos em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="30d02-118">Represents a Contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="30d02-119">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="30d02-119">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="30d02-120">Representa uma pasta de pesquisa contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="30d02-120">Represents a Search folder contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="30d02-121">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="30d02-121">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="30d02-122">Representa uma pasta de tarefas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="30d02-122">Represents a Tasks folder in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="30d02-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="30d02-123">Parent elements</span></span>

|<span data-ttu-id="30d02-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="30d02-124">**Element**</span></span>|<span data-ttu-id="30d02-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="30d02-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30d02-126">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="30d02-126">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md) <br/> |<span data-ttu-id="30d02-127">Contém o status e o resultado de uma única [operação CopyFolder](copyfolder-operation.md) solicitação.</span><span class="sxs-lookup"><span data-stu-id="30d02-127">Contains the status and result of a single [CopyFolder operation](copyfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="30d02-128">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="30d02-128">CreateFolder</span></span>](createfolder.md) <br/> |<span data-ttu-id="30d02-129">Define uma solicitação para criar uma pasta no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="30d02-129">Defines a request to create a folder in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="30d02-130">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="30d02-130">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md) <br/> |<span data-ttu-id="30d02-131">Contém o status e o resultado de uma única [operação CreateFolder](createfolder-operation.md) solicitação.</span><span class="sxs-lookup"><span data-stu-id="30d02-131">Contains the status and result of a single [CreateFolder operation](createfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="30d02-132">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="30d02-132">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md) <br/> |<span data-ttu-id="30d02-133">Contém o status e o resultado de uma única [operação CreateManagedFolder](createmanagedfolder-operation.md) solicitação.</span><span class="sxs-lookup"><span data-stu-id="30d02-133">Contains the status and result of a single [CreateManagedFolder operation](createmanagedfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="30d02-134">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="30d02-134">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md) <br/> |<span data-ttu-id="30d02-135">Contém o status e o resultado de uma solicitação de [operação GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="30d02-135">Contains the status and result of a [GetFolder operation](getfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="30d02-136">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="30d02-136">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md) <br/> |<span data-ttu-id="30d02-137">Contém o status e o resultado de uma solicitação de [operação MoveFolder](movefolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="30d02-137">Contains the status and result of a [MoveFolder operation](movefolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="30d02-138">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="30d02-138">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="30d02-139">Identifica a pasta onde uma nova pasta é criada.</span><span class="sxs-lookup"><span data-stu-id="30d02-139">Identifies the folder where a new folder is created.</span></span>  <br/> |
|[<span data-ttu-id="30d02-140">RootFolder (FindFolderResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="30d02-140">RootFolder (FindFolderResponseMessage)</span></span>](rootfolder-findfolderresponsemessage.md) <br/> |<span data-ttu-id="30d02-141">Contém os resultados de verificação ortográfica de uma pasta raiz única durante uma [operação FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="30d02-141">Contains the results from searching a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="30d02-142">UpdateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="30d02-142">UpdateFolderResponseMessage</span></span>](updatefolderresponsemessage.md) <br/> |<span data-ttu-id="30d02-143">Contém o status e o resultado de uma única [operação UpdateFolder](updatefolder-operation.md) solicitação.</span><span class="sxs-lookup"><span data-stu-id="30d02-143">Contains the status and result of a single [UpdateFolder operation](updatefolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="30d02-144">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="30d02-144">Remarks</span></span>

<span data-ttu-id="30d02-145">Este é um elemento necessário filho do elemento [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .</span><span class="sxs-lookup"><span data-stu-id="30d02-145">This element is a required child element of the [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) element.</span></span> 
  
<span data-ttu-id="30d02-146">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="30d02-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="30d02-147">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="30d02-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30d02-148">Namespace</span><span class="sxs-lookup"><span data-stu-id="30d02-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="30d02-149">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="30d02-149">Schema Name</span></span>  <br/> |<span data-ttu-id="30d02-150">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="30d02-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="30d02-151">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="30d02-151">Validation File</span></span>  <br/> |<span data-ttu-id="30d02-152">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="30d02-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="30d02-153">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="30d02-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="30d02-154">False</span><span class="sxs-lookup"><span data-stu-id="30d02-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="30d02-155">Ver também</span><span class="sxs-lookup"><span data-stu-id="30d02-155">See also</span></span>



[<span data-ttu-id="30d02-156">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="30d02-156">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)

