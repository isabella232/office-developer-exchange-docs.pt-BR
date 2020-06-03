---
title: ReceivedBy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReceivedBy
api_type:
- schema
ms.assetid: ac84c9c5-d2fe-4b6f-bf4d-0444131d835b
description: O elemento ReceivedBy identifica o representante em um cenário de acesso de representante.
ms.openlocfilehash: 7cee996c15e81f77d71f42e052b14b1d21772ba1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468247"
---
# <a name="receivedby"></a><span data-ttu-id="b4d73-103">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="b4d73-103">ReceivedBy</span></span>

<span data-ttu-id="b4d73-104">O elemento **ReceivedBy** identifica o representante em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="b4d73-104">The **ReceivedBy** element identifies the delegate in a delegate access scenario.</span></span> 
  
```xml
<ReceivedBy>
   <Mailbox/>
</ReceivedBy>
```

 <span data-ttu-id="b4d73-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="b4d73-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b4d73-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b4d73-106">Attributes and elements</span></span>

<span data-ttu-id="b4d73-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b4d73-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b4d73-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b4d73-108">Attributes</span></span>

<span data-ttu-id="b4d73-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b4d73-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b4d73-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b4d73-110">Child elements</span></span>

|<span data-ttu-id="b4d73-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b4d73-111">**Element**</span></span>|<span data-ttu-id="b4d73-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b4d73-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b4d73-113">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="b4d73-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="b4d73-114">Identifica um objeto de serviço de diretório do Active Directory habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="b4d73-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b4d73-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b4d73-115">Parent elements</span></span>

|<span data-ttu-id="b4d73-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b4d73-116">**Element**</span></span>|<span data-ttu-id="b4d73-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b4d73-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b4d73-118">Message</span><span class="sxs-lookup"><span data-stu-id="b4d73-118">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b4d73-119">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b4d73-119">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="b4d73-120">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="b4d73-120">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="b4d73-121">Representa uma reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b4d73-121">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b4d73-122">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="b4d73-122">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="b4d73-123">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b4d73-123">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b4d73-124">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="b4d73-124">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="b4d73-125">Representa uma resposta de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b4d73-125">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b4d73-126">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="b4d73-126">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="b4d73-127">Representa um cancelamento de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b4d73-127">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b4d73-128">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="b4d73-128">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="b4d73-129">Representa uma resposta de aceitação para uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="b4d73-129">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="b4d73-130">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="b4d73-130">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="b4d73-131">Representa uma resposta provisória a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="b4d73-131">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="b4d73-132">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="b4d73-132">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="b4d73-133">Representa uma resposta de recusa a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="b4d73-133">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="b4d73-134">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="b4d73-134">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="b4d73-135">Contém uma resposta para o criador de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b4d73-135">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b4d73-136">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="b4d73-136">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="b4d73-137">Contém uma resposta a todos os destinatários identificados de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b4d73-137">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b4d73-138">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="b4d73-138">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="b4d73-139">Contém um item de repositório do Exchange para encaminhar aos destinatários.</span><span class="sxs-lookup"><span data-stu-id="b4d73-139">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="b4d73-140">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="b4d73-140">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="b4d73-141">Representa o objeto Response que é usado para cancelar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="b4d73-141">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b4d73-142">Comentários</span><span class="sxs-lookup"><span data-stu-id="b4d73-142">Remarks</span></span>

<span data-ttu-id="b4d73-143">O elemento **ReceivedRepresenting** é usado em conjunto com os elementos from e **ReceivedBy** nos cenários **de** acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="b4d73-143">The **ReceivedRepresenting** element is used together with the **From** and **ReceivedBy** elements in delegate access scenarios.</span></span> <span data-ttu-id="b4d73-144">A tabela a seguir lista as entidades que esses elementos representam em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="b4d73-144">The following table lists the entities that these elements represent in a delegate access scenario.</span></span> 
  
<span data-ttu-id="b4d73-145">**Elementos em um cenário de acesso de representante**</span><span class="sxs-lookup"><span data-stu-id="b4d73-145">**Elements in a delegate access scenario**</span></span>

|<span data-ttu-id="b4d73-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b4d73-146">**Element**</span></span>|<span data-ttu-id="b4d73-147">**Entidade que o elemento representa**</span><span class="sxs-lookup"><span data-stu-id="b4d73-147">**Entity that the element represent**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b4d73-148">De</span><span class="sxs-lookup"><span data-stu-id="b4d73-148">From</span></span>](from.md) <br/> |<span data-ttu-id="b4d73-149">Terceiros</span><span class="sxs-lookup"><span data-stu-id="b4d73-149">ThirdParty</span></span>  <br/> |
|[<span data-ttu-id="b4d73-150">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="b4d73-150">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="b4d73-151">Delegar</span><span class="sxs-lookup"><span data-stu-id="b4d73-151">Delegate</span></span>  <br/> |
|[<span data-ttu-id="b4d73-152">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="b4d73-152">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="b4d73-153">Principal</span><span class="sxs-lookup"><span data-stu-id="b4d73-153">Principal</span></span>  <br/> |
   
<span data-ttu-id="b4d73-154">Em um cenário de acesso de representante, se um terceiros envia uma solicitação de reunião para uma entidade que tenha um representante, o representante verá uma nova solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="b4d73-154">In a delegate access scenario, if a ThirdParty sends a meeting request to a Principal who has a Delegate, the Delegate will see a new meeting request.</span></span> <span data-ttu-id="b4d73-155">Esses elementos permitem que os representantes diferenciem mensagens que são enviadas diretamente a elas e mensagens que são enviadas a elas devido a uma regra de encaminhamento de representante.</span><span class="sxs-lookup"><span data-stu-id="b4d73-155">These elements enable delegates to distinguish between messages that are sent directly to them and messages that are sent to them because of a delegate forwarding rule.</span></span>
  
<span data-ttu-id="b4d73-156">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b4d73-156">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b4d73-157">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b4d73-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b4d73-158">Namespace</span><span class="sxs-lookup"><span data-stu-id="b4d73-158">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b4d73-159">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b4d73-159">Schema Name</span></span>  <br/> |<span data-ttu-id="b4d73-160">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b4d73-160">Types schema</span></span>  <br/> |
|<span data-ttu-id="b4d73-161">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b4d73-161">Validation File</span></span>  <br/> |<span data-ttu-id="b4d73-162">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b4d73-162">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b4d73-163">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b4d73-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="b4d73-164">False</span><span class="sxs-lookup"><span data-stu-id="b4d73-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b4d73-165">Confira também</span><span class="sxs-lookup"><span data-stu-id="b4d73-165">See also</span></span>



- [<span data-ttu-id="b4d73-166">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b4d73-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

