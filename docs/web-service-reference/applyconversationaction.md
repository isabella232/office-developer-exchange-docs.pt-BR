---
title: ApplyConversationAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ApplyConversationAction
api_type:
- schema
ms.assetid: e0ee8f30-529b-4d87-8bc0-b6616e75fb6b
description: O elemento ApplyConversationAction define uma solicitação para aplicar ações a itens em uma conversa.
ms.openlocfilehash: 659b3392778bb1a318c3942a0c8e314f12110c12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461685"
---
# <a name="applyconversationaction"></a><span data-ttu-id="8f6f0-103">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="8f6f0-103">ApplyConversationAction</span></span>

<span data-ttu-id="8f6f0-104">O elemento **ApplyConversationAction** define uma solicitação para aplicar ações a itens em uma conversa.</span><span class="sxs-lookup"><span data-stu-id="8f6f0-104">The **ApplyConversationAction** element defines a request to apply actions to items in a conversation.</span></span> 
  
[<span data-ttu-id="8f6f0-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="8f6f0-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
```XML
<ApplyConversationAction>
   <ConversationActions/>
</ApplyConversationAction>
```

 <span data-ttu-id="8f6f0-106">**ApplyConversationActionType**</span><span class="sxs-lookup"><span data-stu-id="8f6f0-106">**ApplyConversationActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8f6f0-107">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="8f6f0-107">Attributes and elements</span></span>

<span data-ttu-id="8f6f0-108">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="8f6f0-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8f6f0-109">Atributos</span><span class="sxs-lookup"><span data-stu-id="8f6f0-109">Attributes</span></span>

<span data-ttu-id="8f6f0-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8f6f0-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8f6f0-111">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="8f6f0-111">Child elements</span></span>

|<span data-ttu-id="8f6f0-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="8f6f0-112">**Element**</span></span>|<span data-ttu-id="8f6f0-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="8f6f0-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8f6f0-114">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="8f6f0-114">ConversationActions</span></span>](conversationactions.md) <br/> |<span data-ttu-id="8f6f0-115">Contém uma coleção de conversas e as ações a serem aplicadas a elas.</span><span class="sxs-lookup"><span data-stu-id="8f6f0-115">Contains a collection of conversations and the actions to apply to them.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8f6f0-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="8f6f0-116">Parent elements</span></span>

<span data-ttu-id="8f6f0-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8f6f0-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="8f6f0-118">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="8f6f0-118">Text value</span></span>

<span data-ttu-id="8f6f0-119">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="8f6f0-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8f6f0-120">Comentários</span><span class="sxs-lookup"><span data-stu-id="8f6f0-120">Remarks</span></span>

<span data-ttu-id="8f6f0-121">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="8f6f0-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8f6f0-122">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="8f6f0-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8f6f0-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="8f6f0-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8f6f0-124">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="8f6f0-124">Schema Name</span></span>  <br/> |<span data-ttu-id="8f6f0-125">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="8f6f0-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8f6f0-126">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="8f6f0-126">Validation File</span></span>  <br/> |<span data-ttu-id="8f6f0-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8f6f0-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8f6f0-128">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="8f6f0-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="8f6f0-129">False</span><span class="sxs-lookup"><span data-stu-id="8f6f0-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8f6f0-130">Confira também</span><span class="sxs-lookup"><span data-stu-id="8f6f0-130">See also</span></span>

- [<span data-ttu-id="8f6f0-131">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="8f6f0-131">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="8f6f0-132">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="8f6f0-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

