---
title: MailboxStat
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5f24dc30-3ac2-4c82-9dfc-be9dbdb585be
description: O elemento MailboxStat Especifica as estatísticas de uma caixa de correio pesquisada por pesquisa de descoberta.
ms.openlocfilehash: 692f15904467ce192074b14f7c2a742b3e76de8e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824296"
---
# <a name="mailboxstat"></a><span data-ttu-id="49b0e-103">MailboxStat</span><span class="sxs-lookup"><span data-stu-id="49b0e-103">MailboxStat</span></span>

<span data-ttu-id="49b0e-104">O elemento **MailboxStat** Especifica as estatísticas de uma caixa de correio pesquisada por pesquisa de descoberta.</span><span class="sxs-lookup"><span data-stu-id="49b0e-104">The **MailboxStat** element specifies statistics for a mailbox searched by discovery search.</span></span> 
  
```XML
<MailboxStat>
   <MailboxId/>
   <DisplayName/>
   <ItemCount/>
   <Size/>
</MailboxStat>
```

<span data-ttu-id="49b0e-105">**MailboxStatisticsItemType**</span><span class="sxs-lookup"><span data-stu-id="49b0e-105">**MailboxStatisticsItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="49b0e-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="49b0e-106">Attributes and elements</span></span>

<span data-ttu-id="49b0e-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="49b0e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="49b0e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="49b0e-108">Attributes</span></span>

<span data-ttu-id="49b0e-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="49b0e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="49b0e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="49b0e-110">Child elements</span></span>

<span data-ttu-id="49b0e-111">[MailboxId](mailboxid.md) | [DisplayName (string)](displayname-string.md) | [ItemCount](itemcount.md) | [tamanho (long)](size-long.md)</span><span class="sxs-lookup"><span data-stu-id="49b0e-111">[MailboxId](mailboxid.md) | [DisplayName (string)](displayname-string.md) | [ItemCount](itemcount.md) | [Size (long)](size-long.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="49b0e-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="49b0e-112">Parent elements</span></span>

[<span data-ttu-id="49b0e-113">MailboxStats</span><span class="sxs-lookup"><span data-stu-id="49b0e-113">MailboxStats</span></span>](mailboxstats.md)
  
## <a name="remarks"></a><span data-ttu-id="49b0e-114">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="49b0e-114">Remarks</span></span>

<span data-ttu-id="49b0e-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="49b0e-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="49b0e-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="49b0e-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="49b0e-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="49b0e-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="49b0e-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="49b0e-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="49b0e-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="49b0e-119">Schema name</span></span>  <br/> |<span data-ttu-id="49b0e-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="49b0e-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="49b0e-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="49b0e-121">Validation file</span></span>  <br/> |<span data-ttu-id="49b0e-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="49b0e-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="49b0e-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="49b0e-123">Can be empty</span></span>  <br/> |<span data-ttu-id="49b0e-124">false</span><span class="sxs-lookup"><span data-stu-id="49b0e-124">false</span></span>  <br/> |
   

