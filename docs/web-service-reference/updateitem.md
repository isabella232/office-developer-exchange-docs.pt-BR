---
title: UpdateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 34643d58-2743-45b0-a08d-bff6dc1da61d
description: O elemento de UpdateItem define uma solicitação de atualização de um item em uma caixa de correio.
ms.openlocfilehash: 7b9b5f1dcffb95eb127572cb91f92d961c05a77e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/21/2018
ms.locfileid: "19837917"
---
# <a name="updateitem"></a><span data-ttu-id="a392b-103">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="a392b-103">UpdateItem</span></span>

<span data-ttu-id="a392b-104">O elemento de **UpdateItem** define uma solicitação de atualização de um item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="a392b-104">The **UpdateItem** element defines a request to update an item in a mailbox.</span></span> 
  
```XML
<UpdateItem ConflictResolution="" MessageDisposition="" SendMeetingInvitationsOrCancellations="" SuppressReadReceipts="">
   <SavedItemFolderId/>
   <ItemChanges/>
</UpdateItem>
```

 <span data-ttu-id="a392b-105">**UpdateItemType**</span><span class="sxs-lookup"><span data-stu-id="a392b-105">**UpdateItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a392b-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="a392b-106">Attributes and elements</span></span>

<span data-ttu-id="a392b-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="a392b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a392b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="a392b-108">Attributes</span></span>

|<span data-ttu-id="a392b-109">**Attribute**</span><span class="sxs-lookup"><span data-stu-id="a392b-109">**Attribute**</span></span>|<span data-ttu-id="a392b-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a392b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a392b-111">**ConflictResolution**</span><span class="sxs-lookup"><span data-stu-id="a392b-111">**ConflictResolution**</span></span> <br/> |<span data-ttu-id="a392b-112">Identifica o tipo de resolução de conflito para tentar durante uma atualização.</span><span class="sxs-lookup"><span data-stu-id="a392b-112">Identifies the type of conflict resolution to try during an update.</span></span> <span data-ttu-id="a392b-113">O valor padrão é resolver automaticamente.</span><span class="sxs-lookup"><span data-stu-id="a392b-113">The default value is AutoResolve.</span></span>  <br/> |
|<span data-ttu-id="a392b-114">**MessageDisposition**</span><span class="sxs-lookup"><span data-stu-id="a392b-114">**MessageDisposition**</span></span> <br/> |<span data-ttu-id="a392b-115">Descreve como o item será tratado após ele ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="a392b-115">Describes how the item will be handled after it is updated.</span></span> <span data-ttu-id="a392b-116">O atributo **MessageDisposition** é necessário para itens de mensagem, incluindo mensagens de reunião como cancelamentos de reunião, solicitações de reunião e respostas de reunião.</span><span class="sxs-lookup"><span data-stu-id="a392b-116">The **MessageDisposition** attribute is required for message items, including meeting messages such as meeting cancellations, meeting requests, and meeting responses.</span></span>  <br/> |
|<span data-ttu-id="a392b-117">**SendMeetingCancellations**</span><span class="sxs-lookup"><span data-stu-id="a392b-117">**SendMeetingInvitationsOrCancellations**</span></span> <br/> |<span data-ttu-id="a392b-118">Descreve como as atualizações de reunião são comunicadas depois que um item de calendário for atualizado.</span><span class="sxs-lookup"><span data-stu-id="a392b-118">Describes how meeting updates are communicated after a calendar item is updated.</span></span> <span data-ttu-id="a392b-119">Este atributo é necessário para itens de calendário e ocorrências de item de calendário.</span><span class="sxs-lookup"><span data-stu-id="a392b-119">This attribute is required for calendar items and calendar item occurrences.</span></span>  <br/> |
|<span data-ttu-id="a392b-120">**SuppressReadReceipts**</span><span class="sxs-lookup"><span data-stu-id="a392b-120">**SuppressReadReceipts**</span></span> <br/> |<span data-ttu-id="a392b-121">Indica se as confirmações de leitura para o item atualizado devem ser suprimidas.</span><span class="sxs-lookup"><span data-stu-id="a392b-121">Indicates whether read receipts for the updated item should be suppressed.</span></span> <span data-ttu-id="a392b-122">Um valor de texto de **true** indica que devem ser suprimidas confirmações de leitura.</span><span class="sxs-lookup"><span data-stu-id="a392b-122">A text value of **true** indicates that read receipts should be suppressed.</span></span> <span data-ttu-id="a392b-123">Um valor **false** indica que as confirmações de leitura serão enviadas ao remetente.</span><span class="sxs-lookup"><span data-stu-id="a392b-123">A value of **false** indicates that the read receipts will be sent to the sender.</span></span> <span data-ttu-id="a392b-124">Este atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="a392b-124">This attribute is optional.</span></span>  <br/> <span data-ttu-id="a392b-125">Este atributo foi introduzido no Exchange Server 2013 SP1.</span><span class="sxs-lookup"><span data-stu-id="a392b-125">This attribute was introduced in Exchange Server 2013 SP1.</span></span>  <br/> |
   
#### <a name="conflictresolution-attribute"></a><span data-ttu-id="a392b-126">Atributo ConflictResolution</span><span class="sxs-lookup"><span data-stu-id="a392b-126">ConflictResolution Attribute</span></span>

|<span data-ttu-id="a392b-127">**Valor**</span><span class="sxs-lookup"><span data-stu-id="a392b-127">**Value**</span></span>|<span data-ttu-id="a392b-128">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a392b-128">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a392b-129">NeverOverwrite</span><span class="sxs-lookup"><span data-stu-id="a392b-129">NeverOverwrite</span></span>  <br/> |<span data-ttu-id="a392b-130">Se houver um conflito, a operação de atualização falhará e um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="a392b-130">If there is a conflict, the update operation fails and an error is returned.</span></span>  <br/> |
|<span data-ttu-id="a392b-131">Resolver automaticamente</span><span class="sxs-lookup"><span data-stu-id="a392b-131">AutoResolve</span></span>  <br/> |<span data-ttu-id="a392b-132">A operação de atualização resolve automaticamente qualquer conflito.</span><span class="sxs-lookup"><span data-stu-id="a392b-132">The update operation automatically resolves any conflict.</span></span>  <br/> |
|<span data-ttu-id="a392b-133">AlwaysOverwrite</span><span class="sxs-lookup"><span data-stu-id="a392b-133">AlwaysOverwrite</span></span>  <br/> |<span data-ttu-id="a392b-134">Se houver um conflito, a operação de atualização substituirá informações.</span><span class="sxs-lookup"><span data-stu-id="a392b-134">If there is a conflict, the update operation will overwrite information.</span></span>  <br/> |
   
#### <a name="messagedisposition-attribute"></a><span data-ttu-id="a392b-135">Atributo MessageDisposition</span><span class="sxs-lookup"><span data-stu-id="a392b-135">MessageDisposition Attribute</span></span>

|<span data-ttu-id="a392b-136">**Valor**</span><span class="sxs-lookup"><span data-stu-id="a392b-136">**Value**</span></span>|<span data-ttu-id="a392b-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a392b-137">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a392b-138">SaveOnly</span><span class="sxs-lookup"><span data-stu-id="a392b-138">SaveOnly</span></span>  <br/> |<span data-ttu-id="a392b-139">O item está atualizado e salvos de volta a sua pasta atual.</span><span class="sxs-lookup"><span data-stu-id="a392b-139">The item is updated and saved back to its current folder.</span></span>  <br/> |
|<span data-ttu-id="a392b-140">SendOnly</span><span class="sxs-lookup"><span data-stu-id="a392b-140">SendOnly</span></span>  <br/> |<span data-ttu-id="a392b-141">O item é atualizado e enviado, mas nenhuma cópia é salva.</span><span class="sxs-lookup"><span data-stu-id="a392b-141">The item is updated and sent but no copy is saved.</span></span>  <br/> |
|<span data-ttu-id="a392b-142">SendAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="a392b-142">SendAndSaveCopy</span></span>  <br/> |<span data-ttu-id="a392b-143">O item é atualizado e uma cópia é salva na pasta identificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="a392b-143">The item is updated and a copy is saved in the folder identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
#### <a name="sendmeetinginvitationsorcancellations-attribute"></a><span data-ttu-id="a392b-144">Atributo SendMeetingCancellations</span><span class="sxs-lookup"><span data-stu-id="a392b-144">SendMeetingInvitationsOrCancellations Attribute</span></span>

|<span data-ttu-id="a392b-145">**Valor**</span><span class="sxs-lookup"><span data-stu-id="a392b-145">**Value**</span></span>|<span data-ttu-id="a392b-146">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a392b-146">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a392b-147">SendToNone</span><span class="sxs-lookup"><span data-stu-id="a392b-147">SendToNone</span></span>  <br/> |<span data-ttu-id="a392b-148">O item de calendário é atualizado mas atualizações não são enviadas aos participantes.</span><span class="sxs-lookup"><span data-stu-id="a392b-148">The calendar item is updated but updates are not sent to attendees.</span></span>  <br/> |
|<span data-ttu-id="a392b-149">SendOnlyToAll</span><span class="sxs-lookup"><span data-stu-id="a392b-149">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="a392b-150">O item de calendário é atualizado e a atualização de reunião é enviada a todos os participantes, mas não é salvo na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="a392b-150">The calendar item is updated and the meeting update is sent to all attendees but is not saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="a392b-151">SendOnlyToChanged</span><span class="sxs-lookup"><span data-stu-id="a392b-151">SendOnlyToChanged</span></span>  <br/> |<span data-ttu-id="a392b-152">O item de calendário é atualizado e a atualização de reunião é enviada apenas aos participantes que são afetados pela alteração na reunião.</span><span class="sxs-lookup"><span data-stu-id="a392b-152">The calendar item is updated and the meeting update is sent only to attendees that are affected by the change in the meeting.</span></span>  <br/> |
|<span data-ttu-id="a392b-153">SendToAllAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="a392b-153">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="a392b-154">O item de calendário é atualizado, a atualização de reunião é enviada a todos os participantes e uma cópia é salva na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="a392b-154">The calendar item is updated, the meeting update is sent to all attendees, and a copy is saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="a392b-155">SendToChangedAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="a392b-155">SendToChangedAndSaveCopy</span></span>  <br/> |<span data-ttu-id="a392b-156">O item de calendário é atualizado, a atualização de reunião é enviada a todos os participantes que são afetados pela alteração na reunião e uma cópia é salva na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="a392b-156">The calendar item is updated, the meeting update is sent to all attendees that are affected by the change in the meeting, and a copy is saved in the Sent Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a392b-157">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="a392b-157">Child elements</span></span>

|<span data-ttu-id="a392b-158">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a392b-158">**Element**</span></span>|<span data-ttu-id="a392b-159">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a392b-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a392b-160">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="a392b-160">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> |<span data-ttu-id="a392b-161">Identifica a pasta de destino para operações de atualização, enviar e crie itens no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a392b-161">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="a392b-162">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="a392b-162">ItemChanges</span></span>](itemchanges.md) <br/> |<span data-ttu-id="a392b-163">Contém uma matriz de elementos [ItemChange](itemchange.md) que identificam os itens e as atualizações para aplicar aos itens.</span><span class="sxs-lookup"><span data-stu-id="a392b-163">Contains an array of [ItemChange](itemchange.md) elements that identify items and the updates to apply to the items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a392b-164">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="a392b-164">Parent elements</span></span>

<span data-ttu-id="a392b-165">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a392b-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a392b-166">Comentários</span><span class="sxs-lookup"><span data-stu-id="a392b-166">Remarks</span></span>

<span data-ttu-id="a392b-167">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="a392b-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a392b-168">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="a392b-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a392b-169">Namespace</span><span class="sxs-lookup"><span data-stu-id="a392b-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a392b-170">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="a392b-170">Schema Name</span></span>  <br/> |<span data-ttu-id="a392b-171">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="a392b-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a392b-172">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="a392b-172">Validation File</span></span>  <br/> |<span data-ttu-id="a392b-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a392b-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a392b-174">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="a392b-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="a392b-175">False</span><span class="sxs-lookup"><span data-stu-id="a392b-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a392b-176">Ver também</span><span class="sxs-lookup"><span data-stu-id="a392b-176">See also</span></span>



[<span data-ttu-id="a392b-177">Operação UpdateItem</span><span class="sxs-lookup"><span data-stu-id="a392b-177">UpdateItem operation</span></span>](updateitem-operation.md)

