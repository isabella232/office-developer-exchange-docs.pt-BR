---
title: Eliminação da duplicação
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a38acc3d-29a8-4466-81a4-73cb30fe5e80
description: O elemento de eliminação da duplicação indica se o resultado de pesquisa deve remover itens duplicados.
ms.openlocfilehash: 3f06bb1dccd0677b7fd43c4ad82eda54a0c3f812
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751717"
---
# <a name="deduplication"></a><span data-ttu-id="73b10-103">Eliminação da duplicação</span><span class="sxs-lookup"><span data-stu-id="73b10-103">Deduplication</span></span>

<span data-ttu-id="73b10-104">O elemento de **eliminação da duplicação** indica se o resultado de pesquisa deve remover itens duplicados.</span><span class="sxs-lookup"><span data-stu-id="73b10-104">The **Deduplication** element indicates whether the search result should remove duplicate items.</span></span> 
  
```XML
<Deduplication> true | false </Deduplication>
```

<span data-ttu-id="73b10-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="73b10-105">**Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="73b10-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="73b10-106">Attributes and elements</span></span>

<span data-ttu-id="73b10-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="73b10-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="73b10-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="73b10-108">Attributes</span></span>

<span data-ttu-id="73b10-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="73b10-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="73b10-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="73b10-110">Child elements</span></span>

<span data-ttu-id="73b10-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="73b10-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="73b10-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="73b10-112">Parent elements</span></span>

<span data-ttu-id="73b10-113">[SearchMailboxes](searchmailboxes.md) | [SetHoldOnMailboxes](setholdonmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="73b10-113">[SearchMailboxes](searchmailboxes.md) | [SetHoldOnMailboxes](setholdonmailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="73b10-114">Text value</span><span class="sxs-lookup"><span data-stu-id="73b10-114">Text value</span></span>

<span data-ttu-id="73b10-115">Um valor de **true** para o elemento de eliminação da duplicação text indica que os resultados da pesquisa não podem conter itens duplicados.</span><span class="sxs-lookup"><span data-stu-id="73b10-115">A text value of **true** for the Deduplication element indicates that search results may not contain duplicate items.</span></span> <span data-ttu-id="73b10-116">Um valor **false** indica que os resultados da pesquisa podem conter itens duplicados.</span><span class="sxs-lookup"><span data-stu-id="73b10-116">A value of **false** indicates that search results may contain duplicate items.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="73b10-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="73b10-117">Remarks</span></span>

<span data-ttu-id="73b10-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="73b10-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="73b10-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="73b10-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="73b10-120">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="73b10-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="73b10-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="73b10-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="73b10-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="73b10-122">Schema name</span></span>  <br/> |<span data-ttu-id="73b10-123">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="73b10-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="73b10-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="73b10-124">Validation file</span></span>  <br/> |<span data-ttu-id="73b10-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="73b10-125">types.xsd</span></span>  <br/> |
|<span data-ttu-id="73b10-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="73b10-126">Can be empty</span></span>  <br/> |<span data-ttu-id="73b10-127">false</span><span class="sxs-lookup"><span data-stu-id="73b10-127">false</span></span>  <br/> |
   

