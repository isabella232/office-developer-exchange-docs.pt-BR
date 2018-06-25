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
description: O elemento ProcessRightAway indica se a resposta é enviada assim que a ação inicia o processamento no servidor ou se a resposta é enviada depois que a ação foi concluída. Este elemento deve estar presente para a resposta a ser enviado assíncrona para a ação solicitada.
ms.openlocfilehash: 940f8e8fa0a53801ce1c3a45c3aecf1bdb6f519d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824898"
---
# <a name="processrightaway"></a><span data-ttu-id="92d8b-104">ProcessRightAway</span><span class="sxs-lookup"><span data-stu-id="92d8b-104">ProcessRightAway</span></span>

<span data-ttu-id="92d8b-105">O elemento **ProcessRightAway** indica se a resposta é enviada assim que a ação inicia o processamento no servidor ou se a resposta é enviada depois que a ação foi concluída.</span><span class="sxs-lookup"><span data-stu-id="92d8b-105">The **ProcessRightAway** element indicates whether the response is sent as soon as the action starts processing on the server or whether the response is sent after the action has completed.</span></span> <span data-ttu-id="92d8b-106">Este elemento deve estar presente para a resposta a ser enviado assíncrona para a ação solicitada.</span><span class="sxs-lookup"><span data-stu-id="92d8b-106">This element must be present for the response to be sent asynchronous to the requested action.</span></span> 
  
[<span data-ttu-id="92d8b-107">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="92d8b-107">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="92d8b-108">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="92d8b-108">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="92d8b-109">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="92d8b-109">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="92d8b-110">ProcessRightAway</span><span class="sxs-lookup"><span data-stu-id="92d8b-110">ProcessRightAway</span></span>](processrightaway.md)
  
```XML
<ProcessRightAway/>
```

 <span data-ttu-id="92d8b-111">**xs:Boolean**</span><span class="sxs-lookup"><span data-stu-id="92d8b-111">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="92d8b-112">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="92d8b-112">Attributes and elements</span></span>

<span data-ttu-id="92d8b-113">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="92d8b-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="92d8b-114">Atributos</span><span class="sxs-lookup"><span data-stu-id="92d8b-114">Attributes</span></span>

<span data-ttu-id="92d8b-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="92d8b-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="92d8b-116">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="92d8b-116">Child elements</span></span>

<span data-ttu-id="92d8b-117">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="92d8b-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="92d8b-118">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="92d8b-118">Parent elements</span></span>

|<span data-ttu-id="92d8b-119">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="92d8b-119">**Element**</span></span>|<span data-ttu-id="92d8b-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="92d8b-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92d8b-121">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="92d8b-121">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="92d8b-122">Contém uma única ação a ser aplicado a uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="92d8b-122">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="92d8b-123">Text value</span><span class="sxs-lookup"><span data-stu-id="92d8b-123">Text value</span></span>

<span data-ttu-id="92d8b-124">Um valor de texto de **true** indica que a resposta é enviada assim que a ação inicia o processamento no servidor.</span><span class="sxs-lookup"><span data-stu-id="92d8b-124">A text value of **true** indicates that the response is sent as soon as the action starts processing on the server.</span></span> <span data-ttu-id="92d8b-125">Um valor de texto de **false** indica que a resposta é enviada depois que a ação foi concluída.</span><span class="sxs-lookup"><span data-stu-id="92d8b-125">A text value of **false** indicates that the response is sent after the action has completed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="92d8b-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="92d8b-126">Remarks</span></span>

<span data-ttu-id="92d8b-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="92d8b-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="92d8b-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="92d8b-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="92d8b-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="92d8b-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="92d8b-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="92d8b-130">Schema Name</span></span>  <br/> |<span data-ttu-id="92d8b-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="92d8b-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="92d8b-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="92d8b-132">Validation File</span></span>  <br/> |<span data-ttu-id="92d8b-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="92d8b-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="92d8b-134">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="92d8b-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="92d8b-135">False</span><span class="sxs-lookup"><span data-stu-id="92d8b-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="92d8b-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="92d8b-136">See also</span></span>



[<span data-ttu-id="92d8b-137">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="92d8b-137">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="92d8b-138">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="92d8b-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

