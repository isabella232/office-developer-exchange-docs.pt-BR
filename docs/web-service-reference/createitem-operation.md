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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751607"
---
# <a name="createitem-operation"></a><span data-ttu-id="fb1ea-103">Operação CreateItem</span><span class="sxs-lookup"><span data-stu-id="fb1ea-103">CreateItem operation</span></span>

<span data-ttu-id="fb1ea-104">A operação CreateItem cria itens no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb1ea-104">The CreateItem operation creates items in the Exchange store.</span></span>
  
## <a name="using-the-createitem-operation"></a><span data-ttu-id="fb1ea-105">Usando a operação CreateItem</span><span class="sxs-lookup"><span data-stu-id="fb1ea-105">Using the CreateItem Operation</span></span>

<span data-ttu-id="fb1ea-106">Você pode usar a operação CreateItem para criar o seguinte:</span><span class="sxs-lookup"><span data-stu-id="fb1ea-106">You can use the CreateItem operation to create the following:</span></span>
  
- <span data-ttu-id="fb1ea-107">Itens de calendário</span><span class="sxs-lookup"><span data-stu-id="fb1ea-107">Calendar items</span></span>
    
- <span data-ttu-id="fb1ea-108">Emails</span><span class="sxs-lookup"><span data-stu-id="fb1ea-108">E-mail messages</span></span>
    
- <span data-ttu-id="fb1ea-109">Solicitações de reunião</span><span class="sxs-lookup"><span data-stu-id="fb1ea-109">Meeting requests</span></span>
    
- <span data-ttu-id="fb1ea-110">Tarefas</span><span class="sxs-lookup"><span data-stu-id="fb1ea-110">Tasks</span></span>
    
- <span data-ttu-id="fb1ea-111">Contatos</span><span class="sxs-lookup"><span data-stu-id="fb1ea-111">Contacts</span></span>
    
<span data-ttu-id="fb1ea-112">Para obter mais informações, consulte o [operação CreateItem (item de calendário)](createitem-operation-calendar-item.md), [operação CreateItem (mensagem de email)](createitem-operation-email-message.md), [operação CreateItem (solicitação de reunião)](createitem-operation-meeting-request.md), [a operação de CreateItem (tarefa)](createitem-operation-task.md)e [operação CreateItem (contato) ](createitem-operation-contact.md).</span><span class="sxs-lookup"><span data-stu-id="fb1ea-112">For more information, see [CreateItem operation (calendar item)](createitem-operation-calendar-item.md), [CreateItem operation (email message)](createitem-operation-email-message.md), [CreateItem operation (meeting request)](createitem-operation-meeting-request.md), [CreateItem operation (task)](createitem-operation-task.md), and [CreateItem operation (contact)](createitem-operation-contact.md).</span></span>
  
<span data-ttu-id="fb1ea-113">A operação CreateItem suporta o uso de objetos de resposta.</span><span class="sxs-lookup"><span data-stu-id="fb1ea-113">The CreateItem operation supports the use of response objects.</span></span> <span data-ttu-id="fb1ea-114">Objetos de resposta suportam a aceitação e rejeição de reuniões e o tratamento de botões de votação que estão incluídos em uma mensagem de email padrão.</span><span class="sxs-lookup"><span data-stu-id="fb1ea-114">Response objects support the acceptance and rejection of meetings and the handling of voting buttons that are included in a standard e-mail message.</span></span> <span data-ttu-id="fb1ea-115">A tabela a seguir lista os objetos de resposta são manipulados na operação CreateItem.</span><span class="sxs-lookup"><span data-stu-id="fb1ea-115">The following table lists the response objects that are handled in the CreateItem operation.</span></span>
  
|<span data-ttu-id="fb1ea-116">**Objeto de resposta**</span><span class="sxs-lookup"><span data-stu-id="fb1ea-116">**Response object**</span></span>|<span data-ttu-id="fb1ea-117">**Action**</span><span class="sxs-lookup"><span data-stu-id="fb1ea-117">**Action**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fb1ea-118">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="fb1ea-118">AcceptItem</span></span>  <br/> |<span data-ttu-id="fb1ea-119">Aceite uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="fb1ea-119">Accept a meeting request.</span></span>  <br/> |
|<span data-ttu-id="fb1ea-120">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="fb1ea-120">CancelCalendarItem</span></span>  <br/> |<span data-ttu-id="fb1ea-121">Cancele uma reunião.</span><span class="sxs-lookup"><span data-stu-id="fb1ea-121">Cancel a meeting.</span></span> <span data-ttu-id="fb1ea-122">Isso difere da exclusão de todos os participantes porque ele exclui a reunião para o organizador também.</span><span class="sxs-lookup"><span data-stu-id="fb1ea-122">This differs from deleting all attendees because it deletes the meeting for the organizer also.</span></span>  <br/> |
|<span data-ttu-id="fb1ea-123">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="fb1ea-123">DeclineItem</span></span>  <br/> |<span data-ttu-id="fb1ea-124">Recuse uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="fb1ea-124">Decline a meeting request.</span></span>  <br/> |
|<span data-ttu-id="fb1ea-125">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="fb1ea-125">ForwardItem</span></span>  <br/> |<span data-ttu-id="fb1ea-126">Envie uma solicitação de reunião para outra pessoa como uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="fb1ea-126">Send a meeting request to another person as a meeting request.</span></span>  <br/> |
|<span data-ttu-id="fb1ea-127">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="fb1ea-127">RemoveItem</span></span>  <br/> |<span data-ttu-id="fb1ea-128">Remova uma reunião cancelada do calendário.</span><span class="sxs-lookup"><span data-stu-id="fb1ea-128">Remove a canceled meeting from the calendar.</span></span>  <br/> |
|<span data-ttu-id="fb1ea-129">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="fb1ea-129">ReplyAllToItem</span></span>  <br/> |<span data-ttu-id="fb1ea-130">Envie uma mensagem que inclui o corpo da solicitação de reunião original para todos os participantes da reunião.</span><span class="sxs-lookup"><span data-stu-id="fb1ea-130">Send a message that includes the body of the original meeting request to all attendees of the meeting.</span></span>  <br/> |
|<span data-ttu-id="fb1ea-131">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="fb1ea-131">ReplyToItem</span></span>  <br/> |<span data-ttu-id="fb1ea-132">Envie uma mensagem que inclui o corpo da solicitação de reunião original para o remetente da solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="fb1ea-132">Send a message that includes the body of the original meeting request to the sender of the meeting request.</span></span>  <br/> |
|<span data-ttu-id="fb1ea-133">SendReadReceipt</span><span class="sxs-lookup"><span data-stu-id="fb1ea-133">SendReadReceipt</span></span>  <br/> |<span data-ttu-id="fb1ea-134">Envie uma confirmação de leitura para o remetente da solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="fb1ea-134">Send a read receipt to the sender of the meeting request.</span></span>  <br/> |
|<span data-ttu-id="fb1ea-135">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="fb1ea-135">TentativelyAcceptItem</span></span>  <br/> |<span data-ttu-id="fb1ea-136">Aceite provisoriamente uma solicitação de reunião.</span><span class="sxs-lookup"><span data-stu-id="fb1ea-136">Tentatively accept a meeting request.</span></span>  <br/> |
   
<span data-ttu-id="fb1ea-137">A operação CreateItem também oferece suporte a objetos de reunião adicionais.</span><span class="sxs-lookup"><span data-stu-id="fb1ea-137">The CreateItem operation also supports additional meeting objects.</span></span> <span data-ttu-id="fb1ea-138">A tabela a seguir lista os objetos adicionais que suporta a operação CreateItem.</span><span class="sxs-lookup"><span data-stu-id="fb1ea-138">The following table lists additional objects that the CreateItem operation supports.</span></span>
  
|<span data-ttu-id="fb1ea-139">**Objeto de reunião**</span><span class="sxs-lookup"><span data-stu-id="fb1ea-139">**Meeting object**</span></span>|<span data-ttu-id="fb1ea-140">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fb1ea-140">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fb1ea-141">Mensagem de reunião</span><span class="sxs-lookup"><span data-stu-id="fb1ea-141">Meeting Message</span></span>  <br/> |<span data-ttu-id="fb1ea-142">Representa uma mensagem de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb1ea-142">Represents a meeting message in the Exchange store.</span></span> <span data-ttu-id="fb1ea-143">Esse é o objeto base para os outros objetos de reunião.</span><span class="sxs-lookup"><span data-stu-id="fb1ea-143">This is the base object for the other meeting objects.</span></span>  <br/> |
|<span data-ttu-id="fb1ea-144">Solicitação de Reunião</span><span class="sxs-lookup"><span data-stu-id="fb1ea-144">Meeting Request</span></span>  <br/> |<span data-ttu-id="fb1ea-145">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb1ea-145">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="fb1ea-146">Resposta à reunião</span><span class="sxs-lookup"><span data-stu-id="fb1ea-146">Meeting Response</span></span>  <br/> |<span data-ttu-id="fb1ea-147">Representa uma resposta de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb1ea-147">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="fb1ea-148">Cancelamento de reunião</span><span class="sxs-lookup"><span data-stu-id="fb1ea-148">Meeting Cancellation</span></span>  <br/> |<span data-ttu-id="fb1ea-149">Representa o cancelamento da reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb1ea-149">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fb1ea-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="fb1ea-150">See also</span></span>



[<span data-ttu-id="fb1ea-151">Operação CreateItem (item de calendário)</span><span class="sxs-lookup"><span data-stu-id="fb1ea-151">CreateItem operation (calendar item)</span></span>](createitem-operation-calendar-item.md)
  
[<span data-ttu-id="fb1ea-152">Operação CreateItem (contato)</span><span class="sxs-lookup"><span data-stu-id="fb1ea-152">CreateItem operation (contact)</span></span>](createitem-operation-contact.md)
  
[<span data-ttu-id="fb1ea-153">Operação CreateItem (mensagem de email)</span><span class="sxs-lookup"><span data-stu-id="fb1ea-153">CreateItem operation (email message)</span></span>](createitem-operation-email-message.md)
  
[<span data-ttu-id="fb1ea-154">Operação CreateItem (solicitação de reunião)</span><span class="sxs-lookup"><span data-stu-id="fb1ea-154">CreateItem operation (meeting request)</span></span>](createitem-operation-meeting-request.md)
  
[<span data-ttu-id="fb1ea-155">Operação CreateItem (tarefa)</span><span class="sxs-lookup"><span data-stu-id="fb1ea-155">CreateItem operation (task)</span></span>](createitem-operation-task.md)
  
 <span data-ttu-id="fb1ea-156">**CreateItemType**</span><span class="sxs-lookup"><span data-stu-id="fb1ea-156">**CreateItemType**</span></span>

