---
title: GetConversationItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4f7bcd0f-140c-4cbc-a5ed-daeffded1df1
description: O elemento de GetConversationItems define uma solicitação para obter um conjunto de itens que são relacionados pelo sendo na mesma conversa.
ms.openlocfilehash: 9be300318a07173e4a8e11e5a6ca78b885de1199
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752432"
---
# <a name="getconversationitems"></a><span data-ttu-id="9e50f-103">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="9e50f-103">GetConversationItems</span></span>

<span data-ttu-id="9e50f-104">O elemento de **GetConversationItems** define uma solicitação para obter um conjunto de itens que são relacionados pelo sendo na mesma conversa.</span><span class="sxs-lookup"><span data-stu-id="9e50f-104">The **GetConversationItems** element defines a request to get a set of items that are related by being in the same conversation.</span></span> 
  
```XML
<GetConversationItems>
   <ItemShape/>
   <FoldersToIgnore/>
   <MaxItemsToReturn/>
   <SortOrder/>
   <MailboxScope/>
   <Conversations/>
</GetConversationItems>
```

 <span data-ttu-id="9e50f-105">**GetConversationItemsType**</span><span class="sxs-lookup"><span data-stu-id="9e50f-105">**GetConversationItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9e50f-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="9e50f-106">Attributes and elements</span></span>

<span data-ttu-id="9e50f-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9e50f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e50f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9e50f-108">Attributes</span></span>

<span data-ttu-id="9e50f-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9e50f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9e50f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9e50f-110">Child elements</span></span>

<span data-ttu-id="9e50f-111">[ItemShape](itemshape.md) | [FoldersToIgnore](folderstoignore.md) | [MaxItemsToReturn](maxitemstoreturn.md) | [SortOrder (ConversationNodeSortOrder)](sortorder-conversationnodesortorder.md) | [MailboxScope](mailboxscope.md) | [conversas](conversations-ex15websvcsotherref.md)</span><span class="sxs-lookup"><span data-stu-id="9e50f-111">[ItemShape](itemshape.md) | [FoldersToIgnore](folderstoignore.md) | [MaxItemsToReturn](maxitemstoreturn.md) | [SortOrder (ConversationNodeSortOrder)](sortorder-conversationnodesortorder.md) | [MailboxScope](mailboxscope.md) | [Conversations](conversations-ex15websvcsotherref.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9e50f-112">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9e50f-112">Parent elements</span></span>

<span data-ttu-id="9e50f-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="9e50f-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9e50f-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="9e50f-114">Remarks</span></span>

<span data-ttu-id="9e50f-115">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9e50f-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9e50f-116">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9e50f-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9e50f-117">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="9e50f-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e50f-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="9e50f-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9e50f-119">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9e50f-119">Schema name</span></span>  <br/> |<span data-ttu-id="9e50f-120">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="9e50f-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9e50f-121">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9e50f-121">Validation file</span></span>  <br/> |<span data-ttu-id="9e50f-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9e50f-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9e50f-123">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="9e50f-123">Can be empty</span></span>  <br/> |<span data-ttu-id="9e50f-124">false</span><span class="sxs-lookup"><span data-stu-id="9e50f-124">false</span></span>  <br/> |
   

