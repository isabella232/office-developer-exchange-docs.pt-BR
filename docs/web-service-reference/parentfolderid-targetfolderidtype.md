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
ms.openlocfilehash: 61072e1dd3321beb5f3b76d9accf20530b443796
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824686"
---
# <a name="parentfolderid-targetfolderidtype"></a><span data-ttu-id="348dd-103">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="348dd-103">ParentFolderId (TargetFolderIdType)</span></span>

<span data-ttu-id="348dd-104">O elemento **ParentFolderId** identifica a pasta na qual uma nova pasta é criada ou a pasta para pesquisar a [operação FindConversation](findconversation-operation.md).</span><span class="sxs-lookup"><span data-stu-id="348dd-104">The **ParentFolderId** element identifies the folder in which a new folder is created or the folder to search for the [FindConversation operation](findconversation-operation.md).</span></span>
  
```xml
<ParentFolderId>
   <DistinguishedFolderId/>
</ParentFolderId>
```

<span data-ttu-id="348dd-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="348dd-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="348dd-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="348dd-106">Attributes and elements</span></span>

<span data-ttu-id="348dd-107">O elemento **ParentFolderId** contém dois elementos filho.</span><span class="sxs-lookup"><span data-stu-id="348dd-107">The **ParentFolderId** element contains two child elements.</span></span> <span data-ttu-id="348dd-108">Os elementos filhos são mutuamente exclusivos no esquema.</span><span class="sxs-lookup"><span data-stu-id="348dd-108">The child elements are mutually exclusive in the schema.</span></span> 
  
### <a name="attributes"></a><span data-ttu-id="348dd-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="348dd-109">Attributes</span></span>

<span data-ttu-id="348dd-110">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="348dd-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="348dd-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="348dd-111">Child elements</span></span>

|<span data-ttu-id="348dd-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="348dd-112">**Element**</span></span>|<span data-ttu-id="348dd-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="348dd-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="348dd-114">FolderId</span><span class="sxs-lookup"><span data-stu-id="348dd-114">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="348dd-115">Contém o identificador necessário e a chave de alteração opcionais de uma pasta na qual uma nova pasta é criada ou a pasta que será pesquisada para a [operação FindConversation](findconversation-operation.md).</span><span class="sxs-lookup"><span data-stu-id="348dd-115">Contains the required identifier and the optional change key of a folder in which a new folder is created or the folder that is searched for the [FindConversation operation](findconversation-operation.md).</span></span> <span data-ttu-id="348dd-116">Usar esse elemento exclui o uso do elemento [DistinguishedFolderId](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="348dd-116">Using this element excludes the use of the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="348dd-117">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="348dd-117">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="348dd-118">Identifica as pastas padrão do Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="348dd-118">Identifies default Microsoft Exchange Server 2007 folders.</span></span> <span data-ttu-id="348dd-119">Usar esse elemento exclui o uso do elemento [FolderId](folderid.md) .</span><span class="sxs-lookup"><span data-stu-id="348dd-119">Using this element excludes the use of the [FolderId](folderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="348dd-120">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="348dd-120">Parent elements</span></span>

|<span data-ttu-id="348dd-121">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="348dd-121">**Element**</span></span>|<span data-ttu-id="348dd-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="348dd-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="348dd-123">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="348dd-123">CreateFolder</span></span>](createfolder.md) <br/> |<span data-ttu-id="348dd-124">Define uma solicitação para criar uma pasta do banco de dados do Exchange.</span><span class="sxs-lookup"><span data-stu-id="348dd-124">Defines a request to create a folder in the Exchange database.</span></span>  <br/> <span data-ttu-id="348dd-125">Este é a expressão XPath para esse elemento:`/CreateFolder`</span><span class="sxs-lookup"><span data-stu-id="348dd-125">The following is the XPath expression to this element:  `/CreateFolder`</span></span> <br/> |
|[<span data-ttu-id="348dd-126">FindConversation</span><span class="sxs-lookup"><span data-stu-id="348dd-126">FindConversation</span></span>](findconversation.md) <br/> |<span data-ttu-id="348dd-127">Define uma solicitação para localizar conversas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="348dd-127">Defines a request to find conversations in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="348dd-128">Text value</span><span class="sxs-lookup"><span data-stu-id="348dd-128">Text value</span></span>

<span data-ttu-id="348dd-129">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="348dd-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="348dd-130">Comentários</span><span class="sxs-lookup"><span data-stu-id="348dd-130">Remarks</span></span>

<span data-ttu-id="348dd-131">Os elementos dois filhos são usados para definir a pasta que conterá a nova pasta.</span><span class="sxs-lookup"><span data-stu-id="348dd-131">The two child elements are used to define the folder that will contain the new folder.</span></span> <span data-ttu-id="348dd-132">Você deve selecionar o [FolderId](folderid.md) ou o elemento [DistinguishedFolderId](distinguishedfolderid.md) para identificar a pasta pai da nova pasta.</span><span class="sxs-lookup"><span data-stu-id="348dd-132">You must select either the [FolderId](folderid.md) or the [DistinguishedFolderId](distinguishedfolderid.md) element to identify the parent folder of the new folder.</span></span> <span data-ttu-id="348dd-133">Você não pode usar ambos os elementos ao mesmo tempo.</span><span class="sxs-lookup"><span data-stu-id="348dd-133">You cannot use both elements at the same time.</span></span> <span data-ttu-id="348dd-134">Esse elemento é necessário para criar pastas.</span><span class="sxs-lookup"><span data-stu-id="348dd-134">This element is required to create folders.</span></span> 
  
<span data-ttu-id="348dd-135">O elemento [ParentFolderId](parentfolderid.md) descreve a localização de itens e pastas existentes.</span><span class="sxs-lookup"><span data-stu-id="348dd-135">The [ParentFolderId](parentfolderid.md) element describes the location of existing items and folders.</span></span> 
  
<span data-ttu-id="348dd-136">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="348dd-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="348dd-137">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="348dd-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="348dd-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="348dd-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="348dd-139">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="348dd-139">Schema Name</span></span>  <br/> |<span data-ttu-id="348dd-140">Esquema de mensagem</span><span class="sxs-lookup"><span data-stu-id="348dd-140">Message schema</span></span>  <br/> |
|<span data-ttu-id="348dd-141">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="348dd-141">Validation File</span></span>  <br/> |<span data-ttu-id="348dd-142">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="348dd-142">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="348dd-143">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="348dd-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="348dd-144">False</span><span class="sxs-lookup"><span data-stu-id="348dd-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="348dd-145">Ver também</span><span class="sxs-lookup"><span data-stu-id="348dd-145">See also</span></span>

- [<span data-ttu-id="348dd-146">Operação CreateFolder</span><span class="sxs-lookup"><span data-stu-id="348dd-146">CreateFolder operation</span></span>](createfolder-operation.md)
- [<span data-ttu-id="348dd-147">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="348dd-147">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="348dd-148">Criação de pastas (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="348dd-148">Creating Folders (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

