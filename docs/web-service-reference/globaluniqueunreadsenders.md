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
description: O elemento GlobalUniqueUnreadSenders especifica uma lista de todas as pessoas que enviaram mensagens não lidas atualmente nesta conversa em todas as pastas da caixa de correio.
ms.openlocfilehash: 5a26053158a262d65993dba4be90888ee97f2112
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530815"
---
# <a name="globaluniqueunreadsenders"></a><span data-ttu-id="44cbc-103">GlobalUniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="44cbc-103">GlobalUniqueUnreadSenders</span></span>

<span data-ttu-id="44cbc-104">O elemento **GlobalUniqueUnreadSenders** especifica uma lista de todas as pessoas que enviaram mensagens não lidas atualmente nesta conversa em todas as pastas da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="44cbc-104">The **GlobalUniqueUnreadSenders** element specifies a list of all the people who have sent messages that are currently unread in this conversation across all folders in the mailbox.</span></span> 
  
[<span data-ttu-id="44cbc-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="44cbc-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="44cbc-106">Conversas</span><span class="sxs-lookup"><span data-stu-id="44cbc-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="44cbc-107">Conversa (Conversatype)</span><span class="sxs-lookup"><span data-stu-id="44cbc-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="44cbc-108">GlobalUniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="44cbc-108">GlobalUniqueUnreadSenders</span></span>](globaluniqueunreadsenders.md)
  
```XML
<GlobalUniqueUnreadSenders>
   <String/>
</GlobalUniqueUnreadSenders>
```

 <span data-ttu-id="44cbc-109">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="44cbc-109">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="44cbc-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="44cbc-110">Attributes and elements</span></span>

<span data-ttu-id="44cbc-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="44cbc-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="44cbc-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="44cbc-112">Attributes</span></span>

<span data-ttu-id="44cbc-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="44cbc-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="44cbc-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="44cbc-114">Child elements</span></span>

|<span data-ttu-id="44cbc-115">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="44cbc-115">**Element**</span></span>|<span data-ttu-id="44cbc-116">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="44cbc-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44cbc-117">String</span><span class="sxs-lookup"><span data-stu-id="44cbc-117">String</span></span>](string.md) <br/> |<span data-ttu-id="44cbc-118">Contém um único remetente de conversa.</span><span class="sxs-lookup"><span data-stu-id="44cbc-118">Contains a single conversation sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="44cbc-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="44cbc-119">Parent elements</span></span>

|<span data-ttu-id="44cbc-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="44cbc-120">**Element**</span></span>|<span data-ttu-id="44cbc-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="44cbc-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44cbc-122">Conversa (Conversatype)</span><span class="sxs-lookup"><span data-stu-id="44cbc-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="44cbc-123">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="44cbc-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="44cbc-124">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="44cbc-124">Text value</span></span>

<span data-ttu-id="44cbc-125">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="44cbc-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="44cbc-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="44cbc-126">Remarks</span></span>

<span data-ttu-id="44cbc-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="44cbc-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="44cbc-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="44cbc-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="44cbc-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="44cbc-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="44cbc-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="44cbc-130">Schema name</span></span>  <br/> |<span data-ttu-id="44cbc-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="44cbc-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="44cbc-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="44cbc-132">Validation file</span></span>  <br/> |<span data-ttu-id="44cbc-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="44cbc-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="44cbc-134">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="44cbc-134">Can be empty</span></span>  <br/> |<span data-ttu-id="44cbc-135">False</span><span class="sxs-lookup"><span data-stu-id="44cbc-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="44cbc-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="44cbc-136">See also</span></span>



[<span data-ttu-id="44cbc-137">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="44cbc-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="44cbc-138">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="44cbc-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="44cbc-139">Conversas no EWS</span><span class="sxs-lookup"><span data-stu-id="44cbc-139">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

