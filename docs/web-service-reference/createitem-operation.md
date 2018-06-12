---
title: Operação CreateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 78a52120-f1d0-4ed7-8748-436e554f75b6
description: A operação CreateItem cria itens no armazenamento do Exchange.
ms.openlocfilehash: 7e1808c685cdbaa1e8867aa7425b2cc52218d001
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751607"
---
# <a name="createitem-operation"></a><span data-ttu-id="c1272-103">Operação CreateItem</span><span class="sxs-lookup"><span data-stu-id="c1272-103">CreateItem operation</span></span>

<span data-ttu-id="c1272-104">A operação CreateItem cria itens no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c1272-104">The CreateItem operation creates items in the Exchange store.</span></span>
  
## <a name="using-the-createitem-operation"></a><span data-ttu-id="c1272-105">Usando a operação CreateItem</span><span class="sxs-lookup"><span data-stu-id="c1272-105">Using the CreateItem Operation</span></span>

<span data-ttu-id="c1272-106">Você pode usar a operação CreateItem para criar o seguinte:</span><span class="sxs-lookup"><span data-stu-id="c1272-106">You can use the CreateItem operation to create the following:</span></span>
  
- <span data-ttu-id="c1272-107">Itens de calendário</span><span class="sxs-lookup"><span data-stu-id="c1272-107">Calendar items</span></span>
    
- <span data-ttu-id="c1272-108">Emails</span><span class="sxs-lookup"><span data-stu-id="c1272-108">E-mail messages</span></span>
    
- <span data-ttu-id="c1272-109">Solicitações de reunião</span><span class="sxs-lookup"><span data-stu-id="c1272-109">Meeting requests</span></span>
    
- <span data-ttu-id="c1272-110">Tarefas</span><span class="sxs-lookup"><span data-stu-id="c1272-110">Tasks</span></span>
    
- <span data-ttu-id="c1272-111">Contatos</span><span class="sxs-lookup"><span data-stu-id="c1272-111">Contacts</span></span>
    
<span data-ttu-id="c1272-112">Para obter mais informações, consulte o [operação CreateItem (item de calendário)](createitem-operation-calendar-item.md), [operação CreateItem (mensagem de email)](createitem-operation-email-message.md), [operação CreateItem (solicitação de reunião)](createitem-operation-meeting-request.md), [a operação de CreateItem (tarefa)](createitem-operation-task.md)e [operação CreateItem (contato) ](createitem-operation-contact.md).</span><span class="sxs-lookup"><span data-stu-id="c1272-112">For more information, see [CreateItem operation (calendar item)](createitem-operation-calendar-item.md), [CreateItem operation (email message)](createitem-operation-email-message.md), [CreateItem operation (meeting request)](createitem-operation-meeting-request.md), [CreateItem operation (task)](createitem-operation-task.md), and [CreateItem operation (contact)](createitem-operation-contact.md).</span></span>
  
<span data-ttu-id="c1272-113">A operação CreateItem suporta o uso de objetos de resposta.</span><span class="sxs-lookup"><span data-stu-id="c1272-113">The CreateItem operation supports the use of response objects.</span></span> <span data-ttu-id="c1272-114">Objetos de resposta suportam a aceitação e rejeição de reuniões e o tratamento de botões de votação que estão incluídos em uma mensagem de email padrão.</span><span class="sxs-lookup"><span data-stu-id="c1272-114">Response objects support the acceptance and rejection of meetings and the handling of voting buttons that are included in a standard e-mail message.</span></span> <span data-ttu-id="c1272-115">A tabela a seguir lista os objetos de resposta são manipulados na operação CreateItem.</span><span class="sxs-lookup"><span data-stu-id="c1272-115">The following table lists the response objects that are handled in the CreateItem operation.</span></span>
  
|<span data-ttu-id="c1272-116">**Objeto de resposta**</span><span class="sxs-lookup"><span data-stu-id="c1272-116">**Response object**</span></span>|<span data-ttu-id="c1272-117">**Action**</span><span class="sxs-lookup"><span data-stu-id="c1272-117">**Action**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c1272-118">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="c1272-118">AcceptItem</span></span>  <br/> |<span data-ttu-id="c1272-119">Aceite uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="c1272-119">Accept a meeting request.</span></span>  <br/> |
|<span data-ttu-id="c1272-120">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="c1272-120">CancelCalendarItem</span></span>  <br/> |<span data-ttu-id="c1272-121">Cancele uma reunião.</span><span class="sxs-lookup"><span data-stu-id="c1272-121">Cancel a meeting.</span></span> <span data-ttu-id="c1272-122">Isso difere da exclusão de todos os participantes porque ele exclui a reunião para o organizador também.</span><span class="sxs-lookup"><span data-stu-id="c1272-122">This differs from deleting all attendees because it deletes the meeting for the organizer also.</span></span>  <br/> |
|<span data-ttu-id="c1272-123">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="c1272-123">DeclineItem</span></span>  <br/> |<span data-ttu-id="c1272-124">Recuse uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="c1272-124">Decline a meeting request.</span></span>  <br/> |
|<span data-ttu-id="c1272-125">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="c1272-125">ForwardItem</span></span>  <br/> |<span data-ttu-id="c1272-126">Envie uma solicitação de reunião para outra pessoa como uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="c1272-126">Send a meeting request to another person as a meeting request.</span></span>  <br/> |
|<span data-ttu-id="c1272-127">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="c1272-127">RemoveItem</span></span>  <br/> |<span data-ttu-id="c1272-128">Remova uma reunião cancelada do calendário.</span><span class="sxs-lookup"><span data-stu-id="c1272-128">Remove a canceled meeting from the calendar.</span></span>  <br/> |
|<span data-ttu-id="c1272-129">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="c1272-129">ReplyAllToItem</span></span>  <br/> |<span data-ttu-id="c1272-130">Envie uma mensagem que inclui o corpo da solicitação de reunião original para todos os participantes da reunião.</span><span class="sxs-lookup"><span data-stu-id="c1272-130">Send a message that includes the body of the original meeting request to all attendees of the meeting.</span></span>  <br/> |
|<span data-ttu-id="c1272-131">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="c1272-131">ReplyToItem</span></span>  <br/> |<span data-ttu-id="c1272-132">Envie uma mensagem que inclui o corpo da solicitação de reunião original para o remetente da solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="c1272-132">Send a message that includes the body of the original meeting request to the sender of the meeting request.</span></span>  <br/> |
|<span data-ttu-id="c1272-133">SendReadReceipt</span><span class="sxs-lookup"><span data-stu-id="c1272-133">SendReadReceipt</span></span>  <br/> |<span data-ttu-id="c1272-134">Envie uma confirmação de leitura para o remetente da solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="c1272-134">Send a read receipt to the sender of the meeting request.</span></span>  <br/> |
|<span data-ttu-id="c1272-135">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="c1272-135">TentativelyAcceptItem</span></span>  <br/> |<span data-ttu-id="c1272-136">Aceite provisoriamente uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="c1272-136">Tentatively accept a meeting request.</span></span>  <br/> |
   
<span data-ttu-id="c1272-137">A operação CreateItem também oferece suporte a objetos de reunião adicionais.</span><span class="sxs-lookup"><span data-stu-id="c1272-137">The CreateItem operation also supports additional meeting objects.</span></span> <span data-ttu-id="c1272-138">A tabela a seguir lista os objetos adicionais que suporta a operação CreateItem.</span><span class="sxs-lookup"><span data-stu-id="c1272-138">The following table lists additional objects that the CreateItem operation supports.</span></span>
  
|<span data-ttu-id="c1272-139">**Objeto de reunião**</span><span class="sxs-lookup"><span data-stu-id="c1272-139">**Meeting object**</span></span>|<span data-ttu-id="c1272-140">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c1272-140">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c1272-141">Mensagem de reunião</span><span class="sxs-lookup"><span data-stu-id="c1272-141">Meeting Message</span></span>  <br/> |<span data-ttu-id="c1272-142">Representa uma mensagem de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c1272-142">Represents a meeting message in the Exchange store.</span></span> <span data-ttu-id="c1272-143">Esse é o objeto base para os outros objetos de reunião.</span><span class="sxs-lookup"><span data-stu-id="c1272-143">This is the base object for the other meeting objects.</span></span>  <br/> |
|<span data-ttu-id="c1272-144">Solicitação de Reunião</span><span class="sxs-lookup"><span data-stu-id="c1272-144">Meeting Request</span></span>  <br/> |<span data-ttu-id="c1272-145">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c1272-145">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="c1272-146">Resposta à reunião</span><span class="sxs-lookup"><span data-stu-id="c1272-146">Meeting Response</span></span>  <br/> |<span data-ttu-id="c1272-147">Representa uma resposta de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c1272-147">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="c1272-148">Cancelamento de reunião</span><span class="sxs-lookup"><span data-stu-id="c1272-148">Meeting Cancellation</span></span>  <br/> |<span data-ttu-id="c1272-149">Representa o cancelamento da reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c1272-149">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c1272-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="c1272-150">See also</span></span>



[<span data-ttu-id="c1272-151">Operação CreateItem (item de calendário)</span><span class="sxs-lookup"><span data-stu-id="c1272-151">CreateItem operation (calendar item)</span></span>](createitem-operation-calendar-item.md)
  
[<span data-ttu-id="c1272-152">Operação CreateItem (contato)</span><span class="sxs-lookup"><span data-stu-id="c1272-152">CreateItem operation (contact)</span></span>](createitem-operation-contact.md)
  
[<span data-ttu-id="c1272-153">Operação CreateItem (mensagem de email)</span><span class="sxs-lookup"><span data-stu-id="c1272-153">CreateItem operation (email message)</span></span>](createitem-operation-email-message.md)
  
[<span data-ttu-id="c1272-154">Operação CreateItem (solicitação de reunião)</span><span class="sxs-lookup"><span data-stu-id="c1272-154">CreateItem operation (meeting request)</span></span>](createitem-operation-meeting-request.md)
  
[<span data-ttu-id="c1272-155">Operação CreateItem (tarefa)</span><span class="sxs-lookup"><span data-stu-id="c1272-155">CreateItem operation (task)</span></span>](createitem-operation-task.md)
  
 <span data-ttu-id="c1272-156">**CreateItemType**</span><span class="sxs-lookup"><span data-stu-id="c1272-156">**CreateItemType**</span></span>

