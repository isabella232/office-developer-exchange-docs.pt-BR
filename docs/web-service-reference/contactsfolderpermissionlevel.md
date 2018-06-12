---
title: ContactsFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContactsFolderPermissionLevel
api_type:
- schema
ms.assetid: 805f05e7-b320-436a-9965-ba1ee235ac41
description: O elemento ContactsFolderPermissionLevel contém as permissões para a pasta padrão Contatos. Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 4b6a109c3a38a20dc5d6f611607b16ada0e4e46b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751452"
---
# <a name="contactsfolderpermissionlevel"></a><span data-ttu-id="6e151-104">ContactsFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="6e151-104">ContactsFolderPermissionLevel</span></span>

<span data-ttu-id="6e151-105">O elemento **ContactsFolderPermissionLevel** contém as permissões para a pasta padrão Contatos.</span><span class="sxs-lookup"><span data-stu-id="6e151-105">The **ContactsFolderPermissionLevel** element contains the permissions for the default Contacts folder.</span></span> <span data-ttu-id="6e151-106">Este elemento foi introduzido no Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6e151-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ContactsFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</ContactsFolderPermissionLevel>
```

 <span data-ttu-id="6e151-107">**DelegateFolderPermissionLevelType**</span><span class="sxs-lookup"><span data-stu-id="6e151-107">**DelegateFolderPermissionLevelType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e151-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="6e151-108">Attributes and elements</span></span>

<span data-ttu-id="6e151-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6e151-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e151-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="6e151-110">Attributes</span></span>

<span data-ttu-id="6e151-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6e151-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e151-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6e151-112">Child elements</span></span>

<span data-ttu-id="6e151-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="6e151-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6e151-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6e151-114">Parent elements</span></span>

|<span data-ttu-id="6e151-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6e151-115">**Element**</span></span>|<span data-ttu-id="6e151-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6e151-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e151-117">DelegatePermissions</span><span class="sxs-lookup"><span data-stu-id="6e151-117">DelegatePermissions</span></span>](delegatepermissions.md) <br/> |<span data-ttu-id="6e151-118">Contém as configurações de nível de permissão do representante de um usuário.</span><span class="sxs-lookup"><span data-stu-id="6e151-118">Contains the delegate permission level settings for a user.</span></span> <span data-ttu-id="6e151-119">Este elemento foi introduzido no Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="6e151-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6e151-120">Text value</span><span class="sxs-lookup"><span data-stu-id="6e151-120">Text value</span></span>

<span data-ttu-id="6e151-121">A tabela a seguir lista os valores de texto que representam os níveis de permissão.</span><span class="sxs-lookup"><span data-stu-id="6e151-121">The following table lists the text values that represent the permission levels.</span></span>
  
<span data-ttu-id="6e151-122">**Valores de texto de nível de permissão**</span><span class="sxs-lookup"><span data-stu-id="6e151-122">**Permission level text values**</span></span>

|<span data-ttu-id="6e151-123">**Nível de permissão**</span><span class="sxs-lookup"><span data-stu-id="6e151-123">**Permission level**</span></span>|<span data-ttu-id="6e151-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6e151-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6e151-125">None</span><span class="sxs-lookup"><span data-stu-id="6e151-125">None</span></span>  <br/> |<span data-ttu-id="6e151-126">O usuário delegado não tem nenhuma permissão de acesso à pasta Contatos.</span><span class="sxs-lookup"><span data-stu-id="6e151-126">The delegate user has no access permissions to the Contacts folder.</span></span>  <br/> |
|<span data-ttu-id="6e151-127">Reviewer</span><span class="sxs-lookup"><span data-stu-id="6e151-127">Reviewer</span></span>  <br/> |<span data-ttu-id="6e151-128">O usuário delegado pode ler itens na pasta Contatos.</span><span class="sxs-lookup"><span data-stu-id="6e151-128">The delegate user can read items in the Contacts folder.</span></span>  <br/> |
|<span data-ttu-id="6e151-129">Autor</span><span class="sxs-lookup"><span data-stu-id="6e151-129">Author</span></span>  <br/> |<span data-ttu-id="6e151-130">O usuário delegado pode ler e criar itens na pasta Contatos.</span><span class="sxs-lookup"><span data-stu-id="6e151-130">The delegate user can read and create items in the Contacts folder.</span></span>  <br/> |
|<span data-ttu-id="6e151-131">Editor</span><span class="sxs-lookup"><span data-stu-id="6e151-131">Editor</span></span>  <br/> |<span data-ttu-id="6e151-132">O usuário delegado pode ler, criar e modificar itens na pasta Contatos.</span><span class="sxs-lookup"><span data-stu-id="6e151-132">The delegate user can read, create, and modify items in the Contacts folder.</span></span>  <br/> |
|<span data-ttu-id="6e151-133">Personalizado</span><span class="sxs-lookup"><span data-stu-id="6e151-133">Custom</span></span>  <br/> |<span data-ttu-id="6e151-134">O usuário delegado tem permissões de acesso personalizada para a pasta Contatos.</span><span class="sxs-lookup"><span data-stu-id="6e151-134">The delegate user has custom access permissions to the Contacts folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6e151-135">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="6e151-135">Remarks</span></span>

<span data-ttu-id="6e151-136">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="6e151-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e151-137">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="6e151-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e151-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="6e151-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6e151-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6e151-139">Schema Name</span></span>  <br/> |<span data-ttu-id="6e151-140">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="6e151-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="6e151-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6e151-141">Validation File</span></span>  <br/> |<span data-ttu-id="6e151-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6e151-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6e151-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="6e151-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="6e151-144">False</span><span class="sxs-lookup"><span data-stu-id="6e151-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6e151-145">Ver também</span><span class="sxs-lookup"><span data-stu-id="6e151-145">See also</span></span>



[<span data-ttu-id="6e151-146">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="6e151-146">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="6e151-147">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="6e151-147">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="6e151-148">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6e151-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="6e151-149">Adicionando representantes</span><span class="sxs-lookup"><span data-stu-id="6e151-149">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

