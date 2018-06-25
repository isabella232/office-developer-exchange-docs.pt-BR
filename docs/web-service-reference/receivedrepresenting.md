---
title: ReceivedRepresenting
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReceivedRepresenting
api_type:
- schema
ms.assetid: 1157b042-6dce-4cdc-9700-e22b749da39f
description: O elemento ReceivedRepresenting identifica a entidade em um cenário de acesso de representante.
ms.openlocfilehash: 1587fcae6975b986711e7223e50c60658833cc80
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19824973"
---
# <a name="receivedrepresenting"></a><span data-ttu-id="ffb75-103">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="ffb75-103">ReceivedRepresenting</span></span>

<span data-ttu-id="ffb75-104">O elemento **ReceivedRepresenting** identifica a entidade em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="ffb75-104">The **ReceivedRepresenting** element identifies the principal in a delegate access scenario.</span></span> 
  
```xml
<ReceivedRepresenting>
   <Mailbox/>
</ReceivedRepresenting>
```

 <span data-ttu-id="ffb75-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="ffb75-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ffb75-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="ffb75-106">Attributes and elements</span></span>

<span data-ttu-id="ffb75-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="ffb75-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ffb75-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="ffb75-108">Attributes</span></span>

<span data-ttu-id="ffb75-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="ffb75-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ffb75-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="ffb75-110">Child elements</span></span>

|<span data-ttu-id="ffb75-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ffb75-111">**Element**</span></span>|<span data-ttu-id="ffb75-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ffb75-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ffb75-113">Caixa de correio</span><span class="sxs-lookup"><span data-stu-id="ffb75-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="ffb75-114">Identifica um objeto de serviço de diretório do Active Directory habilitado para email.</span><span class="sxs-lookup"><span data-stu-id="ffb75-114">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ffb75-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="ffb75-115">Parent elements</span></span>

|<span data-ttu-id="ffb75-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ffb75-116">**Element**</span></span>|<span data-ttu-id="ffb75-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="ffb75-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ffb75-118">Message</span><span class="sxs-lookup"><span data-stu-id="ffb75-118">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ffb75-119">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ffb75-119">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="ffb75-120">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="ffb75-120">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="ffb75-121">Representa uma reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ffb75-121">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ffb75-122">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="ffb75-122">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="ffb75-123">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ffb75-123">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ffb75-124">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="ffb75-124">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="ffb75-125">Representa uma resposta de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ffb75-125">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ffb75-126">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="ffb75-126">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="ffb75-127">Representa o cancelamento da reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ffb75-127">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ffb75-128">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="ffb75-128">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="ffb75-129">Representa uma resposta de aceitar a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="ffb75-129">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="ffb75-130">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="ffb75-130">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="ffb75-131">Representa um provisório responde a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="ffb75-131">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="ffb75-132">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="ffb75-132">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="ffb75-133">Representa uma resposta recusar a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="ffb75-133">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="ffb75-134">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="ffb75-134">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="ffb75-135">Contém uma resposta para o criador de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ffb75-135">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ffb75-136">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="ffb75-136">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="ffb75-137">Contém uma resposta a todos os destinatários identificados de um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ffb75-137">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="ffb75-138">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="ffb75-138">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="ffb75-139">Contém um item de armazenamento do Exchange para encaminhar para destinatários.</span><span class="sxs-lookup"><span data-stu-id="ffb75-139">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="ffb75-140">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="ffb75-140">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="ffb75-141">Representa o objeto de resposta é usado para cancelar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="ffb75-141">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ffb75-142">Comentários</span><span class="sxs-lookup"><span data-stu-id="ffb75-142">Remarks</span></span>

<span data-ttu-id="ffb75-143">O elemento **ReceivedRepresenting** é usado em conjunto com a **partir** e **ReceivedBy** elementos em Delegar cenários de acesso.</span><span class="sxs-lookup"><span data-stu-id="ffb75-143">The **ReceivedRepresenting** element is used together with the **From** and **ReceivedBy** elements in delegate access scenarios.</span></span> <span data-ttu-id="ffb75-144">A tabela a seguir lista as entidades que esses elementos representam em um cenário de acesso de representante.</span><span class="sxs-lookup"><span data-stu-id="ffb75-144">The following table lists the entities that these elements represent in a delegate access scenario.</span></span> 
  
<span data-ttu-id="ffb75-145">**Elementos em um cenário de acesso de representante**</span><span class="sxs-lookup"><span data-stu-id="ffb75-145">**Elements in a delegate access scenario**</span></span>

|<span data-ttu-id="ffb75-146">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="ffb75-146">**Element**</span></span>|<span data-ttu-id="ffb75-147">**Entidade que representam o elemento**</span><span class="sxs-lookup"><span data-stu-id="ffb75-147">**Entity that the element represent**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ffb75-148">From</span><span class="sxs-lookup"><span data-stu-id="ffb75-148">From</span></span>](from.md) <br/> |<span data-ttu-id="ffb75-149">ThirdParty</span><span class="sxs-lookup"><span data-stu-id="ffb75-149">ThirdParty</span></span>  <br/> |
|[<span data-ttu-id="ffb75-150">ReceivedBy</span><span class="sxs-lookup"><span data-stu-id="ffb75-150">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="ffb75-151">Delegar</span><span class="sxs-lookup"><span data-stu-id="ffb75-151">Delegate</span></span>  <br/> |
|[<span data-ttu-id="ffb75-152">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="ffb75-152">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="ffb75-153">Principal</span><span class="sxs-lookup"><span data-stu-id="ffb75-153">Principal</span></span>  <br/> |
   
<span data-ttu-id="ffb75-154">Em um cenário de acesso de representante, se um ThirdParty envia uma solicitação de reunião para uma entidade que tenha um representante, o delegado verá uma nova solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="ffb75-154">In a delegate access scenario, if a ThirdParty sends a meeting request to a Principal who has a Delegate, the Delegate will see a new meeting request.</span></span> <span data-ttu-id="ffb75-155">Esses elementos permitem representantes distinguir entre as mensagens enviadas a eles por causa de um representante de regra de encaminhamento e de mensagens que são enviadas diretamente a eles.</span><span class="sxs-lookup"><span data-stu-id="ffb75-155">These elements enable delegates to distinguish between messages that are sent directly to them and messages that are sent to them because of a delegate forwarding rule.</span></span>
  
<span data-ttu-id="ffb75-156">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ffb75-156">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ffb75-157">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="ffb75-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ffb75-158">Namespace</span><span class="sxs-lookup"><span data-stu-id="ffb75-158">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ffb75-159">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="ffb75-159">Schema Name</span></span>  <br/> |<span data-ttu-id="ffb75-160">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="ffb75-160">Types schema</span></span>  <br/> |
|<span data-ttu-id="ffb75-161">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="ffb75-161">Validation File</span></span>  <br/> |<span data-ttu-id="ffb75-162">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ffb75-162">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ffb75-163">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="ffb75-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="ffb75-164">False</span><span class="sxs-lookup"><span data-stu-id="ffb75-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ffb75-165">Ver também</span><span class="sxs-lookup"><span data-stu-id="ffb75-165">See also</span></span>



- [<span data-ttu-id="ffb75-166">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="ffb75-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

