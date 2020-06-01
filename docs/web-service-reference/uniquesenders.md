---
title: UniqueSenders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UniqueSenders
api_type:
- schema
ms.assetid: 1f55f2fe-b2f2-4169-83c1-fa5c752bd695
description: O elemento UniqueSenders contém uma lista de todos os remetentes de itens de conversa na pasta atual. Este elemento é somente leitura.
ms.openlocfilehash: 5c9a98a3083d02f3900cc263e0b99a570203b544
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459872"
---
# <a name="uniquesenders"></a><span data-ttu-id="8388c-104">UniqueSenders</span><span class="sxs-lookup"><span data-stu-id="8388c-104">UniqueSenders</span></span>

<span data-ttu-id="8388c-105">O elemento **UniqueSenders** contém uma lista de todos os remetentes de itens de conversa na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="8388c-105">The **UniqueSenders** element contains a list of all the senders of conversation items in the current folder.</span></span> <span data-ttu-id="8388c-106">Este elemento é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8388c-106">This element is read-only.</span></span> 
  
[<span data-ttu-id="8388c-107">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="8388c-107">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="8388c-108">Conversas</span><span class="sxs-lookup"><span data-stu-id="8388c-108">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="8388c-109">Conversa (Conversatype)</span><span class="sxs-lookup"><span data-stu-id="8388c-109">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="8388c-110">UniqueSenders</span><span class="sxs-lookup"><span data-stu-id="8388c-110">UniqueSenders</span></span>](uniquesenders.md)
  
```XML
<UniqueSenders>
   <String/>
</UniqueSenders>
```

 <span data-ttu-id="8388c-111">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="8388c-111">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8388c-112">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8388c-112">Attributes and elements</span></span>

<span data-ttu-id="8388c-113">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8388c-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8388c-114">Atributos</span><span class="sxs-lookup"><span data-stu-id="8388c-114">Attributes</span></span>

<span data-ttu-id="8388c-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8388c-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8388c-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8388c-116">Child elements</span></span>

|<span data-ttu-id="8388c-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8388c-117">**Element**</span></span>|<span data-ttu-id="8388c-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8388c-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8388c-119">String</span><span class="sxs-lookup"><span data-stu-id="8388c-119">String</span></span>](string.md) <br/> |<span data-ttu-id="8388c-120">Contém um único remetente de conversa.</span><span class="sxs-lookup"><span data-stu-id="8388c-120">Contains a single conversation sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8388c-121">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8388c-121">Parent elements</span></span>

|<span data-ttu-id="8388c-122">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8388c-122">**Element**</span></span>|<span data-ttu-id="8388c-123">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8388c-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8388c-124">Conversa (Conversatype)</span><span class="sxs-lookup"><span data-stu-id="8388c-124">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="8388c-125">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="8388c-125">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8388c-126">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="8388c-126">Text value</span></span>

<span data-ttu-id="8388c-127">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8388c-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8388c-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="8388c-128">Remarks</span></span>

<span data-ttu-id="8388c-129">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="8388c-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8388c-130">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="8388c-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8388c-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="8388c-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8388c-132">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8388c-132">Schema name</span></span>  <br/> |<span data-ttu-id="8388c-133">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="8388c-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="8388c-134">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8388c-134">Validation file</span></span>  <br/> |<span data-ttu-id="8388c-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8388c-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8388c-136">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="8388c-136">Can be empty</span></span>  <br/> |<span data-ttu-id="8388c-137">False</span><span class="sxs-lookup"><span data-stu-id="8388c-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8388c-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="8388c-138">See also</span></span>



[<span data-ttu-id="8388c-139">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="8388c-139">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="8388c-140">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="8388c-140">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="8388c-141">Conversas no EWS</span><span class="sxs-lookup"><span data-stu-id="8388c-141">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

