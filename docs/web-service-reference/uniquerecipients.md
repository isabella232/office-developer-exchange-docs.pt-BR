---
title: UniqueRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UniqueRecipients
api_type:
- schema
ms.assetid: 9f46ed05-5370-46ee-80f5-83f97224c76e
description: O elemento UniqueRecipients contém a lista de destinatários de uma conversa em uma pasta específica. Este elemento é somente leitura.
ms.openlocfilehash: 710559e599c6cec1db371165f01187f8960024f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837854"
---
# <a name="uniquerecipients"></a><span data-ttu-id="47652-104">UniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="47652-104">UniqueRecipients</span></span>

<span data-ttu-id="47652-105">O elemento **UniqueRecipients** contém a lista de destinatários de uma conversa em uma pasta específica.</span><span class="sxs-lookup"><span data-stu-id="47652-105">The **UniqueRecipients** element contains the recipient list of a conversation in a particular folder.</span></span> <span data-ttu-id="47652-106">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="47652-106">This element is read-only.</span></span> 
  
[<span data-ttu-id="47652-107">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="47652-107">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="47652-108">Conversas</span><span class="sxs-lookup"><span data-stu-id="47652-108">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="47652-109">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="47652-109">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="47652-110">UniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="47652-110">UniqueRecipients</span></span>](uniquerecipients.md)
  
```XML
<UniqueRecpients>
   <String/>
</UniqueRecpients>
```

 <span data-ttu-id="47652-111">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="47652-111">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="47652-112">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="47652-112">Attributes and elements</span></span>

<span data-ttu-id="47652-113">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="47652-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="47652-114">Atributos</span><span class="sxs-lookup"><span data-stu-id="47652-114">Attributes</span></span>

<span data-ttu-id="47652-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="47652-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="47652-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="47652-116">Child elements</span></span>

|<span data-ttu-id="47652-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="47652-117">**Element**</span></span>|<span data-ttu-id="47652-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="47652-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47652-119">String</span><span class="sxs-lookup"><span data-stu-id="47652-119">String</span></span>](string.md) <br/> |<span data-ttu-id="47652-120">Representa um único destinatário de uma conversa.</span><span class="sxs-lookup"><span data-stu-id="47652-120">Represents a unique recipient of a conversation.</span></span> <span data-ttu-id="47652-121">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="47652-121">This element is read-only.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="47652-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="47652-122">Parent elements</span></span>

|<span data-ttu-id="47652-123">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="47652-123">**Element**</span></span>|<span data-ttu-id="47652-124">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="47652-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47652-125">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="47652-125">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="47652-126">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="47652-126">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="47652-127">Text value</span><span class="sxs-lookup"><span data-stu-id="47652-127">Text value</span></span>

<span data-ttu-id="47652-128">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="47652-128">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="47652-129">Comentários</span><span class="sxs-lookup"><span data-stu-id="47652-129">Remarks</span></span>

<span data-ttu-id="47652-130">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="47652-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="47652-131">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="47652-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="47652-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="47652-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="47652-133">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="47652-133">Schema name</span></span>  <br/> |<span data-ttu-id="47652-134">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="47652-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="47652-135">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="47652-135">Validation file</span></span>  <br/> |<span data-ttu-id="47652-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="47652-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="47652-137">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="47652-137">Can be empty</span></span>  <br/> |<span data-ttu-id="47652-138">False</span><span class="sxs-lookup"><span data-stu-id="47652-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="47652-139">Ver também</span><span class="sxs-lookup"><span data-stu-id="47652-139">See also</span></span>



[<span data-ttu-id="47652-140">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="47652-140">FindConversation operation</span></span>](findconversation-operation.md)


[<span data-ttu-id="47652-141">Conversas no EWS</span><span class="sxs-lookup"><span data-stu-id="47652-141">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

