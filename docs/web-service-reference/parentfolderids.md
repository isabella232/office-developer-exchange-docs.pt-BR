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
description: O elemento ParentFolderIds identifica pastas para as operações FindItem e FindFolder pesquisar.
ms.openlocfilehash: 7c4dcc98d1cabc8e97f2846880c73111dd307dfb
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354166"
---
# <a name="parentfolderids"></a><span data-ttu-id="8d3c4-103">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="8d3c4-103">ParentFolderIds</span></span>

<span data-ttu-id="8d3c4-104">O elemento **ParentFolderIds** identifica pastas para as operações FindItem e FindFolder pesquisar.</span><span class="sxs-lookup"><span data-stu-id="8d3c4-104">The **ParentFolderIds** element identifies folders for the FindItem and FindFolder operations to search.</span></span> 
  
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

<span data-ttu-id="8d3c4-105">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="8d3c4-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8d3c4-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8d3c4-106">Attributes and elements</span></span>

<span data-ttu-id="8d3c4-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8d3c4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d3c4-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8d3c4-108">Attributes</span></span>

<span data-ttu-id="8d3c4-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8d3c4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8d3c4-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8d3c4-110">Child elements</span></span>

|<span data-ttu-id="8d3c4-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8d3c4-111">**Element**</span></span>|<span data-ttu-id="8d3c4-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8d3c4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d3c4-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="8d3c4-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="8d3c4-114">Contém o identificador e alterar a chave de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="8d3c4-114">Contains the identifier and change key of a folder.</span></span> <span data-ttu-id="8d3c4-115">O elemento **ParentFolderIds** deve usar esse elemento ou o elemento [DistinguishedFolderId](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="8d3c4-115">The **ParentFolderIds** element must use either this element or the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="8d3c4-116">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="8d3c4-116">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="8d3c4-117">Identifica as pastas do Microsoft Exchange Server 2007 que podem ser referidas por nome.</span><span class="sxs-lookup"><span data-stu-id="8d3c4-117">Identifies Microsoft Exchange Server 2007 folders that can be referenced by name.</span></span> <span data-ttu-id="8d3c4-118">O elemento **ParentFolderIds** deve usar esse elemento ou o elemento [FolderId](folderid.md) .</span><span class="sxs-lookup"><span data-stu-id="8d3c4-118">The **ParentFolderIds** element must use either this element or the [FolderId](folderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8d3c4-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8d3c4-119">Parent elements</span></span>

|<span data-ttu-id="8d3c4-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8d3c4-120">**Element**</span></span>|<span data-ttu-id="8d3c4-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8d3c4-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d3c4-122">FindFolder</span><span class="sxs-lookup"><span data-stu-id="8d3c4-122">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="8d3c4-123">Define uma solicitação para identificar pastas em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="8d3c4-123">Defines a request to identify folders in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8d3c4-124">FindItem</span><span class="sxs-lookup"><span data-stu-id="8d3c4-124">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="8d3c4-125">Define uma solicitação para localizar itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="8d3c4-125">Defines a request to find items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="8d3c4-126">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="8d3c4-126">ResolveNames</span></span>](resolvenames.md) <br/> |<span data-ttu-id="8d3c4-127">Define uma solicitação para resolver nomes de ambíguos.</span><span class="sxs-lookup"><span data-stu-id="8d3c4-127">Defines a request to resolve ambiguous names.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8d3c4-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="8d3c4-128">Remarks</span></span>

<span data-ttu-id="8d3c4-129">O elemento **ParentFolderIds** deve usar o [FolderId](folderid.md) ou o elemento [DistinguishedFolderId](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="8d3c4-129">The **ParentFolderIds** element must use either the [FolderId](folderid.md) or the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span> <span data-ttu-id="8d3c4-130">Um número ilimitado de pastas pode ser definido para a pesquisa.</span><span class="sxs-lookup"><span data-stu-id="8d3c4-130">An unlimited number of folders can be defined for the search.</span></span> 
  
## <a name="example"></a><span data-ttu-id="8d3c4-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8d3c4-131">Example</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="element-information"></a><span data-ttu-id="8d3c4-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8d3c4-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8d3c4-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="8d3c4-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8d3c4-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8d3c4-134">Schema Name</span></span>  <br/> |<span data-ttu-id="8d3c4-135">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="8d3c4-135">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8d3c4-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8d3c4-136">Validation File</span></span>  <br/> |<span data-ttu-id="8d3c4-137">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8d3c4-137">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8d3c4-138">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8d3c4-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="8d3c4-139">False</span><span class="sxs-lookup"><span data-stu-id="8d3c4-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8d3c4-140">Ver também</span><span class="sxs-lookup"><span data-stu-id="8d3c4-140">See also</span></span>

- [<span data-ttu-id="8d3c4-141">Operação FindFolder</span><span class="sxs-lookup"><span data-stu-id="8d3c4-141">FindFolder operation</span></span>](findfolder-operation.md)  
- [<span data-ttu-id="8d3c4-142">Operação FindItem</span><span class="sxs-lookup"><span data-stu-id="8d3c4-142">FindItem operation</span></span>](finditem-operation.md) 
- [<span data-ttu-id="8d3c4-143">Operação ResolveNames</span><span class="sxs-lookup"><span data-stu-id="8d3c4-143">ResolveNames operation</span></span>](resolvenames-operation.md)

