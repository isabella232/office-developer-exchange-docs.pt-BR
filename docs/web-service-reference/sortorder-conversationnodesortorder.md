---
title: SortOrder (ConversationNodeSortOrder)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9c4295c-8089-4533-b92f-2051eae9afeb
description: O elemento SortOrder especifica a ordem de classificação usada para o resultado de uma solicitação GetConversationItems.
ms.openlocfilehash: 69d362b9f769749bcc9692825b64ff486e8b60a0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530962"
---
# <a name="sortorder-conversationnodesortorder"></a><span data-ttu-id="c73c7-103">SortOrder (ConversationNodeSortOrder)</span><span class="sxs-lookup"><span data-stu-id="c73c7-103">SortOrder (ConversationNodeSortOrder)</span></span>

<span data-ttu-id="c73c7-104">O elemento **SortOrder** especifica a ordem de classificação usada para o resultado de uma solicitação **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="c73c7-104">The **SortOrder** element specifies the sort order used for the result of a **GetConversationItems** request.</span></span> 
  
```XML
<SortOrder>TreeOrderAscending | TreeOrderDescending | DateOrderAscending | DateOrderDescending</SortOrder>
```

 <span data-ttu-id="c73c7-105">**ConversationNodeSortOrder**</span><span class="sxs-lookup"><span data-stu-id="c73c7-105">**ConversationNodeSortOrder**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c73c7-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c73c7-106">Attributes and elements</span></span>

<span data-ttu-id="c73c7-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c73c7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c73c7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c73c7-108">Attributes</span></span>

<span data-ttu-id="c73c7-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c73c7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c73c7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c73c7-110">Child elements</span></span>

<span data-ttu-id="c73c7-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c73c7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c73c7-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c73c7-112">Parent elements</span></span>

[<span data-ttu-id="c73c7-113">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="c73c7-113">GetConversationItems</span></span>](getconversationitems.md)
  
## <a name="text-value"></a><span data-ttu-id="c73c7-114">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="c73c7-114">Text value</span></span>

<span data-ttu-id="c73c7-115">O valor de texto do elemento **SortOrder** é a ordem na qual as conversas foram solicitadas.</span><span class="sxs-lookup"><span data-stu-id="c73c7-115">The text value of the **SortOrder** element is the order in which conversations ordered.</span></span> <span data-ttu-id="c73c7-116">Um valor de texto de **TreeOrderAscending** indica que as conversas são ordenadas de acordo com a árvore de conversa em ordem crescente.</span><span class="sxs-lookup"><span data-stu-id="c73c7-116">A text value of **TreeOrderAscending** indicates that the conversations are ordered according to the conversation tree in ascending order.</span></span> <span data-ttu-id="c73c7-117">Um valor de texto de **TreeOrderDescending** indica que as conversas são ordenadas de acordo com a árvore de conversa em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="c73c7-117">A text value of **TreeOrderDescending** indicates that the conversations are ordered according to the conversation tree in descending order.</span></span> <span data-ttu-id="c73c7-118">Um valor de texto de **DateOrderAscending** indica que as conversas são ordenadas de acordo com a data da conversa em ordem crescente.</span><span class="sxs-lookup"><span data-stu-id="c73c7-118">A text value of **DateOrderAscending** indicates that the conversations are ordered according to the conversation date in ascending order.</span></span> <span data-ttu-id="c73c7-119">Um valor de texto de **DateOrderDescending** indica que as conversas são ordenadas de acordo com a data da conversa em ordem decrescente.</span><span class="sxs-lookup"><span data-stu-id="c73c7-119">A text value of **DateOrderDescending** indicates that the conversations are ordered according to the conversation date in descending order.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c73c7-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="c73c7-120">Remarks</span></span>

<span data-ttu-id="c73c7-121">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c73c7-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c73c7-122">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c73c7-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c73c7-123">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c73c7-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c73c7-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="c73c7-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c73c7-125">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c73c7-125">Schema name</span></span>  <br/> |<span data-ttu-id="c73c7-126">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c73c7-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c73c7-127">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c73c7-127">Validation file</span></span>  <br/> |<span data-ttu-id="c73c7-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c73c7-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c73c7-129">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="c73c7-129">Can be empty</span></span>  <br/> ||
   

