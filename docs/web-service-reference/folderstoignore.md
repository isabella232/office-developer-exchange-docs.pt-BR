---
title: FoldersToIgnore
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b5d18516-a617-4daf-8baf-c7ce29c76f6b
description: O elemento FoldersToIgnore identifica uma lista de pastas que são ignoradas ao obter itens em uma conversa. Todos os itens de conversa nas pastas ignoradas não são retornados em uma resposta GetConversationItems.
ms.openlocfilehash: 07813a54a9a3afa3de23ae94f1c9b191d1cb6fac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44453354"
---
# <a name="folderstoignore"></a><span data-ttu-id="eb9f5-104">FoldersToIgnore</span><span class="sxs-lookup"><span data-stu-id="eb9f5-104">FoldersToIgnore</span></span>

<span data-ttu-id="eb9f5-105">O elemento **FoldersToIgnore** identifica uma lista de pastas que são ignoradas ao obter itens em uma conversa.</span><span class="sxs-lookup"><span data-stu-id="eb9f5-105">The **FoldersToIgnore** element identifies a list of folders that are ignored when getting items in a conversation.</span></span> <span data-ttu-id="eb9f5-106">Todos os itens de conversa nas pastas ignoradas não são retornados em uma resposta **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="eb9f5-106">All conversation items in the ignored folders are not returned in a **GetConversationItems** response.</span></span> 
  
```XML
<FoldersToIgnore>
   <FolderId/>
   <DistinguishedFolderId/>
</FoldersToIgnore>
```

 <span data-ttu-id="eb9f5-107">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="eb9f5-107">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eb9f5-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="eb9f5-108">Attributes and elements</span></span>

<span data-ttu-id="eb9f5-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="eb9f5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eb9f5-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="eb9f5-110">Attributes</span></span>

<span data-ttu-id="eb9f5-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb9f5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eb9f5-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="eb9f5-112">Child elements</span></span>

<span data-ttu-id="eb9f5-113">[FolderId](folderid.md)  |  [DistinguishedFolderId](distinguishedfolderid.md)</span><span class="sxs-lookup"><span data-stu-id="eb9f5-113">[FolderId](folderid.md) | [DistinguishedFolderId](distinguishedfolderid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="eb9f5-114">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="eb9f5-114">Parent elements</span></span>

[<span data-ttu-id="eb9f5-115">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="eb9f5-115">GetConversationItems</span></span>](getconversationitems.md)
  
## <a name="remarks"></a><span data-ttu-id="eb9f5-116">Comentários</span><span class="sxs-lookup"><span data-stu-id="eb9f5-116">Remarks</span></span>

<span data-ttu-id="eb9f5-117">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="eb9f5-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="eb9f5-118">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="eb9f5-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eb9f5-119">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="eb9f5-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eb9f5-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="eb9f5-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eb9f5-121">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="eb9f5-121">Schema name</span></span>  <br/> |<span data-ttu-id="eb9f5-122">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="eb9f5-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="eb9f5-123">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="eb9f5-123">Validation file</span></span>  <br/> |<span data-ttu-id="eb9f5-124">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="eb9f5-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="eb9f5-125">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="eb9f5-125">Can be empty</span></span>  <br/> |<span data-ttu-id="eb9f5-126">falso</span><span class="sxs-lookup"><span data-stu-id="eb9f5-126">false</span></span>  <br/> |
   

