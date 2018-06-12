---
title: CalendarPermission
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarPermission
api_type:
- schema
ms.assetid: 3aafb221-a04b-41f6-804e-eda810f1ba28
description: O elemento de CalendarPermission define o que um usuário tem acesso a uma pasta de calendário. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 7f6ceb6895add3fdd82cdd595463b3a80db822e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751359"
---
# <a name="calendarpermission"></a><span data-ttu-id="4321d-104">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="4321d-104">CalendarPermission</span></span>

<span data-ttu-id="4321d-105">O elemento de **CalendarPermission** define o que um usuário tem acesso a uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="4321d-105">The **CalendarPermission** element defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="4321d-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="4321d-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<Permission>
   <CalendarPermissionLevel/>
   <CanCreateItems/>
   <CanCreateSubfolders/>
   <IsFolderOwner/>
   <IsFolderVisible/>
   <IsFolderContact/>
   <EditItems/>
   <DeleteItems/>
   <ReadItems/>
   <UserId/>
</Permission>
```

 <span data-ttu-id="4321d-107">**CalendarPermissionType**</span><span class="sxs-lookup"><span data-stu-id="4321d-107">**CalendarPermissionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4321d-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="4321d-108">Attributes and elements</span></span>

<span data-ttu-id="4321d-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4321d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4321d-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="4321d-110">Attributes</span></span>

<span data-ttu-id="4321d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="4321d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4321d-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4321d-112">Child elements</span></span>

|<span data-ttu-id="4321d-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4321d-113">**Element**</span></span>|<span data-ttu-id="4321d-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4321d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4321d-115">CalendarPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="4321d-115">CalendarPermissionLevel</span></span>](calendarpermissionlevel.md) <br/> |<span data-ttu-id="4321d-116">Representa o nível de permissão que um usuário tem em uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="4321d-116">Represents the permission level that a user has on a Calendar folder.</span></span> <span data-ttu-id="4321d-117">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="4321d-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="4321d-118">CanCreateItems</span><span class="sxs-lookup"><span data-stu-id="4321d-118">CanCreateItems</span></span>](cancreateitems.md) <br/> |<span data-ttu-id="4321d-119">Indica se um usuário tem permissão para criar itens em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="4321d-119">Indicates whether a user has permission to create items in a folder.</span></span> <span data-ttu-id="4321d-120">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="4321d-120">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="4321d-121">CanCreateSubFolders</span><span class="sxs-lookup"><span data-stu-id="4321d-121">CanCreateSubFolders</span></span>](cancreatesubfolders.md) <br/> |<span data-ttu-id="4321d-122">Indica se um usuário tem permissão para criar subpastas em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="4321d-122">Indicates whether a user has permission to create subfolders in a folder.</span></span> <span data-ttu-id="4321d-123">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="4321d-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="4321d-124">DeleteItems</span><span class="sxs-lookup"><span data-stu-id="4321d-124">DeleteItems</span></span>](deleteitems.md) <br/> |<span data-ttu-id="4321d-125">Indica se um usuário tem permissão para excluir itens em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="4321d-125">Indicates whether a user has permission to delete items in a folder.</span></span> <span data-ttu-id="4321d-126">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="4321d-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="4321d-127">EditItems</span><span class="sxs-lookup"><span data-stu-id="4321d-127">EditItems</span></span>](edititems.md) <br/> |<span data-ttu-id="4321d-128">Indica se um usuário tem permissão para editar itens em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="4321d-128">Indicates whether a user has permission to edit items in a folder.</span></span> <span data-ttu-id="4321d-129">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="4321d-129">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="4321d-130">IsFolderContact</span><span class="sxs-lookup"><span data-stu-id="4321d-130">IsFolderContact</span></span>](isfoldercontact.md) <br/> |<span data-ttu-id="4321d-131">Indica se um usuário é um contato para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="4321d-131">Indicates whether a user is a contact for a folder.</span></span> <span data-ttu-id="4321d-132">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="4321d-132">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="4321d-133">IsFolderOwner</span><span class="sxs-lookup"><span data-stu-id="4321d-133">IsFolderOwner</span></span>](isfolderowner.md) <br/> |<span data-ttu-id="4321d-134">Indica se um usuário é o proprietário de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="4321d-134">Indicates whether a user is the owner of a folder.</span></span> <span data-ttu-id="4321d-135">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="4321d-135">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="4321d-136">IsFolderVisible</span><span class="sxs-lookup"><span data-stu-id="4321d-136">IsFolderVisible</span></span>](isfoldervisible.md) <br/> |<span data-ttu-id="4321d-137">Indica se um usuário pode exibir uma pasta.</span><span class="sxs-lookup"><span data-stu-id="4321d-137">Indicates whether a user can view a folder.</span></span> <span data-ttu-id="4321d-138">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="4321d-138">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="4321d-139">ReadItems (CalendarPermissionType)</span><span class="sxs-lookup"><span data-stu-id="4321d-139">ReadItems (CalendarPermissionType)</span></span>](readitems-calendarpermissiontype.md) <br/> |<span data-ttu-id="4321d-140">Indica se um usuário tem permissão para ler itens dentro de uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="4321d-140">Indicates whether a user has permission to read items within a calendar folder.</span></span> <span data-ttu-id="4321d-141">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="4321d-141">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="4321d-142">UserId</span><span class="sxs-lookup"><span data-stu-id="4321d-142">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="4321d-143">Identifica um usuário delegado ou um usuário que tem permissões de acesso de pasta.</span><span class="sxs-lookup"><span data-stu-id="4321d-143">Identifies a delegate user or a user who has folder access permissions.</span></span> <span data-ttu-id="4321d-144">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="4321d-144">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4321d-145">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4321d-145">Parent elements</span></span>

|<span data-ttu-id="4321d-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4321d-146">**Element**</span></span>|<span data-ttu-id="4321d-147">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4321d-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4321d-148">CalendarPermissions</span><span class="sxs-lookup"><span data-stu-id="4321d-148">CalendarPermissions</span></span>](calendarpermissions.md) <br/> |<span data-ttu-id="4321d-149">Contém uma matriz de permissões de calendário de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="4321d-149">Contains an array of calendar permissions for a folder.</span></span> <span data-ttu-id="4321d-150">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="4321d-150">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4321d-151">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="4321d-151">Remarks</span></span>

<span data-ttu-id="4321d-152">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="4321d-152">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4321d-153">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="4321d-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4321d-154">Namespace</span><span class="sxs-lookup"><span data-stu-id="4321d-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4321d-155">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4321d-155">Schema Name</span></span>  <br/> |<span data-ttu-id="4321d-156">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="4321d-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="4321d-157">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4321d-157">Validation File</span></span>  <br/> |<span data-ttu-id="4321d-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4321d-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4321d-159">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="4321d-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="4321d-160">False</span><span class="sxs-lookup"><span data-stu-id="4321d-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4321d-161">Ver também</span><span class="sxs-lookup"><span data-stu-id="4321d-161">See also</span></span>



- [<span data-ttu-id="4321d-162">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4321d-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="4321d-163">Definindo permissões de nível de pasta</span><span class="sxs-lookup"><span data-stu-id="4321d-163">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

