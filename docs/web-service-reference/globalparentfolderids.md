---
title: GlobalParentFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8f5fcbcb-05ed-462a-99cf-a6b112a4aef6
description: O elemento GlobalParentFolderIds Especifica os identificadores das pastas pai global.
ms.openlocfilehash: b0ff9ab00f3e46351b5a2db9bc4b6282fa4385cd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823747"
---
# <a name="globalparentfolderids"></a><span data-ttu-id="31707-103">GlobalParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="31707-103">GlobalParentFolderIds</span></span>

<span data-ttu-id="31707-104">O elemento **GlobalParentFolderIds** Especifica os identificadores das pastas pai global.</span><span class="sxs-lookup"><span data-stu-id="31707-104">The **GlobalParentFolderIds** element specifies the identifiers of the global parent folders.</span></span> 
  
```XML
<GlobalParentFolderIds>
    <FolderId/>
    <DistinguishedFolderId/>
</GlobalParentFolderIds>
```

 <span data-ttu-id="31707-105">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="31707-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="31707-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="31707-106">Attributes and elements</span></span>

<span data-ttu-id="31707-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="31707-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="31707-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="31707-108">Attributes</span></span>

<span data-ttu-id="31707-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="31707-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="31707-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="31707-110">Child elements</span></span>

|<span data-ttu-id="31707-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="31707-111">**Element**</span></span>|<span data-ttu-id="31707-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="31707-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31707-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="31707-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="31707-114">Contém o identificador e alterar a chave de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="31707-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="31707-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="31707-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="31707-116">Identifica as pastas que podem ser referidas por nome.</span><span class="sxs-lookup"><span data-stu-id="31707-116">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="31707-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="31707-117">Parent elements</span></span>

|<span data-ttu-id="31707-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="31707-118">**Element**</span></span>|<span data-ttu-id="31707-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="31707-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31707-120">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="31707-120">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="31707-121">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="31707-121">Represents a single conversation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="31707-122">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="31707-122">Remarks</span></span>

<span data-ttu-id="31707-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="31707-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="31707-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="31707-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="31707-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="31707-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="31707-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="31707-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="31707-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="31707-127">Schema Name</span></span>  <br/> |<span data-ttu-id="31707-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="31707-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="31707-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="31707-129">Validation File</span></span>  <br/> |<span data-ttu-id="31707-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="31707-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="31707-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="31707-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="31707-132">Confira também</span><span class="sxs-lookup"><span data-stu-id="31707-132">See also</span></span>



- [<span data-ttu-id="31707-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="31707-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

