---
title: DeleteFolderField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolderField
api_type:
- schema
ms.assetid: f9c2187b-4c60-4358-b4b4-ede50eadae48
description: O elemento DeleteFolderField representa uma operação para excluir uma determinada propriedade de uma pasta durante uma chamada UpdateFolder.
ms.openlocfilehash: a0b48b667c8c8afbd5729d5deb84359a6a6ccc25
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462154"
---
# <a name="deletefolderfield"></a><span data-ttu-id="070f4-103">DeleteFolderField</span><span class="sxs-lookup"><span data-stu-id="070f4-103">DeleteFolderField</span></span>

<span data-ttu-id="070f4-104">O elemento **DeleteFolderField** representa uma operação para excluir uma determinada propriedade de uma pasta durante uma chamada UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="070f4-104">The **DeleteFolderField** element represents an operation to delete a given property from a folder during an UpdateFolder call.</span></span> 
  
- [<span data-ttu-id="070f4-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="070f4-105">UpdateFolder</span></span>](updatefolder.md) 
- [<span data-ttu-id="070f4-106">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="070f4-106">FolderChanges</span></span>](folderchanges.md)  
- [<span data-ttu-id="070f4-107">FolderChange</span><span class="sxs-lookup"><span data-stu-id="070f4-107">FolderChange</span></span>](folderchange.md)  
- [<span data-ttu-id="070f4-108">Atualizações (pasta)</span><span class="sxs-lookup"><span data-stu-id="070f4-108">Updates (Folder)</span></span>](updates-folder.md) 
- [<span data-ttu-id="070f4-109">DeleteFolderField</span><span class="sxs-lookup"><span data-stu-id="070f4-109">DeleteFolderField</span></span>](deletefolderfield.md)
  
```xml
<DeleteFolderField>
   <FieldURI/>
</DeleteFolderField>
```

```xml
<DeleteFolderField>
   <ExtendedFieldURI/>
</DeleteFolderField>
```

```xml
<DeleteFolderField>
   <IndexedFieldURI/>
</DeleteFolderField>
```

<span data-ttu-id="070f4-110">**DeleteFolderFieldType**</span><span class="sxs-lookup"><span data-stu-id="070f4-110">**DeleteFolderFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="070f4-111">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="070f4-111">Attributes and elements</span></span>

<span data-ttu-id="070f4-112">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="070f4-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="070f4-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="070f4-113">Attributes</span></span>

<span data-ttu-id="070f4-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="070f4-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="070f4-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="070f4-115">Child elements</span></span>

|<span data-ttu-id="070f4-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="070f4-116">**Element**</span></span>|<span data-ttu-id="070f4-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="070f4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="070f4-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="070f4-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="070f4-119">Identifica as propriedades com frequência referenciadas por URI.</span><span class="sxs-lookup"><span data-stu-id="070f4-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="070f4-120">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="070f4-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="070f4-121">Identifica membros individuais de uma propriedade de dicionário.</span><span class="sxs-lookup"><span data-stu-id="070f4-121">Identifies individual members of a dictionary property.</span></span>  <br/> |
|[<span data-ttu-id="070f4-122">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="070f4-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="070f4-123">Identifica as propriedades de MAPI estendidas.</span><span class="sxs-lookup"><span data-stu-id="070f4-123">Identifies extended MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="070f4-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="070f4-124">Parent elements</span></span>

|<span data-ttu-id="070f4-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="070f4-125">**Element**</span></span>|<span data-ttu-id="070f4-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="070f4-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="070f4-127">Atualizações (pasta)</span><span class="sxs-lookup"><span data-stu-id="070f4-127">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="070f4-128">Contém um conjunto de elementos que definem Append, set e Delete alterações nas propriedades da pasta.</span><span class="sxs-lookup"><span data-stu-id="070f4-128">Contains a set of elements that define append, set, and delete changes to folder properties.</span></span>  <br/> <span data-ttu-id="070f4-129">A seguir está a expressão XPath para este elemento:`/UpdateFolder/FolderChanges/FolderChange[i]/Updates`</span><span class="sxs-lookup"><span data-stu-id="070f4-129">The following is the XPath expression to this element:  `/UpdateFolder/FolderChanges/FolderChange[i]/Updates`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="070f4-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="070f4-130">Remarks</span></span>

<span data-ttu-id="070f4-131">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="070f4-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="070f4-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="070f4-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="070f4-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="070f4-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="070f4-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="070f4-134">Schema Name</span></span>  <br/> |<span data-ttu-id="070f4-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="070f4-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="070f4-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="070f4-136">Validation File</span></span>  <br/> |<span data-ttu-id="070f4-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="070f4-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="070f4-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="070f4-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="070f4-139">False</span><span class="sxs-lookup"><span data-stu-id="070f4-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="070f4-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="070f4-140">See also</span></span>

- [<span data-ttu-id="070f4-141">Operação UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="070f4-141">UpdateFolder operation</span></span>](updatefolder-operation.md)

