---
title: Conversas
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
description: O elemento conversas contém uma matriz de conversas que são retornadas na resposta FindConversation.
ms.openlocfilehash: 8af1023db51dd955c544422520ec5565f09f5372
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463794"
---
# <a name="conversations"></a><span data-ttu-id="cb5f4-103">Conversas</span><span class="sxs-lookup"><span data-stu-id="cb5f4-103">Conversations</span></span>

<span data-ttu-id="cb5f4-104">O elemento **conversas** contém uma matriz de conversas que são retornadas na resposta **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="cb5f4-104">The **Conversations** element contains an array of conversations that are returned in the **FindConversation** response.</span></span> 
  
[<span data-ttu-id="cb5f4-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="cb5f4-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="cb5f4-106">Conversas</span><span class="sxs-lookup"><span data-stu-id="cb5f4-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
```xml
<Conversations>
   <Conversation/>
</Conversations>
```

 <span data-ttu-id="cb5f4-107">**ArrayOfConversationsType**</span><span class="sxs-lookup"><span data-stu-id="cb5f4-107">**ArrayOfConversationsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cb5f4-108">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="cb5f4-108">Attributes and elements</span></span>

<span data-ttu-id="cb5f4-109">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="cb5f4-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cb5f4-110">Atributos</span><span class="sxs-lookup"><span data-stu-id="cb5f4-110">Attributes</span></span>

<span data-ttu-id="cb5f4-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cb5f4-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cb5f4-112">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="cb5f4-112">Child elements</span></span>

|<span data-ttu-id="cb5f4-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cb5f4-113">**Element**</span></span>|<span data-ttu-id="cb5f4-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cb5f4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb5f4-115">Conversa (Conversatype)</span><span class="sxs-lookup"><span data-stu-id="cb5f4-115">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="cb5f4-116">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="cb5f4-116">Represents a single conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cb5f4-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="cb5f4-117">Parent elements</span></span>

|<span data-ttu-id="cb5f4-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="cb5f4-118">**Element**</span></span>|<span data-ttu-id="cb5f4-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="cb5f4-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb5f4-120">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="cb5f4-120">FindConversationResponse</span></span>](findconversationresponse.md) <br/> |<span data-ttu-id="cb5f4-121">Define uma resposta a uma solicitação **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="cb5f4-121">Defines a response to a **FindConversation** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cb5f4-122">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="cb5f4-122">Text value</span></span>

<span data-ttu-id="cb5f4-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="cb5f4-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cb5f4-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="cb5f4-124">Remarks</span></span>

<span data-ttu-id="cb5f4-125">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="cb5f4-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cb5f4-126">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="cb5f4-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cb5f4-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="cb5f4-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cb5f4-128">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="cb5f4-128">Schema name</span></span>  <br/> |<span data-ttu-id="cb5f4-129">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="cb5f4-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cb5f4-130">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="cb5f4-130">Validation file</span></span>  <br/> |<span data-ttu-id="cb5f4-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cb5f4-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cb5f4-132">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="cb5f4-132">Can be empty</span></span>  <br/> |<span data-ttu-id="cb5f4-133">False</span><span class="sxs-lookup"><span data-stu-id="cb5f4-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cb5f4-134">Confira também</span><span class="sxs-lookup"><span data-stu-id="cb5f4-134">See also</span></span>



[<span data-ttu-id="cb5f4-135">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="cb5f4-135">FindConversation operation</span></span>](findconversation-operation.md)


[<span data-ttu-id="cb5f4-136">Conversas no EWS</span><span class="sxs-lookup"><span data-stu-id="cb5f4-136">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

