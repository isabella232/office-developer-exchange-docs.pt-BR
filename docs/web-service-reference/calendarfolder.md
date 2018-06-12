---
title: CalendarFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarFolder
api_type:
- schema
ms.assetid: 48687a78-e757-4c04-9641-bf4302c6b565
description: O elemento CalendarFolder representa uma pasta que contém principalmente itens de calendário.
ms.openlocfilehash: 7dc90706eb45eb4617a68b9fdcf37669921af966
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751351"
---
# <a name="calendarfolder"></a><span data-ttu-id="a9c3d-103">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="a9c3d-103">CalendarFolder</span></span>

<span data-ttu-id="a9c3d-104">O elemento **CalendarFolder** representa uma pasta que contém principalmente itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="a9c3d-104">The **CalendarFolder** element represents a folder that primarily contains calendar items.</span></span> 
  
```xml
<CalendarFolder>
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
</CalendarFolder>
```

 <span data-ttu-id="a9c3d-105">**CalendarFolderType**</span><span class="sxs-lookup"><span data-stu-id="a9c3d-105">**CalendarFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a9c3d-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a9c3d-106">Attributes and elements</span></span>

<span data-ttu-id="a9c3d-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a9c3d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a9c3d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a9c3d-108">Attributes</span></span>

<span data-ttu-id="a9c3d-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a9c3d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a9c3d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a9c3d-110">Child elements</span></span>

|<span data-ttu-id="a9c3d-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a9c3d-111">**Element**</span></span>|<span data-ttu-id="a9c3d-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a9c3d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a9c3d-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="a9c3d-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="a9c3d-114">Contém o identificador e alterar a chave de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="a9c3d-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="a9c3d-115">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="a9c3d-115">ParentFolderId</span></span>](parentfolderid.md) <br/> |<span data-ttu-id="a9c3d-116">Representa o identificador da pasta pai que contém a pasta.</span><span class="sxs-lookup"><span data-stu-id="a9c3d-116">Represents the identifier of the parent folder that contains the folder.</span></span>  <br/> |
|[<span data-ttu-id="a9c3d-117">FolderClass</span><span class="sxs-lookup"><span data-stu-id="a9c3d-117">FolderClass</span></span>](folderclass.md) <br/> |<span data-ttu-id="a9c3d-118">Representa a classe de pasta para uma determinada pasta.</span><span class="sxs-lookup"><span data-stu-id="a9c3d-118">Represents the folder class for a given folder.</span></span>  <br/> |
|[<span data-ttu-id="a9c3d-119">DisplayName (string)</span><span class="sxs-lookup"><span data-stu-id="a9c3d-119">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="a9c3d-120">Contém o nome de exibição de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="a9c3d-120">Contains the display name of a folder.</span></span>  <br/> |
|[<span data-ttu-id="a9c3d-121">TotalCount</span><span class="sxs-lookup"><span data-stu-id="a9c3d-121">TotalCount</span></span>](totalcount.md) <br/> |<span data-ttu-id="a9c3d-122">Representa a contagem total de itens dentro de uma determinada pasta.</span><span class="sxs-lookup"><span data-stu-id="a9c3d-122">Represents the total count of items within a given folder.</span></span>  <br/> |
|[<span data-ttu-id="a9c3d-123">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="a9c3d-123">ChildFolderCount</span></span>](childfoldercount.md) <br/> |<span data-ttu-id="a9c3d-124">Representa o número de pastas filho que está contido dentro de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="a9c3d-124">Represents the number of child folders that are contained within a folder.</span></span> <span data-ttu-id="a9c3d-125">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a9c3d-125">This property is read-only.</span></span>  <br/> |
|[<span data-ttu-id="a9c3d-126">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="a9c3d-126">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="a9c3d-127">Identifica as propriedades estendidas de pastas.</span><span class="sxs-lookup"><span data-stu-id="a9c3d-127">Identifies extended properties on folders.</span></span>  <br/> |
|[<span data-ttu-id="a9c3d-128">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="a9c3d-128">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="a9c3d-129">Contém informações sobre uma pasta gerenciada.</span><span class="sxs-lookup"><span data-stu-id="a9c3d-129">Contains information about a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="a9c3d-130">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="a9c3d-130">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="a9c3d-131">Contém os direitos do cliente com base nas configurações de permissão para o item ou a pasta.</span><span class="sxs-lookup"><span data-stu-id="a9c3d-131">Contains the client's rights based on the permission settings for the item or folder.</span></span> <span data-ttu-id="a9c3d-132">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a9c3d-132">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="a9c3d-133">SharingEffectiveRights (CalendarPermissionReadAccessType)</span><span class="sxs-lookup"><span data-stu-id="a9c3d-133">SharingEffectiveRights (CalendarPermissionReadAccessType)</span></span>](sharingeffectiverights-calendarpermissionreadaccesstype.md) <br/> |<span data-ttu-id="a9c3d-134">Indica as permissões que o usuário tem para os dados do calendário que está sendo compartilhados.</span><span class="sxs-lookup"><span data-stu-id="a9c3d-134">Indicates the permissions that the user has for the calendar data that is being shared.</span></span>  <br/> |
|[<span data-ttu-id="a9c3d-135">PermissionSet (CalendarPermissionSetType)</span><span class="sxs-lookup"><span data-stu-id="a9c3d-135">PermissionSet (CalendarPermissionSetType)</span></span>](permissionset-calendarpermissionsettype.md) <br/> |<span data-ttu-id="a9c3d-136">Contém todas as permissões configuradas para uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="a9c3d-136">Contains all the configured permissions for a calendar folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a9c3d-137">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a9c3d-137">Parent elements</span></span>

|<span data-ttu-id="a9c3d-138">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a9c3d-138">**Element**</span></span>|<span data-ttu-id="a9c3d-139">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a9c3d-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a9c3d-140">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="a9c3d-140">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="a9c3d-141">Especifica os dados a serem acrescentados a uma propriedade de pasta durante uma [operação UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="a9c3d-141">Specifies data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="a9c3d-142">Criar (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="a9c3d-142">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="a9c3d-143">Identifica uma única pasta para criar no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="a9c3d-143">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="a9c3d-144">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="a9c3d-144">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="a9c3d-145">Representa uma atualização para uma única propriedade em uma pasta em uma [operação UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="a9c3d-145">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="a9c3d-146">Atualização (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="a9c3d-146">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="a9c3d-147">Identifica uma única pasta ao atualizar no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="a9c3d-147">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="a9c3d-148">Pastas</span><span class="sxs-lookup"><span data-stu-id="a9c3d-148">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="a9c3d-149">Contém uma matriz das pastas que são usadas nas operações da pasta.</span><span class="sxs-lookup"><span data-stu-id="a9c3d-149">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a9c3d-150">Comentários</span><span class="sxs-lookup"><span data-stu-id="a9c3d-150">Remarks</span></span>

<span data-ttu-id="a9c3d-151">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a9c3d-151">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a9c3d-152">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a9c3d-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a9c3d-153">Namespace</span><span class="sxs-lookup"><span data-stu-id="a9c3d-153">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a9c3d-154">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a9c3d-154">Schema Name</span></span>  <br/> |<span data-ttu-id="a9c3d-155">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="a9c3d-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="a9c3d-156">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a9c3d-156">Validation File</span></span>  <br/> |<span data-ttu-id="a9c3d-157">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a9c3d-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a9c3d-158">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a9c3d-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="a9c3d-159">False</span><span class="sxs-lookup"><span data-stu-id="a9c3d-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a9c3d-160">Ver também</span><span class="sxs-lookup"><span data-stu-id="a9c3d-160">See also</span></span>



- [<span data-ttu-id="a9c3d-161">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a9c3d-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

