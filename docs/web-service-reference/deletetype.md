---
title: DeleteType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteType
api_type:
- schema
ms.assetid: 6e3136cd-9cb4-493a-aa85-9678f719002d
description: O elemento DeleteType indica como os itens em uma conversa são excluídos.
ms.openlocfilehash: 199f7afc29fe866865509d2fb90d24944113d5c0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44442630"
---
# <a name="deletetype"></a><span data-ttu-id="989a0-103">DeleteType</span><span class="sxs-lookup"><span data-stu-id="989a0-103">DeleteType</span></span>

<span data-ttu-id="989a0-104">O elemento **DeleteType** indica como os itens em uma conversa são excluídos.</span><span class="sxs-lookup"><span data-stu-id="989a0-104">The **DeleteType** element indicates how items in a conversation are deleted.</span></span> 
  
- [<span data-ttu-id="989a0-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="989a0-105">ApplyConversationAction</span></span>](applyconversationaction.md)  
- [<span data-ttu-id="989a0-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="989a0-106">ConversationActions</span></span>](conversationactions.md)  
- [<span data-ttu-id="989a0-107">Conversation</span><span class="sxs-lookup"><span data-stu-id="989a0-107">ConversationAction</span></span>](conversationaction.md)  
- [<span data-ttu-id="989a0-108">DeleteType</span><span class="sxs-lookup"><span data-stu-id="989a0-108">DeleteType</span></span>](deletetype.md)
  
```XML
<DeleteType> HardDelete | MoveToDeletedItems | SoftDelete </DeleteType>
```

 <span data-ttu-id="989a0-109">**Alienatype**</span><span class="sxs-lookup"><span data-stu-id="989a0-109">**DisposalType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="989a0-110">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="989a0-110">Attributes and elements</span></span>

<span data-ttu-id="989a0-111">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="989a0-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="989a0-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="989a0-112">Attributes</span></span>

<span data-ttu-id="989a0-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="989a0-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="989a0-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="989a0-114">Child elements</span></span>

<span data-ttu-id="989a0-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="989a0-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="989a0-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="989a0-116">Parent elements</span></span>

|<span data-ttu-id="989a0-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="989a0-117">**Element**</span></span>|<span data-ttu-id="989a0-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="989a0-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="989a0-119">Conversation</span><span class="sxs-lookup"><span data-stu-id="989a0-119">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="989a0-120">Contém uma única ação a ser aplicada a uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="989a0-120">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="989a0-121">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="989a0-121">Text value</span></span>

<span data-ttu-id="989a0-122">O valor de texto do elemento **DeleteType** indica como os itens em uma conversa são excluídos.</span><span class="sxs-lookup"><span data-stu-id="989a0-122">The text value of the **DeleteType** element indicates how items in a conversation are deleted.</span></span> <span data-ttu-id="989a0-123">Estes são os valores de texto possíveis:</span><span class="sxs-lookup"><span data-stu-id="989a0-123">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="989a0-124">HardDelete-indica que os itens em uma conversa são removidos permanentemente do banco de dados de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="989a0-124">HardDelete - Indicates that items in a conversation are permanently removed from the mailbox database.</span></span>
    
- <span data-ttu-id="989a0-125">MoveToDeleteItems-indica que os itens em uma conversa são movidos para a pasta itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="989a0-125">MoveToDeleteItems - Indicates that items in a conversation are moved to the Deleted Items folder.</span></span>
    
- <span data-ttu-id="989a0-126">SoftDelete-indica que os itens em uma conversa serão movidos para o dumpster se o dumpster estiver habilitado.</span><span class="sxs-lookup"><span data-stu-id="989a0-126">SoftDelete - Indicates that items in a conversation are moved to the dumpster if the dumpster is enabled.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="989a0-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="989a0-127">Remarks</span></span>

<span data-ttu-id="989a0-128">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="989a0-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="989a0-129">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="989a0-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="989a0-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="989a0-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="989a0-131">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="989a0-131">Schema Name</span></span>  <br/> |<span data-ttu-id="989a0-132">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="989a0-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="989a0-133">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="989a0-133">Validation File</span></span>  <br/> |<span data-ttu-id="989a0-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="989a0-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="989a0-135">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="989a0-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="989a0-136">False</span><span class="sxs-lookup"><span data-stu-id="989a0-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="989a0-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="989a0-137">See also</span></span>

- [<span data-ttu-id="989a0-138">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="989a0-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="989a0-139">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="989a0-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

