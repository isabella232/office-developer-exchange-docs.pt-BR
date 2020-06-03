---
title: JournalFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- JournalFolderPermissionLevel
api_type:
- schema
ms.assetid: 564525fa-cd95-4c1a-9d6c-3806be664579
description: O elemento JournalFolderPermissionLevel contém as permissões para a pasta de diário padrão. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 5c0f30932eb3fbbeef1a8e34611deeb1ffef402c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529046"
---
# <a name="journalfolderpermissionlevel"></a><span data-ttu-id="dc758-104">JournalFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="dc758-104">JournalFolderPermissionLevel</span></span>

<span data-ttu-id="dc758-105">O elemento **JournalFolderPermissionLevel** contém as permissões para a pasta de diário padrão.</span><span class="sxs-lookup"><span data-stu-id="dc758-105">The **JournalFolderPermissionLevel** element contains the permissions for the default Journal folder.</span></span> <span data-ttu-id="dc758-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="dc758-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<JournalFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</JournalFolderPermissionLevel>
```

 <span data-ttu-id="dc758-107">**DelegateFolderPermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="dc758-107">**DelegateFolderPermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dc758-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="dc758-108">Attributes and elements</span></span>

<span data-ttu-id="dc758-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="dc758-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dc758-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="dc758-110">Attributes</span></span>

<span data-ttu-id="dc758-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dc758-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dc758-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="dc758-112">Child elements</span></span>

<span data-ttu-id="dc758-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="dc758-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dc758-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="dc758-114">Parent elements</span></span>

|<span data-ttu-id="dc758-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="dc758-115">**Element**</span></span>|<span data-ttu-id="dc758-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dc758-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc758-117">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="dc758-117">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="dc758-118">Contém as configurações de nível de permissão de representante para um usuário.</span><span class="sxs-lookup"><span data-stu-id="dc758-118">Contains the delegate permission level settings for a user.</span></span> <span data-ttu-id="dc758-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="dc758-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dc758-120">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="dc758-120">Text value</span></span>

<span data-ttu-id="dc758-121">A tabela a seguir lista os valores de texto que representam os níveis de permissão.</span><span class="sxs-lookup"><span data-stu-id="dc758-121">The following table lists the text values that represent the permission levels.</span></span>
  
<span data-ttu-id="dc758-122">**Valores de texto do nível de permissão**</span><span class="sxs-lookup"><span data-stu-id="dc758-122">**Permission level text values**</span></span>

|<span data-ttu-id="dc758-123">**Nível de permissão**</span><span class="sxs-lookup"><span data-stu-id="dc758-123">**Permission level**</span></span>|<span data-ttu-id="dc758-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="dc758-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dc758-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dc758-125">None</span></span>  <br/> |<span data-ttu-id="dc758-126">O usuário delegado não tem permissões de acesso à pasta diário.</span><span class="sxs-lookup"><span data-stu-id="dc758-126">The delegate user has no access permissions to the Journal folder.</span></span>  <br/> |
|<span data-ttu-id="dc758-127">Revisor</span><span class="sxs-lookup"><span data-stu-id="dc758-127">Reviewer</span></span>  <br/> |<span data-ttu-id="dc758-128">O usuário delegado pode ler itens na pasta diário.</span><span class="sxs-lookup"><span data-stu-id="dc758-128">The delegate user can read items in the Journal folder.</span></span>  <br/> |
|<span data-ttu-id="dc758-129">Autor</span><span class="sxs-lookup"><span data-stu-id="dc758-129">Author</span></span>  <br/> |<span data-ttu-id="dc758-130">O usuário delegado pode ler e criar itens na pasta de diário.</span><span class="sxs-lookup"><span data-stu-id="dc758-130">The delegate user can read and create items in the Journal folder.</span></span>  <br/> |
|<span data-ttu-id="dc758-131">Editor</span><span class="sxs-lookup"><span data-stu-id="dc758-131">Editor</span></span>  <br/> |<span data-ttu-id="dc758-132">O usuário delegado pode ler, criar e modificar itens na pasta de diário.</span><span class="sxs-lookup"><span data-stu-id="dc758-132">The delegate user can read, create, and modify items in the Journal folder.</span></span>  <br/> |
|<span data-ttu-id="dc758-133">Personalizado</span><span class="sxs-lookup"><span data-stu-id="dc758-133">Custom</span></span>  <br/> |<span data-ttu-id="dc758-134">O usuário delegado tem permissões de acesso personalizadas para a pasta de diário.</span><span class="sxs-lookup"><span data-stu-id="dc758-134">The delegate user has custom access permissions to the Journal folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dc758-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="dc758-135">Remarks</span></span>

<span data-ttu-id="dc758-136">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="dc758-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dc758-137">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="dc758-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dc758-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="dc758-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dc758-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="dc758-139">Schema Name</span></span>  <br/> |<span data-ttu-id="dc758-140">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="dc758-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="dc758-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="dc758-141">Validation File</span></span>  <br/> |<span data-ttu-id="dc758-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="dc758-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dc758-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="dc758-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="dc758-144">False</span><span class="sxs-lookup"><span data-stu-id="dc758-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dc758-145">Confira também</span><span class="sxs-lookup"><span data-stu-id="dc758-145">See also</span></span>



[<span data-ttu-id="dc758-146">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="dc758-146">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="dc758-147">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="dc758-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="dc758-148">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="dc758-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="dc758-149">Adicionar representantes</span><span class="sxs-lookup"><span data-stu-id="dc758-149">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

