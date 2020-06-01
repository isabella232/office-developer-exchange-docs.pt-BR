---
title: Alterações (hierarquia)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Changes
api_type:
- schema
ms.assetid: 918a0d1f-90a5-4eef-9592-07e15bef94e6
description: O elemento changes contém uma matriz em sequência de tipos de alteração que representam o tipo de diferença entre as pastas no cliente e as pastas no computador que está executando o Microsoft Exchange Server 2007.
ms.openlocfilehash: a296d87f23e85d42b4c8c858e92eddfb586a8324
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463269"
---
# <a name="changes-hierarchy"></a><span data-ttu-id="6bfc9-103">Alterações (hierarquia)</span><span class="sxs-lookup"><span data-stu-id="6bfc9-103">Changes (Hierarchy)</span></span>

<span data-ttu-id="6bfc9-104">O elemento **Changes** contém uma matriz em sequência de tipos de alteração que representam o tipo de diferença entre as pastas no cliente e as pastas no computador que está executando o Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="6bfc9-104">The **Changes** element contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the computer that is running Microsoft Exchange Server 2007.</span></span> 
  
[<span data-ttu-id="6bfc9-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="6bfc9-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
  
[<span data-ttu-id="6bfc9-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="6bfc9-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="6bfc9-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6bfc9-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
[<span data-ttu-id="6bfc9-108">Alterações (hierarquia)</span><span class="sxs-lookup"><span data-stu-id="6bfc9-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
  
```xml
<Changes>
   <Create/>
   <Update/>
   <Delete/>
</Changes>
```

 <span data-ttu-id="6bfc9-109">**SyncFolderHierarchyChangesType**</span><span class="sxs-lookup"><span data-stu-id="6bfc9-109">**SyncFolderHierarchyChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6bfc9-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="6bfc9-110">Attributes and elements</span></span>

<span data-ttu-id="6bfc9-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="6bfc9-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6bfc9-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="6bfc9-112">Attributes</span></span>

<span data-ttu-id="6bfc9-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6bfc9-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6bfc9-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="6bfc9-114">Child elements</span></span>

|<span data-ttu-id="6bfc9-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6bfc9-115">**Element**</span></span>|<span data-ttu-id="6bfc9-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6bfc9-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6bfc9-117">Criar (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="6bfc9-117">Create (FolderSync)</span></span>](create-foldersync.md) <br/> |<span data-ttu-id="6bfc9-118">Identifica uma única pasta a ser criada no armazenamento do cliente local.</span><span class="sxs-lookup"><span data-stu-id="6bfc9-118">Identifies a single folder to create in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="6bfc9-119">Atualização (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="6bfc9-119">Update (FolderSync)</span></span>](update-foldersync.md) <br/> |<span data-ttu-id="6bfc9-120">Identifica uma única pasta a ser atualizada no repositório do cliente local.</span><span class="sxs-lookup"><span data-stu-id="6bfc9-120">Identifies a single folder to update in the local client store.</span></span>  <br/> |
|[<span data-ttu-id="6bfc9-121">Excluir (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="6bfc9-121">Delete (FolderSync)</span></span>](delete-foldersync.md) <br/> |<span data-ttu-id="6bfc9-122">Identifica uma única pasta a ser excluída no repositório do cliente local.</span><span class="sxs-lookup"><span data-stu-id="6bfc9-122">Identifies a single folder to delete in the local client store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6bfc9-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="6bfc9-123">Parent elements</span></span>

|<span data-ttu-id="6bfc9-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6bfc9-124">**Element**</span></span>|<span data-ttu-id="6bfc9-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6bfc9-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6bfc9-126">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6bfc9-126">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md) <br/> |<span data-ttu-id="6bfc9-127">Contém o status e o resultado de uma solicitação SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="6bfc9-127">Contains the status and result of a SyncFolderHierarchy request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6bfc9-128">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="6bfc9-128">Text value</span></span>

<span data-ttu-id="6bfc9-129">Um valor de texto que representa um valor booliano é necessário.</span><span class="sxs-lookup"><span data-stu-id="6bfc9-129">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6bfc9-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="6bfc9-130">Remarks</span></span>

<span data-ttu-id="6bfc9-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador Exchange 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="6bfc9-131">The schema that describes this element is located in the EWS virtual directory of the Exchange 2007 computer that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6bfc9-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="6bfc9-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6bfc9-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="6bfc9-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6bfc9-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="6bfc9-134">Schema name</span></span>  <br/> |<span data-ttu-id="6bfc9-135">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="6bfc9-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6bfc9-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="6bfc9-136">Validation file</span></span>  <br/> |<span data-ttu-id="6bfc9-137">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6bfc9-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6bfc9-138">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="6bfc9-138">Can be empty</span></span>  <br/> |<span data-ttu-id="6bfc9-139">False</span><span class="sxs-lookup"><span data-stu-id="6bfc9-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6bfc9-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="6bfc9-140">See also</span></span>



[<span data-ttu-id="6bfc9-141">Operação SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="6bfc9-141">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


[<span data-ttu-id="6bfc9-142">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="6bfc9-142">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
  
- [<span data-ttu-id="6bfc9-143">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6bfc9-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

