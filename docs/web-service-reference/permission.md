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
description: O elemento de permissão define o que um usuário tem acesso a uma pasta.
ms.openlocfilehash: 600d60f481c4f1d407c3a39ab65d6ddcf46d04e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824735"
---
# <a name="permission"></a><span data-ttu-id="145c6-103">Permissão</span><span class="sxs-lookup"><span data-stu-id="145c6-103">Permission</span></span>

<span data-ttu-id="145c6-104">O elemento de **permissão** define o que um usuário tem acesso a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="145c6-104">The **Permission** element defines the access that a user has to a folder.</span></span> 
  
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

 <span data-ttu-id="145c6-105">**PermissionType**</span><span class="sxs-lookup"><span data-stu-id="145c6-105">**PermissionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="145c6-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="145c6-106">Attributes and elements</span></span>

<span data-ttu-id="145c6-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="145c6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="145c6-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="145c6-108">Attributes</span></span>

<span data-ttu-id="145c6-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="145c6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="145c6-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="145c6-110">Child elements</span></span>

|<span data-ttu-id="145c6-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="145c6-111">**Element**</span></span>|<span data-ttu-id="145c6-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="145c6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="145c6-113">CanCreateItems</span><span class="sxs-lookup"><span data-stu-id="145c6-113">CanCreateItems</span></span>](cancreateitems.md) <br/> |<span data-ttu-id="145c6-114">Indica se um usuário tem permissão para criar itens em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="145c6-114">Indicates whether a user has permission to create items in a folder.</span></span> <span data-ttu-id="145c6-115">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="145c6-115">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="145c6-116">CanCreateSubFolders</span><span class="sxs-lookup"><span data-stu-id="145c6-116">CanCreateSubFolders</span></span>](cancreatesubfolders.md) <br/> |<span data-ttu-id="145c6-117">Indica se um usuário tem permissão para criar subpastas em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="145c6-117">Indicates whether a user has permission to create subfolders in a folder.</span></span> <span data-ttu-id="145c6-118">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="145c6-118">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="145c6-119">DeleteItems</span><span class="sxs-lookup"><span data-stu-id="145c6-119">DeleteItems</span></span>](deleteitems.md) <br/> |<span data-ttu-id="145c6-120">Indica se um usuário tem permissão para excluir itens em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="145c6-120">Indicates whether a user has permission to delete items in a folder.</span></span> <span data-ttu-id="145c6-121">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="145c6-121">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="145c6-122">EditItems</span><span class="sxs-lookup"><span data-stu-id="145c6-122">EditItems</span></span>](edititems.md) <br/> |<span data-ttu-id="145c6-123">Indica se um usuário tem permissão para editar itens em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="145c6-123">Indicates whether a user has permission to edit items in a folder.</span></span> <span data-ttu-id="145c6-124">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="145c6-124">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="145c6-125">IsFolderContact</span><span class="sxs-lookup"><span data-stu-id="145c6-125">IsFolderContact</span></span>](isfoldercontact.md) <br/> |<span data-ttu-id="145c6-126">Indica se um usuário é um contato para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="145c6-126">Indicates whether a user is a contact for a folder.</span></span> <span data-ttu-id="145c6-127">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="145c6-127">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="145c6-128">IsFolderOwner</span><span class="sxs-lookup"><span data-stu-id="145c6-128">IsFolderOwner</span></span>](isfolderowner.md) <br/> |<span data-ttu-id="145c6-129">Indica se um usuário é o proprietário de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="145c6-129">Indicates whether a user is the owner of a folder.</span></span> <span data-ttu-id="145c6-130">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="145c6-130">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="145c6-131">IsFolderVisible</span><span class="sxs-lookup"><span data-stu-id="145c6-131">IsFolderVisible</span></span>](isfoldervisible.md) <br/> |<span data-ttu-id="145c6-132">Indica se um usuário pode exibir uma pasta.</span><span class="sxs-lookup"><span data-stu-id="145c6-132">Indicates whether a user can view a folder.</span></span> <span data-ttu-id="145c6-133">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="145c6-133">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="145c6-134">PermissionLevel</span><span class="sxs-lookup"><span data-stu-id="145c6-134">PermissionLevel</span></span>](permissionlevel.md) <br/> |<span data-ttu-id="145c6-135">Representa a combinação de permissões que um usuário tem em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="145c6-135">Represents the combination of permissions that a user has on a folder.</span></span> <span data-ttu-id="145c6-136">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="145c6-136">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="145c6-137">ReadItems (PermissionType)</span><span class="sxs-lookup"><span data-stu-id="145c6-137">ReadItems (PermissionType)</span></span>](readitems-permissiontype.md) <br/> |<span data-ttu-id="145c6-138">Indica se um usuário tem permissão para ler itens dentro de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="145c6-138">Indicates whether a user has permission to read items within a folder.</span></span> <span data-ttu-id="145c6-139">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="145c6-139">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="145c6-140">UserId</span><span class="sxs-lookup"><span data-stu-id="145c6-140">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="145c6-141">Identifica um usuário delegado ou um usuário que tem permissões de acesso de pasta.</span><span class="sxs-lookup"><span data-stu-id="145c6-141">Identifies a delegate user or a user who has folder access permissions.</span></span> <span data-ttu-id="145c6-142">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="145c6-142">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="145c6-143">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="145c6-143">Parent elements</span></span>

|<span data-ttu-id="145c6-144">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="145c6-144">**Element**</span></span>|<span data-ttu-id="145c6-145">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="145c6-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="145c6-146">Permissões</span><span class="sxs-lookup"><span data-stu-id="145c6-146">Permissions</span></span>](permissions.md) <br/> |<span data-ttu-id="145c6-147">Contém todas as permissões configuradas para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="145c6-147">Contains all the configured permissions for a folder.</span></span> <span data-ttu-id="145c6-148">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="145c6-148">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="145c6-149">Comentários</span><span class="sxs-lookup"><span data-stu-id="145c6-149">Remarks</span></span>

<span data-ttu-id="145c6-150">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="145c6-150">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="145c6-151">Este elemento foi introduzido no Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="145c6-151">This element was introduced in Exchange Server 2007 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="145c6-152">Diferenças de versão</span><span class="sxs-lookup"><span data-stu-id="145c6-152">Version differences</span></span>

<span data-ttu-id="145c6-153">Para aplicativos de destino Exchange Online, Exchange Online como parte do Office 365 ou uma versão local do Exchange, começando com o Exchange 2013, permissões de pasta não serão retornadas quando o elemento [BaseShape](baseshape.md) tem um valor de **AllProperties** na solicitação de operação [GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="145c6-153">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="145c6-154">Para recuperar as permissões da pasta, adicione o elemento [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) ao elemento [AdditionalProperties](additionalproperties.md) na solicitação **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="145c6-154">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="145c6-155">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="145c6-155">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="145c6-156">Namespace</span><span class="sxs-lookup"><span data-stu-id="145c6-156">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="145c6-157">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="145c6-157">Schema Name</span></span>  <br/> |<span data-ttu-id="145c6-158">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="145c6-158">Types schema</span></span>  <br/> |
|<span data-ttu-id="145c6-159">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="145c6-159">Validation File</span></span>  <br/> |<span data-ttu-id="145c6-160">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="145c6-160">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="145c6-161">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="145c6-161">Can be Empty</span></span>  <br/> |<span data-ttu-id="145c6-162">False</span><span class="sxs-lookup"><span data-stu-id="145c6-162">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="145c6-163">Ver também</span><span class="sxs-lookup"><span data-stu-id="145c6-163">See also</span></span>



- [<span data-ttu-id="145c6-164">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="145c6-164">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="145c6-165">Definindo permissões de nível de pasta</span><span class="sxs-lookup"><span data-stu-id="145c6-165">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

