---
title: SearchMailboxesResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddb276c4-6c8a-46ef-a2eb-46b6a0bfce09
description: O elemento SearchMailboxesResult contém o resultado da solicitação SearchMailboxes.
ms.openlocfilehash: 79d593d99762aedc6290578b5458f9ac3cad3d26
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466700"
---
# <a name="searchmailboxesresult"></a><span data-ttu-id="b668e-103">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="b668e-103">SearchMailboxesResult</span></span>

<span data-ttu-id="b668e-104">O elemento **SearchMailboxesResult** contém o resultado da solicitação **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="b668e-104">The **SearchMailboxesResult** element contains the result of the **SearchMailboxes** request.</span></span> 
  
```XML
<SearchMailboxesResult>
   <SearchQueries/>
   <ResultType/>
   <ItemCount/>
   <Size/>
   <PageItemCount/>
   <PageItemSize/>
   <KeywordStats/>
   <Items/>
   <FailedMailboxes/>
   <Refiners/>
   <MailboxStats/>
</SearchMailboxesResult>
```

 <span data-ttu-id="b668e-105">**SearchMailboxesResultType**</span><span class="sxs-lookup"><span data-stu-id="b668e-105">**SearchMailboxesResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b668e-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b668e-106">Attributes and elements</span></span>

<span data-ttu-id="b668e-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b668e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b668e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b668e-108">Attributes</span></span>

<span data-ttu-id="b668e-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b668e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b668e-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b668e-110">Child elements</span></span>

<span data-ttu-id="b668e-111">[SearchQueries](searchqueries.md)  |  [ResultType](resulttype.md)  |  [ItemCount](itemcount.md)  |  [Tamanho (longo)](size-long.md)  |  [PageItemCount](pageitemcount.md)  |  [PageItemSize](pageitemsize.md)  |  [KeywordStats](keywordstats.md)  |  [Itens (ArrayOfSearchPreviewItemsType)](items-arrayofsearchpreviewitemstype.md)  |  [FailedMailboxes](failedmailboxes.md)  |  [Refinadores](refiners.md)  |  [MailboxStats](mailboxstats.md)</span><span class="sxs-lookup"><span data-stu-id="b668e-111">[SearchQueries](searchqueries.md) | [ResultType](resulttype.md) | [ItemCount](itemcount.md) | [Size (long)](size-long.md) | [PageItemCount](pageitemcount.md) | [PageItemSize](pageitemsize.md) | [KeywordStats](keywordstats.md) | [Items (ArrayOfSearchPreviewItemsType)](items-arrayofsearchpreviewitemstype.md) | [FailedMailboxes](failedmailboxes.md) | [Refiners](refiners.md) | [MailboxStats](mailboxstats.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b668e-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b668e-112">Parent elements</span></span>

[<span data-ttu-id="b668e-113">SearchMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b668e-113">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
  
## <a name="remarks"></a><span data-ttu-id="b668e-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="b668e-114">Remarks</span></span>

<span data-ttu-id="b668e-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b668e-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b668e-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b668e-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b668e-117">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b668e-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b668e-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="b668e-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b668e-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b668e-119">Schema name</span></span>  <br/> |<span data-ttu-id="b668e-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="b668e-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b668e-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b668e-121">Validation file</span></span>  <br/> |<span data-ttu-id="b668e-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b668e-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b668e-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b668e-123">Can be empty</span></span>  <br/> |<span data-ttu-id="b668e-124">falso</span><span class="sxs-lookup"><span data-stu-id="b668e-124">false</span></span>  <br/> |
   

