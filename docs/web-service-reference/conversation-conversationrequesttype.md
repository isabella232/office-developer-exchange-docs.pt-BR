---
title: Conversa (ConversationRequestType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0308b71c-d4ff-44a8-b9ca-d5965291ee1d
description: O elemento Conversation representa uma única conversa retornada em uma resposta GetConversationItems.
ms.openlocfilehash: ef56e26fda7d2bf6556069355918aa576ce14cb6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751514"
---
# <a name="conversation-conversationrequesttype"></a><span data-ttu-id="ad33c-103">Conversa (ConversationRequestType)</span><span class="sxs-lookup"><span data-stu-id="ad33c-103">Conversation (ConversationRequestType)</span></span>

<span data-ttu-id="ad33c-104">O elemento **Conversation** representa uma única conversa retornada em uma resposta **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="ad33c-104">The **Conversation** element represents a single conversation returned in a **GetConversationItems** response.</span></span> 
  
```XML
<Conversation>
   <ConversationId/>
   <SyncState/>
</Conversation>
```

 ****
## <a name="attributes-and-elements"></a><span data-ttu-id="ad33c-105">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ad33c-105">Attributes and elements</span></span>

<span data-ttu-id="ad33c-106">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ad33c-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad33c-107">Atributos</span><span class="sxs-lookup"><span data-stu-id="ad33c-107">Attributes</span></span>

<span data-ttu-id="ad33c-108">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ad33c-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad33c-109">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ad33c-109">Child elements</span></span>

<span data-ttu-id="ad33c-110">[ConversationId](conversationid.md) | [o estado de sincronização (base64Binary)](syncstate-base64binary.md)</span><span class="sxs-lookup"><span data-stu-id="ad33c-110">[ConversationId](conversationid.md) | [SyncState (base64Binary)](syncstate-base64binary.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ad33c-111">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ad33c-111">Parent elements</span></span>

[<span data-ttu-id="ad33c-112">Conversas</span><span class="sxs-lookup"><span data-stu-id="ad33c-112">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="ad33c-113">Comentários</span><span class="sxs-lookup"><span data-stu-id="ad33c-113">Remarks</span></span>

<span data-ttu-id="ad33c-114">Este elemento foi introduzido no Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ad33c-114">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ad33c-115">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ad33c-115">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ad33c-116">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ad33c-116">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad33c-117">Namespace</span><span class="sxs-lookup"><span data-stu-id="ad33c-117">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ad33c-118">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ad33c-118">Schema name</span></span>  <br/> |<span data-ttu-id="ad33c-119">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ad33c-119">Types schema</span></span>  <br/> |
|<span data-ttu-id="ad33c-120">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ad33c-120">Validation file</span></span>  <br/> |<span data-ttu-id="ad33c-121">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ad33c-121">types.xsd</span></span>  <br/> |
|<span data-ttu-id="ad33c-122">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="ad33c-122">Can be empty</span></span>  <br/> |<span data-ttu-id="ad33c-123">false</span><span class="sxs-lookup"><span data-stu-id="ad33c-123">false</span></span>  <br/> |
   

