---
title: ReferenceItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReferenceItemId
api_type:
- schema
ms.assetid: 8fd4bb12-a94b-43f5-be3b-f435684e311d
description: O elemento ReferenceItemId identifica o item ao qual se refere no objeto response.
ms.openlocfilehash: d29f2dfec8f2c23fe0ac8c84d2bb9029fce613d2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825032"
---
# <a name="referenceitemid"></a><span data-ttu-id="87113-103">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="87113-103">ReferenceItemId</span></span>

<span data-ttu-id="87113-104">O elemento **ReferenceItemId** identifica o item ao qual se refere no objeto response.</span><span class="sxs-lookup"><span data-stu-id="87113-104">The **ReferenceItemId** element identifies the item to which the response object refers.</span></span> 
  
```xml
<ReferenceItemId Id="" ChangeKey="" />
```

 <span data-ttu-id="87113-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="87113-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="87113-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="87113-106">Attributes and elements</span></span>

<span data-ttu-id="87113-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="87113-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="87113-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="87113-108">Attributes</span></span>

|<span data-ttu-id="87113-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="87113-109">**Attribute**</span></span>|<span data-ttu-id="87113-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="87113-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="87113-111">**ID de**</span><span class="sxs-lookup"><span data-stu-id="87113-111">**Id**</span></span> <br/> |<span data-ttu-id="87113-112">Identifica um item específico no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="87113-112">Identifies a specific item in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="87113-113">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="87113-113">**ChangeKey**</span></span> <br/> |<span data-ttu-id="87113-114">Identifica uma versão específica de um item.</span><span class="sxs-lookup"><span data-stu-id="87113-114">Identifies a specific version of an item.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="87113-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="87113-115">Child elements</span></span>

<span data-ttu-id="87113-116">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="87113-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="87113-117">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="87113-117">Parent elements</span></span>

|<span data-ttu-id="87113-118">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="87113-118">**Element**</span></span>|<span data-ttu-id="87113-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="87113-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="87113-120">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="87113-120">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="87113-121">Representa uma resposta de aceitar a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="87113-121">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="87113-122">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="87113-122">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md) <br/> |<span data-ttu-id="87113-123">Representa uma resposta de aceitar a um convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="87113-123">Represents an Accept reply to a sharing invitation.</span></span>  <br/> |
|[<span data-ttu-id="87113-124">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="87113-124">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="87113-125">Representa o objeto de resposta é usado para cancelar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="87113-125">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
|[<span data-ttu-id="87113-126">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="87113-126">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="87113-127">Representa uma resposta recusar a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="87113-127">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="87113-128">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="87113-128">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="87113-129">Contém um item de armazenamento do Exchange para encaminhar para destinatários.</span><span class="sxs-lookup"><span data-stu-id="87113-129">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="87113-130">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="87113-130">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="87113-131">Remove um item de armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="87113-131">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="87113-132">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="87113-132">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="87113-133">Contém uma resposta a todos os destinatários identificados de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="87113-133">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="87113-134">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="87113-134">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="87113-135">Contém uma resposta para o criador de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="87113-135">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="87113-136">SuppressReadReceipt</span><span class="sxs-lookup"><span data-stu-id="87113-136">SuppressReadReceipt</span></span>](suppressreadreceipt.md) <br/> |<span data-ttu-id="87113-137">Usada para responder às solicitações de confirmação de leitura.</span><span class="sxs-lookup"><span data-stu-id="87113-137">Used to respond to read receipt requests.</span></span>  <br/> |
|[<span data-ttu-id="87113-138">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="87113-138">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="87113-139">Representa um provisório responde a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="87113-139">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="87113-140">Comentários</span><span class="sxs-lookup"><span data-stu-id="87113-140">Remarks</span></span>

<span data-ttu-id="87113-141">O esquema que descreve este elemento está localizado no diretório Virtual do IIS que hospeda o Exchange Web Services do computador que está executando o Microsoft Exchange Server que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="87113-141">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="87113-142">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="87113-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="87113-143">Namespace</span><span class="sxs-lookup"><span data-stu-id="87113-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="87113-144">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="87113-144">Schema Name</span></span>  <br/> |<span data-ttu-id="87113-145">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="87113-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="87113-146">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="87113-146">Validation File</span></span>  <br/> |<span data-ttu-id="87113-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="87113-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="87113-148">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="87113-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="87113-149">False</span><span class="sxs-lookup"><span data-stu-id="87113-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="87113-150">Ver também</span><span class="sxs-lookup"><span data-stu-id="87113-150">See also</span></span>



- [<span data-ttu-id="87113-151">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="87113-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

