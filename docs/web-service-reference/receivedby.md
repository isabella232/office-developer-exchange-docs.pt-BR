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
description: O elemento ReceivedBy identifica o delegado em um cenário de acesso de representante.
ms.openlocfilehash: 7918fa3320223e5cf02dd225912adfae3181e29c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19824969"
---
# <a name="receivedby"></a><span data-ttu-id="0f81c-103">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="0f81c-103">ReceivedBy</span></span>

<span data-ttu-id="0f81c-104">O elemento **ReceivedBy** identifica o delegado em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="0f81c-104">The **ReceivedBy** element identifies the delegate in a delegate access scenario.</span></span> 
  
```xml
<ReceivedBy>
   <Mailbox/>
</ReceivedBy>
```

 <span data-ttu-id="0f81c-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="0f81c-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0f81c-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="0f81c-106">Attributes and elements</span></span>

<span data-ttu-id="0f81c-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="0f81c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0f81c-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="0f81c-108">Attributes</span></span>

<span data-ttu-id="0f81c-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="0f81c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0f81c-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="0f81c-110">Child elements</span></span>

|<span data-ttu-id="0f81c-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0f81c-111">**Element**</span></span>|<span data-ttu-id="0f81c-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0f81c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f81c-113">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="0f81c-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="0f81c-114">Identifica um objeto de serviço de diretório do Active Directory habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="0f81c-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0f81c-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="0f81c-115">Parent elements</span></span>

|<span data-ttu-id="0f81c-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0f81c-116">**Element**</span></span>|<span data-ttu-id="0f81c-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0f81c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f81c-118">Message</span><span class="sxs-lookup"><span data-stu-id="0f81c-118">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="0f81c-119">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f81c-119">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="0f81c-120">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="0f81c-120">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="0f81c-121">Representa uma reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f81c-121">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0f81c-122">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="0f81c-122">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="0f81c-123">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f81c-123">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0f81c-124">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="0f81c-124">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="0f81c-125">Representa uma resposta de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f81c-125">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0f81c-126">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="0f81c-126">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="0f81c-127">Representa o cancelamento da reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f81c-127">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0f81c-128">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="0f81c-128">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="0f81c-129">Representa uma resposta de aceitar a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="0f81c-129">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="0f81c-130">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="0f81c-130">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="0f81c-131">Representa um provisório responde a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="0f81c-131">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="0f81c-132">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="0f81c-132">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="0f81c-133">Representa uma resposta recusar a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="0f81c-133">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="0f81c-134">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="0f81c-134">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="0f81c-135">Contém uma resposta para o criador de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f81c-135">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0f81c-136">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="0f81c-136">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="0f81c-137">Contém uma resposta a todos os destinatários identificados de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f81c-137">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="0f81c-138">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="0f81c-138">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="0f81c-139">Contém um item de armazenamento do Exchange para encaminhar para destinatários.</span><span class="sxs-lookup"><span data-stu-id="0f81c-139">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="0f81c-140">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="0f81c-140">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="0f81c-141">Representa o objeto de resposta é usado para cancelar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="0f81c-141">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0f81c-142">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="0f81c-142">Remarks</span></span>

<span data-ttu-id="0f81c-143">O elemento **ReceivedRepresenting** é usado em conjunto com a **partir** e **ReceivedBy** elementos em Delegar cenários de acesso.</span><span class="sxs-lookup"><span data-stu-id="0f81c-143">The **ReceivedRepresenting** element is used together with the **From** and **ReceivedBy** elements in delegate access scenarios.</span></span> <span data-ttu-id="0f81c-144">A tabela a seguir lista as entidades que esses elementos representam em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="0f81c-144">The following table lists the entities that these elements represent in a delegate access scenario.</span></span> 
  
<span data-ttu-id="0f81c-145">**Elementos em um cenário de acesso de representante**</span><span class="sxs-lookup"><span data-stu-id="0f81c-145">**Elements in a delegate access scenario**</span></span>

|<span data-ttu-id="0f81c-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0f81c-146">**Element**</span></span>|<span data-ttu-id="0f81c-147">**Entidade que representam o elemento**</span><span class="sxs-lookup"><span data-stu-id="0f81c-147">**Entity that the element represent**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f81c-148">From</span><span class="sxs-lookup"><span data-stu-id="0f81c-148">From</span></span>](from.md) <br/> |<span data-ttu-id="0f81c-149">ThirdParty</span><span class="sxs-lookup"><span data-stu-id="0f81c-149">ThirdParty</span></span>  <br/> |
|[<span data-ttu-id="0f81c-150">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="0f81c-150">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="0f81c-151">Delegar</span><span class="sxs-lookup"><span data-stu-id="0f81c-151">Delegate</span></span>  <br/> |
|[<span data-ttu-id="0f81c-152">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="0f81c-152">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="0f81c-153">Principal</span><span class="sxs-lookup"><span data-stu-id="0f81c-153">Principal</span></span>  <br/> |
   
<span data-ttu-id="0f81c-154">Em um cenário de acesso de representante, se um ThirdParty envia uma solicitação de reunião para uma entidade que tenha um representante, o delegado verá uma nova solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="0f81c-154">In a delegate access scenario, if a ThirdParty sends a meeting request to a Principal who has a Delegate, the Delegate will see a new meeting request.</span></span> <span data-ttu-id="0f81c-155">Esses elementos permitem representantes distinguir entre as mensagens enviadas a eles por causa de um representante de regra de encaminhamento e de mensagens que são enviadas diretamente a eles.</span><span class="sxs-lookup"><span data-stu-id="0f81c-155">These elements enable delegates to distinguish between messages that are sent directly to them and messages that are sent to them because of a delegate forwarding rule.</span></span>
  
<span data-ttu-id="0f81c-156">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f81c-156">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0f81c-157">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="0f81c-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0f81c-158">Namespace</span><span class="sxs-lookup"><span data-stu-id="0f81c-158">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0f81c-159">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="0f81c-159">Schema Name</span></span>  <br/> |<span data-ttu-id="0f81c-160">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="0f81c-160">Types schema</span></span>  <br/> |
|<span data-ttu-id="0f81c-161">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="0f81c-161">Validation File</span></span>  <br/> |<span data-ttu-id="0f81c-162">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0f81c-162">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0f81c-163">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="0f81c-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="0f81c-164">False</span><span class="sxs-lookup"><span data-stu-id="0f81c-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0f81c-165">Ver também</span><span class="sxs-lookup"><span data-stu-id="0f81c-165">See also</span></span>



- [<span data-ttu-id="0f81c-166">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0f81c-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

