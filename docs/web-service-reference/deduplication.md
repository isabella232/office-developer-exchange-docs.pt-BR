---
title: Duplicidades
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a38acc3d-29a8-4466-81a4-73cb30fe5e80
description: O elemento de eliminação de duplicatas indica se o resultado da pesquisa deve remover itens duplicados.
ms.openlocfilehash: c39f980658aba7036cfabb3b51af5a41005f97b6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463710"
---
# <a name="deduplication"></a><span data-ttu-id="ed84c-103">Duplicidades</span><span class="sxs-lookup"><span data-stu-id="ed84c-103">Deduplication</span></span>

<span data-ttu-id="ed84c-104">O elemento de **eliminação de duplicatas** indica se o resultado da pesquisa deve remover itens duplicados.</span><span class="sxs-lookup"><span data-stu-id="ed84c-104">The **Deduplication** element indicates whether the search result should remove duplicate items.</span></span> 
  
```XML
<Deduplication> true | false </Deduplication>
```

<span data-ttu-id="ed84c-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="ed84c-105">**Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ed84c-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="ed84c-106">Attributes and elements</span></span>

<span data-ttu-id="ed84c-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ed84c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ed84c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ed84c-108">Attributes</span></span>

<span data-ttu-id="ed84c-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ed84c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ed84c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ed84c-110">Child elements</span></span>

<span data-ttu-id="ed84c-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ed84c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ed84c-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ed84c-112">Parent elements</span></span>

<span data-ttu-id="ed84c-113">[SearchMailboxes](searchmailboxes.md)  |  [SetHoldOnMailboxes](setholdonmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="ed84c-113">[SearchMailboxes](searchmailboxes.md) | [SetHoldOnMailboxes](setholdonmailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="ed84c-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="ed84c-114">Text value</span></span>

<span data-ttu-id="ed84c-115">Um valor de texto **true** para o elemento de eliminação de duplicatas indica que os resultados da pesquisa não podem conter itens duplicados.</span><span class="sxs-lookup"><span data-stu-id="ed84c-115">A text value of **true** for the Deduplication element indicates that search results may not contain duplicate items.</span></span> <span data-ttu-id="ed84c-116">Um valor **false** indica que os resultados da pesquisa podem conter itens duplicados.</span><span class="sxs-lookup"><span data-stu-id="ed84c-116">A value of **false** indicates that search results may contain duplicate items.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ed84c-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="ed84c-117">Remarks</span></span>

<span data-ttu-id="ed84c-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ed84c-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ed84c-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ed84c-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ed84c-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="ed84c-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ed84c-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="ed84c-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ed84c-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ed84c-122">Schema name</span></span>  <br/> |<span data-ttu-id="ed84c-123">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ed84c-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="ed84c-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ed84c-124">Validation file</span></span>  <br/> |<span data-ttu-id="ed84c-125">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ed84c-125">types.xsd</span></span>  <br/> |
|<span data-ttu-id="ed84c-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="ed84c-126">Can be empty</span></span>  <br/> |<span data-ttu-id="ed84c-127">falso</span><span class="sxs-lookup"><span data-stu-id="ed84c-127">false</span></span>  <br/> |
   

