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
description: O elemento de DeleteItem define uma solicitação para excluir um item de uma caixa de correio no armazenamento do Exchange.
ms.openlocfilehash: de64787750c88c8a47bb69daddc0a1d2ebe8bde9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751758"
---
# <a name="deleteitem"></a><span data-ttu-id="e20d7-103">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="e20d7-103">DeleteItem</span></span>

<span data-ttu-id="e20d7-104">O elemento de **DeleteItem** define uma solicitação para excluir um item de uma caixa de correio no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e20d7-104">The **DeleteItem** element defines a request to delete an item from a mailbox in the Exchange store.</span></span> 
  
```XML
<DeleteItem DeleteType="" SendMeetingCancellations="" AffectedTaskOccurrences="" SuppressReadReceipts="">
   <ItemIds/>
</DeleteItem>
```

 <span data-ttu-id="e20d7-105">**DeleteItemType**</span><span class="sxs-lookup"><span data-stu-id="e20d7-105">**DeleteItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e20d7-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e20d7-106">Attributes and elements</span></span>

<span data-ttu-id="e20d7-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e20d7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e20d7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e20d7-108">Attributes</span></span>

|<span data-ttu-id="e20d7-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="e20d7-109">**Attribute**</span></span>|<span data-ttu-id="e20d7-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e20d7-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e20d7-111">**DeleteType**</span><span class="sxs-lookup"><span data-stu-id="e20d7-111">**DeleteType**</span></span> <br/> |<span data-ttu-id="e20d7-112">Descreve como um item é excluído.</span><span class="sxs-lookup"><span data-stu-id="e20d7-112">Describes how an item is deleted.</span></span> <span data-ttu-id="e20d7-113">Este atributo é necessário.</span><span class="sxs-lookup"><span data-stu-id="e20d7-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="e20d7-114">**SendMeetingCancellations**</span><span class="sxs-lookup"><span data-stu-id="e20d7-114">**SendMeetingCancellations**</span></span> <br/> |<span data-ttu-id="e20d7-115">Descreve se uma exclusão de item de calendário é comunicada aos participantes.</span><span class="sxs-lookup"><span data-stu-id="e20d7-115">Describes whether a calendar item deletion is communicated to attendees.</span></span> <span data-ttu-id="e20d7-116">Este atributo é necessário quando itens de calendário são excluídas.</span><span class="sxs-lookup"><span data-stu-id="e20d7-116">This attribute is required when calendar items are deleted.</span></span> <span data-ttu-id="e20d7-117">Este atributo é opcional se os itens de calendário não são excluídos.</span><span class="sxs-lookup"><span data-stu-id="e20d7-117">This attribute is optional if non-calendar items are deleted.</span></span>  <br/> |
|<span data-ttu-id="e20d7-118">**AffectedTaskOccurrences**</span><span class="sxs-lookup"><span data-stu-id="e20d7-118">**AffectedTaskOccurrences**</span></span> <br/> |<span data-ttu-id="e20d7-119">Descreve se uma instância de tarefa ou um mestre de tarefa é excluído por uma [operação DeleteItem](deleteitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="e20d7-119">Describes whether a task instance or a task master is deleted by a [DeleteItem operation](deleteitem-operation.md).</span></span> <span data-ttu-id="e20d7-120">Este atributo é necessário quando as tarefas são excluídas.</span><span class="sxs-lookup"><span data-stu-id="e20d7-120">This attribute is required when tasks are deleted.</span></span> <span data-ttu-id="e20d7-121">Este atributo é opcional quando os itens de tarefa não são excluídos.</span><span class="sxs-lookup"><span data-stu-id="e20d7-121">This attribute is optional when non-task items are deleted.</span></span>  <br/> |
|<span data-ttu-id="e20d7-122">**SuppressReadReceipts**</span><span class="sxs-lookup"><span data-stu-id="e20d7-122">**SuppressReadReceipts**</span></span> <br/> |<span data-ttu-id="e20d7-123">Indica se as confirmações de leitura para o item excluído são suprimidas.</span><span class="sxs-lookup"><span data-stu-id="e20d7-123">Indicates whether read receipts for the deleted item are suppressed.</span></span> <span data-ttu-id="e20d7-124">Um valor de texto de **true**, indica que as confirmações de leitura estão suprimidas.</span><span class="sxs-lookup"><span data-stu-id="e20d7-124">A text value of **true**, indicates that the read receipts are suppressed.</span></span> <span data-ttu-id="e20d7-125">Um valor **false** indica que as confirmações de leitura são enviadas para o remetente.</span><span class="sxs-lookup"><span data-stu-id="e20d7-125">A value of **false** indicates that the read receipts are sent to the sender.</span></span> <span data-ttu-id="e20d7-126">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="e20d7-126">This attribute is optional.</span></span>  <br/> |
   
#### <a name="deletetype-attribute"></a><span data-ttu-id="e20d7-127">Atributo DeleteType</span><span class="sxs-lookup"><span data-stu-id="e20d7-127">DeleteType attribute</span></span>

|<span data-ttu-id="e20d7-128">**Valor**</span><span class="sxs-lookup"><span data-stu-id="e20d7-128">**Value**</span></span>|<span data-ttu-id="e20d7-129">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e20d7-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e20d7-130">HardDelete</span><span class="sxs-lookup"><span data-stu-id="e20d7-130">HardDelete</span></span>  <br/> |<span data-ttu-id="e20d7-131">Um item é removido permanentemente do repositório.</span><span class="sxs-lookup"><span data-stu-id="e20d7-131">An item is permanently removed from the store.</span></span>  <br/> |
|<span data-ttu-id="e20d7-132">SoftDelete</span><span class="sxs-lookup"><span data-stu-id="e20d7-132">SoftDelete</span></span>  <br/> |<span data-ttu-id="e20d7-133">Um item é movido para o dumpster se o dumpster está habilitado.</span><span class="sxs-lookup"><span data-stu-id="e20d7-133">An item is moved to the dumpster if the dumpster is enabled.</span></span>  <br/> |
|<span data-ttu-id="e20d7-134">MoveToDeletedItems</span><span class="sxs-lookup"><span data-stu-id="e20d7-134">MoveToDeletedItems</span></span>  <br/> |<span data-ttu-id="e20d7-135">Um item é movido para a pasta Itens excluídos.</span><span class="sxs-lookup"><span data-stu-id="e20d7-135">An item is moved to the Deleted Items folder.</span></span>  <br/> |
   
#### <a name="sendmeetingcancellations-attribute"></a><span data-ttu-id="e20d7-136">Atributo SendMeetingCancellations</span><span class="sxs-lookup"><span data-stu-id="e20d7-136">SendMeetingCancellations attribute</span></span>

|<span data-ttu-id="e20d7-137">**Valor**</span><span class="sxs-lookup"><span data-stu-id="e20d7-137">**Value**</span></span>|<span data-ttu-id="e20d7-138">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e20d7-138">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e20d7-139">SendToNone</span><span class="sxs-lookup"><span data-stu-id="e20d7-139">SendToNone</span></span>  <br/> |<span data-ttu-id="e20d7-140">Um item de calendário será excluído sem enviar uma mensagem de cancelamento.</span><span class="sxs-lookup"><span data-stu-id="e20d7-140">A calendar item is deleted without sending a cancellation message.</span></span>  <br/> |
|<span data-ttu-id="e20d7-141">SendOnlyToAll</span><span class="sxs-lookup"><span data-stu-id="e20d7-141">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="e20d7-142">Um item de calendário é excluído e uma mensagem de cancelamento é enviada a todos os participantes.</span><span class="sxs-lookup"><span data-stu-id="e20d7-142">A calendar item is deleted and a cancellation message is sent to all attendees.</span></span>  <br/> |
|<span data-ttu-id="e20d7-143">SendToAllAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="e20d7-143">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="e20d7-144">Um item de calendário é excluído e uma mensagem de cancelamento é enviada a todos os participantes.</span><span class="sxs-lookup"><span data-stu-id="e20d7-144">A calendar item is deleted and a cancellation message is sent to all attendees.</span></span> <span data-ttu-id="e20d7-145">Uma cópia da mensagem de cancelamento é salva na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="e20d7-145">A copy of the cancellation message is saved in the Sent Items folder.</span></span>  <br/> |
   
#### <a name="affectedtaskoccurrences-attribute"></a><span data-ttu-id="e20d7-146">Atributo AffectedTaskOccurrences</span><span class="sxs-lookup"><span data-stu-id="e20d7-146">AffectedTaskOccurrences attribute</span></span>

|<span data-ttu-id="e20d7-147">**Valor**</span><span class="sxs-lookup"><span data-stu-id="e20d7-147">**Value**</span></span>|<span data-ttu-id="e20d7-148">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e20d7-148">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e20d7-149">AllOccurrences</span><span class="sxs-lookup"><span data-stu-id="e20d7-149">AllOccurrences</span></span>  <br/> |<span data-ttu-id="e20d7-150">Uma solicitação de item delete Exclui a tarefa mestre e, portanto, todas as tarefas recorrentes que estão associados a tarefa mestre.</span><span class="sxs-lookup"><span data-stu-id="e20d7-150">A delete item request deletes the master task, and therefore all recurring tasks that are associated with the master task.</span></span>  <br/> |
|<span data-ttu-id="e20d7-151">SpecifiedOccurrenceOnly</span><span class="sxs-lookup"><span data-stu-id="e20d7-151">SpecifiedOccurrenceOnly</span></span>  <br/> |<span data-ttu-id="e20d7-152">Uma solicitação de item delete Exclui apenas as ocorrências específicas de uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="e20d7-152">A delete item request deletes only specific occurrences of a task.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e20d7-153">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e20d7-153">Child elements</span></span>

|<span data-ttu-id="e20d7-154">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="e20d7-154">**Element**</span></span>|<span data-ttu-id="e20d7-155">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="e20d7-155">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e20d7-156">ItemIds</span><span class="sxs-lookup"><span data-stu-id="e20d7-156">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="e20d7-157">Contém uma matriz de itens, itens de ocorrência e itens recorrentes de mestres para excluir de uma caixa de correio no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e20d7-157">Contains an array of items, occurrence items, and recurring master items to delete from a mailbox in the Exchange store.</span></span> <span data-ttu-id="e20d7-158">A [operação DeleteItem](deleteitem-operation.md) pode ser executado em qualquer tipo de item.</span><span class="sxs-lookup"><span data-stu-id="e20d7-158">The [DeleteItem operation](deleteitem-operation.md) can be performed on any item type.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e20d7-159">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e20d7-159">Parent elements</span></span>

<span data-ttu-id="e20d7-160">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e20d7-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e20d7-161">Comentários</span><span class="sxs-lookup"><span data-stu-id="e20d7-161">Remarks</span></span>

<span data-ttu-id="e20d7-162">As opções **MoveToDeletedItems** e **HardDelete** são transacionais, o que significa que no momento em uma chamada de serviço da Web for concluído, o banco de dados tiver movido o item para a pasta Itens excluídos ou removido permanentemente o item do banco de dados do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e20d7-162">The **MoveToDeletedItems** and **HardDelete** options are transactional, which means that by the time a Web service call completes, the database has moved the item to the Deleted Items folder or permanently removed the item from the Exchange database.</span></span> <span data-ttu-id="e20d7-163">Esse comportamento é o mesmo para MicrosoftExchange Server 2007 e o Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="e20d7-163">This behavior is the same for MicrosoftExchange Server 2007 and Exchange Server 2010.</span></span> 
  
<span data-ttu-id="e20d7-164">A opção **SoftDelete** funciona de modo diferente para versões diferentes de destino do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e20d7-164">The **SoftDelete** option works differently for different target versions of Exchange.</span></span> <span data-ttu-id="e20d7-165">**SoftDelete** para o Exchange 2007 define um pouco no item que indica no banco de dados do Exchange que o item será movido para o dumpster pasta em um tempo indeterminado no futuro.</span><span class="sxs-lookup"><span data-stu-id="e20d7-165">**SoftDelete** for Exchange 2007 sets a bit on the item that indicates to the Exchange database that the item will be moved to the dumpster folder at an indeterminate time in the future.</span></span> <span data-ttu-id="e20d7-166">**SoftDelete** para o Exchange 2010 imediatamente move o item para o dumpster.</span><span class="sxs-lookup"><span data-stu-id="e20d7-166">**SoftDelete** for Exchange 2010 immediately moves the item to the dumpster.</span></span> <span data-ttu-id="e20d7-167">**SoftDelete** não é uma opção para exclusão da pasta.</span><span class="sxs-lookup"><span data-stu-id="e20d7-167">**SoftDelete** is not an option for folder deletion.</span></span> <span data-ttu-id="e20d7-168">Pesquisas de passagem **SoftDelete** para itens e pastas não retornará nenhum resultado.</span><span class="sxs-lookup"><span data-stu-id="e20d7-168">**SoftDelete** traversal searches for items and folders will not return any results.</span></span> 
  
<span data-ttu-id="e20d7-169">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e20d7-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e20d7-170">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e20d7-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e20d7-171">Namespace</span><span class="sxs-lookup"><span data-stu-id="e20d7-171">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e20d7-172">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e20d7-172">Schema Name</span></span>  <br/> |<span data-ttu-id="e20d7-173">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e20d7-173">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e20d7-174">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e20d7-174">Validation File</span></span>  <br/> |<span data-ttu-id="e20d7-175">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e20d7-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e20d7-176">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e20d7-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="e20d7-177">False</span><span class="sxs-lookup"><span data-stu-id="e20d7-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e20d7-178">Ver também</span><span class="sxs-lookup"><span data-stu-id="e20d7-178">See also</span></span>

- [<span data-ttu-id="e20d7-179">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="e20d7-179">DeleteItemResponse</span></span>](deleteitemresponse.md)  
- [<span data-ttu-id="e20d7-180">Operação DeleteItem</span><span class="sxs-lookup"><span data-stu-id="e20d7-180">DeleteItem operation</span></span>](deleteitem-operation.md)

