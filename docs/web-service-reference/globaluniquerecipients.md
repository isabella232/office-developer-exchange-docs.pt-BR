---
title: GlobalUniqueRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalUniqueRecipients
api_type:
- schema
ms.assetid: 67379c1c-85d9-4b11-8f17-ad9d24904788
description: O elemento GlobalUniqueRecipients contém a lista de destinatários de uma conversa agregada em uma caixa de correio.
ms.openlocfilehash: 5eb6e60d3ece8d8369f4603e36ffaaf72a3e459d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823742"
---
# <a name="globaluniquerecipients"></a><span data-ttu-id="0c1da-103">GlobalUniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="0c1da-103">GlobalUniqueRecipients</span></span>

<span data-ttu-id="0c1da-104">O elemento **GlobalUniqueRecipients** contém a lista de destinatários de uma conversa agregada em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0c1da-104">The **GlobalUniqueRecipients** element contains the recipient list of a conversation aggregated across a mailbox.</span></span> 
  
[<span data-ttu-id="0c1da-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="0c1da-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="0c1da-106">Conversas</span><span class="sxs-lookup"><span data-stu-id="0c1da-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="0c1da-107">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="0c1da-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="0c1da-108">GlobalUniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="0c1da-108">GlobalUniqueRecipients</span></span>](globaluniquerecipients.md)
  
```XML
<GlobalUniqueRecipients>
   <String/>
</GlobalUniqueRecipients>
```

 <span data-ttu-id="0c1da-109">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="0c1da-109">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0c1da-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0c1da-110">Attributes and elements</span></span>

<span data-ttu-id="0c1da-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0c1da-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0c1da-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="0c1da-112">Attributes</span></span>

<span data-ttu-id="0c1da-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0c1da-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0c1da-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0c1da-114">Child elements</span></span>

|<span data-ttu-id="0c1da-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0c1da-115">**Element**</span></span>|<span data-ttu-id="0c1da-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0c1da-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c1da-117">String</span><span class="sxs-lookup"><span data-stu-id="0c1da-117">String</span></span>](string.md) <br/> |<span data-ttu-id="0c1da-118">Contém um destinatário única conversa.</span><span class="sxs-lookup"><span data-stu-id="0c1da-118">Contains a single conversation recipient.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0c1da-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0c1da-119">Parent elements</span></span>

|<span data-ttu-id="0c1da-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0c1da-120">**Element**</span></span>|<span data-ttu-id="0c1da-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0c1da-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c1da-122">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="0c1da-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="0c1da-123">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="0c1da-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0c1da-124">Text value</span><span class="sxs-lookup"><span data-stu-id="0c1da-124">Text value</span></span>

<span data-ttu-id="0c1da-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0c1da-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0c1da-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="0c1da-126">Remarks</span></span>

<span data-ttu-id="0c1da-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0c1da-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0c1da-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0c1da-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0c1da-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="0c1da-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0c1da-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0c1da-130">Schema name</span></span>  <br/> |<span data-ttu-id="0c1da-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0c1da-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="0c1da-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0c1da-132">Validation file</span></span>  <br/> |<span data-ttu-id="0c1da-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0c1da-133">types.xsd</span></span>  <br/> |
|<span data-ttu-id="0c1da-134">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="0c1da-134">Can be empty</span></span>  <br/> |<span data-ttu-id="0c1da-135">False</span><span class="sxs-lookup"><span data-stu-id="0c1da-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0c1da-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="0c1da-136">See also</span></span>



[<span data-ttu-id="0c1da-137">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="0c1da-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="0c1da-138">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="0c1da-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="0c1da-139">Conversas no EWS</span><span class="sxs-lookup"><span data-stu-id="0c1da-139">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

