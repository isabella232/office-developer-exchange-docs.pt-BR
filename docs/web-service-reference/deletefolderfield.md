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
description: O elemento DeleteFolderField representa uma operação para excluir uma determinada propriedade de uma pasta durante uma chamada de UpdateFolder.
ms.openlocfilehash: 60d4a5c19d89c109913e83fea99c2f7910566c72
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354089"
---
# <a name="deletefolderfield"></a><span data-ttu-id="5bdb2-103">DeleteFolderField</span><span class="sxs-lookup"><span data-stu-id="5bdb2-103">DeleteFolderField</span></span>

<span data-ttu-id="5bdb2-104">O elemento **DeleteFolderField** representa uma operação para excluir uma determinada propriedade de uma pasta durante uma chamada de UpdateFolder.</span><span class="sxs-lookup"><span data-stu-id="5bdb2-104">The **DeleteFolderField** element represents an operation to delete a given property from a folder during an UpdateFolder call.</span></span> 
  
- [<span data-ttu-id="5bdb2-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="5bdb2-105">UpdateFolder</span></span>](updatefolder.md) 
- [<span data-ttu-id="5bdb2-106">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="5bdb2-106">FolderChanges</span></span>](folderchanges.md)  
- [<span data-ttu-id="5bdb2-107">FolderChange</span><span class="sxs-lookup"><span data-stu-id="5bdb2-107">FolderChange</span></span>](folderchange.md)  
- [<span data-ttu-id="5bdb2-108">Updates (Folder)</span><span class="sxs-lookup"><span data-stu-id="5bdb2-108">Updates (Folder)</span></span>](updates-folder.md) 
- [<span data-ttu-id="5bdb2-109">DeleteFolderField</span><span class="sxs-lookup"><span data-stu-id="5bdb2-109">DeleteFolderField</span></span>](deletefolderfield.md)
  
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

<span data-ttu-id="5bdb2-110">**DeleteFolderFieldType**</span><span class="sxs-lookup"><span data-stu-id="5bdb2-110">**DeleteFolderFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="5bdb2-111">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="5bdb2-111">Attributes and elements</span></span>

<span data-ttu-id="5bdb2-112">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5bdb2-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5bdb2-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="5bdb2-113">Attributes</span></span>

<span data-ttu-id="5bdb2-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5bdb2-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5bdb2-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5bdb2-115">Child elements</span></span>

|<span data-ttu-id="5bdb2-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5bdb2-116">**Element**</span></span>|<span data-ttu-id="5bdb2-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5bdb2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5bdb2-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="5bdb2-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="5bdb2-119">Identifica as propriedades frequentemente referenciadas pelo URI.</span><span class="sxs-lookup"><span data-stu-id="5bdb2-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="5bdb2-120">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="5bdb2-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="5bdb2-121">Identifica a membros individuais de uma propriedade de dicionário.</span><span class="sxs-lookup"><span data-stu-id="5bdb2-121">Identifies individual members of a dictionary property.</span></span>  <br/> |
|[<span data-ttu-id="5bdb2-122">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="5bdb2-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="5bdb2-123">Identifica as propriedades estendidas de MAPI.</span><span class="sxs-lookup"><span data-stu-id="5bdb2-123">Identifies extended MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5bdb2-124">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5bdb2-124">Parent elements</span></span>

|<span data-ttu-id="5bdb2-125">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="5bdb2-125">**Element**</span></span>|<span data-ttu-id="5bdb2-126">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="5bdb2-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5bdb2-127">Updates (Folder)</span><span class="sxs-lookup"><span data-stu-id="5bdb2-127">Updates (Folder)</span></span>](updates-folder.md) <br/> |<span data-ttu-id="5bdb2-128">Contém um conjunto de elementos que definem append, definir e excluir as alterações nas propriedades da pasta.</span><span class="sxs-lookup"><span data-stu-id="5bdb2-128">Contains a set of elements that define append, set, and delete changes to folder properties.</span></span>  <br/> <span data-ttu-id="5bdb2-129">Este é a expressão XPath para esse elemento:`/UpdateFolder/FolderChanges/FolderChange[i]/Updates`</span><span class="sxs-lookup"><span data-stu-id="5bdb2-129">The following is the XPath expression to this element:  `/UpdateFolder/FolderChanges/FolderChange[i]/Updates`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5bdb2-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="5bdb2-130">Remarks</span></span>

<span data-ttu-id="5bdb2-131">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="5bdb2-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5bdb2-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="5bdb2-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5bdb2-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="5bdb2-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5bdb2-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5bdb2-134">Schema Name</span></span>  <br/> |<span data-ttu-id="5bdb2-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5bdb2-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="5bdb2-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5bdb2-136">Validation File</span></span>  <br/> |<span data-ttu-id="5bdb2-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5bdb2-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5bdb2-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="5bdb2-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="5bdb2-139">False</span><span class="sxs-lookup"><span data-stu-id="5bdb2-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5bdb2-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="5bdb2-140">See also</span></span>

- [<span data-ttu-id="5bdb2-141">Operação UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="5bdb2-141">UpdateFolder operation</span></span>](updatefolder-operation.md)

