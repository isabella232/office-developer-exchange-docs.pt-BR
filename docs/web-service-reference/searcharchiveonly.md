---
title: SearchArchiveOnly
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cce5344c-b622-44d4-bc14-a0de346c9335
description: O elemento SearchArchiveOnly indica se somente a caixa de correio de arquivo morto é pesquisada para itens não indexados.
ms.openlocfilehash: 9014044ed06c697cc43dd62103d7a1a907bda5a8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460495"
---
# <a name="searcharchiveonly"></a><span data-ttu-id="b340d-103">SearchArchiveOnly</span><span class="sxs-lookup"><span data-stu-id="b340d-103">SearchArchiveOnly</span></span>

<span data-ttu-id="b340d-104">O elemento **SearchArchiveOnly** indica se somente a caixa de correio de arquivo morto é pesquisada para itens não indexados.</span><span class="sxs-lookup"><span data-stu-id="b340d-104">The **SearchArchiveOnly** element indicates whether only the archive mailbox is searched for non-indexable items.</span></span> 
  
```xml
<SearchArchiveOnly>true | false</SearchArchiveOnly>
```

 <span data-ttu-id="b340d-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="b340d-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b340d-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b340d-106">Attributes and elements</span></span>

<span data-ttu-id="b340d-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b340d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b340d-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b340d-108">Attributes</span></span>

<span data-ttu-id="b340d-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b340d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b340d-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b340d-110">Child elements</span></span>

<span data-ttu-id="b340d-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b340d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b340d-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b340d-112">Parent elements</span></span>

<span data-ttu-id="b340d-113">[GetNonIndexableItemStatistics](getnonindexableitemstatistics.md) │ [GetNonIndexableItemDetails](getnonindexableitemdetails.md)</span><span class="sxs-lookup"><span data-stu-id="b340d-113">[GetNonIndexableItemStatistics](getnonindexableitemstatistics.md) │ [GetNonIndexableItemDetails](getnonindexableitemdetails.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="b340d-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="b340d-114">Text value</span></span>

<span data-ttu-id="b340d-115">Um valor de texto **true** para o elemento **SearchArchiveOnly** indica que a pesquisa de item não indexável é executada apenas na caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="b340d-115">A text value of **true** for the **SearchArchiveOnly** element indicates that non-indexable item search is only performed on the archive mailbox.</span></span> <span data-ttu-id="b340d-116">Um valor **false** indica que a pesquisa é executada em relação à caixa de correio principal e à caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="b340d-116">A text value of **false** indicates that the search is performed against the primary mailbox and archive mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b340d-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="b340d-117">Remarks</span></span>

<span data-ttu-id="b340d-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b340d-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b340d-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b340d-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b340d-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b340d-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b340d-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="b340d-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b340d-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b340d-122">Schema name</span></span>  <br/> |<span data-ttu-id="b340d-123">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="b340d-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b340d-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b340d-124">Validation file</span></span>  <br/> |<span data-ttu-id="b340d-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b340d-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b340d-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b340d-126">Can be empty</span></span>  <br/> ||
   

