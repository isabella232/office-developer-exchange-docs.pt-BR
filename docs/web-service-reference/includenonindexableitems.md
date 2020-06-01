---
title: IncludeNonIndexableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: af7f202b-2889-447e-bdeb-aaad18ce6b46
description: O elemento IncludeNonIndexableItems contém um valor booleano para indicar se deve incluir itens que não podem ser indexados.
ms.openlocfilehash: eab559e938f0b949d79626ae5bf61b3d4a838924
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460621"
---
# <a name="includenonindexableitems"></a><span data-ttu-id="500fd-103">IncludeNonIndexableItems</span><span class="sxs-lookup"><span data-stu-id="500fd-103">IncludeNonIndexableItems</span></span>

<span data-ttu-id="500fd-104">O elemento **IncludeNonIndexableItems** contém um valor **booleano** para indicar se deve incluir itens que não podem ser indexados.</span><span class="sxs-lookup"><span data-stu-id="500fd-104">The **IncludeNonIndexableItems** element contains a **Boolean** value to indicate whether to include items that cannot be indexed.</span></span> 
  
```XML
<IncludeNonIndexableItems>true | false</IncludeNonIndexableItems>
```

 <span data-ttu-id="500fd-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="500fd-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="500fd-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="500fd-106">Attributes and elements</span></span>

<span data-ttu-id="500fd-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="500fd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="500fd-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="500fd-108">Attributes</span></span>

<span data-ttu-id="500fd-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="500fd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="500fd-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="500fd-110">Child elements</span></span>

<span data-ttu-id="500fd-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="500fd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="500fd-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="500fd-112">Parent elements</span></span>

[<span data-ttu-id="500fd-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="500fd-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="500fd-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="500fd-114">Text value</span></span>

<span data-ttu-id="500fd-115">Um valor de texto **true** para o elemento **IncludeNonIndexableItems** indica que os itens que não podem ser indexados estão incluídos no bloqueio de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="500fd-115">A text value of **true** for the **IncludeNonIndexableItems** element indicates that items that cannot be indexed are included with mailbox holds.</span></span> <span data-ttu-id="500fd-116">Um valor **false** indica que os itens que não podem ser indexados não estão incluídos nas isenções de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="500fd-116">A value of **false** indicates that the items that cannot be indexed are not included in mailbox holds.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="500fd-117">Comentários</span><span class="sxs-lookup"><span data-stu-id="500fd-117">Remarks</span></span>

<span data-ttu-id="500fd-118">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="500fd-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="500fd-119">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="500fd-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="500fd-120">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="500fd-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="500fd-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="500fd-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="500fd-122">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="500fd-122">Schema name</span></span>  <br/> |<span data-ttu-id="500fd-123">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="500fd-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="500fd-124">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="500fd-124">Validation file</span></span>  <br/> |<span data-ttu-id="500fd-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="500fd-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="500fd-126">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="500fd-126">Can be empty</span></span>  <br/> |<span data-ttu-id="500fd-127">falso</span><span class="sxs-lookup"><span data-stu-id="500fd-127">false</span></span>  <br/> |
   

