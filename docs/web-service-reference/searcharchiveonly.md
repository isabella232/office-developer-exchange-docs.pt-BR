---
title: SearchArchiveOnly
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cce5344c-b622-44d4-bc14-a0de346c9335
description: O elemento SearchArchiveOnly indica se somente a caixa de correio de arquivo morto é pesquisada para itens não indexáveis.
ms.openlocfilehash: ac9d3262784d8052486c631ef3e99e650d4757c7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825293"
---
# <a name="searcharchiveonly"></a><span data-ttu-id="45524-103">SearchArchiveOnly</span><span class="sxs-lookup"><span data-stu-id="45524-103">SearchArchiveOnly</span></span>

<span data-ttu-id="45524-104">O elemento **SearchArchiveOnly** indica se somente a caixa de correio de arquivo morto é pesquisada para itens não indexáveis.</span><span class="sxs-lookup"><span data-stu-id="45524-104">The **SearchArchiveOnly** element indicates whether only the archive mailbox is searched for non-indexable items.</span></span> 
  
```xml
<SearchArchiveOnly>true | false</SearchArchiveOnly>
```

 <span data-ttu-id="45524-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="45524-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="45524-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="45524-106">Attributes and elements</span></span>

<span data-ttu-id="45524-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="45524-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="45524-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="45524-108">Attributes</span></span>

<span data-ttu-id="45524-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="45524-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="45524-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="45524-110">Child elements</span></span>

<span data-ttu-id="45524-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="45524-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="45524-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="45524-112">Parent elements</span></span>

<span data-ttu-id="45524-113">[GetNonIndexableItemStatistics](getnonindexableitemstatistics.md) │ [GetNonIndexableItemDetails](getnonindexableitemdetails.md)</span><span class="sxs-lookup"><span data-stu-id="45524-113">[GetNonIndexableItemStatistics](getnonindexableitemstatistics.md) │ [GetNonIndexableItemDetails](getnonindexableitemdetails.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="45524-114">Text value</span><span class="sxs-lookup"><span data-stu-id="45524-114">Text value</span></span>

<span data-ttu-id="45524-115">Um valor de texto de **true** para o elemento **SearchArchiveOnly** indica que o item não indexáveis a pesquisa é executada somente na caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="45524-115">A text value of **true** for the **SearchArchiveOnly** element indicates that non-indexable item search is only performed on the archive mailbox.</span></span> <span data-ttu-id="45524-116">Um valor de texto de **false** indica que a pesquisa é realizada em relação à caixa de correio principal e a caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="45524-116">A text value of **false** indicates that the search is performed against the primary mailbox and archive mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="45524-117">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="45524-117">Remarks</span></span>

<span data-ttu-id="45524-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="45524-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="45524-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="45524-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="45524-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="45524-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="45524-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="45524-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="45524-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="45524-122">Schema name</span></span>  <br/> |<span data-ttu-id="45524-123">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="45524-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="45524-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="45524-124">Validation file</span></span>  <br/> |<span data-ttu-id="45524-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="45524-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="45524-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="45524-126">Can be empty</span></span>  <br/> ||
   

