---
title: SearchItemKind
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 89513c26-b751-4619-a300-0ed8f55b0102
description: O elemento SearchItemKind indica o tipo de itens que são pesquisados para uma operação de FindMailboxStatisticsByKeyword.
ms.openlocfilehash: 1c099fc49ec882c1672b265ff0e3aa2c71c5f95b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825298"
---
# <a name="searchitemkind"></a><span data-ttu-id="8a167-103">SearchItemKind</span><span class="sxs-lookup"><span data-stu-id="8a167-103">SearchItemKind</span></span>

<span data-ttu-id="8a167-104">O elemento **SearchItemKind** indica o tipo de itens que são pesquisados para uma operação de **FindMailboxStatisticsByKeyword** .</span><span class="sxs-lookup"><span data-stu-id="8a167-104">The **SearchItemKind** element indicates the type of items that are searched for a **FindMailboxStatisticsByKeyword** operation.</span></span> 
  
```XML
<SearchItemKind>Email | Meetings | Tasks | Notes | Docs | Journals | Contacts | Im | Voicemail | Faxes | Posts | Rssfeeds</SearchItemKind>
```

 <span data-ttu-id="8a167-105">**SearchItemKindType**</span><span class="sxs-lookup"><span data-stu-id="8a167-105">**SearchItemKindType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8a167-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="8a167-106">Attributes and elements</span></span>

<span data-ttu-id="8a167-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8a167-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8a167-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="8a167-108">Attributes</span></span>

<span data-ttu-id="8a167-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8a167-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8a167-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8a167-110">Child elements</span></span>

<span data-ttu-id="8a167-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8a167-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8a167-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8a167-112">Parent elements</span></span>

[<span data-ttu-id="8a167-113">MessageTypes</span><span class="sxs-lookup"><span data-stu-id="8a167-113">MessageTypes</span></span>](messagetypes.md)
  
## <a name="text-value"></a><span data-ttu-id="8a167-114">Text value</span><span class="sxs-lookup"><span data-stu-id="8a167-114">Text value</span></span>

<span data-ttu-id="8a167-115">O valor de texto do elemento **SearchItemKind** é o tipo de item que será pesquisada para palavras-chave.</span><span class="sxs-lookup"><span data-stu-id="8a167-115">The text value of the **SearchItemKind** element is the type of item that is searched for keywords.</span></span> <span data-ttu-id="8a167-116">A lista a seguir contém os valores de texto que podem ser usados no elemento **SearchItemKind** .</span><span class="sxs-lookup"><span data-stu-id="8a167-116">The following list contains the text values that can be used in the **SearchItemKind** element.</span></span> 
  
- <span data-ttu-id="8a167-117">**Email** – indica que as mensagens de email são pesquisadas para palavras-chave.</span><span class="sxs-lookup"><span data-stu-id="8a167-117">**Email** - Indicates that email messages are searched for keywords.</span></span> 
    
- <span data-ttu-id="8a167-118">**Reuniões** - indica que as reuniões são pesquisados para palavras-chave.</span><span class="sxs-lookup"><span data-stu-id="8a167-118">**Meetings** - Indicates that meetings are searched for keywords.</span></span> 
    
- <span data-ttu-id="8a167-119">**Tarefas** - indica que as tarefas são pesquisadas para palavras-chave.</span><span class="sxs-lookup"><span data-stu-id="8a167-119">**Tasks** - Indicates that tasks are searched for keywords.</span></span> 
    
- <span data-ttu-id="8a167-120">**Observações** - indica que as notas são pesquisadas para palavras-chave.</span><span class="sxs-lookup"><span data-stu-id="8a167-120">**Notes** - Indicates that notes are searched for keywords.</span></span> 
    
- <span data-ttu-id="8a167-121">**Documentos** - indica que os documentos são pesquisados para palavras-chave.</span><span class="sxs-lookup"><span data-stu-id="8a167-121">**Docs** - Indicates that documents are searched for keywords.</span></span> 
    
- <span data-ttu-id="8a167-122">**Diários** - indica que o diários são pesquisados para palavras-chave.</span><span class="sxs-lookup"><span data-stu-id="8a167-122">**Journals** - Indicates that journals are searched for keywords.</span></span> 
    
- <span data-ttu-id="8a167-123">**Contatos** - indica que os contatos são pesquisados para palavras-chave.</span><span class="sxs-lookup"><span data-stu-id="8a167-123">**Contacts** - Indicates that contacts are searched for keywords.</span></span> 
    
- <span data-ttu-id="8a167-124">**Mensagens instantâneas** - indica que as mensagens instantâneas são pesquisadas para palavras-chave.</span><span class="sxs-lookup"><span data-stu-id="8a167-124">**Im** - Indicates that instant messages are searched for keywords.</span></span> 
    
- <span data-ttu-id="8a167-125">**Caixa postal** - indica que o postais são pesquisados para palavras-chave.</span><span class="sxs-lookup"><span data-stu-id="8a167-125">**Voicemail** - Indicates that voice mails are searched for keywords.</span></span> 
    
- <span data-ttu-id="8a167-126">**Aparelhos de fax** - indica que os faxes são pesquisados para palavras-chave.</span><span class="sxs-lookup"><span data-stu-id="8a167-126">**Faxes** - Indicates that faxes are searched for keywords.</span></span> 
    
- <span data-ttu-id="8a167-127">**Postagens** - indica que as postagens são pesquisadas para palavras-chave.</span><span class="sxs-lookup"><span data-stu-id="8a167-127">**Posts** - Indicates that posts are searched for keywords.</span></span> 
    
- <span data-ttu-id="8a167-128">**Rssfeeds** - indica que o RSS feeds são pesquisados para palavras-chave.</span><span class="sxs-lookup"><span data-stu-id="8a167-128">**Rssfeeds** - Indicates that RSS feeds are searched for keywords.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="8a167-129">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="8a167-129">Remarks</span></span>

<span data-ttu-id="8a167-130">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8a167-130">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8a167-131">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="8a167-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8a167-132">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="8a167-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8a167-133">Namespace</span><span class="sxs-lookup"><span data-stu-id="8a167-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8a167-134">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8a167-134">Schema name</span></span>  <br/> |<span data-ttu-id="8a167-135">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8a167-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="8a167-136">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8a167-136">Validation file</span></span>  <br/> |<span data-ttu-id="8a167-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8a167-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8a167-138">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="8a167-138">Can be empty</span></span>  <br/> ||
   

