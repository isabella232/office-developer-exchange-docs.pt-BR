---
title: ProcessRightAway
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ProcessRightAway
api_type:
- schema
ms.assetid: f6bba68b-ae4f-41c1-b3e7-c8a31cdb1b0c
description: O elemento ProcessRightAway indica se a resposta é enviada assim que a ação começa o processamento no servidor ou se a resposta é enviada após a conclusão da ação. Esse elemento deve estar presente para que a resposta seja enviada de assíncrono para a ação solicitada.
ms.openlocfilehash: 58d2b926c48db5e7395df64e1f8ee9d6a8f0e73c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44434068"
---
# <a name="processrightaway"></a><span data-ttu-id="75905-104">ProcessRightAway</span><span class="sxs-lookup"><span data-stu-id="75905-104">ProcessRightAway</span></span>

<span data-ttu-id="75905-105">O elemento **ProcessRightAway** indica se a resposta é enviada assim que a ação começa o processamento no servidor ou se a resposta é enviada após a conclusão da ação.</span><span class="sxs-lookup"><span data-stu-id="75905-105">The **ProcessRightAway** element indicates whether the response is sent as soon as the action starts processing on the server or whether the response is sent after the action has completed.</span></span> <span data-ttu-id="75905-106">Esse elemento deve estar presente para que a resposta seja enviada de assíncrono para a ação solicitada.</span><span class="sxs-lookup"><span data-stu-id="75905-106">This element must be present for the response to be sent asynchronous to the requested action.</span></span> 
  
[<span data-ttu-id="75905-107">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="75905-107">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="75905-108">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="75905-108">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="75905-109">Conversation</span><span class="sxs-lookup"><span data-stu-id="75905-109">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="75905-110">ProcessRightAway</span><span class="sxs-lookup"><span data-stu-id="75905-110">ProcessRightAway</span></span>](processrightaway.md)
  
```XML
<ProcessRightAway/>
```

 <span data-ttu-id="75905-111">**xs: Boolean**</span><span class="sxs-lookup"><span data-stu-id="75905-111">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="75905-112">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="75905-112">Attributes and elements</span></span>

<span data-ttu-id="75905-113">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="75905-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="75905-114">Atributos</span><span class="sxs-lookup"><span data-stu-id="75905-114">Attributes</span></span>

<span data-ttu-id="75905-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="75905-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="75905-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="75905-116">Child elements</span></span>

<span data-ttu-id="75905-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="75905-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="75905-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="75905-118">Parent elements</span></span>

|<span data-ttu-id="75905-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="75905-119">**Element**</span></span>|<span data-ttu-id="75905-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="75905-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75905-121">Conversation</span><span class="sxs-lookup"><span data-stu-id="75905-121">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="75905-122">Contém uma única ação a ser aplicada a uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="75905-122">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="75905-123">Valor de texto</span><span class="sxs-lookup"><span data-stu-id="75905-123">Text value</span></span>

<span data-ttu-id="75905-124">Um valor **true** indica que a resposta é enviada assim que a ação começa o processamento no servidor.</span><span class="sxs-lookup"><span data-stu-id="75905-124">A text value of **true** indicates that the response is sent as soon as the action starts processing on the server.</span></span> <span data-ttu-id="75905-125">Um valor **false** indica que a resposta é enviada após a conclusão da ação.</span><span class="sxs-lookup"><span data-stu-id="75905-125">A text value of **false** indicates that the response is sent after the action has completed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="75905-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="75905-126">Remarks</span></span>

<span data-ttu-id="75905-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os serviços Web do Exchange. este elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="75905-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="75905-128">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="75905-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="75905-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="75905-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="75905-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="75905-130">Schema Name</span></span>  <br/> |<span data-ttu-id="75905-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="75905-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="75905-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="75905-132">Validation File</span></span>  <br/> |<span data-ttu-id="75905-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="75905-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="75905-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="75905-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="75905-135">False</span><span class="sxs-lookup"><span data-stu-id="75905-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="75905-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="75905-136">See also</span></span>



[<span data-ttu-id="75905-137">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="75905-137">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="75905-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="75905-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

