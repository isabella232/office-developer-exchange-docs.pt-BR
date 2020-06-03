---
title: ReplyTo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReplyTo
api_type:
- schema
ms.assetid: 6b6ae792-e2c4-4aa0-95cb-b49b446f1e08
description: O elemento ReplyTo identifica uma matriz de endereços aos quais as respostas devem ser enviadas.
ms.openlocfilehash: 08f9edce76fd01111922a2a07d1a63e288a0c1ee
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468324"
---
# <a name="replyto"></a><span data-ttu-id="72a47-103">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="72a47-103">ReplyTo</span></span>

<span data-ttu-id="72a47-104">O elemento **ReplyTo** identifica uma matriz de endereços aos quais as respostas devem ser enviadas.</span><span class="sxs-lookup"><span data-stu-id="72a47-104">The **ReplyTo** element identifies an array of addresses to which replies should be sent.</span></span> 
  
```xml
<ReplyTo>
   <Mailbox/>
</ReplyTo>
```

 <span data-ttu-id="72a47-105">**ArrayOfRecipientsType**</span><span class="sxs-lookup"><span data-stu-id="72a47-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="72a47-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="72a47-106">Attributes and elements</span></span>

<span data-ttu-id="72a47-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="72a47-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="72a47-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="72a47-108">Attributes</span></span>

<span data-ttu-id="72a47-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="72a47-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="72a47-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="72a47-110">Child elements</span></span>

|<span data-ttu-id="72a47-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="72a47-111">**Element**</span></span>|<span data-ttu-id="72a47-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="72a47-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="72a47-113">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="72a47-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="72a47-114">Identifica um objeto de serviço de diretório do Active Directory habilitado para email para o qual uma resposta é enviada.</span><span class="sxs-lookup"><span data-stu-id="72a47-114">Identifies a mail-enabled Active Directory directory service object to which a reply is sent.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="72a47-115">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="72a47-115">Parent elements</span></span>

|<span data-ttu-id="72a47-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="72a47-116">**Element**</span></span>|<span data-ttu-id="72a47-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="72a47-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="72a47-118">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="72a47-118">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="72a47-119">Remove um item do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="72a47-119">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="72a47-120">Mensagem</span><span class="sxs-lookup"><span data-stu-id="72a47-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="72a47-121">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="72a47-121">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="72a47-122">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="72a47-122">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="72a47-123">Representa uma reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="72a47-123">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="72a47-124">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="72a47-124">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="72a47-125">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="72a47-125">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="72a47-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="72a47-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="72a47-127">Representa uma resposta de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="72a47-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="72a47-128">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="72a47-128">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="72a47-129">Representa um cancelamento de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="72a47-129">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="72a47-130">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="72a47-130">AcceptItem</span></span>](acceptitem.md) <br/> |<span data-ttu-id="72a47-131">Representa uma resposta de aceitação para uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="72a47-131">Represents an Accept reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="72a47-132">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="72a47-132">TentativelyAcceptItem</span></span>](tentativelyacceptitem.md) <br/> |<span data-ttu-id="72a47-133">Representa uma resposta provisória a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="72a47-133">Represents a Tentative reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="72a47-134">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="72a47-134">DeclineItem</span></span>](declineitem.md) <br/> |<span data-ttu-id="72a47-135">Representa uma resposta de recusa a uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="72a47-135">Represents a Decline reply to a meeting request.</span></span>  <br/> |
|[<span data-ttu-id="72a47-136">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="72a47-136">ReplyToItem</span></span>](replytoitem.md) <br/> |<span data-ttu-id="72a47-137">Contém uma resposta para o criador de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="72a47-137">Contains a reply to the creator of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="72a47-138">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="72a47-138">ReplyAllToItem</span></span>](replyalltoitem.md) <br/> |<span data-ttu-id="72a47-139">Contém uma resposta a todos os destinatários identificados de um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="72a47-139">Contains a reply to all identified recipients of an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="72a47-140">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="72a47-140">ForwardItem</span></span>](forwarditem.md) <br/> |<span data-ttu-id="72a47-141">Contém um item de repositório do Exchange para encaminhar aos destinatários.</span><span class="sxs-lookup"><span data-stu-id="72a47-141">Contains an Exchange store item to forward to recipients.</span></span>  <br/> |
|[<span data-ttu-id="72a47-142">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="72a47-142">CancelCalendarItem</span></span>](cancelcalendaritem.md) <br/> |<span data-ttu-id="72a47-143">Representa o objeto Response que é usado para cancelar uma reunião.</span><span class="sxs-lookup"><span data-stu-id="72a47-143">Represents the response object that is used to cancel a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="72a47-144">Comentários</span><span class="sxs-lookup"><span data-stu-id="72a47-144">Remarks</span></span>

<span data-ttu-id="72a47-145">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="72a47-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="72a47-146">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="72a47-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="72a47-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="72a47-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="72a47-148">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="72a47-148">Schema Name</span></span>  <br/> |<span data-ttu-id="72a47-149">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="72a47-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="72a47-150">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="72a47-150">Validation File</span></span>  <br/> |<span data-ttu-id="72a47-151">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="72a47-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="72a47-152">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="72a47-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="72a47-153">False</span><span class="sxs-lookup"><span data-stu-id="72a47-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="72a47-154">Confira também</span><span class="sxs-lookup"><span data-stu-id="72a47-154">See also</span></span>



- [<span data-ttu-id="72a47-155">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="72a47-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

