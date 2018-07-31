---
title: ParentFolderId (TargetFolderIdType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentFolderId
api_type:
- schema
ms.assetid: 0e3e6e5f-06d0-499b-8ca4-d36036521658
description: O elemento ParentFolderId identifica a pasta na qual uma nova pasta é criada ou a pasta para pesquisar a operação FindConversation.
ms.openlocfilehash: 8e80b9b342274a8b2004838ebd16f8425a2d3fa3
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353823"
---
# <a name="parentfolderid-targetfolderidtype"></a><span data-ttu-id="afdff-103">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="afdff-103">ParentFolderId (TargetFolderIdType)</span></span>

<span data-ttu-id="afdff-104">O elemento **ParentFolderId** identifica a pasta na qual uma nova pasta é criada ou a pasta para pesquisar a [operação FindConversation](findconversation-operation.md).</span><span class="sxs-lookup"><span data-stu-id="afdff-104">The **ParentFolderId** element identifies the folder in which a new folder is created or the folder to search for the [FindConversation operation](findconversation-operation.md).</span></span>
  
```xml
<ParentFolderId>
   <DistinguishedFolderId/>
</ParentFolderId>
```

```xml
<ParentFolderId>
   <FolderId/> 
</ParentFolderId>
```

<span data-ttu-id="afdff-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="afdff-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="afdff-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="afdff-106">Attributes and elements</span></span>

<span data-ttu-id="afdff-107">O elemento **ParentFolderId** contém dois elementos filho.</span><span class="sxs-lookup"><span data-stu-id="afdff-107">The **ParentFolderId** element contains two child elements.</span></span> <span data-ttu-id="afdff-108">Os elementos filhos são mutuamente exclusivos no esquema.</span><span class="sxs-lookup"><span data-stu-id="afdff-108">The child elements are mutually exclusive in the schema.</span></span> 
  
### <a name="attributes"></a><span data-ttu-id="afdff-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="afdff-109">Attributes</span></span>

<span data-ttu-id="afdff-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="afdff-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="afdff-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="afdff-111">Child elements</span></span>

|<span data-ttu-id="afdff-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="afdff-112">**Element**</span></span>|<span data-ttu-id="afdff-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="afdff-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="afdff-114">FolderId</span><span class="sxs-lookup"><span data-stu-id="afdff-114">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="afdff-115">Contém o identificador necessário e a chave de alteração opcionais de uma pasta na qual uma nova pasta é criada ou a pasta que será pesquisada para a [operação FindConversation](findconversation-operation.md).</span><span class="sxs-lookup"><span data-stu-id="afdff-115">Contains the required identifier and the optional change key of a folder in which a new folder is created or the folder that is searched for the [FindConversation operation](findconversation-operation.md).</span></span> <span data-ttu-id="afdff-116">Usar esse elemento exclui o uso do elemento [DistinguishedFolderId](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="afdff-116">Using this element excludes the use of the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="afdff-117">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="afdff-117">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="afdff-118">Identifica as pastas padrão do Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="afdff-118">Identifies default Microsoft Exchange Server 2007 folders.</span></span> <span data-ttu-id="afdff-119">Usar esse elemento exclui o uso do elemento [FolderId](folderid.md) .</span><span class="sxs-lookup"><span data-stu-id="afdff-119">Using this element excludes the use of the [FolderId](folderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="afdff-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="afdff-120">Parent elements</span></span>

|<span data-ttu-id="afdff-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="afdff-121">**Element**</span></span>|<span data-ttu-id="afdff-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="afdff-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="afdff-123">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="afdff-123">CreateFolder</span></span>](createfolder.md) <br/> |<span data-ttu-id="afdff-124">Define uma solicitação para criar uma pasta do banco de dados do Exchange.</span><span class="sxs-lookup"><span data-stu-id="afdff-124">Defines a request to create a folder in the Exchange database.</span></span>  <br/> <span data-ttu-id="afdff-125">Este é a expressão XPath para esse elemento:`/CreateFolder`</span><span class="sxs-lookup"><span data-stu-id="afdff-125">The following is the XPath expression to this element:  `/CreateFolder`</span></span> <br/> |
|[<span data-ttu-id="afdff-126">FindConversation</span><span class="sxs-lookup"><span data-stu-id="afdff-126">FindConversation</span></span>](findconversation.md) <br/> |<span data-ttu-id="afdff-127">Define uma solicitação para localizar conversas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="afdff-127">Defines a request to find conversations in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="afdff-128">Text value</span><span class="sxs-lookup"><span data-stu-id="afdff-128">Text value</span></span>

<span data-ttu-id="afdff-129">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="afdff-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="afdff-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="afdff-130">Remarks</span></span>

<span data-ttu-id="afdff-131">Os elementos dois filhos são usados para definir a pasta que conterá a nova pasta.</span><span class="sxs-lookup"><span data-stu-id="afdff-131">The two child elements are used to define the folder that will contain the new folder.</span></span> <span data-ttu-id="afdff-132">Você deve selecionar o [FolderId](folderid.md) ou o elemento [DistinguishedFolderId](distinguishedfolderid.md) para identificar a pasta pai da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="afdff-132">You must select either the [FolderId](folderid.md) or the [DistinguishedFolderId](distinguishedfolderid.md) element to identify the parent folder of the new folder.</span></span> <span data-ttu-id="afdff-133">Você não pode usar ambos os elementos ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="afdff-133">You cannot use both elements at the same time.</span></span> <span data-ttu-id="afdff-134">Esse elemento é necessário para criar pastas.</span><span class="sxs-lookup"><span data-stu-id="afdff-134">This element is required to create folders.</span></span> 
  
<span data-ttu-id="afdff-135">O elemento [ParentFolderId](parentfolderid.md) descreve a localização de itens e pastas existentes.</span><span class="sxs-lookup"><span data-stu-id="afdff-135">The [ParentFolderId](parentfolderid.md) element describes the location of existing items and folders.</span></span> 
  
<span data-ttu-id="afdff-136">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="afdff-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="afdff-137">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="afdff-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="afdff-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="afdff-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="afdff-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="afdff-139">Schema Name</span></span>  <br/> |<span data-ttu-id="afdff-140">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="afdff-140">Message schema</span></span>  <br/> |
|<span data-ttu-id="afdff-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="afdff-141">Validation File</span></span>  <br/> |<span data-ttu-id="afdff-142">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="afdff-142">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="afdff-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="afdff-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="afdff-144">False</span><span class="sxs-lookup"><span data-stu-id="afdff-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="afdff-145">Ver também</span><span class="sxs-lookup"><span data-stu-id="afdff-145">See also</span></span>

- [<span data-ttu-id="afdff-146">Operação CreateFolder</span><span class="sxs-lookup"><span data-stu-id="afdff-146">CreateFolder operation</span></span>](createfolder-operation.md)
- [<span data-ttu-id="afdff-147">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="afdff-147">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="afdff-148">Criação de pastas (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="afdff-148">Creating Folders (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

