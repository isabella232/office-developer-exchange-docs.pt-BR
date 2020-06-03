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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463710"
---
# <a name="deduplication"></a><span data-ttu-id="5df67-103">Duplicidades</span><span class="sxs-lookup"><span data-stu-id="5df67-103">Deduplication</span></span>

<span data-ttu-id="5df67-104">O elemento de **eliminação de duplicatas** indica se o resultado da pesquisa deve remover itens duplicados.</span><span class="sxs-lookup"><span data-stu-id="5df67-104">The **Deduplication** element indicates whether the search result should remove duplicate items.</span></span> 
  
```XML
<Deduplication> true | false </Deduplication>
```

<span data-ttu-id="5df67-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="5df67-105">**Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="5df67-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="5df67-106">Attributes and elements</span></span>

<span data-ttu-id="5df67-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="5df67-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5df67-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="5df67-108">Attributes</span></span>

<span data-ttu-id="5df67-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5df67-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5df67-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="5df67-110">Child elements</span></span>

<span data-ttu-id="5df67-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="5df67-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5df67-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="5df67-112">Parent elements</span></span>

<span data-ttu-id="5df67-113">[SearchMailboxes](searchmailboxes.md)  |  [SetHoldOnMailboxes](setholdonmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="5df67-113">[SearchMailboxes](searchmailboxes.md) | [SetHoldOnMailboxes](setholdonmailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="5df67-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="5df67-114">Text value</span></span>

<span data-ttu-id="5df67-115">Um valor de texto **true** para o elemento de eliminação de duplicatas indica que os resultados da pesquisa não podem conter itens duplicados.</span><span class="sxs-lookup"><span data-stu-id="5df67-115">A text value of **true** for the Deduplication element indicates that search results may not contain duplicate items.</span></span> <span data-ttu-id="5df67-116">Um valor **false** indica que os resultados da pesquisa podem conter itens duplicados.</span><span class="sxs-lookup"><span data-stu-id="5df67-116">A value of **false** indicates that search results may contain duplicate items.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5df67-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="5df67-117">Remarks</span></span>

<span data-ttu-id="5df67-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5df67-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5df67-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5df67-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5df67-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="5df67-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5df67-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="5df67-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5df67-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="5df67-122">Schema name</span></span>  <br/> |<span data-ttu-id="5df67-123">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="5df67-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="5df67-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="5df67-124">Validation file</span></span>  <br/> |<span data-ttu-id="5df67-125">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5df67-125">types.xsd</span></span>  <br/> |
|<span data-ttu-id="5df67-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="5df67-126">Can be empty</span></span>  <br/> |<span data-ttu-id="5df67-127">falso</span><span class="sxs-lookup"><span data-stu-id="5df67-127">false</span></span>  <br/> |
   

