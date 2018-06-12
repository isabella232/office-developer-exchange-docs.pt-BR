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
description: O elemento Updates contém um conjunto de elementos que definem append, definir e excluir as alterações nas propriedades da pasta.
ms.openlocfilehash: 31f25b1e88fb8756f189a6d75259dd4fc198582f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837939"
---
# <a name="updates-folder"></a><span data-ttu-id="f8ba7-103">Atualizações (pasta)</span><span class="sxs-lookup"><span data-stu-id="f8ba7-103">Updates (Folder)</span></span>

<span data-ttu-id="f8ba7-104">O elemento **Updates** contém um conjunto de elementos que definem append, definir e excluir as alterações nas propriedades da pasta.</span><span class="sxs-lookup"><span data-stu-id="f8ba7-104">The **Updates** element contains a set of elements that define append, set, and delete changes to folder properties.</span></span> 
  
- [<span data-ttu-id="f8ba7-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="f8ba7-105">UpdateFolder</span></span>](updatefolder.md)
  
- [<span data-ttu-id="f8ba7-106">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="f8ba7-106">FolderChanges</span></span>](folderchanges.md)
  
- [<span data-ttu-id="f8ba7-107">FolderChange</span><span class="sxs-lookup"><span data-stu-id="f8ba7-107">FolderChange</span></span>](folderchange.md)
  
- [<span data-ttu-id="f8ba7-108">Atualizações (pasta)</span><span class="sxs-lookup"><span data-stu-id="f8ba7-108">Updates (Folder)</span></span>](updates-folder.md)
  
```xml
<Updates>
   <AppendToFolderField/>
   <SetFolderField/>
   <DeleteFolderField/>
</Updates>
```

<span data-ttu-id="f8ba7-109">**NonEmptyArrayOfFolderChangeDescriptionsType**</span><span class="sxs-lookup"><span data-stu-id="f8ba7-109">**NonEmptyArrayOfFolderChangeDescriptionsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f8ba7-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f8ba7-110">Attributes and elements</span></span>

<span data-ttu-id="f8ba7-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f8ba7-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f8ba7-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="f8ba7-112">Attributes</span></span>

<span data-ttu-id="f8ba7-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f8ba7-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f8ba7-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f8ba7-114">Child elements</span></span>

|<span data-ttu-id="f8ba7-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f8ba7-115">**Element**</span></span>|<span data-ttu-id="f8ba7-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f8ba7-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f8ba7-117">AppendToFolderField</span><span class="sxs-lookup"><span data-stu-id="f8ba7-117">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="f8ba7-118">Representa os dados a serem acrescentados a uma propriedade de pasta durante uma [operação UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="f8ba7-118">Represents data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="f8ba7-119">SetFolderField</span><span class="sxs-lookup"><span data-stu-id="f8ba7-119">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="f8ba7-120">Representa uma atualização para uma única propriedade em uma pasta em uma [operação UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="f8ba7-120">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="f8ba7-121">DeleteFolderField</span><span class="sxs-lookup"><span data-stu-id="f8ba7-121">DeleteFolderField</span></span>](deletefolderfield.md) <br/> |<span data-ttu-id="f8ba7-122">Representa uma operação para excluir uma determinada propriedade de uma pasta durante uma [operação UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="f8ba7-122">Represents an operation to delete a given property from a folder during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f8ba7-123">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f8ba7-123">Parent elements</span></span>

|<span data-ttu-id="f8ba7-124">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f8ba7-124">**Element**</span></span>|<span data-ttu-id="f8ba7-125">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f8ba7-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f8ba7-126">FolderChange</span><span class="sxs-lookup"><span data-stu-id="f8ba7-126">FolderChange</span></span>](folderchange.md) <br/> |<span data-ttu-id="f8ba7-127">Representa uma coleção de alterações a serem realizadas em uma única pasta.</span><span class="sxs-lookup"><span data-stu-id="f8ba7-127">Represents a collection of changes to be performed on a single folder.</span></span>  <br/> <span data-ttu-id="f8ba7-128">Este é a expressão XPath para esse elemento:`/UpdateFolder/FolderChanges/FolderChange[i]`</span><span class="sxs-lookup"><span data-stu-id="f8ba7-128">The following is the XPath expression to this element:  `/UpdateFolder/FolderChanges/FolderChange[i]`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f8ba7-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="f8ba7-129">Remarks</span></span>

<span data-ttu-id="f8ba7-130">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="f8ba7-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f8ba7-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f8ba7-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f8ba7-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="f8ba7-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f8ba7-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f8ba7-133">Schema Name</span></span>  <br/> |<span data-ttu-id="f8ba7-134">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f8ba7-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="f8ba7-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f8ba7-135">Validation File</span></span>  <br/> |<span data-ttu-id="f8ba7-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f8ba7-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f8ba7-137">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f8ba7-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="f8ba7-138">False</span><span class="sxs-lookup"><span data-stu-id="f8ba7-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f8ba7-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="f8ba7-139">See also</span></span>

- [<span data-ttu-id="f8ba7-140">Operação UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="f8ba7-140">UpdateFolder operation</span></span>](updatefolder-operation.md)
- [<span data-ttu-id="f8ba7-141">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f8ba7-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

