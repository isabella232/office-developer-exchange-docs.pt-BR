---
title: FoldersToIgnore
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b5d18516-a617-4daf-8baf-c7ce29c76f6b
description: O elemento FoldersToIgnore identifica uma lista de pastas que devem ser ignoradas quando Obtendo itens em uma conversa. Todos os itens de conversa nas pastas ignorados não são retornados em uma resposta GetConversationItems.
ms.openlocfilehash: 96c094996c601e685dc1c7e6b869a790ce7d74a1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752348"
---
# <a name="folderstoignore"></a><span data-ttu-id="d5610-104">FoldersToIgnore</span><span class="sxs-lookup"><span data-stu-id="d5610-104">FoldersToIgnore</span></span>

<span data-ttu-id="d5610-105">O elemento **FoldersToIgnore** identifica uma lista de pastas que devem ser ignoradas quando Obtendo itens em uma conversa.</span><span class="sxs-lookup"><span data-stu-id="d5610-105">The **FoldersToIgnore** element identifies a list of folders that are ignored when getting items in a conversation.</span></span> <span data-ttu-id="d5610-106">Todos os itens de conversa nas pastas ignorados não são retornados em uma resposta **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="d5610-106">All conversation items in the ignored folders are not returned in a **GetConversationItems** response.</span></span> 
  
```XML
<FoldersToIgnore>
   <FolderId/>
   <DistinguishedFolderId/>
</FoldersToIgnore>
```

 <span data-ttu-id="d5610-107">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="d5610-107">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d5610-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="d5610-108">Attributes and elements</span></span>

<span data-ttu-id="d5610-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="d5610-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d5610-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="d5610-110">Attributes</span></span>

<span data-ttu-id="d5610-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="d5610-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d5610-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="d5610-112">Child elements</span></span>

<span data-ttu-id="d5610-113">[FolderId](folderid.md) | [DistinguishedFolderId](distinguishedfolderid.md)</span><span class="sxs-lookup"><span data-stu-id="d5610-113">[FolderId](folderid.md) | [DistinguishedFolderId](distinguishedfolderid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d5610-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="d5610-114">Parent elements</span></span>

[<span data-ttu-id="d5610-115">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="d5610-115">GetConversationItems</span></span>](getconversationitems.md)
  
## <a name="remarks"></a><span data-ttu-id="d5610-116">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="d5610-116">Remarks</span></span>

<span data-ttu-id="d5610-117">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d5610-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d5610-118">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d5610-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d5610-119">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="d5610-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d5610-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="d5610-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d5610-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="d5610-121">Schema name</span></span>  <br/> |<span data-ttu-id="d5610-122">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="d5610-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="d5610-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="d5610-123">Validation file</span></span>  <br/> |<span data-ttu-id="d5610-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d5610-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d5610-125">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="d5610-125">Can be empty</span></span>  <br/> |<span data-ttu-id="d5610-126">false</span><span class="sxs-lookup"><span data-stu-id="d5610-126">false</span></span>  <br/> |
   

