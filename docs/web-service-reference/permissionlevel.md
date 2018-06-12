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
ms.openlocfilehash: 7cc734f5807fe039467065315c220341f47d3fb4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824730"
---
# <a name="permissionlevel"></a><span data-ttu-id="8d8df-104">PermissionLevel</span><span class="sxs-lookup"><span data-stu-id="8d8df-104">PermissionLevel</span></span>

<span data-ttu-id="8d8df-105">O elemento **PermissionLevel** representa o nível de permissão que um usuário tem em uma pasta.</span><span class="sxs-lookup"><span data-stu-id="8d8df-105">The **PermissionLevel** element represents the permission level that a user has on a folder.</span></span> <span data-ttu-id="8d8df-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="8d8df-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<PermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or Custom</PermissionLevel>
```

 <span data-ttu-id="8d8df-107">**PermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="8d8df-107">**PermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8d8df-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8d8df-108">Attributes and elements</span></span>

<span data-ttu-id="8d8df-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8d8df-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d8df-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="8d8df-110">Attributes</span></span>

<span data-ttu-id="8d8df-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8d8df-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8d8df-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8d8df-112">Child elements</span></span>

<span data-ttu-id="8d8df-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8d8df-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8d8df-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8d8df-114">Parent elements</span></span>

|<span data-ttu-id="8d8df-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8d8df-115">**Element**</span></span>|<span data-ttu-id="8d8df-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8d8df-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d8df-117">Permissão</span><span class="sxs-lookup"><span data-stu-id="8d8df-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="8d8df-118">Define o que um usuário tem acesso a uma pasta.</span><span class="sxs-lookup"><span data-stu-id="8d8df-118">Defines the access that a user has to a folder.</span></span> <span data-ttu-id="8d8df-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="8d8df-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8d8df-120">Text value</span><span class="sxs-lookup"><span data-stu-id="8d8df-120">Text value</span></span>

<span data-ttu-id="8d8df-121">A tabela a seguir lista os valores possíveis para o elemento **PermissionLevel** .</span><span class="sxs-lookup"><span data-stu-id="8d8df-121">The following table lists the possible values for the **PermissionLevel** element.</span></span> 
  
<span data-ttu-id="8d8df-122">**Valores de texto do elemento PermissionLevel**</span><span class="sxs-lookup"><span data-stu-id="8d8df-122">**PermissionLevel element text values**</span></span>

|<span data-ttu-id="8d8df-123">**Valor**</span><span class="sxs-lookup"><span data-stu-id="8d8df-123">**Value**</span></span>|<span data-ttu-id="8d8df-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8d8df-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8d8df-125">None</span><span class="sxs-lookup"><span data-stu-id="8d8df-125">None</span></span>  <br/> |<span data-ttu-id="8d8df-126">Indica que o usuário não tem nenhuma permissão na pasta.</span><span class="sxs-lookup"><span data-stu-id="8d8df-126">Indicates that the user has no permissions on the folder.</span></span>  <br/> |
|<span data-ttu-id="8d8df-127">Proprietário</span><span class="sxs-lookup"><span data-stu-id="8d8df-127">Owner</span></span>  <br/> |<span data-ttu-id="8d8df-128">Indica que o usuário pode criar, ler, editar, excluir todos os itens na pasta e criar subpastas.</span><span class="sxs-lookup"><span data-stu-id="8d8df-128">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span> <span data-ttu-id="8d8df-129">O usuário é o proprietário da pasta e o contato da pasta.</span><span class="sxs-lookup"><span data-stu-id="8d8df-129">The user is both folder owner and folder contact.</span></span>  <br/> |
|<span data-ttu-id="8d8df-130">PublishingEditor</span><span class="sxs-lookup"><span data-stu-id="8d8df-130">PublishingEditor</span></span>  <br/> |<span data-ttu-id="8d8df-131">Indica que o usuário pode criar, ler, editar, excluir todos os itens na pasta e criar subpastas.</span><span class="sxs-lookup"><span data-stu-id="8d8df-131">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="8d8df-132">Editor</span><span class="sxs-lookup"><span data-stu-id="8d8df-132">Editor</span></span>  <br/> |<span data-ttu-id="8d8df-133">Indica que o usuário pode criar, ler, editar e excluir todos os itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="8d8df-133">Indicates that the user can create, read, edit, and delete all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="8d8df-134">PublishingAuthor</span><span class="sxs-lookup"><span data-stu-id="8d8df-134">PublishingAuthor</span></span>  <br/> |<span data-ttu-id="8d8df-135">Indica que o usuário pode criar e ler todos os itens na pasta, editar e excluir apenas os itens que o usuário cria e criar subpastas.</span><span class="sxs-lookup"><span data-stu-id="8d8df-135">Indicates that the user can create and read all items in the folder, edit and delete only items that the user creates, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="8d8df-136">Autor</span><span class="sxs-lookup"><span data-stu-id="8d8df-136">Author</span></span>  <br/> |<span data-ttu-id="8d8df-137">Indica que o usuário pode criar e ler todos os itens na pasta e editar e excluir apenas os itens que o usuário cria.</span><span class="sxs-lookup"><span data-stu-id="8d8df-137">Indicates that the user can create and read all items in the folder, and edit and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="8d8df-138">NoneditingAuthor</span><span class="sxs-lookup"><span data-stu-id="8d8df-138">NoneditingAuthor</span></span>  <br/> |<span data-ttu-id="8d8df-139">Indica que o usuário pode criar e ler todos os itens na pasta e excluir apenas os itens que o usuário cria.</span><span class="sxs-lookup"><span data-stu-id="8d8df-139">Indicates that the user can create and read all items in the folder, and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="8d8df-140">Reviewer</span><span class="sxs-lookup"><span data-stu-id="8d8df-140">Reviewer</span></span>  <br/> |<span data-ttu-id="8d8df-141">Indica que o usuário pode ler todos os itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="8d8df-141">Indicates that the user can read all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="8d8df-142">Colaborador</span><span class="sxs-lookup"><span data-stu-id="8d8df-142">Contributor</span></span>  <br/> |<span data-ttu-id="8d8df-143">Indica que o usuário pode criar itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="8d8df-143">Indicates that the user can create items in the folder.</span></span> <span data-ttu-id="8d8df-144">O conteúdo da pasta não aparecem.</span><span class="sxs-lookup"><span data-stu-id="8d8df-144">The contents of the folder do not appear.</span></span>  <br/> |
|<span data-ttu-id="8d8df-145">Personalizado</span><span class="sxs-lookup"><span data-stu-id="8d8df-145">Custom</span></span>  <br/> |<span data-ttu-id="8d8df-146">Indica que o usuário tem permissões de acesso personalizadas na pasta.</span><span class="sxs-lookup"><span data-stu-id="8d8df-146">Indicates that the user has custom access permissions on the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8d8df-147">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="8d8df-147">Remarks</span></span>

<span data-ttu-id="8d8df-148">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="8d8df-148">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8d8df-149">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8d8df-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8d8df-150">Namespace</span><span class="sxs-lookup"><span data-stu-id="8d8df-150">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8d8df-151">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8d8df-151">Schema Name</span></span>  <br/> |<span data-ttu-id="8d8df-152">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8d8df-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="8d8df-153">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8d8df-153">Validation File</span></span>  <br/> |<span data-ttu-id="8d8df-154">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8d8df-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8d8df-155">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8d8df-155">Can be Empty</span></span>  <br/> |<span data-ttu-id="8d8df-156">False</span><span class="sxs-lookup"><span data-stu-id="8d8df-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8d8df-157">Ver também</span><span class="sxs-lookup"><span data-stu-id="8d8df-157">See also</span></span>



- [<span data-ttu-id="8d8df-158">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8d8df-158">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="8d8df-159">Definindo permissões de nível de pasta</span><span class="sxs-lookup"><span data-stu-id="8d8df-159">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

