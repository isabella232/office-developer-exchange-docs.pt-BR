---
title: TasksFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TasksFolderPermissionLevel
api_type:
- schema
ms.assetid: 0f70b79b-3443-4048-b410-692d4e2464fc
description: O elemento TasksFolderPermissionLevel contém as permissões para a pasta padrão tarefas. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 49807896f9175bafbef106c41d1c9dff8f6178c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837697"
---
# <a name="tasksfolderpermissionlevel"></a><span data-ttu-id="6af1c-104">TasksFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="6af1c-104">TasksFolderPermissionLevel</span></span>

<span data-ttu-id="6af1c-105">O elemento **TasksFolderPermissionLevel** contém as permissões para a pasta padrão tarefas.</span><span class="sxs-lookup"><span data-stu-id="6af1c-105">The **TasksFolderPermissionLevel** element contains the permissions for the default Tasks folder.</span></span> <span data-ttu-id="6af1c-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6af1c-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<TasksFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</TasksFolderPermissionLevel>
```

<span data-ttu-id="6af1c-107">**DelegateFolderPermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="6af1c-107">**DelegateFolderPermissionLevelType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6af1c-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6af1c-108">Attributes and elements</span></span>

<span data-ttu-id="6af1c-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6af1c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6af1c-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="6af1c-110">Attributes</span></span>

<span data-ttu-id="6af1c-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6af1c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6af1c-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6af1c-112">Child elements</span></span>

<span data-ttu-id="6af1c-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6af1c-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6af1c-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6af1c-114">Parent elements</span></span>

|<span data-ttu-id="6af1c-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6af1c-115">**Element**</span></span>|<span data-ttu-id="6af1c-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6af1c-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6af1c-117">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="6af1c-117">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="6af1c-118">Contém as configurações de nível de permissão do representante de um usuário.</span><span class="sxs-lookup"><span data-stu-id="6af1c-118">Contains the delegate permission level settings for a user.</span></span> <span data-ttu-id="6af1c-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="6af1c-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6af1c-120">Text value</span><span class="sxs-lookup"><span data-stu-id="6af1c-120">Text value</span></span>

<span data-ttu-id="6af1c-121">A tabela a seguir lista os valores de texto que representam os níveis de permissão.</span><span class="sxs-lookup"><span data-stu-id="6af1c-121">The following table lists the text values that represent the permission levels.</span></span>
  
<span data-ttu-id="6af1c-122">**Valores de texto de nível de permissão**</span><span class="sxs-lookup"><span data-stu-id="6af1c-122">**Permission level text values**</span></span>

|<span data-ttu-id="6af1c-123">**Nível de permissão**</span><span class="sxs-lookup"><span data-stu-id="6af1c-123">**Permission level**</span></span>|<span data-ttu-id="6af1c-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6af1c-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6af1c-125">None</span><span class="sxs-lookup"><span data-stu-id="6af1c-125">None</span></span>  <br/> |<span data-ttu-id="6af1c-126">O usuário delegado não tem nenhuma permissão de acesso à pasta tarefas.</span><span class="sxs-lookup"><span data-stu-id="6af1c-126">The delegate user has no access permissions to the Tasks folder.</span></span>  <br/> |
|<span data-ttu-id="6af1c-127">Reviewer</span><span class="sxs-lookup"><span data-stu-id="6af1c-127">Reviewer</span></span>  <br/> |<span data-ttu-id="6af1c-128">O usuário delegado pode ler itens na pasta tarefas.</span><span class="sxs-lookup"><span data-stu-id="6af1c-128">The delegate user can read items in the Tasks folder.</span></span>  <br/> |
|<span data-ttu-id="6af1c-129">Autor</span><span class="sxs-lookup"><span data-stu-id="6af1c-129">Author</span></span>  <br/> |<span data-ttu-id="6af1c-130">O usuário delegado pode ler e criar itens na pasta tarefas.</span><span class="sxs-lookup"><span data-stu-id="6af1c-130">The delegate user can read and create items in the Tasks folder.</span></span>  <br/> |
|<span data-ttu-id="6af1c-131">Editor</span><span class="sxs-lookup"><span data-stu-id="6af1c-131">Editor</span></span>  <br/> |<span data-ttu-id="6af1c-132">O usuário delegado pode ler, criar e modificar itens na pasta tarefas.</span><span class="sxs-lookup"><span data-stu-id="6af1c-132">The delegate user can read, create, and modify items in the Tasks folder.</span></span>  <br/> |
|<span data-ttu-id="6af1c-133">Personalizado</span><span class="sxs-lookup"><span data-stu-id="6af1c-133">Custom</span></span>  <br/> |<span data-ttu-id="6af1c-134">O usuário delegado tem permissões personalizadas de acesso à pasta tarefas.</span><span class="sxs-lookup"><span data-stu-id="6af1c-134">The delegate user has custom access permissions to the Tasks folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6af1c-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="6af1c-135">Remarks</span></span>

<span data-ttu-id="6af1c-136">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="6af1c-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6af1c-137">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6af1c-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6af1c-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="6af1c-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6af1c-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6af1c-139">Schema Name</span></span>  <br/> |<span data-ttu-id="6af1c-140">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="6af1c-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="6af1c-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6af1c-141">Validation File</span></span>  <br/> |<span data-ttu-id="6af1c-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6af1c-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6af1c-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6af1c-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="6af1c-144">False</span><span class="sxs-lookup"><span data-stu-id="6af1c-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6af1c-145">Ver também</span><span class="sxs-lookup"><span data-stu-id="6af1c-145">See also</span></span>

- [<span data-ttu-id="6af1c-146">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="6af1c-146">AddDelegate operation</span></span>](adddelegate-operation.md)
- [<span data-ttu-id="6af1c-147">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="6af1c-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="6af1c-148">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6af1c-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="6af1c-149">Adicionando representantes</span><span class="sxs-lookup"><span data-stu-id="6af1c-149">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

