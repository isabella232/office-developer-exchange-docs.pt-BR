---
title: Atualizações (pasta)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Updates
api_type:
- schema
ms.assetid: b047e3a4-a5ab-4098-b7a0-273bc809e702
description: O elemento updates contém um conjunto de elementos que definem Append, set e Delete alterações nas propriedades da pasta.
ms.openlocfilehash: 3282171dfc188a9d4735a19a97e80fe0e2f79b89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457176"
---
# <a name="updates-folder"></a><span data-ttu-id="b9a50-103">Atualizações (pasta)</span><span class="sxs-lookup"><span data-stu-id="b9a50-103">Updates (Folder)</span></span>

<span data-ttu-id="b9a50-104">O elemento **updates** contém um conjunto de elementos que definem Append, set e Delete alterações nas propriedades da pasta.</span><span class="sxs-lookup"><span data-stu-id="b9a50-104">The **Updates** element contains a set of elements that define append, set, and delete changes to folder properties.</span></span> 
  
- [<span data-ttu-id="b9a50-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="b9a50-105">UpdateFolder</span></span>](updatefolder.md)
  
- [<span data-ttu-id="b9a50-106">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="b9a50-106">FolderChanges</span></span>](folderchanges.md)
  
- [<span data-ttu-id="b9a50-107">FolderChange</span><span class="sxs-lookup"><span data-stu-id="b9a50-107">FolderChange</span></span>](folderchange.md)
  
- [<span data-ttu-id="b9a50-108">Atualizações (pasta)</span><span class="sxs-lookup"><span data-stu-id="b9a50-108">Updates (Folder)</span></span>](updates-folder.md)
  
```xml
<Updates>
   <AppendToFolderField/>
   <SetFolderField/>
   <DeleteFolderField/>
</Updates>
```

<span data-ttu-id="b9a50-109">**NonEmptyArrayOfFolderChangeDescriptionsType**</span><span class="sxs-lookup"><span data-stu-id="b9a50-109">**NonEmptyArrayOfFolderChangeDescriptionsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b9a50-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b9a50-110">Attributes and elements</span></span>

<span data-ttu-id="b9a50-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b9a50-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b9a50-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="b9a50-112">Attributes</span></span>

<span data-ttu-id="b9a50-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9a50-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b9a50-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b9a50-114">Child elements</span></span>

|<span data-ttu-id="b9a50-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b9a50-115">**Element**</span></span>|<span data-ttu-id="b9a50-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b9a50-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9a50-117">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="b9a50-117">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="b9a50-118">Representa os dados a serem acrescentados a uma propriedade Folder durante uma [operação UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="b9a50-118">Represents data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="b9a50-119">Setfolderfield</span><span class="sxs-lookup"><span data-stu-id="b9a50-119">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="b9a50-120">Representa uma atualização de uma única propriedade em uma pasta em uma [operação UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="b9a50-120">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="b9a50-121">DeleteFolderField</span><span class="sxs-lookup"><span data-stu-id="b9a50-121">DeleteFolderField</span></span>](deletefolderfield.md) <br/> |<span data-ttu-id="b9a50-122">Representa uma operação para excluir uma determinada propriedade de uma pasta durante uma [operação UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="b9a50-122">Represents an operation to delete a given property from a folder during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b9a50-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b9a50-123">Parent elements</span></span>

|<span data-ttu-id="b9a50-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b9a50-124">**Element**</span></span>|<span data-ttu-id="b9a50-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b9a50-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9a50-126">FolderChange</span><span class="sxs-lookup"><span data-stu-id="b9a50-126">FolderChange</span></span>](folderchange.md) <br/> |<span data-ttu-id="b9a50-127">Representa uma coleção de alterações a serem realizadas em uma única pasta.</span><span class="sxs-lookup"><span data-stu-id="b9a50-127">Represents a collection of changes to be performed on a single folder.</span></span>  <br/> <span data-ttu-id="b9a50-128">A seguir está a expressão XPath para este elemento:`/UpdateFolder/FolderChanges/FolderChange[i]`</span><span class="sxs-lookup"><span data-stu-id="b9a50-128">The following is the XPath expression to this element:  `/UpdateFolder/FolderChanges/FolderChange[i]`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b9a50-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="b9a50-129">Remarks</span></span>

<span data-ttu-id="b9a50-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="b9a50-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b9a50-131">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b9a50-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b9a50-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="b9a50-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b9a50-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b9a50-133">Schema Name</span></span>  <br/> |<span data-ttu-id="b9a50-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b9a50-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="b9a50-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b9a50-135">Validation File</span></span>  <br/> |<span data-ttu-id="b9a50-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b9a50-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b9a50-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b9a50-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="b9a50-138">False</span><span class="sxs-lookup"><span data-stu-id="b9a50-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b9a50-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="b9a50-139">See also</span></span>

- [<span data-ttu-id="b9a50-140">Operação UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="b9a50-140">UpdateFolder operation</span></span>](updatefolder-operation.md)
- [<span data-ttu-id="b9a50-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b9a50-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

