---
title: MailboxStat
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5f24dc30-3ac2-4c82-9dfc-be9dbdb585be
description: O elemento MailboxStat especifica estatísticas para uma caixa de correio pesquisada pela pesquisa de descoberta.
ms.openlocfilehash: 417f63f5e1aa34c2157b1d5ad868461113afec7b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44451429"
---
# <a name="mailboxstat"></a><span data-ttu-id="4ee27-103">MailboxStat</span><span class="sxs-lookup"><span data-stu-id="4ee27-103">MailboxStat</span></span>

<span data-ttu-id="4ee27-104">O elemento **MailboxStat** especifica estatísticas para uma caixa de correio pesquisada pela pesquisa de descoberta.</span><span class="sxs-lookup"><span data-stu-id="4ee27-104">The **MailboxStat** element specifies statistics for a mailbox searched by discovery search.</span></span> 
  
```XML
<MailboxStat>
   <MailboxId/>
   <DisplayName/>
   <ItemCount/>
   <Size/>
</MailboxStat>
```

<span data-ttu-id="4ee27-105">**MailboxStatisticsItemType**</span><span class="sxs-lookup"><span data-stu-id="4ee27-105">**MailboxStatisticsItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4ee27-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="4ee27-106">Attributes and elements</span></span>

<span data-ttu-id="4ee27-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="4ee27-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ee27-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="4ee27-108">Attributes</span></span>

<span data-ttu-id="4ee27-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4ee27-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ee27-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="4ee27-110">Child elements</span></span>

<span data-ttu-id="4ee27-111">[Mailboxid](mailboxid.md)  |  [DisplayName (cadeia de caracteres)](displayname-string.md)  |  [ItemCount](itemcount.md)  |  [Tamanho (longo)](size-long.md)</span><span class="sxs-lookup"><span data-stu-id="4ee27-111">[MailboxId](mailboxid.md) | [DisplayName (string)](displayname-string.md) | [ItemCount](itemcount.md) | [Size (long)](size-long.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4ee27-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="4ee27-112">Parent elements</span></span>

[<span data-ttu-id="4ee27-113">MailboxStats</span><span class="sxs-lookup"><span data-stu-id="4ee27-113">MailboxStats</span></span>](mailboxstats.md)
  
## <a name="remarks"></a><span data-ttu-id="4ee27-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="4ee27-114">Remarks</span></span>

<span data-ttu-id="4ee27-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4ee27-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4ee27-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ee27-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ee27-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="4ee27-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ee27-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="4ee27-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4ee27-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="4ee27-119">Schema name</span></span>  <br/> |<span data-ttu-id="4ee27-120">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="4ee27-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="4ee27-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="4ee27-121">Validation file</span></span>  <br/> |<span data-ttu-id="4ee27-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4ee27-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4ee27-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="4ee27-123">Can be empty</span></span>  <br/> |<span data-ttu-id="4ee27-124">falso</span><span class="sxs-lookup"><span data-stu-id="4ee27-124">false</span></span>  <br/> |
   

