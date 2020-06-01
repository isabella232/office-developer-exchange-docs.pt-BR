---
title: GlobalParentFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8f5fcbcb-05ed-462a-99cf-a6b112a4aef6
description: O elemento GlobalParentFolderIds especifica os identificadores das pastas pai global.
ms.openlocfilehash: 11c520fa0f4a1ed6d6c9d694b407e39cd036b9cd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459094"
---
# <a name="globalparentfolderids"></a><span data-ttu-id="482ba-103">GlobalParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="482ba-103">GlobalParentFolderIds</span></span>

<span data-ttu-id="482ba-104">O elemento **GlobalParentFolderIds** especifica os identificadores das pastas pai global.</span><span class="sxs-lookup"><span data-stu-id="482ba-104">The **GlobalParentFolderIds** element specifies the identifiers of the global parent folders.</span></span> 
  
```XML
<GlobalParentFolderIds>
    <FolderId/>
    <DistinguishedFolderId/>
</GlobalParentFolderIds>
```

 <span data-ttu-id="482ba-105">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="482ba-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="482ba-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="482ba-106">Attributes and elements</span></span>

<span data-ttu-id="482ba-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="482ba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="482ba-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="482ba-108">Attributes</span></span>

<span data-ttu-id="482ba-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="482ba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="482ba-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="482ba-110">Child elements</span></span>

|<span data-ttu-id="482ba-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="482ba-111">**Element**</span></span>|<span data-ttu-id="482ba-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="482ba-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="482ba-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="482ba-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="482ba-114">Contém o identificador e a chave de alteração de uma pasta.</span><span class="sxs-lookup"><span data-stu-id="482ba-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="482ba-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="482ba-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="482ba-116">Identifica pastas que podem ser referenciadas por nome.</span><span class="sxs-lookup"><span data-stu-id="482ba-116">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="482ba-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="482ba-117">Parent elements</span></span>

|<span data-ttu-id="482ba-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="482ba-118">**Element**</span></span>|<span data-ttu-id="482ba-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="482ba-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="482ba-120">Conversa (Conversatype)</span><span class="sxs-lookup"><span data-stu-id="482ba-120">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="482ba-121">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="482ba-121">Represents a single conversation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="482ba-122">Comentários</span><span class="sxs-lookup"><span data-stu-id="482ba-122">Remarks</span></span>

<span data-ttu-id="482ba-123">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="482ba-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="482ba-124">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="482ba-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="482ba-125">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="482ba-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="482ba-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="482ba-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="482ba-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="482ba-127">Schema Name</span></span>  <br/> |<span data-ttu-id="482ba-128">Esquema de tipo</span><span class="sxs-lookup"><span data-stu-id="482ba-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="482ba-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="482ba-129">Validation File</span></span>  <br/> |<span data-ttu-id="482ba-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="482ba-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="482ba-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="482ba-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="482ba-132">Também consulte</span><span class="sxs-lookup"><span data-stu-id="482ba-132">See also</span></span>



- [<span data-ttu-id="482ba-133">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="482ba-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

