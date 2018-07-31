---
title: CreateItem
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
ms.assetid: c3707feb-3fd4-4b8a-a68f-2abadd455163
description: O elemento de CreateItem define uma solicitação para criar um item no armazenamento do Exchange.
ms.openlocfilehash: 9453323bff07749f5852dae75284c61c0895adb6
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353123"
---
# <a name="createitem"></a><span data-ttu-id="e4962-103">CreateItem</span><span class="sxs-lookup"><span data-stu-id="e4962-103">CreateItem</span></span>

<span data-ttu-id="e4962-104">O elemento de **CreateItem** define uma solicitação para criar um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e4962-104">The **CreateItem** element defines a request to create an item in the Exchange store.</span></span> 
  
```xml
<CreateItem MessageDisposition="" SendMeetingInvitations="">
   <SavedItemFolderId/>
   <Items/>
</CreateItem>
```

<span data-ttu-id="e4962-105">**CreateItemType**</span><span class="sxs-lookup"><span data-stu-id="e4962-105">**CreateItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e4962-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="e4962-106">Attributes and elements</span></span>

<span data-ttu-id="e4962-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="e4962-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e4962-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="e4962-108">Attributes</span></span>

|<span data-ttu-id="e4962-109">Atributo</span><span class="sxs-lookup"><span data-stu-id="e4962-109">Attribute</span></span>|<span data-ttu-id="e4962-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4962-110">Description</span></span>|
|:-----|:-----|
|<span data-ttu-id="e4962-111">**MessageDisposition**</span><span class="sxs-lookup"><span data-stu-id="e4962-111">**MessageDisposition**</span></span> <br/> |<span data-ttu-id="e4962-112">Descreve como o item será tratado após sua criação.</span><span class="sxs-lookup"><span data-stu-id="e4962-112">Describes how the item will be handled after it is created.</span></span> <span data-ttu-id="e4962-113">O atributo é necessário para mensagens de email.</span><span class="sxs-lookup"><span data-stu-id="e4962-113">The attribute is required for e-mail messages.</span></span> <span data-ttu-id="e4962-114">Este atributo só é aplicável às mensagens de email.</span><span class="sxs-lookup"><span data-stu-id="e4962-114">This attribute is only applicable to e-mail messages.</span></span>  <br/> |
|<span data-ttu-id="e4962-115">**SendMeetingInvitations**</span><span class="sxs-lookup"><span data-stu-id="e4962-115">**SendMeetingInvitations**</span></span> <br/> |<span data-ttu-id="e4962-116">Descreve como as solicitações de reunião são manipuladas depois que eles são criados.</span><span class="sxs-lookup"><span data-stu-id="e4962-116">Describes how meeting requests are handled after they are created.</span></span> <span data-ttu-id="e4962-117">Este atributo é exigido para itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="e4962-117">This attribute is required for calendar items.</span></span>  <br/> |
   
#### <a name="messagedisposition-attribute"></a><span data-ttu-id="e4962-118">Atributo MessageDisposition</span><span class="sxs-lookup"><span data-stu-id="e4962-118">MessageDisposition Attribute</span></span>

|<span data-ttu-id="e4962-119">Valor</span><span class="sxs-lookup"><span data-stu-id="e4962-119">Value</span></span>|<span data-ttu-id="e4962-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4962-120">Description</span></span>|
|:-----|:-----|
|<span data-ttu-id="e4962-121">SaveOnly</span><span class="sxs-lookup"><span data-stu-id="e4962-121">SaveOnly</span></span>  <br/> |<span data-ttu-id="e4962-122">O item de mensagem é salvo na pasta especificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="e4962-122">The message item is saved in the folder that is specified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span> <span data-ttu-id="e4962-123">Mensagens podem ser enviadas posteriormente usando a [operação SendItem](senditem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="e4962-123">Messages can be sent later by using the [SendItem operation](senditem-operation.md).</span></span> <span data-ttu-id="e4962-124">Um identificador de item é retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="e4962-124">An item identifier is returned in the response.</span></span> <span data-ttu-id="e4962-125">Identificadores de item não são retornados para todos os tipos de item, exceto itens de mensagem.</span><span class="sxs-lookup"><span data-stu-id="e4962-125">Item identifiers are not returned for any item types except for message items.</span></span> <span data-ttu-id="e4962-126">Isso inclui objetos de resposta.</span><span class="sxs-lookup"><span data-stu-id="e4962-126">This includes response objects.</span></span>  <br/> |
|<span data-ttu-id="e4962-127">SendOnly</span><span class="sxs-lookup"><span data-stu-id="e4962-127">SendOnly</span></span>  <br/> |<span data-ttu-id="e4962-128">O item é enviado, mas nenhuma cópia é salva na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="e4962-128">The item is sent but no copy is saved in the Sent Items folder.</span></span> <span data-ttu-id="e4962-129">Um identificador de item não será retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="e4962-129">An item identifier is not returned in the response.</span></span><br/><br/><span data-ttu-id="e4962-130">**Observação**: **CreateItem** não oferece suporte a acesso de representante quando a opção SendOnly é usada como uma pasta de destino não pode ser especificada com essa opção.</span><span class="sxs-lookup"><span data-stu-id="e4962-130">**NOTE**: **CreateItem** does not support delegate access when the SendOnly option is used because a destination folder cannot be specified with this option.</span></span> <span data-ttu-id="e4962-131">A solução alternativa é criar o item, obtenha o identificador do item e, em seguida, use a operação SendItem para enviar o item.</span><span class="sxs-lookup"><span data-stu-id="e4962-131">The workaround is to create the item, get the item identifier, and then use the SendItem operation to send the item.</span></span>           |
|<span data-ttu-id="e4962-132">SendAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="e4962-132">SendAndSaveCopy</span></span>  <br/> |<span data-ttu-id="e4962-133">O item será enviado e uma cópia é salva na pasta que é identificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="e4962-133">The item is sent and a copy is saved in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span> <span data-ttu-id="e4962-134">Um identificador de item não será retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="e4962-134">An item identifier is not returned in the response.</span></span><br/><br/><span data-ttu-id="e4962-135">**Observação**: solicitações de reunião não são salvas na pasta que é identificado pela propriedade [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="e4962-135">**NOTE**: Meeting requests are not saved to the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) property.</span></span> <span data-ttu-id="e4962-136">Para o calendário, somente o salvar local dos itens do calendário pode ser especificada pela propriedade **SavedItemFolderId** .</span><span class="sxs-lookup"><span data-stu-id="e4962-136">For calendaring, only the save location for calendar items can be specified by the **SavedItemFolderId** property.</span></span> <span data-ttu-id="e4962-137">Não é possível controlar onde uma solicitação de reunião item é salva.</span><span class="sxs-lookup"><span data-stu-id="e4962-137">You cannot control where a meeting request item is saved.</span></span> <span data-ttu-id="e4962-138">Apenas os itens de calendário associadas são copiados e salvo na pasta que é identificada pela propriedade **SavedItemFolderId** .</span><span class="sxs-lookup"><span data-stu-id="e4962-138">Only the associated calendar items are copied and saved into the folder that is identified by the **SavedItemFolderId** property.</span></span>           |
   
#### <a name="sendmeetinginvitations-attribute"></a><span data-ttu-id="e4962-139">Atributo SendMeetingInvitations</span><span class="sxs-lookup"><span data-stu-id="e4962-139">SendMeetingInvitations Attribute</span></span>

|<span data-ttu-id="e4962-140">Valor</span><span class="sxs-lookup"><span data-stu-id="e4962-140">Value</span></span>|<span data-ttu-id="e4962-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4962-141">Description</span></span>|
|:-----|:-----|
|<span data-ttu-id="e4962-142">SendToNone</span><span class="sxs-lookup"><span data-stu-id="e4962-142">SendToNone</span></span>  <br/> |<span data-ttu-id="e4962-143">Se o item tem uma solicitação de reunião, ele é salvo como um item de calendário, mas não enviado.</span><span class="sxs-lookup"><span data-stu-id="e4962-143">If the item is a meeting request, it is saved as a calendar item but not sent.</span></span>  <br/> |
|<span data-ttu-id="e4962-144">SendOnlyToAll</span><span class="sxs-lookup"><span data-stu-id="e4962-144">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="e4962-145">A solicitação de reunião é enviada a todos os participantes, mas não é salvo na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="e4962-145">The meeting request is sent to all attendees but is not saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="e4962-146">SendToAllAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="e4962-146">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="e4962-147">A solicitação de reunião é enviada a todos os participantes e uma cópia é salva na pasta que é identificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="e4962-147">The meeting request is sent to all attendees and a copy is saved in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e4962-148">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="e4962-148">Child elements</span></span>

|<span data-ttu-id="e4962-149">Elemento</span><span class="sxs-lookup"><span data-stu-id="e4962-149">Element</span></span>|<span data-ttu-id="e4962-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4962-150">Description</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e4962-151">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="e4962-151">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> |<span data-ttu-id="e4962-152">Identifica a pasta de destino onde um novo item pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="e4962-152">Identifies the target folder where a new item can be created.</span></span> <span data-ttu-id="e4962-153">Se o atributo **MessageDisposition** é definido como SendOnly, uma mensagem criada só será enviada.</span><span class="sxs-lookup"><span data-stu-id="e4962-153">If the **MessageDisposition** attribute is set to SendOnly, a created message will only be sent.</span></span> <span data-ttu-id="e4962-154">A mensagem não será colocada na pasta que é identificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="e4962-154">The message will not be put in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="e4962-155">Items (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="e4962-155">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="e4962-156">Contém uma matriz de itens para criar a pasta que é identificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="e4962-156">Contains an array of items to create in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e4962-157">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="e4962-157">Parent elements</span></span>

<span data-ttu-id="e4962-158">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="e4962-158">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e4962-159">Comentários</span><span class="sxs-lookup"><span data-stu-id="e4962-159">Remarks</span></span>

<span data-ttu-id="e4962-160">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="e4962-160">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e4962-161">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="e4962-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e4962-162">Namespace</span><span class="sxs-lookup"><span data-stu-id="e4962-162">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e4962-163">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="e4962-163">Schema Name</span></span>  <br/> |<span data-ttu-id="e4962-164">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="e4962-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e4962-165">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="e4962-165">Validation File</span></span>  <br/> |<span data-ttu-id="e4962-166">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e4962-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e4962-167">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="e4962-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="e4962-168">False</span><span class="sxs-lookup"><span data-stu-id="e4962-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e4962-169">Ver também</span><span class="sxs-lookup"><span data-stu-id="e4962-169">See also</span></span>

- [<span data-ttu-id="e4962-170">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="e4962-170">CreateItemResponse</span></span>](createitemresponse.md)  
- [<span data-ttu-id="e4962-171">Operação CreateItem</span><span class="sxs-lookup"><span data-stu-id="e4962-171">CreateItem operation</span></span>](createitem-operation.md)
- [<span data-ttu-id="e4962-172">Criando mensagens de email</span><span class="sxs-lookup"><span data-stu-id="e4962-172">Creating E-mail Messages</span></span>](http://msdn.microsoft.com/library/05bfb83c-2866-427d-a9fe-14ba3cb02793%28Office.15%29.aspx) 
- [<span data-ttu-id="e4962-173">Criação de contatos (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="e4962-173">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [<span data-ttu-id="e4962-174">Criação de tarefas</span><span class="sxs-lookup"><span data-stu-id="e4962-174">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx) 
- [<span data-ttu-id="e4962-175">Criando compromissos</span><span class="sxs-lookup"><span data-stu-id="e4962-175">Creating Appointments</span></span>](http://msdn.microsoft.com/library/2385391e-c9e7-4d45-b803-c4ff94d5c94e%28Office.15%29.aspx)

