---
title: PermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermissionLevel
api_type:
- schema
ms.assetid: 87978600-3523-451e-a725-ef092c543e2a
description: O elemento PermissionLevel representa o nível de permissão que um usuário tem em uma pasta. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: e1e441c53b5c40c16051eb852a6b35a8af7476e2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458037"
---
# <a name="permissionlevel"></a><span data-ttu-id="d2b31-104">PermissionLevel</span><span class="sxs-lookup"><span data-stu-id="d2b31-104">PermissionLevel</span></span>

<span data-ttu-id="d2b31-105">O elemento **PermissionLevel** representa o nível de permissão que um usuário tem em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="d2b31-105">The **PermissionLevel** element represents the permission level that a user has on a folder.</span></span> <span data-ttu-id="d2b31-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d2b31-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<PermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or Custom</PermissionLevel>
```

 <span data-ttu-id="d2b31-107">**PermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="d2b31-107">**PermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d2b31-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="d2b31-108">Attributes and elements</span></span>

<span data-ttu-id="d2b31-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d2b31-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2b31-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="d2b31-110">Attributes</span></span>

<span data-ttu-id="d2b31-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2b31-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d2b31-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d2b31-112">Child elements</span></span>

<span data-ttu-id="d2b31-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d2b31-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d2b31-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d2b31-114">Parent elements</span></span>

|<span data-ttu-id="d2b31-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d2b31-115">**Element**</span></span>|<span data-ttu-id="d2b31-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d2b31-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2b31-117">Permissão</span><span class="sxs-lookup"><span data-stu-id="d2b31-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="d2b31-118">Define o acesso que um usuário tem a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="d2b31-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="d2b31-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="d2b31-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d2b31-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="d2b31-120">Text value</span></span>

<span data-ttu-id="d2b31-121">A tabela a seguir lista os valores possíveis para o elemento **PermissionLevel** .</span><span class="sxs-lookup"><span data-stu-id="d2b31-121">The following table lists the possible values for the **PermissionLevel** element.</span></span> 
  
<span data-ttu-id="d2b31-122">**Valores de texto do elemento PermissionLevel**</span><span class="sxs-lookup"><span data-stu-id="d2b31-122">**PermissionLevel element text values**</span></span>

|<span data-ttu-id="d2b31-123">**Valor**</span><span class="sxs-lookup"><span data-stu-id="d2b31-123">**Value**</span></span>|<span data-ttu-id="d2b31-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d2b31-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d2b31-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2b31-125">None</span></span>  <br/> |<span data-ttu-id="d2b31-126">Indica que o usuário não tem permissões na pasta.</span><span class="sxs-lookup"><span data-stu-id="d2b31-126">Indicates that the user has no permissions on the folder.</span></span>  <br/> |
|<span data-ttu-id="d2b31-127">Proprietário</span><span class="sxs-lookup"><span data-stu-id="d2b31-127">Owner</span></span>  <br/> |<span data-ttu-id="d2b31-128">Indica que o usuário pode criar, ler, editar e excluir todos os itens na pasta e criar subpastas.</span><span class="sxs-lookup"><span data-stu-id="d2b31-128">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span> <span data-ttu-id="d2b31-129">O usuário é o proprietário da pasta e o contato da pasta.</span><span class="sxs-lookup"><span data-stu-id="d2b31-129">The user is both folder owner and folder contact.</span></span>  <br/> |
|<span data-ttu-id="d2b31-130">Publishingeditorcreateitems</span><span class="sxs-lookup"><span data-stu-id="d2b31-130">PublishingEditor</span></span>  <br/> |<span data-ttu-id="d2b31-131">Indica que o usuário pode criar, ler, editar e excluir todos os itens na pasta e criar subpastas.</span><span class="sxs-lookup"><span data-stu-id="d2b31-131">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="d2b31-132">Editor</span><span class="sxs-lookup"><span data-stu-id="d2b31-132">Editor</span></span>  <br/> |<span data-ttu-id="d2b31-133">Indica que o usuário pode criar, ler, editar e excluir todos os itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="d2b31-133">Indicates that the user can create, read, edit, and delete all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="d2b31-134">Publishingauthorcreateitems</span><span class="sxs-lookup"><span data-stu-id="d2b31-134">PublishingAuthor</span></span>  <br/> |<span data-ttu-id="d2b31-135">Indica que o usuário pode criar e ler todos os itens na pasta, editar e excluir somente os itens que o usuário cria e criar subpastas.</span><span class="sxs-lookup"><span data-stu-id="d2b31-135">Indicates that the user can create and read all items in the folder, edit and delete only items that the user creates, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="d2b31-136">Autor</span><span class="sxs-lookup"><span data-stu-id="d2b31-136">Author</span></span>  <br/> |<span data-ttu-id="d2b31-137">Indica que o usuário pode criar e ler todos os itens na pasta e editar e excluir somente os itens que o usuário cria.</span><span class="sxs-lookup"><span data-stu-id="d2b31-137">Indicates that the user can create and read all items in the folder, and edit and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="d2b31-138">Noneditingauthorcreateitems</span><span class="sxs-lookup"><span data-stu-id="d2b31-138">NoneditingAuthor</span></span>  <br/> |<span data-ttu-id="d2b31-139">Indica que o usuário pode criar e ler todos os itens na pasta e excluir apenas os itens que o usuário cria.</span><span class="sxs-lookup"><span data-stu-id="d2b31-139">Indicates that the user can create and read all items in the folder, and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="d2b31-140">Revisor</span><span class="sxs-lookup"><span data-stu-id="d2b31-140">Reviewer</span></span>  <br/> |<span data-ttu-id="d2b31-141">Indica que o usuário pode ler todos os itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="d2b31-141">Indicates that the user can read all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="d2b31-142">Colaborador</span><span class="sxs-lookup"><span data-stu-id="d2b31-142">Contributor</span></span>  <br/> |<span data-ttu-id="d2b31-143">Indica que o usuário pode criar itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="d2b31-143">Indicates that the user can create items in the folder.</span></span> <span data-ttu-id="d2b31-144">O conteúdo da pasta não é exibido.</span><span class="sxs-lookup"><span data-stu-id="d2b31-144">The contents of the folder do not appear.</span></span>  <br/> |
|<span data-ttu-id="d2b31-145">Personalizado</span><span class="sxs-lookup"><span data-stu-id="d2b31-145">Custom</span></span>  <br/> |<span data-ttu-id="d2b31-146">Indica que o usuário tem permissões de acesso personalizadas na pasta.</span><span class="sxs-lookup"><span data-stu-id="d2b31-146">Indicates that the user has custom access permissions on the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d2b31-147">Comentários</span><span class="sxs-lookup"><span data-stu-id="d2b31-147">Remarks</span></span>

<span data-ttu-id="d2b31-148">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="d2b31-148">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2b31-149">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="d2b31-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2b31-150">Namespace</span><span class="sxs-lookup"><span data-stu-id="d2b31-150">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d2b31-151">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d2b31-151">Schema Name</span></span>  <br/> |<span data-ttu-id="d2b31-152">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d2b31-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="d2b31-153">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d2b31-153">Validation File</span></span>  <br/> |<span data-ttu-id="d2b31-154">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d2b31-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d2b31-155">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="d2b31-155">Can be Empty</span></span>  <br/> |<span data-ttu-id="d2b31-156">False</span><span class="sxs-lookup"><span data-stu-id="d2b31-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d2b31-157">Confira também</span><span class="sxs-lookup"><span data-stu-id="d2b31-157">See also</span></span>



- [<span data-ttu-id="d2b31-158">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d2b31-158">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="d2b31-159">Definindo permissões no nível de pasta</span><span class="sxs-lookup"><span data-stu-id="d2b31-159">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

