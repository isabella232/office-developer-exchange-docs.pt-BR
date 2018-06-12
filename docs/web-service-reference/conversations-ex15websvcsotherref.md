---
title: Conversations
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Conversations
api_type:
- schema
ms.assetid: 1d18f98c-6457-45e9-a934-32da20885ac6
description: O elemento de conversas contém uma matriz de conversas que são retornados na resposta FindConversation.
ms.openlocfilehash: cd36364bd975d1464af9a1114c64c29543b4ec47
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751537"
---
# <a name="conversations"></a><span data-ttu-id="b987f-103">Conversations</span><span class="sxs-lookup"><span data-stu-id="b987f-103">Conversations</span></span>

<span data-ttu-id="b987f-104">O elemento de **conversas** contém uma matriz de conversas que são retornados na resposta **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="b987f-104">The **Conversations** element contains an array of conversations that are returned in the **FindConversation** response.</span></span> 
  
[<span data-ttu-id="b987f-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="b987f-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="b987f-106">Conversas</span><span class="sxs-lookup"><span data-stu-id="b987f-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
```xml
<Conversations>
   <Conversation/>
</Conversations>
```

 <span data-ttu-id="b987f-107">**ArrayOfConversationsType**</span><span class="sxs-lookup"><span data-stu-id="b987f-107">**ArrayOfConversationsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b987f-108">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b987f-108">Attributes and elements</span></span>

<span data-ttu-id="b987f-109">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b987f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b987f-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="b987f-110">Attributes</span></span>

<span data-ttu-id="b987f-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b987f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b987f-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b987f-112">Child elements</span></span>

|<span data-ttu-id="b987f-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b987f-113">**Element**</span></span>|<span data-ttu-id="b987f-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b987f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b987f-115">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="b987f-115">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="b987f-116">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="b987f-116">Represents a single conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b987f-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b987f-117">Parent elements</span></span>

|<span data-ttu-id="b987f-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b987f-118">**Element**</span></span>|<span data-ttu-id="b987f-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b987f-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b987f-120">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="b987f-120">FindConversationResponse</span></span>](findconversationresponse.md) <br/> |<span data-ttu-id="b987f-121">Define uma resposta a uma solicitação **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="b987f-121">Defines a response to a **FindConversation** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b987f-122">Text value</span><span class="sxs-lookup"><span data-stu-id="b987f-122">Text value</span></span>

<span data-ttu-id="b987f-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b987f-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b987f-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="b987f-124">Remarks</span></span>

<span data-ttu-id="b987f-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="b987f-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b987f-126">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b987f-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b987f-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="b987f-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b987f-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b987f-128">Schema name</span></span>  <br/> |<span data-ttu-id="b987f-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="b987f-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b987f-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b987f-130">Validation file</span></span>  <br/> |<span data-ttu-id="b987f-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b987f-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b987f-132">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b987f-132">Can be empty</span></span>  <br/> |<span data-ttu-id="b987f-133">False</span><span class="sxs-lookup"><span data-stu-id="b987f-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b987f-134">Ver também</span><span class="sxs-lookup"><span data-stu-id="b987f-134">See also</span></span>



[<span data-ttu-id="b987f-135">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="b987f-135">FindConversation operation</span></span>](findconversation-operation.md)


[<span data-ttu-id="b987f-136">Conversas no EWS</span><span class="sxs-lookup"><span data-stu-id="b987f-136">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

