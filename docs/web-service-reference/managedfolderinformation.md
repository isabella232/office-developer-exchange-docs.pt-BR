---
title: ManagedFolderInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ManagedFolderInformation
api_type:
- schema
ms.assetid: dea980eb-8303-47fe-a380-20a8efc9ead6
description: O elemento ManagedFolderInformation contém informações sobre uma pasta personalizada gerenciada.
ms.openlocfilehash: ce15dcb15cccdce253494beefd2f4a2a7a0c0ad8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44450946"
---
# <a name="managedfolderinformation"></a><span data-ttu-id="12b2b-103">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="12b2b-103">ManagedFolderInformation</span></span>

<span data-ttu-id="12b2b-104">O elemento **ManagedFolderInformation** contém informações sobre uma pasta personalizada gerenciada.</span><span class="sxs-lookup"><span data-stu-id="12b2b-104">The **ManagedFolderInformation** element contains information about a managed custom folder.</span></span> 
  
```xml
<ManagedFolderInformation>
   <CanDelete/>
   <CanRenameOrMove/>
   <MustDisplayComment/>
   <HasQuota/>
   <IsManagedFoldersRoot/>
   <ManagedFolderId/>
   <Comment/>
   <StorageQuota/>
   <FolderSize/>
   <HomePage/>
</ManagedFolderInformation>
```

 <span data-ttu-id="12b2b-105">**ManagedFolderInformationType**</span><span class="sxs-lookup"><span data-stu-id="12b2b-105">**ManagedFolderInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="12b2b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="12b2b-106">Attributes and elements</span></span>

<span data-ttu-id="12b2b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="12b2b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="12b2b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="12b2b-108">Attributes</span></span>

<span data-ttu-id="12b2b-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="12b2b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="12b2b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="12b2b-110">Child elements</span></span>

|<span data-ttu-id="12b2b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="12b2b-111">**Element**</span></span>|<span data-ttu-id="12b2b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="12b2b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12b2b-113">CanDelete</span><span class="sxs-lookup"><span data-stu-id="12b2b-113">CanDelete</span></span>](candelete.md) <br/> |<span data-ttu-id="12b2b-114">Indica se uma pasta gerenciada pode ser excluída por um cliente.</span><span class="sxs-lookup"><span data-stu-id="12b2b-114">Indicates whether a managed folder can be deleted by a customer.</span></span>  <br/> |
|[<span data-ttu-id="12b2b-115">CanRenameOrMove</span><span class="sxs-lookup"><span data-stu-id="12b2b-115">CanRenameOrMove</span></span>](canrenameormove.md) <br/> |<span data-ttu-id="12b2b-116">Indica se uma determinada pasta gerenciada pode ser renomeada ou movida pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="12b2b-116">Indicates whether a given managed folder can be renamed or moved by the customer.</span></span>  <br/> |
|[<span data-ttu-id="12b2b-117">MustDisplayComment</span><span class="sxs-lookup"><span data-stu-id="12b2b-117">MustDisplayComment</span></span>](mustdisplaycomment.md) <br/> |<span data-ttu-id="12b2b-118">Indica se o comentário da pasta gerenciada deve ser exibido.</span><span class="sxs-lookup"><span data-stu-id="12b2b-118">Indicates whether the managed folder comment must be displayed.</span></span>  <br/> |
|[<span data-ttu-id="12b2b-119">HasQuota</span><span class="sxs-lookup"><span data-stu-id="12b2b-119">HasQuota</span></span>](hasquota.md) <br/> |<span data-ttu-id="12b2b-120">Indica se a pasta gerenciada tem uma cota.</span><span class="sxs-lookup"><span data-stu-id="12b2b-120">Indicates whether the managed folder has a quota.</span></span>  <br/> |
|[<span data-ttu-id="12b2b-121">IsManagedFoldersRoot</span><span class="sxs-lookup"><span data-stu-id="12b2b-121">IsManagedFoldersRoot</span></span>](ismanagedfoldersroot.md) <br/> |<span data-ttu-id="12b2b-122">Indica se a pasta gerenciada é a raiz de todas as pastas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="12b2b-122">Indicates whether the managed folder is the root for all managed folders.</span></span>  <br/> |
|[<span data-ttu-id="12b2b-123">ManagedFolderId</span><span class="sxs-lookup"><span data-stu-id="12b2b-123">ManagedFolderId</span></span>](managedfolderid.md) <br/> |<span data-ttu-id="12b2b-124">Contém a ID da pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="12b2b-124">Contains the folder ID of the managed folder.</span></span>  <br/> |
|[<span data-ttu-id="12b2b-125">Comment</span><span class="sxs-lookup"><span data-stu-id="12b2b-125">Comment</span></span>](comment.md) <br/> |<span data-ttu-id="12b2b-126">Contém o comentário associado a uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="12b2b-126">Contains the comment that is associated with a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="12b2b-127">StorageQuota</span><span class="sxs-lookup"><span data-stu-id="12b2b-127">StorageQuota</span></span>](storagequota.md) <br/> |<span data-ttu-id="12b2b-128">Descreve a cota de armazenamento da pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="12b2b-128">Describes the storage quota for the managed folder.</span></span>  <br/> |
|[<span data-ttu-id="12b2b-129">FolderSize</span><span class="sxs-lookup"><span data-stu-id="12b2b-129">FolderSize</span></span>](foldersize.md) <br/> |<span data-ttu-id="12b2b-130">Descreve o tamanho total de todo o conteúdo de uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="12b2b-130">Describes the total size of all the contents of a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="12b2b-131">HomePage</span><span class="sxs-lookup"><span data-stu-id="12b2b-131">HomePage</span></span>](homepage.md) <br/> |<span data-ttu-id="12b2b-132">Especifica a URL que será a Home Page padrão para a pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="12b2b-132">Specifies the URL that will be the default home page for the managed folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="12b2b-133">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="12b2b-133">Parent elements</span></span>

|<span data-ttu-id="12b2b-134">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="12b2b-134">**Element**</span></span>|<span data-ttu-id="12b2b-135">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="12b2b-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12b2b-136">Folder</span><span class="sxs-lookup"><span data-stu-id="12b2b-136">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="12b2b-137">Representa uma pasta no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="12b2b-137">Represents a folder in the Exchange store.</span></span> <span data-ttu-id="12b2b-138">Pastas personalizadas gerenciadas só podem ser subpastas da pasta denominada **pastas gerenciadas**.</span><span class="sxs-lookup"><span data-stu-id="12b2b-138">Managed custom folders can only be subfolders of the folder named **Managed Folders**.</span></span>  <br/> |
|[<span data-ttu-id="12b2b-139">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="12b2b-139">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="12b2b-140">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="12b2b-140">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="12b2b-141">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="12b2b-141">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="12b2b-142">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="12b2b-142">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="12b2b-143">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="12b2b-143">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="12b2b-144">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="12b2b-144">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="12b2b-145">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="12b2b-145">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="12b2b-146">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="12b2b-146">Not applicable.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="12b2b-147">Comentários</span><span class="sxs-lookup"><span data-stu-id="12b2b-147">Remarks</span></span>

<span data-ttu-id="12b2b-148">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="12b2b-148">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="12b2b-149">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="12b2b-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="12b2b-150">Namespace</span><span class="sxs-lookup"><span data-stu-id="12b2b-150">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="12b2b-151">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="12b2b-151">Schema name</span></span>  <br/> |<span data-ttu-id="12b2b-152">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="12b2b-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="12b2b-153">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="12b2b-153">Validation file</span></span>  <br/> |<span data-ttu-id="12b2b-154">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="12b2b-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="12b2b-155">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="12b2b-155">Can be empty</span></span>  <br/> |<span data-ttu-id="12b2b-156">False</span><span class="sxs-lookup"><span data-stu-id="12b2b-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="12b2b-157">Confira também</span><span class="sxs-lookup"><span data-stu-id="12b2b-157">See also</span></span>



[<span data-ttu-id="12b2b-158">Operação CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="12b2b-158">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="12b2b-159">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="12b2b-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="12b2b-160">Adicionando pastas gerenciadas</span><span class="sxs-lookup"><span data-stu-id="12b2b-160">Adding Managed Folders</span></span>](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

