---
title: GlobalUniqueUnreadSenders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalUniqueUnreadSenders
api_type:
- schema
ms.assetid: 490abe30-7608-407a-923b-a4b3ddbca610
description: O elemento GlobalUniqueUnreadSenders Especifica uma lista de todas as pessoas que tenham enviado mensagens que estão atualmente não lidas nesta conversa entre todas as pastas na caixa de correio.
ms.openlocfilehash: ae088577f5aac0c7c3ee9c11fde184b70ab12e64
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823749"
---
# <a name="globaluniqueunreadsenders"></a><span data-ttu-id="49fba-103">GlobalUniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="49fba-103">GlobalUniqueUnreadSenders</span></span>

<span data-ttu-id="49fba-104">O elemento **GlobalUniqueUnreadSenders** Especifica uma lista de todas as pessoas que tenham enviado mensagens que estão atualmente não lidas nesta conversa entre todas as pastas na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="49fba-104">The **GlobalUniqueUnreadSenders** element specifies a list of all the people who have sent messages that are currently unread in this conversation across all folders in the mailbox.</span></span> 
  
[<span data-ttu-id="49fba-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="49fba-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="49fba-106">Conversas</span><span class="sxs-lookup"><span data-stu-id="49fba-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="49fba-107">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="49fba-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="49fba-108">GlobalUniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="49fba-108">GlobalUniqueUnreadSenders</span></span>](globaluniqueunreadsenders.md)
  
```XML
<GlobalUniqueUnreadSenders>
   <String/>
</GlobalUniqueUnreadSenders>
```

 <span data-ttu-id="49fba-109">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="49fba-109">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="49fba-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="49fba-110">Attributes and elements</span></span>

<span data-ttu-id="49fba-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="49fba-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="49fba-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="49fba-112">Attributes</span></span>

<span data-ttu-id="49fba-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="49fba-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="49fba-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="49fba-114">Child elements</span></span>

|<span data-ttu-id="49fba-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="49fba-115">**Element**</span></span>|<span data-ttu-id="49fba-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="49fba-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49fba-117">String</span><span class="sxs-lookup"><span data-stu-id="49fba-117">String</span></span>](string.md) <br/> |<span data-ttu-id="49fba-118">Contém um remetente única conversa.</span><span class="sxs-lookup"><span data-stu-id="49fba-118">Contains a single conversation sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="49fba-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="49fba-119">Parent elements</span></span>

|<span data-ttu-id="49fba-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="49fba-120">**Element**</span></span>|<span data-ttu-id="49fba-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="49fba-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49fba-122">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="49fba-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="49fba-123">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="49fba-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="49fba-124">Text value</span><span class="sxs-lookup"><span data-stu-id="49fba-124">Text value</span></span>

<span data-ttu-id="49fba-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="49fba-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="49fba-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="49fba-126">Remarks</span></span>

<span data-ttu-id="49fba-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="49fba-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="49fba-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="49fba-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="49fba-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="49fba-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="49fba-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="49fba-130">Schema name</span></span>  <br/> |<span data-ttu-id="49fba-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="49fba-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="49fba-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="49fba-132">Validation file</span></span>  <br/> |<span data-ttu-id="49fba-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="49fba-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="49fba-134">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="49fba-134">Can be empty</span></span>  <br/> |<span data-ttu-id="49fba-135">False</span><span class="sxs-lookup"><span data-stu-id="49fba-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="49fba-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="49fba-136">See also</span></span>



[<span data-ttu-id="49fba-137">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="49fba-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="49fba-138">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="49fba-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="49fba-139">Conversas no EWS</span><span class="sxs-lookup"><span data-stu-id="49fba-139">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

