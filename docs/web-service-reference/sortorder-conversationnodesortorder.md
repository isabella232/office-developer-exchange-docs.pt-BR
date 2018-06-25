---
title: SortOrder (ConversationNodeSortOrder)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9c4295c-8089-4533-b92f-2051eae9afeb
description: O elemento SortOrder Especifica a ordem de classificação usada para o resultado de uma solicitação de GetConversationItems.
ms.openlocfilehash: 397aead62d32e72f991af783bff02e79a6e4b0fb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825520"
---
# <a name="sortorder-conversationnodesortorder"></a><span data-ttu-id="ee002-103">SortOrder (ConversationNodeSortOrder)</span><span class="sxs-lookup"><span data-stu-id="ee002-103">SortOrder (ConversationNodeSortOrder)</span></span>

<span data-ttu-id="ee002-104">O elemento **SortOrder** Especifica a ordem de classificação usada para o resultado de uma solicitação de **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="ee002-104">The **SortOrder** element specifies the sort order used for the result of a **GetConversationItems** request.</span></span> 
  
```XML
<SortOrder>TreeOrderAscending | TreeOrderDescending | DateOrderAscending | DateOrderDescending</SortOrder>
```

 <span data-ttu-id="ee002-105">**ConversationNodeSortOrder**</span><span class="sxs-lookup"><span data-stu-id="ee002-105">**ConversationNodeSortOrder**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ee002-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ee002-106">Attributes and elements</span></span>

<span data-ttu-id="ee002-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ee002-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ee002-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ee002-108">Attributes</span></span>

<span data-ttu-id="ee002-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ee002-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ee002-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ee002-110">Child elements</span></span>

<span data-ttu-id="ee002-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ee002-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ee002-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ee002-112">Parent elements</span></span>

[<span data-ttu-id="ee002-113">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="ee002-113">GetConversationItems</span></span>](getconversationitems.md)
  
## <a name="text-value"></a><span data-ttu-id="ee002-114">Text value</span><span class="sxs-lookup"><span data-stu-id="ee002-114">Text value</span></span>

<span data-ttu-id="ee002-115">O valor de texto do elemento **SortOrder** é a ordem na qual as conversas ordenadas.</span><span class="sxs-lookup"><span data-stu-id="ee002-115">The text value of the **SortOrder** element is the order in which conversations ordered.</span></span> <span data-ttu-id="ee002-116">Um valor de texto de **TreeOrderAscending** indica que as conversas são ordenadas de acordo com a árvore de conversa em ordem crescente.</span><span class="sxs-lookup"><span data-stu-id="ee002-116">A text value of **TreeOrderAscending** indicates that the conversations are ordered according to the conversation tree in ascending order.</span></span> <span data-ttu-id="ee002-117">Um valor de texto de **TreeOrderDescending** indica que as conversas são ordenadas de acordo com a árvore de conversa em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="ee002-117">A text value of **TreeOrderDescending** indicates that the conversations are ordered according to the conversation tree in descending order.</span></span> <span data-ttu-id="ee002-118">Um valor de texto de **DateOrderAscending** indica que as conversas são ordenadas de acordo com a data de conversa em ordem crescente.</span><span class="sxs-lookup"><span data-stu-id="ee002-118">A text value of **DateOrderAscending** indicates that the conversations are ordered according to the conversation date in ascending order.</span></span> <span data-ttu-id="ee002-119">Um valor de texto de **DateOrderDescending** indica que as conversas são ordenadas de acordo com a data de conversa em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="ee002-119">A text value of **DateOrderDescending** indicates that the conversations are ordered according to the conversation date in descending order.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ee002-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="ee002-120">Remarks</span></span>

<span data-ttu-id="ee002-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ee002-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ee002-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ee002-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ee002-123">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ee002-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ee002-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="ee002-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ee002-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ee002-125">Schema name</span></span>  <br/> |<span data-ttu-id="ee002-126">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="ee002-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ee002-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ee002-127">Validation file</span></span>  <br/> |<span data-ttu-id="ee002-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ee002-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ee002-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="ee002-129">Can be empty</span></span>  <br/> ||
   

