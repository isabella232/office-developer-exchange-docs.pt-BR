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
ms.openlocfilehash: e4a025bef100fdd478be545b6448b15886e47c60
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530236"
---
# <a name="folderchange"></a><span data-ttu-id="26f0f-103">FolderChange</span><span class="sxs-lookup"><span data-stu-id="26f0f-103">FolderChange</span></span>

<span data-ttu-id="26f0f-104">O elemento **FolderChange** representa uma coleção de alterações a serem realizadas em uma única pasta.</span><span class="sxs-lookup"><span data-stu-id="26f0f-104">The **FolderChange** element represents a collection of changes to be performed on a single folder.</span></span> 
  
- [<span data-ttu-id="26f0f-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="26f0f-105">UpdateFolder</span></span>](updatefolder.md) 
- [<span data-ttu-id="26f0f-106">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="26f0f-106">FolderChanges</span></span>](folderchanges.md) 
- [<span data-ttu-id="26f0f-107">FolderChange</span><span class="sxs-lookup"><span data-stu-id="26f0f-107">FolderChange</span></span>](folderchange.md)
  
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

<span data-ttu-id="26f0f-108">**FolderChangeType**</span><span class="sxs-lookup"><span data-stu-id="26f0f-108">**FolderChangeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="26f0f-109">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="26f0f-109">Attributes and elements</span></span>

<span data-ttu-id="26f0f-110">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="26f0f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26f0f-111">Atributos</span><span class="sxs-lookup"><span data-stu-id="26f0f-111">Attributes</span></span>

<span data-ttu-id="26f0f-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="26f0f-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="26f0f-113">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="26f0f-113">Child elements</span></span>

|<span data-ttu-id="26f0f-114">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="26f0f-114">**Element**</span></span>|<span data-ttu-id="26f0f-115">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="26f0f-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26f0f-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="26f0f-116">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="26f0f-117">Contém o identificador e a chave de alteração de uma pasta a ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="26f0f-117">Contains the identifier and change key of a folder to update.</span></span>  <br/> |
|[<span data-ttu-id="26f0f-118">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="26f0f-118">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="26f0f-119">Identifica as pastas do MicrosoftExchange Server 2007 que podem ser referenciadas por nome.</span><span class="sxs-lookup"><span data-stu-id="26f0f-119">Identifies MicrosoftExchange Server 2007 folders that can be referenced by name.</span></span>  <br/> |
|[<span data-ttu-id="26f0f-120">Atualizações (pasta)</span><span class="sxs-lookup"><span data-stu-id="26f0f-120">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="26f0f-121">Define o tipo de atualização que é executada em uma pasta que é identificada pelo elemento [FolderId](folderid.md) ou [DistinguishedFolderId](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="26f0f-121">Defines the type of update that is performed on a folder that is identified by either the [FolderId](folderid.md) or [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="26f0f-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="26f0f-122">Parent elements</span></span>

|<span data-ttu-id="26f0f-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="26f0f-123">**Element**</span></span>|<span data-ttu-id="26f0f-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="26f0f-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26f0f-125">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="26f0f-125">FolderChanges</span></span>](folderchanges.md) <br/> |<span data-ttu-id="26f0f-126">Representa uma coleção de alterações para uma pasta.</span><span class="sxs-lookup"><span data-stu-id="26f0f-126">Represents a collection of changes for a folder.</span></span>  <br/> <span data-ttu-id="26f0f-127">A seguir está a expressão XPath para este elemento:</span><span class="sxs-lookup"><span data-stu-id="26f0f-127">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateFolder/FolderChanges` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="26f0f-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="26f0f-128">Remarks</span></span>

<span data-ttu-id="26f0f-129">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="26f0f-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26f0f-130">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="26f0f-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26f0f-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="26f0f-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="26f0f-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="26f0f-132">Schema name</span></span>  <br/> |<span data-ttu-id="26f0f-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="26f0f-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="26f0f-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="26f0f-134">Validation file</span></span>  <br/> |<span data-ttu-id="26f0f-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="26f0f-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="26f0f-136">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="26f0f-136">Can be empty</span></span>  <br/> |<span data-ttu-id="26f0f-137">False</span><span class="sxs-lookup"><span data-stu-id="26f0f-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="26f0f-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="26f0f-138">See also</span></span>

- [<span data-ttu-id="26f0f-139">Operação UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="26f0f-139">UpdateFolder operation</span></span>](updatefolder-operation.md)

