---
title: NotesFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NotesFolderPermissionLevel
api_type:
- schema
ms.assetid: 76a2520c-f453-4fd7-b3eb-1c5f4666680a
description: O elemento NotesFolderPermissionLevel contém as permissões para a pasta de anotações padrão. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: dd8644210692e0c342079d055ddf00b8d9283d7d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824552"
---
# <a name="notesfolderpermissionlevel"></a><span data-ttu-id="f6c57-104">NotesFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="f6c57-104">NotesFolderPermissionLevel</span></span>

<span data-ttu-id="f6c57-105">O elemento **NotesFolderPermissionLevel** contém as permissões para a pasta de anotações padrão.</span><span class="sxs-lookup"><span data-stu-id="f6c57-105">The **NotesFolderPermissionLevel** element contains the permissions for the default Notes folder.</span></span> <span data-ttu-id="f6c57-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f6c57-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<NotesFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</NotesFolderPermissionLevel>
```

 <span data-ttu-id="f6c57-107">**DelegateFolderPermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="f6c57-107">**DelegateFolderPermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f6c57-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f6c57-108">Attributes and elements</span></span>

<span data-ttu-id="f6c57-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f6c57-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f6c57-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="f6c57-110">Attributes</span></span>

<span data-ttu-id="f6c57-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f6c57-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f6c57-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f6c57-112">Child elements</span></span>

<span data-ttu-id="f6c57-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f6c57-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f6c57-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f6c57-114">Parent elements</span></span>

|<span data-ttu-id="f6c57-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f6c57-115">**Element**</span></span>|<span data-ttu-id="f6c57-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f6c57-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6c57-117">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="f6c57-117">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="f6c57-118">Contém as configurações de nível de permissão do representante de um usuário.</span><span class="sxs-lookup"><span data-stu-id="f6c57-118">Contains the delegate permission level settings for a user.</span></span> <span data-ttu-id="f6c57-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="f6c57-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f6c57-120">Text value</span><span class="sxs-lookup"><span data-stu-id="f6c57-120">Text value</span></span>

<span data-ttu-id="f6c57-121">A tabela a seguir lista os valores de texto que representam os níveis de permissão.</span><span class="sxs-lookup"><span data-stu-id="f6c57-121">The following table lists the text values that represent the permission levels.</span></span>
  
<span data-ttu-id="f6c57-122">**Valores de texto de nível de permissão**</span><span class="sxs-lookup"><span data-stu-id="f6c57-122">**Permission level text values**</span></span>

|<span data-ttu-id="f6c57-123">**Nível de permissão**</span><span class="sxs-lookup"><span data-stu-id="f6c57-123">**Permission level**</span></span>|<span data-ttu-id="f6c57-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f6c57-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f6c57-125">None</span><span class="sxs-lookup"><span data-stu-id="f6c57-125">None</span></span>  <br/> |<span data-ttu-id="f6c57-126">O usuário delegado não tem nenhuma permissão de acesso para a pasta anotações.</span><span class="sxs-lookup"><span data-stu-id="f6c57-126">The delegate user has no access permissions to the Notes folder.</span></span>  <br/> |
|<span data-ttu-id="f6c57-127">Reviewer</span><span class="sxs-lookup"><span data-stu-id="f6c57-127">Reviewer</span></span>  <br/> |<span data-ttu-id="f6c57-128">O usuário delegado pode ler itens na pasta anotações.</span><span class="sxs-lookup"><span data-stu-id="f6c57-128">The delegate user can read items in the Notes folder.</span></span>  <br/> |
|<span data-ttu-id="f6c57-129">Autor</span><span class="sxs-lookup"><span data-stu-id="f6c57-129">Author</span></span>  <br/> |<span data-ttu-id="f6c57-130">O usuário delegado pode ler e criar itens na pasta anotações.</span><span class="sxs-lookup"><span data-stu-id="f6c57-130">The delegate user can read and create items in the Notes folder.</span></span>  <br/> |
|<span data-ttu-id="f6c57-131">Editor</span><span class="sxs-lookup"><span data-stu-id="f6c57-131">Editor</span></span>  <br/> |<span data-ttu-id="f6c57-132">O usuário delegado pode ler, criar e modificar itens na pasta anotações.</span><span class="sxs-lookup"><span data-stu-id="f6c57-132">The delegate user can read, create, and modify items in the Notes folder.</span></span>  <br/> |
|<span data-ttu-id="f6c57-133">Personalizado</span><span class="sxs-lookup"><span data-stu-id="f6c57-133">Custom</span></span>  <br/> |<span data-ttu-id="f6c57-134">O usuário delegado tem permissões de acesso personalizada para a pasta anotações.</span><span class="sxs-lookup"><span data-stu-id="f6c57-134">The delegate user has custom access permissions to the Notes folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f6c57-135">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="f6c57-135">Remarks</span></span>

<span data-ttu-id="f6c57-136">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f6c57-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f6c57-137">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f6c57-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f6c57-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="f6c57-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f6c57-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f6c57-139">Schema Name</span></span>  <br/> |<span data-ttu-id="f6c57-140">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f6c57-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="f6c57-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f6c57-141">Validation File</span></span>  <br/> |<span data-ttu-id="f6c57-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f6c57-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f6c57-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f6c57-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="f6c57-144">False</span><span class="sxs-lookup"><span data-stu-id="f6c57-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f6c57-145">Ver também</span><span class="sxs-lookup"><span data-stu-id="f6c57-145">See also</span></span>



[<span data-ttu-id="f6c57-146">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="f6c57-146">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="f6c57-147">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="f6c57-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="f6c57-148">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f6c57-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="f6c57-149">Adicionando representantes</span><span class="sxs-lookup"><span data-stu-id="f6c57-149">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

