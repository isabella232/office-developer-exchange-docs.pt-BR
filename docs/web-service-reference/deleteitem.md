---
title: DeleteItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItem
api_type:
- schema
ms.assetid: 055cdee8-3c7d-47db-9f27-740f4a674729
description: O elemento DeleteItem define uma solicitação para excluir um item de uma caixa de correio no repositório do Exchange.
ms.openlocfilehash: ed13ee32b487f49740aed80e8705257d3e2e6938
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529200"
---
# <a name="deleteitem"></a><span data-ttu-id="89168-103">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="89168-103">DeleteItem</span></span>

<span data-ttu-id="89168-104">O elemento **DeleteItem** define uma solicitação para excluir um item de uma caixa de correio no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="89168-104">The **DeleteItem** element defines a request to delete an item from a mailbox in the Exchange store.</span></span> 
  
```XML
<DeleteItem DeleteType="" SendMeetingCancellations="" AffectedTaskOccurrences="" SuppressReadReceipts="">
   <ItemIds/>
</DeleteItem>
```

 <span data-ttu-id="89168-105">**DeleteItemType**</span><span class="sxs-lookup"><span data-stu-id="89168-105">**DeleteItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="89168-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="89168-106">Attributes and elements</span></span>

<span data-ttu-id="89168-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="89168-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89168-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="89168-108">Attributes</span></span>

|<span data-ttu-id="89168-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="89168-109">**Attribute**</span></span>|<span data-ttu-id="89168-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="89168-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="89168-111">**DeleteType**</span><span class="sxs-lookup"><span data-stu-id="89168-111">**DeleteType**</span></span> <br/> |<span data-ttu-id="89168-112">Descreve como um item é excluído.</span><span class="sxs-lookup"><span data-stu-id="89168-112">Describes how an item is deleted.</span></span> <span data-ttu-id="89168-113">Esse atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="89168-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="89168-114">**SendMeetingCancellations**</span><span class="sxs-lookup"><span data-stu-id="89168-114">**SendMeetingCancellations**</span></span> <br/> |<span data-ttu-id="89168-115">Descreve se uma exclusão de item de calendário é comunicada aos participantes.</span><span class="sxs-lookup"><span data-stu-id="89168-115">Describes whether a calendar item deletion is communicated to attendees.</span></span> <span data-ttu-id="89168-116">Esse atributo é obrigatório quando os itens de calendário são excluídos.</span><span class="sxs-lookup"><span data-stu-id="89168-116">This attribute is required when calendar items are deleted.</span></span> <span data-ttu-id="89168-117">Esse atributo é opcional se itens que não são de calendário são excluídos.</span><span class="sxs-lookup"><span data-stu-id="89168-117">This attribute is optional if non-calendar items are deleted.</span></span>  <br/> |
|<span data-ttu-id="89168-118">**AffectedTaskOccurrences**</span><span class="sxs-lookup"><span data-stu-id="89168-118">**AffectedTaskOccurrences**</span></span> <br/> |<span data-ttu-id="89168-119">Descreve se uma instância de tarefa ou um mestre de tarefa é excluído por uma [Operação DeleteItem](deleteitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="89168-119">Describes whether a task instance or a task master is deleted by a [DeleteItem operation](deleteitem-operation.md).</span></span> <span data-ttu-id="89168-120">Esse atributo é necessário quando as tarefas são excluídas.</span><span class="sxs-lookup"><span data-stu-id="89168-120">This attribute is required when tasks are deleted.</span></span> <span data-ttu-id="89168-121">Este atributo é opcional quando itens de não tarefa são excluídos.</span><span class="sxs-lookup"><span data-stu-id="89168-121">This attribute is optional when non-task items are deleted.</span></span>  <br/> |
|<span data-ttu-id="89168-122">**SuppressReadReceipts**</span><span class="sxs-lookup"><span data-stu-id="89168-122">**SuppressReadReceipts**</span></span> <br/> |<span data-ttu-id="89168-123">Indica se as confirmações de leitura para o item excluído são suprimidas.</span><span class="sxs-lookup"><span data-stu-id="89168-123">Indicates whether read receipts for the deleted item are suppressed.</span></span> <span data-ttu-id="89168-124">Um valor de texto **true**, indica que as confirmações de leitura são suprimidas.</span><span class="sxs-lookup"><span data-stu-id="89168-124">A text value of **true**, indicates that the read receipts are suppressed.</span></span> <span data-ttu-id="89168-125">Um valor **false** indica que as confirmações de leitura são enviadas para o remetente.</span><span class="sxs-lookup"><span data-stu-id="89168-125">A value of **false** indicates that the read receipts are sent to the sender.</span></span> <span data-ttu-id="89168-126">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="89168-126">This attribute is optional.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="89168-127">Atributo DeleteType</span><span class="sxs-lookup"><span data-stu-id="89168-127">DeleteType attribute</span></span>

|<span data-ttu-id="89168-128">**Valor**</span><span class="sxs-lookup"><span data-stu-id="89168-128">**Value**</span></span>|<span data-ttu-id="89168-129">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="89168-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="89168-130">HardDelete</span><span class="sxs-lookup"><span data-stu-id="89168-130">HardDelete</span></span>  <br/> |<span data-ttu-id="89168-131">Um item é removido permanentemente da loja.</span><span class="sxs-lookup"><span data-stu-id="89168-131">An item is permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="89168-132">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="89168-132">SoftDelete</span></span>  <br/> |<span data-ttu-id="89168-133">Um item será movido para o dumpster se o dumpster estiver habilitado.</span><span class="sxs-lookup"><span data-stu-id="89168-133">An item is moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="89168-134">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="89168-134">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="89168-135">Um item é movido para a Itens Excluídos.</span><span class="sxs-lookup"><span data-stu-id="89168-135">An item is moved to the Deleted Items folder.</span></span>  <br/> |
   
#### <a name="sendmeetingcancellations-attribute"></a><span data-ttu-id="89168-136">Atributo SendMeetingCancellations</span><span class="sxs-lookup"><span data-stu-id="89168-136">SendMeetingCancellations attribute</span></span>

|<span data-ttu-id="89168-137">**Valor**</span><span class="sxs-lookup"><span data-stu-id="89168-137">**Value**</span></span>|<span data-ttu-id="89168-138">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="89168-138">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="89168-139">SendToNone</span><span class="sxs-lookup"><span data-stu-id="89168-139">SendToNone</span></span>  <br/> |<span data-ttu-id="89168-140">Um item de calendário é excluído sem enviar uma mensagem de cancelamento.</span><span class="sxs-lookup"><span data-stu-id="89168-140">A calendar item is deleted without sending a cancellation message.</span></span>  <br/> |
|<span data-ttu-id="89168-141">SendOnlyToAll</span><span class="sxs-lookup"><span data-stu-id="89168-141">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="89168-142">Um item de calendário é excluído e uma mensagem de cancelamento é enviada a todos os participantes.</span><span class="sxs-lookup"><span data-stu-id="89168-142">A calendar item is deleted and a cancellation message is sent to all attendees.</span></span>  <br/> |
|<span data-ttu-id="89168-143">SendToAllAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="89168-143">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="89168-144">Um item de calendário é excluído e uma mensagem de cancelamento é enviada a todos os participantes.</span><span class="sxs-lookup"><span data-stu-id="89168-144">A calendar item is deleted and a cancellation message is sent to all attendees.</span></span> <span data-ttu-id="89168-145">Uma cópia da mensagem de cancelamento é salva na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="89168-145">A copy of the cancellation message is saved in the Sent Items folder.</span></span>  <br/> |
   
#### <a name="affectedtaskoccurrences-attribute"></a><span data-ttu-id="89168-146">Atributo AffectedTaskOccurrences</span><span class="sxs-lookup"><span data-stu-id="89168-146">AffectedTaskOccurrences attribute</span></span>

|<span data-ttu-id="89168-147">**Valor**</span><span class="sxs-lookup"><span data-stu-id="89168-147">**Value**</span></span>|<span data-ttu-id="89168-148">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="89168-148">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="89168-149">Todas as ocorrências</span><span class="sxs-lookup"><span data-stu-id="89168-149">AllOccurrences</span></span>  <br/> |<span data-ttu-id="89168-150">Uma solicitação de exclusão de item exclui a tarefa mestre e, portanto, todas as tarefas recorrentes associadas à tarefa mestre.</span><span class="sxs-lookup"><span data-stu-id="89168-150">A delete item request deletes the master task, and therefore all recurring tasks that are associated with the master task.</span></span>  <br/> |
|<span data-ttu-id="89168-151">SpecifiedOccurrenceOnly</span><span class="sxs-lookup"><span data-stu-id="89168-151">SpecifiedOccurrenceOnly</span></span>  <br/> |<span data-ttu-id="89168-152">Uma solicitação de exclusão de item exclui apenas ocorrências específicas de uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="89168-152">A delete item request deletes only specific occurrences of a task.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="89168-153">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="89168-153">Child elements</span></span>

|<span data-ttu-id="89168-154">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="89168-154">**Element**</span></span>|<span data-ttu-id="89168-155">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="89168-155">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89168-156">ItemIds</span><span class="sxs-lookup"><span data-stu-id="89168-156">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="89168-157">Contém uma matriz de itens, itens de ocorrência e itens mestres recorrentes para excluir de uma caixa de correio no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="89168-157">Contains an array of items, occurrence items, and recurring master items to delete from a mailbox in the Exchange store.</span></span> <span data-ttu-id="89168-158">A [Operação DeleteItem](deleteitem-operation.md) pode ser executada em qualquer tipo de item.</span><span class="sxs-lookup"><span data-stu-id="89168-158">The [DeleteItem operation](deleteitem-operation.md) can be performed on any item type.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="89168-159">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="89168-159">Parent elements</span></span>

<span data-ttu-id="89168-160">Nenhum</span><span class="sxs-lookup"><span data-stu-id="89168-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="89168-161">Comentários</span><span class="sxs-lookup"><span data-stu-id="89168-161">Remarks</span></span>

<span data-ttu-id="89168-162">As opções **MoveToDeletedItems** e **HardDelete** são transacionais, o que significa que, quando uma chamada de serviço Web é concluída, o banco de dados moveu o item para a pasta itens excluídos ou removeu permanentemente o item do banco de dados do Exchange.</span><span class="sxs-lookup"><span data-stu-id="89168-162">The **MoveToDeletedItems** and **HardDelete** options are transactional, which means that by the time a Web service call completes, the database has moved the item to the Deleted Items folder or permanently removed the item from the Exchange database.</span></span> <span data-ttu-id="89168-163">Esse comportamento é o mesmo para o MicrosoftExchange Server 2007 e o Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="89168-163">This behavior is the same for MicrosoftExchange Server 2007 and Exchange Server 2010.</span></span> 
  
<span data-ttu-id="89168-164">A opção **SoftDelete** funciona de forma diferente para diferentes versões de destino do Exchange.</span><span class="sxs-lookup"><span data-stu-id="89168-164">The **SoftDelete** option works differently for different target versions of Exchange.</span></span> <span data-ttu-id="89168-165">**SoftDelete** para o Exchange 2007 define um bit no item que indica ao banco de dados do Exchange que o item será movido para a pasta dumpster em um momento indeterminado no futuro.</span><span class="sxs-lookup"><span data-stu-id="89168-165">**SoftDelete** for Exchange 2007 sets a bit on the item that indicates to the Exchange database that the item will be moved to the dumpster folder at an indeterminate time in the future.</span></span> <span data-ttu-id="89168-166">**SoftDelete** para Exchange 2010 move imediatamente o item para o dumpster.</span><span class="sxs-lookup"><span data-stu-id="89168-166">**SoftDelete** for Exchange 2010 immediately moves the item to the dumpster.</span></span> <span data-ttu-id="89168-167">**SoftDelete** não é uma opção para exclusão de pasta.</span><span class="sxs-lookup"><span data-stu-id="89168-167">**SoftDelete** is not an option for folder deletion.</span></span> <span data-ttu-id="89168-168">**SoftDelete** passagem pesquisa por itens e pastas não retornará nenhum resultado.</span><span class="sxs-lookup"><span data-stu-id="89168-168">**SoftDelete** traversal searches for items and folders will not return any results.</span></span> 
  
<span data-ttu-id="89168-169">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="89168-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89168-170">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="89168-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89168-171">Namespace</span><span class="sxs-lookup"><span data-stu-id="89168-171">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="89168-172">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="89168-172">Schema Name</span></span>  <br/> |<span data-ttu-id="89168-173">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="89168-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="89168-174">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="89168-174">Validation File</span></span>  <br/> |<span data-ttu-id="89168-175">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="89168-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="89168-176">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="89168-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="89168-177">False</span><span class="sxs-lookup"><span data-stu-id="89168-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="89168-178">Confira também</span><span class="sxs-lookup"><span data-stu-id="89168-178">See also</span></span>

- [<span data-ttu-id="89168-179">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="89168-179">DeleteItemResponse</span></span>](deleteitemresponse.md)  
- [<span data-ttu-id="89168-180">Operação DeleteItem</span><span class="sxs-lookup"><span data-stu-id="89168-180">DeleteItem operation</span></span>](deleteitem-operation.md)

