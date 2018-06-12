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
description: O elemento de excluir identifica uma única pasta a ser excluído no repositório de cliente local.
ms.openlocfilehash: 5cad36c6fcff782195fdb285e2d3c4f3c5ec0f1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751725"
---
# <a name="delete-foldersync"></a><span data-ttu-id="f1713-103">Excluir (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="f1713-103">Delete (FolderSync)</span></span>

<span data-ttu-id="f1713-104">O elemento de **Excluir** identifica uma única pasta a ser excluído no repositório de cliente local.</span><span class="sxs-lookup"><span data-stu-id="f1713-104">The **Delete** element identifies a single folder to delete in the local client store.</span></span> 
  
- [<span data-ttu-id="f1713-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="f1713-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)  
- [<span data-ttu-id="f1713-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f1713-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="f1713-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f1713-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)  
- [<span data-ttu-id="f1713-108">Alterações (hierarquia)</span><span class="sxs-lookup"><span data-stu-id="f1713-108">Changes (Hierarchy)</span></span>](changes-hierarchy.md)  
- [<span data-ttu-id="f1713-109">Excluir (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="f1713-109">Delete (FolderSync)</span></span>](delete-foldersync.md)
  
```xml
<Delete>
   <FolderId/>
</Delete>
```

<span data-ttu-id="f1713-110">**SyncFolderHierarchyDeleteType**</span><span class="sxs-lookup"><span data-stu-id="f1713-110">**SyncFolderHierarchyDeleteType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f1713-111">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f1713-111">Attributes and elements</span></span>

<span data-ttu-id="f1713-112">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f1713-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f1713-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="f1713-113">Attributes</span></span>

<span data-ttu-id="f1713-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f1713-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f1713-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f1713-115">Child elements</span></span>

|<span data-ttu-id="f1713-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f1713-116">**Element**</span></span>|<span data-ttu-id="f1713-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f1713-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1713-118">FolderId</span><span class="sxs-lookup"><span data-stu-id="f1713-118">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="f1713-119">Contém o identificador e alterar a chave de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="f1713-119">Contains the identifier and change key of a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f1713-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f1713-120">Parent elements</span></span>

|<span data-ttu-id="f1713-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f1713-121">**Element**</span></span>|<span data-ttu-id="f1713-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f1713-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1713-123">Alterações (hierarquia)</span><span class="sxs-lookup"><span data-stu-id="f1713-123">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="f1713-124">Contém uma matriz sequenciada dos tipos de alteração que representam o tipo das diferenças entre as pastas no cliente e as pastas no computador que está executando o Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="f1713-124">Contains a sequenced array of change types that represent the type of differences between the folders on the client and the folders on the computer that is running Microsoft Exchange Server 2007.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f1713-125">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="f1713-125">Remarks</span></span>

<span data-ttu-id="f1713-126">O esquema que descreve este elemento está localizado no diretório virtual EWS do Exchange 2007 computador que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f1713-126">The schema that describes this element is located in the EWS virtual directory of the Exchange 2007 computer that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f1713-127">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f1713-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f1713-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="f1713-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f1713-129">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f1713-129">Schema name</span></span>  <br/> |<span data-ttu-id="f1713-130">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f1713-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="f1713-131">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f1713-131">Validation file</span></span>  <br/> |<span data-ttu-id="f1713-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f1713-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f1713-133">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="f1713-133">Can be empty</span></span>  <br/> |<span data-ttu-id="f1713-134">False</span><span class="sxs-lookup"><span data-stu-id="f1713-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f1713-135">Ver também</span><span class="sxs-lookup"><span data-stu-id="f1713-135">See also</span></span>

- [<span data-ttu-id="f1713-136">Operação SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="f1713-136">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)
- [<span data-ttu-id="f1713-137">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="f1713-137">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="f1713-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f1713-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

