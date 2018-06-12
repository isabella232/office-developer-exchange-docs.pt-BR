---
title: UniqueUnreadSenders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UniqueUnreadSenders
api_type:
- schema
ms.assetid: eb7d1274-ce2e-4ef8-b47f-e911174aab0c
description: O elemento UniqueUnreadSenders contém uma lista de todas as pessoas que tenham enviado mensagens que estão atualmente não lidas nesta conversa na pasta atual. Este elemento é somente leitura.
ms.openlocfilehash: d1f5593f6b86745aa27d86e9d25487f5855cb0cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837847"
---
# <a name="uniqueunreadsenders"></a><span data-ttu-id="f127f-104">UniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="f127f-104">UniqueUnreadSenders</span></span>

<span data-ttu-id="f127f-105">O elemento **UniqueUnreadSenders** contém uma lista de todas as pessoas que tenham enviado mensagens que estão atualmente não lidas nesta conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="f127f-105">The **UniqueUnreadSenders** element contains a list of all the people who have sent messages that are currently unread in this conversation in the current folder.</span></span> <span data-ttu-id="f127f-106">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f127f-106">This element is read-only.</span></span> 
  
[<span data-ttu-id="f127f-107">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="f127f-107">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="f127f-108">Conversas</span><span class="sxs-lookup"><span data-stu-id="f127f-108">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="f127f-109">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="f127f-109">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="f127f-110">UniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="f127f-110">UniqueUnreadSenders</span></span>](uniqueunreadsenders.md)
  
```XML
<UniqueUnreadSenders>
   <String/>
</UniqueUnreadSenders>
```

 <span data-ttu-id="f127f-111">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="f127f-111">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f127f-112">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="f127f-112">Attributes and elements</span></span>

<span data-ttu-id="f127f-113">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f127f-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f127f-114">Atributos</span><span class="sxs-lookup"><span data-stu-id="f127f-114">Attributes</span></span>

<span data-ttu-id="f127f-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f127f-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f127f-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f127f-116">Child elements</span></span>

|<span data-ttu-id="f127f-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f127f-117">**Element**</span></span>|<span data-ttu-id="f127f-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f127f-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f127f-119">String</span><span class="sxs-lookup"><span data-stu-id="f127f-119">String</span></span>](string.md) <br/> |<span data-ttu-id="f127f-120">Contém um remetente única conversa.</span><span class="sxs-lookup"><span data-stu-id="f127f-120">Contains a single conversation sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f127f-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f127f-121">Parent elements</span></span>

|<span data-ttu-id="f127f-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f127f-122">**Element**</span></span>|<span data-ttu-id="f127f-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f127f-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f127f-124">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="f127f-124">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="f127f-125">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="f127f-125">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f127f-126">Text value</span><span class="sxs-lookup"><span data-stu-id="f127f-126">Text value</span></span>

<span data-ttu-id="f127f-127">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="f127f-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f127f-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="f127f-128">Remarks</span></span>

<span data-ttu-id="f127f-129">Este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1). O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f127f-129">This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f127f-130">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="f127f-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f127f-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="f127f-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f127f-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f127f-132">Schema name</span></span>  <br/> |<span data-ttu-id="f127f-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f127f-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="f127f-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f127f-134">Validation file</span></span>  <br/> |<span data-ttu-id="f127f-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f127f-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f127f-136">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="f127f-136">Can be empty</span></span>  <br/> |<span data-ttu-id="f127f-137">False</span><span class="sxs-lookup"><span data-stu-id="f127f-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f127f-138">Ver também</span><span class="sxs-lookup"><span data-stu-id="f127f-138">See also</span></span>



[<span data-ttu-id="f127f-139">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="f127f-139">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="f127f-140">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="f127f-140">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="f127f-141">Conversas no EWS</span><span class="sxs-lookup"><span data-stu-id="f127f-141">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

