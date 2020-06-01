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
description: O elemento UpdateItem define uma solicitação para atualizar um item em uma caixa de correio.
ms.openlocfilehash: 43821db58457ffce22be918a7ba6427f57230010
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466567"
---
# <a name="updateitem"></a><span data-ttu-id="42708-103">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="42708-103">UpdateItem</span></span>

<span data-ttu-id="42708-104">O elemento **UpdateItem** define uma solicitação para atualizar um item em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="42708-104">The **UpdateItem** element defines a request to update an item in a mailbox.</span></span> 
  
```XML
<UpdateItem ConflictResolution="" MessageDisposition="" SendMeetingInvitationsOrCancellations="" SuppressReadReceipts="">
   <SavedItemFolderId/>
   <ItemChanges/>
</UpdateItem>
```

 <span data-ttu-id="42708-105">**UpdateItemType**</span><span class="sxs-lookup"><span data-stu-id="42708-105">**UpdateItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="42708-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="42708-106">Attributes and elements</span></span>

<span data-ttu-id="42708-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="42708-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="42708-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="42708-108">Attributes</span></span>

|<span data-ttu-id="42708-109">**Atributo**</span><span class="sxs-lookup"><span data-stu-id="42708-109">**Attribute**</span></span>|<span data-ttu-id="42708-110">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="42708-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="42708-111">**ConflictResolution**</span><span class="sxs-lookup"><span data-stu-id="42708-111">**ConflictResolution**</span></span> <br/> |<span data-ttu-id="42708-112">Identifica o tipo de resolução de conflitos a ser tentada durante uma atualização.</span><span class="sxs-lookup"><span data-stu-id="42708-112">Identifies the type of conflict resolution to try during an update.</span></span> <span data-ttu-id="42708-113">O valor padrão é autoresolver.</span><span class="sxs-lookup"><span data-stu-id="42708-113">The default value is AutoResolve.</span></span>  <br/> |
|<span data-ttu-id="42708-114">**MessageDisposition**</span><span class="sxs-lookup"><span data-stu-id="42708-114">**MessageDisposition**</span></span> <br/> |<span data-ttu-id="42708-115">Descreve como o item será manipulado após a atualização.</span><span class="sxs-lookup"><span data-stu-id="42708-115">Describes how the item will be handled after it is updated.</span></span> <span data-ttu-id="42708-116">O atributo **MessageDisposition** é necessário para itens de mensagem, incluindo mensagens de reunião, como cancelamentos de reunião, solicitações de reunião e respostas de reunião.</span><span class="sxs-lookup"><span data-stu-id="42708-116">The **MessageDisposition** attribute is required for message items, including meeting messages such as meeting cancellations, meeting requests, and meeting responses.</span></span>  <br/> |
|<span data-ttu-id="42708-117">**SendMeetingInvitationsOrCancellations**</span><span class="sxs-lookup"><span data-stu-id="42708-117">**SendMeetingInvitationsOrCancellations**</span></span> <br/> |<span data-ttu-id="42708-118">Descreve como as atualizações de reunião são comunicadas após a atualização de um item de calendário.</span><span class="sxs-lookup"><span data-stu-id="42708-118">Describes how meeting updates are communicated after a calendar item is updated.</span></span> <span data-ttu-id="42708-119">Esse atributo é necessário para itens de calendário e ocorrências de itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="42708-119">This attribute is required for calendar items and calendar item occurrences.</span></span>  <br/> |
|<span data-ttu-id="42708-120">**SuppressReadReceipts**</span><span class="sxs-lookup"><span data-stu-id="42708-120">**SuppressReadReceipts**</span></span> <br/> |<span data-ttu-id="42708-121">Indica se as confirmações de leitura para o item atualizado devem ser suprimidas.</span><span class="sxs-lookup"><span data-stu-id="42708-121">Indicates whether read receipts for the updated item should be suppressed.</span></span> <span data-ttu-id="42708-122">Um valor de texto **true** indica que as confirmações de leitura devem ser suprimidas.</span><span class="sxs-lookup"><span data-stu-id="42708-122">A text value of **true** indicates that read receipts should be suppressed.</span></span> <span data-ttu-id="42708-123">Um valor **false** indica que as confirmações de leitura serão enviadas ao remetente.</span><span class="sxs-lookup"><span data-stu-id="42708-123">A value of **false** indicates that the read receipts will be sent to the sender.</span></span> <span data-ttu-id="42708-124">Esse atributo é opcional.</span><span class="sxs-lookup"><span data-stu-id="42708-124">This attribute is optional.</span></span>  <br/> <span data-ttu-id="42708-125">Este atributo foi introduzido no Exchange Server 2013 SP1.</span><span class="sxs-lookup"><span data-stu-id="42708-125">This attribute was introduced in Exchange Server 2013 SP1.</span></span>  <br/> |
   
#### <a name="conflictresolution-attribute"></a><span data-ttu-id="42708-126">Atributo ConflictResolution</span><span class="sxs-lookup"><span data-stu-id="42708-126">ConflictResolution Attribute</span></span>

|<span data-ttu-id="42708-127">**Valor**</span><span class="sxs-lookup"><span data-stu-id="42708-127">**Value**</span></span>|<span data-ttu-id="42708-128">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="42708-128">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="42708-129">NeverOverwrite</span><span class="sxs-lookup"><span data-stu-id="42708-129">NeverOverwrite</span></span>  <br/> |<span data-ttu-id="42708-130">Se houver um conflito, a operação de atualização falhará e um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="42708-130">If there is a conflict, the update operation fails and an error is returned.</span></span>  <br/> |
|<span data-ttu-id="42708-131">Resolver automaticamente</span><span class="sxs-lookup"><span data-stu-id="42708-131">AutoResolve</span></span>  <br/> |<span data-ttu-id="42708-132">A operação de atualização resolve qualquer conflito automaticamente.</span><span class="sxs-lookup"><span data-stu-id="42708-132">The update operation automatically resolves any conflict.</span></span>  <br/> |
|<span data-ttu-id="42708-133">AlwaysOverwrite</span><span class="sxs-lookup"><span data-stu-id="42708-133">AlwaysOverwrite</span></span>  <br/> |<span data-ttu-id="42708-134">Se houver um conflito, a operação de atualização substituirá as informações.</span><span class="sxs-lookup"><span data-stu-id="42708-134">If there is a conflict, the update operation will overwrite information.</span></span>  <br/> |
   
#### <a name="messagedisposition-attribute"></a><span data-ttu-id="42708-135">Atributo MessageDisposition</span><span class="sxs-lookup"><span data-stu-id="42708-135">MessageDisposition Attribute</span></span>

|<span data-ttu-id="42708-136">**Valor**</span><span class="sxs-lookup"><span data-stu-id="42708-136">**Value**</span></span>|<span data-ttu-id="42708-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="42708-137">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="42708-138">SaveOnly</span><span class="sxs-lookup"><span data-stu-id="42708-138">SaveOnly</span></span>  <br/> |<span data-ttu-id="42708-139">O item é atualizado e salvo novamente na pasta atual.</span><span class="sxs-lookup"><span data-stu-id="42708-139">The item is updated and saved back to its current folder.</span></span>  <br/> |
|<span data-ttu-id="42708-140">SendOnly</span><span class="sxs-lookup"><span data-stu-id="42708-140">SendOnly</span></span>  <br/> |<span data-ttu-id="42708-141">O item é atualizado e enviado, mas nenhuma cópia é salva.</span><span class="sxs-lookup"><span data-stu-id="42708-141">The item is updated and sent but no copy is saved.</span></span>  <br/> |
|<span data-ttu-id="42708-142">SendAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="42708-142">SendAndSaveCopy</span></span>  <br/> |<span data-ttu-id="42708-143">O item é atualizado e uma cópia é salva na pasta identificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="42708-143">The item is updated and a copy is saved in the folder identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
#### <a name="sendmeetinginvitationsorcancellations-attribute"></a><span data-ttu-id="42708-144">Atributo SendMeetingInvitationsOrCancellations</span><span class="sxs-lookup"><span data-stu-id="42708-144">SendMeetingInvitationsOrCancellations Attribute</span></span>

|<span data-ttu-id="42708-145">**Valor**</span><span class="sxs-lookup"><span data-stu-id="42708-145">**Value**</span></span>|<span data-ttu-id="42708-146">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="42708-146">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="42708-147">SendToNone</span><span class="sxs-lookup"><span data-stu-id="42708-147">SendToNone</span></span>  <br/> |<span data-ttu-id="42708-148">O item de calendário é atualizado, mas as atualizações não são enviadas aos participantes.</span><span class="sxs-lookup"><span data-stu-id="42708-148">The calendar item is updated but updates are not sent to attendees.</span></span>  <br/> |
|<span data-ttu-id="42708-149">SendOnlyToAll</span><span class="sxs-lookup"><span data-stu-id="42708-149">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="42708-150">O item de calendário é atualizado e a atualização da reunião é enviada a todos os participantes, mas não é salvo na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="42708-150">The calendar item is updated and the meeting update is sent to all attendees but is not saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="42708-151">SendOnlyToChanged</span><span class="sxs-lookup"><span data-stu-id="42708-151">SendOnlyToChanged</span></span>  <br/> |<span data-ttu-id="42708-152">O item de calendário é atualizado e a atualização da reunião é enviada somente para os participantes afetados pela alteração na reunião.</span><span class="sxs-lookup"><span data-stu-id="42708-152">The calendar item is updated and the meeting update is sent only to attendees that are affected by the change in the meeting.</span></span>  <br/> |
|<span data-ttu-id="42708-153">SendToAllAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="42708-153">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="42708-154">O item de calendário é atualizado, a atualização da reunião é enviada a todos os participantes e uma cópia é salva na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="42708-154">The calendar item is updated, the meeting update is sent to all attendees, and a copy is saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="42708-155">SendToChangedAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="42708-155">SendToChangedAndSaveCopy</span></span>  <br/> |<span data-ttu-id="42708-156">O item de calendário é atualizado, a atualização da reunião é enviada a todos os participantes afetados pela alteração na reunião, e uma cópia é salva na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="42708-156">The calendar item is updated, the meeting update is sent to all attendees that are affected by the change in the meeting, and a copy is saved in the Sent Items folder.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="42708-157">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="42708-157">Child elements</span></span>

|<span data-ttu-id="42708-158">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="42708-158">**Element**</span></span>|<span data-ttu-id="42708-159">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="42708-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="42708-160">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="42708-160">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> |<span data-ttu-id="42708-161">Identifica a pasta de destino para operações que atualizam, enviam e criam itens no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="42708-161">Identifies the target folder for operations that update, send, and create items in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="42708-162">Alterações</span><span class="sxs-lookup"><span data-stu-id="42708-162">ItemChanges</span></span>](itemchanges.md) <br/> |<span data-ttu-id="42708-163">Contém uma matriz de elementos [ItemChange](itemchange.md) que identificam itens e as atualizações a serem aplicadas aos itens.</span><span class="sxs-lookup"><span data-stu-id="42708-163">Contains an array of [ItemChange](itemchange.md) elements that identify items and the updates to apply to the items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="42708-164">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="42708-164">Parent elements</span></span>

<span data-ttu-id="42708-165">Nenhum</span><span class="sxs-lookup"><span data-stu-id="42708-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="42708-166">Comentários</span><span class="sxs-lookup"><span data-stu-id="42708-166">Remarks</span></span>

<span data-ttu-id="42708-167">O esquema que descreve este elemento está localizado no diretório virtual do IIS que hospeda os Serviços Web do Exchange.</span><span class="sxs-lookup"><span data-stu-id="42708-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="42708-168">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="42708-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="42708-169">Namespace</span><span class="sxs-lookup"><span data-stu-id="42708-169">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="42708-170">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="42708-170">Schema Name</span></span>  <br/> |<span data-ttu-id="42708-171">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="42708-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="42708-172">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="42708-172">Validation File</span></span>  <br/> |<span data-ttu-id="42708-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="42708-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="42708-174">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="42708-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="42708-175">False</span><span class="sxs-lookup"><span data-stu-id="42708-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="42708-176">Confira também</span><span class="sxs-lookup"><span data-stu-id="42708-176">See also</span></span>



[<span data-ttu-id="42708-177">Operação UpdateItem</span><span class="sxs-lookup"><span data-stu-id="42708-177">UpdateItem operation</span></span>](updateitem-operation.md)

