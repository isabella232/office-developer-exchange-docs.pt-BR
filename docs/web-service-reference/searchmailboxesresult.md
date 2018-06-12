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
ms.openlocfilehash: 93e5837216ef8942b77ac2a91f5ef5f0ad001756
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825300"
---
# <a name="searchmailboxesresult"></a><span data-ttu-id="e6ce3-103">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="e6ce3-103">SearchMailboxesResult</span></span>

<span data-ttu-id="e6ce3-104">O elemento **SearchMailboxesResult** contém o resultado da solicitação **SearchMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="e6ce3-104">The **SearchMailboxesResult** element contains the result of the **SearchMailboxes** request.</span></span> 
  
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

 <span data-ttu-id="e6ce3-105">**SearchMailboxesResultType**</span><span class="sxs-lookup"><span data-stu-id="e6ce3-105">**SearchMailboxesResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e6ce3-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e6ce3-106">Attributes and elements</span></span>

<span data-ttu-id="e6ce3-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e6ce3-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e6ce3-108">Attributes</span></span>

<span data-ttu-id="e6ce3-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e6ce3-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e6ce3-110">Child elements</span></span>

<span data-ttu-id="e6ce3-111">[SearchQueries](searchqueries.md) | [ResultType](resulttype.md) | [ItemCount](itemcount.md) | [tamanho (long)](size-long.md) | [PageItemCount](pageitemcount.md) | [PageItemSize](pageitemsize.md) | [KeywordStats](keywordstats.md) | [itens ( ArrayOfSearchPreviewItemsType)](items-arrayofsearchpreviewitemstype.md) | [FailedMailboxes](failedmailboxes.md) | [refinadores](refiners.md) | [MailboxStats](mailboxstats.md)</span><span class="sxs-lookup"><span data-stu-id="e6ce3-111">[SearchQueries](searchqueries.md) | [ResultType](resulttype.md) | [ItemCount](itemcount.md) | [Size (long)](size-long.md) | [PageItemCount](pageitemcount.md) | [PageItemSize](pageitemsize.md) | [KeywordStats](keywordstats.md) | [Items (ArrayOfSearchPreviewItemsType)](items-arrayofsearchpreviewitemstype.md) | [FailedMailboxes](failedmailboxes.md) | [Refiners](refiners.md) | [MailboxStats](mailboxstats.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e6ce3-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e6ce3-112">Parent elements</span></span>

[<span data-ttu-id="e6ce3-113">SearchMailboxesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e6ce3-113">SearchMailboxesResponseMessage</span></span>](searchmailboxesresponsemessage.md)
  
## <a name="remarks"></a><span data-ttu-id="e6ce3-114">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="e6ce3-114">Remarks</span></span>

<span data-ttu-id="e6ce3-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e6ce3-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e6ce3-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e6ce3-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e6ce3-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e6ce3-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="e6ce3-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e6ce3-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e6ce3-119">Schema name</span></span>  <br/> |<span data-ttu-id="e6ce3-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e6ce3-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e6ce3-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e6ce3-121">Validation file</span></span>  <br/> |<span data-ttu-id="e6ce3-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e6ce3-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e6ce3-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="e6ce3-123">Can be empty</span></span>  <br/> |<span data-ttu-id="e6ce3-124">false</span><span class="sxs-lookup"><span data-stu-id="e6ce3-124">false</span></span>  <br/> |
   

