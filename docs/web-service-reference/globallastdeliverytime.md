---
title: GlobalLastDeliveryTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalLastDeliveryTime
api_type:
- schema
ms.assetid: a88dada9-c527-43a7-b2d3-31aad330def9
description: O elemento GlobalLastDeliveryTime contém o tempo de entrega da mensagem foi recebida pela última nesta conversa entre todas as pastas na caixa de correio.
ms.openlocfilehash: fded5cd1891a406f0979cf4bec7321779d70ab3a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823733"
---
# <a name="globallastdeliverytime"></a><span data-ttu-id="88ce6-103">GlobalLastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="88ce6-103">GlobalLastDeliveryTime</span></span>

<span data-ttu-id="88ce6-104">O elemento **GlobalLastDeliveryTime** contém o tempo de entrega da mensagem foi recebida pela última nesta conversa entre todas as pastas na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="88ce6-104">The **GlobalLastDeliveryTime** element contains the delivery time of the message that was last received in this conversation across all folders in the mailbox.</span></span> 
  
[<span data-ttu-id="88ce6-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="88ce6-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="88ce6-106">Conversas</span><span class="sxs-lookup"><span data-stu-id="88ce6-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="88ce6-107">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="88ce6-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="88ce6-108">GlobalLastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="88ce6-108">GlobalLastDeliveryTime</span></span>](globallastdeliverytime.md)
  
```XML
<GlobalLastDeliveryTime/>
```

 <span data-ttu-id="88ce6-109">**xs**</span><span class="sxs-lookup"><span data-stu-id="88ce6-109">**xs:dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88ce6-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="88ce6-110">Attributes and elements</span></span>

<span data-ttu-id="88ce6-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="88ce6-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88ce6-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="88ce6-112">Attributes</span></span>

<span data-ttu-id="88ce6-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="88ce6-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="88ce6-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="88ce6-114">Child elements</span></span>

<span data-ttu-id="88ce6-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="88ce6-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="88ce6-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="88ce6-116">Parent elements</span></span>

|<span data-ttu-id="88ce6-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="88ce6-117">**Element**</span></span>|<span data-ttu-id="88ce6-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="88ce6-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88ce6-119">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="88ce6-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="88ce6-120">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="88ce6-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="88ce6-121">Text value</span><span class="sxs-lookup"><span data-stu-id="88ce6-121">Text value</span></span>

<span data-ttu-id="88ce6-122">O valor de texto do elemento **GlobalLastDeliveryTime** é a data e hora da mensagem foi recebida pela última nesta conversa entre todas as pastas na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="88ce6-122">The text value of the **GlobalLastDeliveryTime** element is the date and time of the message that was last received in this conversation across all folders in the mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="88ce6-123">Comentários</span><span class="sxs-lookup"><span data-stu-id="88ce6-123">Remarks</span></span>

<span data-ttu-id="88ce6-124">Este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1). O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="88ce6-124">This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="88ce6-125">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="88ce6-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88ce6-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="88ce6-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="88ce6-127">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="88ce6-127">Schema name</span></span>  <br/> |<span data-ttu-id="88ce6-128">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="88ce6-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="88ce6-129">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="88ce6-129">Validation file</span></span>  <br/> |<span data-ttu-id="88ce6-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="88ce6-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="88ce6-131">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="88ce6-131">Can be empty</span></span>  <br/> |<span data-ttu-id="88ce6-132">False</span><span class="sxs-lookup"><span data-stu-id="88ce6-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="88ce6-133">Ver também</span><span class="sxs-lookup"><span data-stu-id="88ce6-133">See also</span></span>



[<span data-ttu-id="88ce6-134">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="88ce6-134">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="88ce6-135">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="88ce6-135">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="88ce6-136">Conversas no EWS</span><span class="sxs-lookup"><span data-stu-id="88ce6-136">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

