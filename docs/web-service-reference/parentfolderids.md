---
title: ParentFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentFolderIds
api_type:
- schema
ms.assetid: e7998023-e5e0-465c-91fa-2aa6d1559f64
description: O elemento ParentFolderIds identifica pastas para as operações FindItem e FindFolder a serem pesquisadas.
ms.openlocfilehash: 6bc4b9cfe96c6c83cbeb623ec176e33177356bbc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465426"
---
# <a name="parentfolderids"></a><span data-ttu-id="06a85-103">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="06a85-103">ParentFolderIds</span></span>

<span data-ttu-id="06a85-104">O elemento **ParentFolderIds** identifica pastas para as operações FindItem e FindFolder a serem pesquisadas.</span><span class="sxs-lookup"><span data-stu-id="06a85-104">The **ParentFolderIds** element identifies folders for the FindItem and FindFolder operations to search.</span></span> 
  
```xml
<ParentFolderIds>
   <DistinguishedFolderId/>
<ParentFolderIds>
```

```xml
<ParentFolderIds>
   <FolderId/> 
<ParentFolderIds>
```

<span data-ttu-id="06a85-105">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="06a85-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="06a85-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="06a85-106">Attributes and elements</span></span>

<span data-ttu-id="06a85-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="06a85-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="06a85-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="06a85-108">Attributes</span></span>

<span data-ttu-id="06a85-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="06a85-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="06a85-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="06a85-110">Child elements</span></span>

|<span data-ttu-id="06a85-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="06a85-111">**Element**</span></span>|<span data-ttu-id="06a85-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="06a85-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06a85-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="06a85-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="06a85-114">Contém o identificador e a chave de alteração de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="06a85-114">Contains the identifier and change key of a folder.</span></span> <span data-ttu-id="06a85-115">O elemento **ParentFolderIds** deve usar esse elemento ou o elemento [DistinguishedFolderId](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="06a85-115">The **ParentFolderIds** element must use either this element or the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="06a85-116">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="06a85-116">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="06a85-117">Identifica as pastas do Microsoft Exchange Server 2007 que podem ser referenciadas por nome.</span><span class="sxs-lookup"><span data-stu-id="06a85-117">Identifies Microsoft Exchange Server 2007 folders that can be referenced by name.</span></span> <span data-ttu-id="06a85-118">O elemento **ParentFolderIds** deve usar este elemento ou o elemento [FolderId](folderid.md) .</span><span class="sxs-lookup"><span data-stu-id="06a85-118">The **ParentFolderIds** element must use either this element or the [FolderId](folderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="06a85-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="06a85-119">Parent elements</span></span>

|<span data-ttu-id="06a85-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="06a85-120">**Element**</span></span>|<span data-ttu-id="06a85-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="06a85-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="06a85-122">FindFolder</span><span class="sxs-lookup"><span data-stu-id="06a85-122">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="06a85-123">Define uma solicitação para identificar pastas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="06a85-123">Defines a request to identify folders in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="06a85-124">FindItem</span><span class="sxs-lookup"><span data-stu-id="06a85-124">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="06a85-125">Define uma solicitação para localizar itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="06a85-125">Defines a request to find items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="06a85-126">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="06a85-126">ResolveNames</span></span>](resolvenames.md) <br/> |<span data-ttu-id="06a85-127">Define uma solicitação para resolver nomes ambíguos.</span><span class="sxs-lookup"><span data-stu-id="06a85-127">Defines a request to resolve ambiguous names.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="06a85-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="06a85-128">Remarks</span></span>

<span data-ttu-id="06a85-129">O elemento **ParentFolderIds** deve usar o elemento [FolderId](folderid.md) ou [DistinguishedFolderId](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="06a85-129">The **ParentFolderIds** element must use either the [FolderId](folderid.md) or the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span> <span data-ttu-id="06a85-130">Um número ilimitado de pastas pode ser definido para a pesquisa.</span><span class="sxs-lookup"><span data-stu-id="06a85-130">An unlimited number of folders can be defined for the search.</span></span> 
  
## <a name="example"></a><span data-ttu-id="06a85-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="06a85-131">Example</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="06a85-132">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="06a85-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="06a85-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="06a85-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="06a85-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="06a85-134">Schema Name</span></span>  <br/> |<span data-ttu-id="06a85-135">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="06a85-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="06a85-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="06a85-136">Validation File</span></span>  <br/> |<span data-ttu-id="06a85-137">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="06a85-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="06a85-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="06a85-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="06a85-139">False</span><span class="sxs-lookup"><span data-stu-id="06a85-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="06a85-140">Confira também</span><span class="sxs-lookup"><span data-stu-id="06a85-140">See also</span></span>

- [<span data-ttu-id="06a85-141">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="06a85-141">FindFolder operation</span></span>](findfolder-operation.md)  
- [<span data-ttu-id="06a85-142">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="06a85-142">FindItem operation</span></span>](finditem-operation.md) 
- [<span data-ttu-id="06a85-143">Operação ResolveNames</span><span class="sxs-lookup"><span data-stu-id="06a85-143">ResolveNames operation</span></span>](resolvenames-operation.md)

