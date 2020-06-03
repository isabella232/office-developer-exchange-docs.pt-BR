---
title: Excluir (FolderSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- schema
ms.assetid: c4397d91-43ef-40a9-a80e-d31501a33caa
description: O elemento delete identifica uma única pasta a ser excluída no repositório do cliente local.
ms.openlocfilehash: 68f8687b8cf0723d7fd63a3d55da8ef7c2f98f8e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44454978"
---
# <a name="delete-foldersync"></a><span data-ttu-id="c9f32-103">Excluir (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="c9f32-103">Delete (FolderSync)</span></span>

<span data-ttu-id="c9f32-104">O elemento **delete** identifica uma única pasta a ser excluída no repositório do cliente local.</span><span class="sxs-lookup"><span data-stu-id="c9f32-104">The **Delete** element identifies a single folder to delete in the local client store.</span></span> 
  
- [<span data-ttu-id="c9f32-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="c9f32-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)  
- [<span data-ttu-id="c9f32-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c9f32-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="c9f32-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c9f32-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)  
- [<span data-ttu-id="c9f32-108">Alterações (hierarquia)</span><span class="sxs-lookup"><span data-stu-id="c9f32-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)  
- [<span data-ttu-id="c9f32-109">Excluir (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="c9f32-109">Delete (FolderSync)</span></span>](delete-foldersync.md)
  
```xml
<Delete>
   <FolderId/>
</Delete>
```

<span data-ttu-id="c9f32-110">**SyncFolderHierarchyDeleteType**</span><span class="sxs-lookup"><span data-stu-id="c9f32-110">**SyncFolderHierarchyDeleteType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c9f32-111">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c9f32-111">Attributes and elements</span></span>

<span data-ttu-id="c9f32-112">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c9f32-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9f32-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="c9f32-113">Attributes</span></span>

<span data-ttu-id="c9f32-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c9f32-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9f32-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c9f32-115">Child elements</span></span>

|<span data-ttu-id="c9f32-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c9f32-116">**Element**</span></span>|<span data-ttu-id="c9f32-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c9f32-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9f32-118">FolderId</span><span class="sxs-lookup"><span data-stu-id="c9f32-118">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="c9f32-119">Contém o identificador e a chave de alteração de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="c9f32-119">Contains the identifier and change key of a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c9f32-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c9f32-120">Parent elements</span></span>

|<span data-ttu-id="c9f32-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c9f32-121">**Element**</span></span>|<span data-ttu-id="c9f32-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c9f32-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9f32-123">Alterações (hierarquia)</span><span class="sxs-lookup"><span data-stu-id="c9f32-123">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="c9f32-124">Contém uma matriz em sequência de tipos de alteração que representam o tipo de diferença entre as pastas no cliente e as pastas no computador que está executando o Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="c9f32-124">Contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the computer that is running Microsoft Exchange Server 2007.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c9f32-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="c9f32-125">Remarks</span></span>

<span data-ttu-id="c9f32-126">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador Exchange 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="c9f32-126">The schema that describes this element is located in the EWS virtual directory of the Exchange 2007 computer that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c9f32-127">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c9f32-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9f32-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="c9f32-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c9f32-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c9f32-129">Schema name</span></span>  <br/> |<span data-ttu-id="c9f32-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c9f32-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="c9f32-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c9f32-131">Validation file</span></span>  <br/> |<span data-ttu-id="c9f32-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c9f32-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c9f32-133">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="c9f32-133">Can be empty</span></span>  <br/> |<span data-ttu-id="c9f32-134">False</span><span class="sxs-lookup"><span data-stu-id="c9f32-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c9f32-135">Confira também</span><span class="sxs-lookup"><span data-stu-id="c9f32-135">See also</span></span>

- [<span data-ttu-id="c9f32-136">Operação SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="c9f32-136">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)
- [<span data-ttu-id="c9f32-137">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="c9f32-137">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="c9f32-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c9f32-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

