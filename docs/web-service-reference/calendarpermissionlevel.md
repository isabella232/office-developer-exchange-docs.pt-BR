---
title: CalendarPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarPermissionLevel
api_type:
- schema
ms.assetid: 6ac2b792-4326-4a3f-b6cb-977bf523b5b2
description: O elemento CalendarPermissionLevel representa o nível de permissão que um usuário tem em uma pasta de calendário. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 646e4df3b70350a16cdd1f3e134260c2984a5161
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751364"
---
# <a name="calendarpermissionlevel"></a><span data-ttu-id="f7ced-104">CalendarPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="f7ced-104">CalendarPermissionLevel</span></span>

<span data-ttu-id="f7ced-105">O elemento **CalendarPermissionLevel** representa o nível de permissão que um usuário tem em uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="f7ced-105">The **CalendarPermissionLevel** element represents the permission level that a user has on a Calendar folder.</span></span> <span data-ttu-id="f7ced-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f7ced-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CalendarPermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or FreeBusyTimeOnly or FreeBusyTimeAndSubjectAndLocation or Custom</CalendarPermissionLevel>
```

 <span data-ttu-id="f7ced-107">**CalendarPermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="f7ced-107">**CalendarPermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f7ced-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f7ced-108">Attributes and elements</span></span>

<span data-ttu-id="f7ced-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f7ced-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f7ced-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="f7ced-110">Attributes</span></span>

<span data-ttu-id="f7ced-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f7ced-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f7ced-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f7ced-112">Child elements</span></span>

<span data-ttu-id="f7ced-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f7ced-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f7ced-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f7ced-114">Parent elements</span></span>

|<span data-ttu-id="f7ced-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f7ced-115">**Element**</span></span>|<span data-ttu-id="f7ced-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f7ced-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7ced-117">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="f7ced-117">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="f7ced-118">Define o que um usuário tem acesso a uma pasta de calendário.</span><span class="sxs-lookup"><span data-stu-id="f7ced-118">Defines the access that a user has to a Calendar folder.</span></span> <span data-ttu-id="f7ced-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f7ced-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f7ced-120">Text value</span><span class="sxs-lookup"><span data-stu-id="f7ced-120">Text value</span></span>

<span data-ttu-id="f7ced-121">A tabela a seguir lista os valores possíveis para o elemento **CalendarPermissionLevel** .</span><span class="sxs-lookup"><span data-stu-id="f7ced-121">The following table lists the possible values for the **CalendarPermissionLevel** element.</span></span> 
  
<span data-ttu-id="f7ced-122">**Valores de texto do elemento CalendarPermissionLevel**</span><span class="sxs-lookup"><span data-stu-id="f7ced-122">**CalendarPermissionLevel element text values**</span></span>

|<span data-ttu-id="f7ced-123">**Valor**</span><span class="sxs-lookup"><span data-stu-id="f7ced-123">**Value**</span></span>|<span data-ttu-id="f7ced-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f7ced-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f7ced-125">None</span><span class="sxs-lookup"><span data-stu-id="f7ced-125">None</span></span>  <br/> |<span data-ttu-id="f7ced-126">Indica que o usuário não tem nenhuma permissão na pasta.</span><span class="sxs-lookup"><span data-stu-id="f7ced-126">Indicates that the user has no permissions on the folder.</span></span>  <br/> |
|<span data-ttu-id="f7ced-127">Proprietário</span><span class="sxs-lookup"><span data-stu-id="f7ced-127">Owner</span></span>  <br/> |<span data-ttu-id="f7ced-128">Indica que o usuário pode criar, ler, editar, excluir todos os itens na pasta e criar subpastas.</span><span class="sxs-lookup"><span data-stu-id="f7ced-128">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span> <span data-ttu-id="f7ced-129">O usuário é o proprietário da pasta e o contato da pasta.</span><span class="sxs-lookup"><span data-stu-id="f7ced-129">The user is both folder owner and folder contact.</span></span>  <br/> |
|<span data-ttu-id="f7ced-130">PublishingEditor</span><span class="sxs-lookup"><span data-stu-id="f7ced-130">PublishingEditor</span></span>  <br/> |<span data-ttu-id="f7ced-131">Indica que o usuário pode criar, ler, editar, excluir todos os itens na pasta e criar subpastas.</span><span class="sxs-lookup"><span data-stu-id="f7ced-131">Indicates that the user can create, read, edit, and delete all items in the folder, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="f7ced-132">Editor</span><span class="sxs-lookup"><span data-stu-id="f7ced-132">Editor</span></span>  <br/> |<span data-ttu-id="f7ced-133">Indica que o usuário pode criar, ler, editar e excluir todos os itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="f7ced-133">Indicates that the user can create, read, edit and delete all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="f7ced-134">PublishingAuthor</span><span class="sxs-lookup"><span data-stu-id="f7ced-134">PublishingAuthor</span></span>  <br/> |<span data-ttu-id="f7ced-135">Indica que o usuário pode criar e ler todos os itens na pasta, editar e excluir apenas os itens que o usuário cria e criar subpastas.</span><span class="sxs-lookup"><span data-stu-id="f7ced-135">Indicates that the user can create and read all items in the folder, edit and delete only items that the user creates, and create subfolders.</span></span>  <br/> |
|<span data-ttu-id="f7ced-136">Autor</span><span class="sxs-lookup"><span data-stu-id="f7ced-136">Author</span></span>  <br/> |<span data-ttu-id="f7ced-137">Indica que o usuário pode criar e ler todos os itens na pasta e editar e excluir apenas os itens que o usuário cria.</span><span class="sxs-lookup"><span data-stu-id="f7ced-137">Indicates that the user can create and read all items in the folder, and edit and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="f7ced-138">NoneditingAuthor</span><span class="sxs-lookup"><span data-stu-id="f7ced-138">NoneditingAuthor</span></span>  <br/> |<span data-ttu-id="f7ced-139">Indica que o usuário pode criar e ler todos os itens na pasta e excluir apenas os itens que o usuário cria.</span><span class="sxs-lookup"><span data-stu-id="f7ced-139">Indicates that the user can create and read all items in the folder, and delete only items that the user creates.</span></span>  <br/> |
|<span data-ttu-id="f7ced-140">Reviewer</span><span class="sxs-lookup"><span data-stu-id="f7ced-140">Reviewer</span></span>  <br/> |<span data-ttu-id="f7ced-141">Indica que o usuário pode ler todos os itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="f7ced-141">Indicates that the user can read all items in the folder.</span></span>  <br/> |
|<span data-ttu-id="f7ced-142">Colaborador</span><span class="sxs-lookup"><span data-stu-id="f7ced-142">Contributor</span></span>  <br/> |<span data-ttu-id="f7ced-143">Indica que o usuário pode criar itens na pasta.</span><span class="sxs-lookup"><span data-stu-id="f7ced-143">Indicates that the user can create items in the folder.</span></span> <span data-ttu-id="f7ced-144">O conteúdo da pasta não aparecem.</span><span class="sxs-lookup"><span data-stu-id="f7ced-144">The contents of the folder do not appear.</span></span>  <br/> |
|<span data-ttu-id="f7ced-145">FreeBusyTimeOnly</span><span class="sxs-lookup"><span data-stu-id="f7ced-145">FreeBusyTimeOnly</span></span>  <br/> |<span data-ttu-id="f7ced-146">Indica que o usuário pode exibir apenas informações de disponibilidade tempo dentro do calendário.</span><span class="sxs-lookup"><span data-stu-id="f7ced-146">Indicates that the user can view only free/busy time within the calendar.</span></span>  <br/> |
|<span data-ttu-id="f7ced-147">FreeBusyTimeAndSubjectAndLocation</span><span class="sxs-lookup"><span data-stu-id="f7ced-147">FreeBusyTimeAndSubjectAndLocation</span></span>  <br/> |<span data-ttu-id="f7ced-148">Indica que o usuário pode exibir informações de disponibilidade de tempo dentro do calendário e o assunto e o local de compromissos.</span><span class="sxs-lookup"><span data-stu-id="f7ced-148">Indicates that the user can view free/busy time within the calendar and the subject and location of appointments.</span></span>  <br/> |
|<span data-ttu-id="f7ced-149">Personalizado</span><span class="sxs-lookup"><span data-stu-id="f7ced-149">Custom</span></span>  <br/> |<span data-ttu-id="f7ced-150">Indica que o usuário tem permissões de acesso personalizadas na pasta.</span><span class="sxs-lookup"><span data-stu-id="f7ced-150">Indicates that the user has custom access permissions on the folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f7ced-151">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="f7ced-151">Remarks</span></span>

<span data-ttu-id="f7ced-152">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f7ced-152">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f7ced-153">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f7ced-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f7ced-154">Namespace</span><span class="sxs-lookup"><span data-stu-id="f7ced-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f7ced-155">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f7ced-155">Schema Name</span></span>  <br/> |<span data-ttu-id="f7ced-156">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f7ced-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="f7ced-157">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f7ced-157">Validation File</span></span>  <br/> |<span data-ttu-id="f7ced-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f7ced-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f7ced-159">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f7ced-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="f7ced-160">False</span><span class="sxs-lookup"><span data-stu-id="f7ced-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f7ced-161">Ver também</span><span class="sxs-lookup"><span data-stu-id="f7ced-161">See also</span></span>



- [<span data-ttu-id="f7ced-162">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f7ced-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="f7ced-163">Definindo permissões de nível de pasta</span><span class="sxs-lookup"><span data-stu-id="f7ced-163">Setting Folder-Level Permissions</span></span>](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

