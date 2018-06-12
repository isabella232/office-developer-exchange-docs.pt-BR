---
title: MailboxScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c9778823-f290-4827-ba19-5f391ed4f877
description: O elemento MailboxScope identifica se uma pesquisa ou fetch para uma conversa deve abranger a caixa de correio primária, caixa de correio de arquivo morto ou ambos os primário e arquivar caixas de correio.
ms.openlocfilehash: 89c9776079d686b114d6b744150f1c6df3711eab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824293"
---
# <a name="mailboxscope"></a><span data-ttu-id="fd405-103">MailboxScope</span><span class="sxs-lookup"><span data-stu-id="fd405-103">MailboxScope</span></span>

<span data-ttu-id="fd405-104">O elemento **MailboxScope** identifica se uma pesquisa ou fetch para uma conversa deve abranger a caixa de correio primária, caixa de correio de arquivo morto ou ambos os primário e arquivar caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="fd405-104">The **MailboxScope** element identifies whether a search or fetch for a conversation should span either the primary mailbox, archive mailbox, or both the primary and archive mailbox.</span></span> 
  
```XML
<MailboxScope> PrimaryOnly | ArchiveOnly | All </MailboxScope>
```

<span data-ttu-id="fd405-105">**MailboxSearchLocationType**</span><span class="sxs-lookup"><span data-stu-id="fd405-105">**MailboxSearchLocationType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="fd405-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="fd405-106">Attributes and elements</span></span>

<span data-ttu-id="fd405-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="fd405-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd405-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="fd405-108">Attributes</span></span>

<span data-ttu-id="fd405-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fd405-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fd405-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="fd405-110">Child elements</span></span>

<span data-ttu-id="fd405-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fd405-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fd405-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="fd405-112">Parent elements</span></span>

<span data-ttu-id="fd405-113">[FindConversation](findconversation.md) | [GetConversationItems](getconversationitems.md) | [conversa (ConversationType)](conversation-conversationtype.md)</span><span class="sxs-lookup"><span data-stu-id="fd405-113">[FindConversation](findconversation.md) | [GetConversationItems](getconversationitems.md) | [Conversation (ConversationType)](conversation-conversationtype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="fd405-114">Text value</span><span class="sxs-lookup"><span data-stu-id="fd405-114">Text value</span></span>

<span data-ttu-id="fd405-115">O valor de texto do elemento **MailboxScope** é o escopo para localizar ou obter itens em uma conversa entre um dos caixas de correio primárias, arquivar caixas de correio ou ambos primário e arquivar caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="fd405-115">The text value of the **MailboxScope** element is the scope for finding or getting items in a conversation across either primary mailboxes, archive mailboxes, or both primary and archive mailboxes.</span></span> <span data-ttu-id="fd405-116">Um valor de texto de **PrimaryOnly** indica um escopo que refere-se a caixa de correio principal para um usuário.</span><span class="sxs-lookup"><span data-stu-id="fd405-116">A text value of **PrimaryOnly** indicates a scope that targets the primary mailbox for a user.</span></span> <span data-ttu-id="fd405-117">Um valor de texto de **ArchiveOnly** indica um escopo que refere-se a caixa de correio de arquivo morto para um usuário.</span><span class="sxs-lookup"><span data-stu-id="fd405-117">A text value of **ArchiveOnly** indicates a scope that targets the archive mailbox for a user.</span></span> <span data-ttu-id="fd405-118">Um valor de texto de **todas as** indica um escopo que refere-se a caixa de correio principal e a caixa de correio de arquivo morto.</span><span class="sxs-lookup"><span data-stu-id="fd405-118">A text value of **All** indicates a scope that targets both the primary mailbox and archive mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="fd405-119">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="fd405-119">Remarks</span></span>

<span data-ttu-id="fd405-120">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="fd405-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fd405-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fd405-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fd405-122">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="fd405-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd405-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="fd405-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fd405-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="fd405-124">Schema name</span></span>  <br/> |<span data-ttu-id="fd405-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="fd405-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fd405-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="fd405-126">Validation file</span></span>  <br/> |<span data-ttu-id="fd405-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fd405-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fd405-128">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="fd405-128">Can be empty</span></span>  <br/> |<span data-ttu-id="fd405-129">false</span><span class="sxs-lookup"><span data-stu-id="fd405-129">false</span></span>  <br/> |
   

