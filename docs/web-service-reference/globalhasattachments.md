---
title: GlobalHasAttachments
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalHasAttachments
api_type:
- schema
ms.assetid: 3d075e93-14bc-479d-957f-9b7873d1db39
description: O elemento GlobalHasAttachments contém um valor que indica se o item de pelo menos uma conversa em uma caixa de correio tem um anexo.
ms.openlocfilehash: 85443c45f611a2f4bff392ffecb26029564d7558
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19823715"
---
# <a name="globalhasattachments"></a><span data-ttu-id="38897-103">GlobalHasAttachments</span><span class="sxs-lookup"><span data-stu-id="38897-103">GlobalHasAttachments</span></span>

<span data-ttu-id="38897-104">O elemento **GlobalHasAttachments** contém um valor que indica se o item de pelo menos uma conversa em uma caixa de correio tem um anexo.</span><span class="sxs-lookup"><span data-stu-id="38897-104">The **GlobalHasAttachments** element contains a value that indicates whether at least one conversation item in a mailbox has an attachment.</span></span> 
  
[<span data-ttu-id="38897-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="38897-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="38897-106">Conversas</span><span class="sxs-lookup"><span data-stu-id="38897-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="38897-107">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="38897-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="38897-108">GlobalHasAttachments</span><span class="sxs-lookup"><span data-stu-id="38897-108">GlobalHasAttachments</span></span>](globalhasattachments.md)
  
```XML
<GlobalHasAttachments/>
```

 <span data-ttu-id="38897-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="38897-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="38897-110">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="38897-110">Attributes and elements</span></span>

<span data-ttu-id="38897-111">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="38897-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="38897-112">Atributos</span><span class="sxs-lookup"><span data-stu-id="38897-112">Attributes</span></span>

<span data-ttu-id="38897-113">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="38897-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="38897-114">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="38897-114">Child elements</span></span>

<span data-ttu-id="38897-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="38897-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="38897-116">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="38897-116">Parent elements</span></span>

|<span data-ttu-id="38897-117">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="38897-117">**Element**</span></span>|<span data-ttu-id="38897-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="38897-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38897-119">Conversa (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="38897-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="38897-120">Representa uma única conversa.</span><span class="sxs-lookup"><span data-stu-id="38897-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="38897-121">Text value</span><span class="sxs-lookup"><span data-stu-id="38897-121">Text value</span></span>

<span data-ttu-id="38897-122">O valor do elemento **GlobalHasAttachments** indica se o item de pelo menos uma conversa em uma caixa de correio tem um anexo.</span><span class="sxs-lookup"><span data-stu-id="38897-122">The value of the **GlobalHasAttachments** element indicates whether at least one conversation item in a mailbox has an attachment.</span></span> <span data-ttu-id="38897-123">É necessário um valor de texto que representa um valor booleano.</span><span class="sxs-lookup"><span data-stu-id="38897-123">A text value that represents a Boolean value is required.</span></span> <span data-ttu-id="38897-124">Um valor **true** significa que a conversa tem pelo menos um anexo visível.</span><span class="sxs-lookup"><span data-stu-id="38897-124">A value of **true** means that the conversation has at least one visible attachment.</span></span> <span data-ttu-id="38897-125">Um valor **false** significa que a conversa sem anexos ou somente tem oculto anexos.</span><span class="sxs-lookup"><span data-stu-id="38897-125">A value of **false** means that the conversation either has no attachments or has only hidden attachments.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="38897-126">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="38897-126">Remarks</span></span>

<span data-ttu-id="38897-127">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda Exchange Web Services.This elemento foi introduzido no Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="38897-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="38897-128">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="38897-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="38897-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="38897-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="38897-130">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="38897-130">Schema name</span></span>  <br/> |<span data-ttu-id="38897-131">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="38897-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="38897-132">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="38897-132">Validation file</span></span>  <br/> |<span data-ttu-id="38897-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="38897-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="38897-134">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="38897-134">Can be empty</span></span>  <br/> |<span data-ttu-id="38897-135">False</span><span class="sxs-lookup"><span data-stu-id="38897-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="38897-136">Ver também</span><span class="sxs-lookup"><span data-stu-id="38897-136">See also</span></span>



[<span data-ttu-id="38897-137">Operação FindConversation</span><span class="sxs-lookup"><span data-stu-id="38897-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="38897-138">Operação ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="38897-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="38897-139">Conversas no EWS</span><span class="sxs-lookup"><span data-stu-id="38897-139">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

