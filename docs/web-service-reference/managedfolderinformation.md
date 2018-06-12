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
ms.openlocfilehash: ef46e2e0db440de2a8acae8316ce98d11bd6710e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824341"
---
# <a name="managedfolderinformation"></a><span data-ttu-id="7a859-103">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="7a859-103">ManagedFolderInformation</span></span>

<span data-ttu-id="7a859-104">O elemento **ManagedFolderInformation** contém informações sobre uma pasta personalizada gerenciada.</span><span class="sxs-lookup"><span data-stu-id="7a859-104">The **ManagedFolderInformation** element contains information about a managed custom folder.</span></span> 
  
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

 <span data-ttu-id="7a859-105">**ManagedFolderInformationType**</span><span class="sxs-lookup"><span data-stu-id="7a859-105">**ManagedFolderInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7a859-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="7a859-106">Attributes and elements</span></span>

<span data-ttu-id="7a859-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7a859-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a859-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7a859-108">Attributes</span></span>

<span data-ttu-id="7a859-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="7a859-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a859-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7a859-110">Child elements</span></span>

|<span data-ttu-id="7a859-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7a859-111">**Element**</span></span>|<span data-ttu-id="7a859-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7a859-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a859-113">CanDelete</span><span class="sxs-lookup"><span data-stu-id="7a859-113">CanDelete</span></span>](candelete.md) <br/> |<span data-ttu-id="7a859-114">Indica se uma pasta gerenciada pode ser excluída por um cliente.</span><span class="sxs-lookup"><span data-stu-id="7a859-114">Indicates whether a managed folder can be deleted by a customer.</span></span>  <br/> |
|[<span data-ttu-id="7a859-115">CanRenameOrMove</span><span class="sxs-lookup"><span data-stu-id="7a859-115">CanRenameOrMove</span></span>](canrenameormove.md) <br/> |<span data-ttu-id="7a859-116">Indica se uma determinada pasta gerenciada pode ser renomeada ou movida pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7a859-116">Indicates whether a given managed folder can be renamed or moved by the customer.</span></span>  <br/> |
|[<span data-ttu-id="7a859-117">MustDisplayComment</span><span class="sxs-lookup"><span data-stu-id="7a859-117">MustDisplayComment</span></span>](mustdisplaycomment.md) <br/> |<span data-ttu-id="7a859-118">Indica se o comentário de pasta gerenciada deve ser exibido.</span><span class="sxs-lookup"><span data-stu-id="7a859-118">Indicates whether the managed folder comment must be displayed.</span></span>  <br/> |
|[<span data-ttu-id="7a859-119">HasQuota</span><span class="sxs-lookup"><span data-stu-id="7a859-119">HasQuota</span></span>](hasquota.md) <br/> |<span data-ttu-id="7a859-120">Indica se a pasta gerenciada tem uma cota.</span><span class="sxs-lookup"><span data-stu-id="7a859-120">Indicates whether the managed folder has a quota.</span></span>  <br/> |
|[<span data-ttu-id="7a859-121">IsManagedFoldersRoot</span><span class="sxs-lookup"><span data-stu-id="7a859-121">IsManagedFoldersRoot</span></span>](ismanagedfoldersroot.md) <br/> |<span data-ttu-id="7a859-122">Indica se a pasta gerenciada é a raiz para todas as pastas gerenciadas.</span><span class="sxs-lookup"><span data-stu-id="7a859-122">Indicates whether the managed folder is the root for all managed folders.</span></span>  <br/> |
|[<span data-ttu-id="7a859-123">ManagedFolderId</span><span class="sxs-lookup"><span data-stu-id="7a859-123">ManagedFolderId</span></span>](managedfolderid.md) <br/> |<span data-ttu-id="7a859-124">Contém a ID de pasta da pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="7a859-124">Contains the folder ID of the managed folder.</span></span>  <br/> |
|[<span data-ttu-id="7a859-125">Comment</span><span class="sxs-lookup"><span data-stu-id="7a859-125">Comment</span></span>](comment.md) <br/> |<span data-ttu-id="7a859-126">Contém o comentário associado uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="7a859-126">Contains the comment that is associated with a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="7a859-127">StorageQuota</span><span class="sxs-lookup"><span data-stu-id="7a859-127">StorageQuota</span></span>](storagequota.md) <br/> |<span data-ttu-id="7a859-128">Descreve a cota de armazenamento para a pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="7a859-128">Describes the storage quota for the managed folder.</span></span>  <br/> |
|[<span data-ttu-id="7a859-129">FolderSize</span><span class="sxs-lookup"><span data-stu-id="7a859-129">FolderSize</span></span>](foldersize.md) <br/> |<span data-ttu-id="7a859-130">Descreve o tamanho total de todo o conteúdo de uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="7a859-130">Describes the total size of all the contents of a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="7a859-131">Home page</span><span class="sxs-lookup"><span data-stu-id="7a859-131">HomePage</span></span>](homepage.md) <br/> |<span data-ttu-id="7a859-132">Especifica a URL que será a home page padrão para a pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="7a859-132">Specifies the URL that will be the default home page for the managed folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7a859-133">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7a859-133">Parent elements</span></span>

|<span data-ttu-id="7a859-134">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7a859-134">**Element**</span></span>|<span data-ttu-id="7a859-135">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7a859-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a859-136">Folder</span><span class="sxs-lookup"><span data-stu-id="7a859-136">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="7a859-137">Representa uma pasta no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7a859-137">Represents a folder in the Exchange store.</span></span> <span data-ttu-id="7a859-138">Pastas personalizadas gerenciadas só podem ser subpastas da pasta denominada **Pastas gerenciadas**.</span><span class="sxs-lookup"><span data-stu-id="7a859-138">Managed custom folders can only be subfolders of the folder named **Managed Folders**.</span></span>  <br/> |
|[<span data-ttu-id="7a859-139">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="7a859-139">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="7a859-140">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="7a859-140">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="7a859-141">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="7a859-141">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="7a859-142">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="7a859-142">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="7a859-143">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="7a859-143">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="7a859-144">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="7a859-144">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="7a859-145">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="7a859-145">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="7a859-146">Não aplicável.</span><span class="sxs-lookup"><span data-stu-id="7a859-146">Not applicable.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7a859-147">Comentários</span><span class="sxs-lookup"><span data-stu-id="7a859-147">Remarks</span></span>

<span data-ttu-id="7a859-148">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="7a859-148">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7a859-149">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="7a859-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a859-150">Namespace</span><span class="sxs-lookup"><span data-stu-id="7a859-150">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7a859-151">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7a859-151">Schema name</span></span>  <br/> |<span data-ttu-id="7a859-152">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="7a859-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="7a859-153">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7a859-153">Validation file</span></span>  <br/> |<span data-ttu-id="7a859-154">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7a859-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7a859-155">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="7a859-155">Can be empty</span></span>  <br/> |<span data-ttu-id="7a859-156">False</span><span class="sxs-lookup"><span data-stu-id="7a859-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7a859-157">Ver também</span><span class="sxs-lookup"><span data-stu-id="7a859-157">See also</span></span>



[<span data-ttu-id="7a859-158">Operação CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="7a859-158">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="7a859-159">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7a859-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="7a859-160">Adicionando pastas gerenciadas</span><span class="sxs-lookup"><span data-stu-id="7a859-160">Adding Managed Folders</span></span>](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

