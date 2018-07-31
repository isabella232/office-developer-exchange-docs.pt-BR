---
title: FolderChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderChange
api_type:
- schema
ms.assetid: 23279750-131b-4e1a-b7d1-be235c4e0891
description: O elemento FolderChange representa uma coleção de alterações a serem realizadas em uma única pasta.
ms.openlocfilehash: f25defa9974f7b5dd0c683c7657983741890d45d
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354327"
---
# <a name="folderchange"></a><span data-ttu-id="243f1-103">FolderChange</span><span class="sxs-lookup"><span data-stu-id="243f1-103">FolderChange</span></span>

<span data-ttu-id="243f1-104">O elemento **FolderChange** representa uma coleção de alterações a serem realizadas em uma única pasta.</span><span class="sxs-lookup"><span data-stu-id="243f1-104">The **FolderChange** element represents a collection of changes to be performed on a single folder.</span></span> 
  
- [<span data-ttu-id="243f1-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="243f1-105">UpdateFolder</span></span>](updatefolder.md) 
- [<span data-ttu-id="243f1-106">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="243f1-106">FolderChanges</span></span>](folderchanges.md) 
- [<span data-ttu-id="243f1-107">FolderChange</span><span class="sxs-lookup"><span data-stu-id="243f1-107">FolderChange</span></span>](folderchange.md)
  
```xml
<FolderChange>
   <FolderId/>
   <Updates/>
</FolderChange>
```

```xml
<FolderChange>
   <DistinguishedFolderId/>
   <Updates/>
</FolderChange>
```

<span data-ttu-id="243f1-108">**FolderChangeType**</span><span class="sxs-lookup"><span data-stu-id="243f1-108">**FolderChangeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="243f1-109">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="243f1-109">Attributes and elements</span></span>

<span data-ttu-id="243f1-110">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="243f1-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="243f1-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="243f1-111">Attributes</span></span>

<span data-ttu-id="243f1-112">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="243f1-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="243f1-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="243f1-113">Child elements</span></span>

|<span data-ttu-id="243f1-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="243f1-114">**Element**</span></span>|<span data-ttu-id="243f1-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="243f1-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="243f1-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="243f1-116">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="243f1-117">Contém o identificador e alterar a chave de uma pasta a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="243f1-117">Contains the identifier and change key of a folder to update.</span></span>  <br/> |
|[<span data-ttu-id="243f1-118">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="243f1-118">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="243f1-119">Identifica as pastas de MicrosoftExchange Server 2007 que podem ser referidas por nome.</span><span class="sxs-lookup"><span data-stu-id="243f1-119">Identifies MicrosoftExchange Server 2007 folders that can be referenced by name.</span></span>  <br/> |
|[<span data-ttu-id="243f1-120">Updates (Folder)</span><span class="sxs-lookup"><span data-stu-id="243f1-120">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="243f1-121">Define o tipo de atualização que é executada em uma pasta que é identificada pela elemento o [FolderId](folderid.md) ou [DistinguishedFolderId](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="243f1-121">Defines the type of update that is performed on a folder that is identified by either the [FolderId](folderid.md) or [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="243f1-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="243f1-122">Parent elements</span></span>

|<span data-ttu-id="243f1-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="243f1-123">**Element**</span></span>|<span data-ttu-id="243f1-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="243f1-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="243f1-125">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="243f1-125">FolderChanges</span></span>](folderchanges.md) <br/> |<span data-ttu-id="243f1-126">Representa uma coleção das alterações de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="243f1-126">Represents a collection of changes for a folder.</span></span>  <br/> <span data-ttu-id="243f1-127">Este é a expressão XPath para esse elemento:</span><span class="sxs-lookup"><span data-stu-id="243f1-127">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateFolder/FolderChanges` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="243f1-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="243f1-128">Remarks</span></span>

<span data-ttu-id="243f1-129">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="243f1-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="243f1-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="243f1-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="243f1-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="243f1-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="243f1-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="243f1-132">Schema name</span></span>  <br/> |<span data-ttu-id="243f1-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="243f1-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="243f1-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="243f1-134">Validation file</span></span>  <br/> |<span data-ttu-id="243f1-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="243f1-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="243f1-136">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="243f1-136">Can be empty</span></span>  <br/> |<span data-ttu-id="243f1-137">False</span><span class="sxs-lookup"><span data-stu-id="243f1-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="243f1-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="243f1-138">See also</span></span>

- [<span data-ttu-id="243f1-139">Operação UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="243f1-139">UpdateFolder operation</span></span>](updatefolder-operation.md)

