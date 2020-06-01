---
title: Permissão
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Permission
api_type:
- schema
ms.assetid: b8d0429a-0e58-4480-9847-4901970c7033
description: O elemento Permission define o acesso de um usuário a uma pasta.
ms.openlocfilehash: 0f7515dbb06f8423f8d4d95e1391496e8ac73653
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459255"
---
# <a name="permission"></a><span data-ttu-id="006a3-103">Permissão</span><span class="sxs-lookup"><span data-stu-id="006a3-103">Permission</span></span>

<span data-ttu-id="006a3-104">O elemento **Permission** define o acesso de um usuário a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="006a3-104">The **Permission** element defines the access that a user has to a folder.</span></span> 
  
```XML
<Permission>
   <CanCreateItems/>
   <CanCreateSubfolders/>
   <IsFolderOwner/>
   <IsFolderVisible/>
   <IsFolderContact/>
   <EditItems/>
   <DeleteItems/>
   <PermissionLevel/>
   <ReadItems/>
   <UserId/>
</Permission>
```

 <span data-ttu-id="006a3-105">**PermissionType**</span><span class="sxs-lookup"><span data-stu-id="006a3-105">**PermissionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="006a3-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="006a3-106">Attributes and elements</span></span>

<span data-ttu-id="006a3-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="006a3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="006a3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="006a3-108">Attributes</span></span>

<span data-ttu-id="006a3-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="006a3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="006a3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="006a3-110">Child elements</span></span>

|<span data-ttu-id="006a3-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="006a3-111">**Element**</span></span>|<span data-ttu-id="006a3-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="006a3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="006a3-113">Excreateitems</span><span class="sxs-lookup"><span data-stu-id="006a3-113">CanCreateItems</span></span>](cancreateitems.md) <br/> |<span data-ttu-id="006a3-114">Indica se um usuário tem permissão para criar itens em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="006a3-114">Indicates whether a user has permission to create items in a folder.</span></span> <span data-ttu-id="006a3-115">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="006a3-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="006a3-116">CanCreateSubFolders</span><span class="sxs-lookup"><span data-stu-id="006a3-116">CanCreateSubFolders</span></span>](cancreatesubfolders.md) <br/> |<span data-ttu-id="006a3-117">Indica se um usuário tem permissão para criar subpastas em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="006a3-117">Indicates whether a user has permission to create subfolders in a folder.</span></span> <span data-ttu-id="006a3-118">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="006a3-118">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="006a3-119">DeleteItems</span><span class="sxs-lookup"><span data-stu-id="006a3-119">DeleteItems</span></span>](deleteitems.md) <br/> |<span data-ttu-id="006a3-120">Indica se um usuário tem permissão para excluir itens em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="006a3-120">Indicates whether a user has permission to delete items in a folder.</span></span> <span data-ttu-id="006a3-121">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="006a3-121">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="006a3-122">EditItems</span><span class="sxs-lookup"><span data-stu-id="006a3-122">EditItems</span></span>](edititems.md) <br/> |<span data-ttu-id="006a3-123">Indica se um usuário tem permissão para editar itens em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="006a3-123">Indicates whether a user has permission to edit items in a folder.</span></span> <span data-ttu-id="006a3-124">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="006a3-124">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="006a3-125">IsFolderContact</span><span class="sxs-lookup"><span data-stu-id="006a3-125">IsFolderContact</span></span>](isfoldercontact.md) <br/> |<span data-ttu-id="006a3-126">Indica se um usuário é um contato para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="006a3-126">Indicates whether a user is a contact for a folder.</span></span> <span data-ttu-id="006a3-127">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="006a3-127">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="006a3-128">IsFolderOwner</span><span class="sxs-lookup"><span data-stu-id="006a3-128">IsFolderOwner</span></span>](isfolderowner.md) <br/> |<span data-ttu-id="006a3-129">Indica se um usuário é o proprietário de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="006a3-129">Indicates whether a user is the owner of a folder.</span></span> <span data-ttu-id="006a3-130">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="006a3-130">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="006a3-131">IsFolderVisible</span><span class="sxs-lookup"><span data-stu-id="006a3-131">IsFolderVisible</span></span>](isfoldervisible.md) <br/> |<span data-ttu-id="006a3-132">Indica se um usuário pode exibir uma pasta.</span><span class="sxs-lookup"><span data-stu-id="006a3-132">Indicates whether a user can view a folder.</span></span> <span data-ttu-id="006a3-133">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="006a3-133">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="006a3-134">PermissionLevel</span><span class="sxs-lookup"><span data-stu-id="006a3-134">PermissionLevel</span></span>](permissionlevel.md) <br/> |<span data-ttu-id="006a3-135">Representa a combinação de permissões que um usuário tem em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="006a3-135">Represents the combination of permissions that a user has on a folder.</span></span> <span data-ttu-id="006a3-136">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="006a3-136">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="006a3-137">ReadItems (PermissionType)</span><span class="sxs-lookup"><span data-stu-id="006a3-137">ReadItems (PermissionType)</span></span>](readitems-permissiontype.md) <br/> |<span data-ttu-id="006a3-138">Indica se um usuário tem permissão para ler itens em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="006a3-138">Indicates whether a user has permission to read items within a folder.</span></span> <span data-ttu-id="006a3-139">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="006a3-139">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="006a3-140">UserId</span><span class="sxs-lookup"><span data-stu-id="006a3-140">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="006a3-141">Identifica um usuário delegado ou um usuário com permissões de acesso à pasta.</span><span class="sxs-lookup"><span data-stu-id="006a3-141">Identifies a delegate user or a user who has folder access permissions.</span></span> <span data-ttu-id="006a3-142">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="006a3-142">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="006a3-143">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="006a3-143">Parent elements</span></span>

|<span data-ttu-id="006a3-144">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="006a3-144">**Element**</span></span>|<span data-ttu-id="006a3-145">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="006a3-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="006a3-146">Permissões</span><span class="sxs-lookup"><span data-stu-id="006a3-146">Permissions</span></span>](permissions.md) <br/> |<span data-ttu-id="006a3-147">Contém todas as permissões configuradas para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="006a3-147">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="006a3-148">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="006a3-148">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="006a3-149">Comentários</span><span class="sxs-lookup"><span data-stu-id="006a3-149">Remarks</span></span>

<span data-ttu-id="006a3-150">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="006a3-150">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="006a3-151">Este elemento foi introduzido no Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="006a3-151">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="006a3-152">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="006a3-152">Version differences</span></span>

<span data-ttu-id="006a3-153">Para aplicativos direcionados para o Exchange Online, o Exchange Online como parte do Office 365, ou uma versão local do Exchange a partir do Exchange 2013, as permissões de pasta não são retornadas quando o elemento [BaseShape](baseshape.md) tem um valor de **myproperties** na solicitação de operação [GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="006a3-153">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="006a3-154">Para recuperar permissões de pasta, adicione o elemento [PermissionSet (permissionsettype)](permissionset-permissionsettype.md) ao elemento [AdditionalProperties](additionalproperties.md) na solicitação **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="006a3-154">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="006a3-155">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="006a3-155">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="006a3-156">Namespace</span><span class="sxs-lookup"><span data-stu-id="006a3-156">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="006a3-157">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="006a3-157">Schema Name</span></span>  <br/> |<span data-ttu-id="006a3-158">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="006a3-158">Types schema</span></span>  <br/> |
|<span data-ttu-id="006a3-159">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="006a3-159">Validation File</span></span>  <br/> |<span data-ttu-id="006a3-160">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="006a3-160">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="006a3-161">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="006a3-161">Can be Empty</span></span>  <br/> |<span data-ttu-id="006a3-162">False</span><span class="sxs-lookup"><span data-stu-id="006a3-162">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="006a3-163">Confira também</span><span class="sxs-lookup"><span data-stu-id="006a3-163">See also</span></span>



- [<span data-ttu-id="006a3-164">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="006a3-164">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="006a3-165">Definindo permissões no nível de pasta</span><span class="sxs-lookup"><span data-stu-id="006a3-165">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

