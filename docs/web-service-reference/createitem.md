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
description: O elemento CreateItem define uma solicitação para criar um item no repositório do Exchange.
ms.openlocfilehash: 235664b7baeceeccb14135fd346123f0f7d99346
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527058"
---
# <a name="createitem"></a><span data-ttu-id="7126e-103">CreateItem</span><span class="sxs-lookup"><span data-stu-id="7126e-103">CreateItem</span></span>

<span data-ttu-id="7126e-104">O elemento **CreateItem** define uma solicitação para criar um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7126e-104">The **CreateItem** element defines a request to create an item in the Exchange store.</span></span> 
  
```xml
<CreateItem MessageDisposition="" SendMeetingInvitations="">
   <SavedItemFolderId/>
   <Items/>
</CreateItem>
```

<span data-ttu-id="7126e-105">**CreateItemType**</span><span class="sxs-lookup"><span data-stu-id="7126e-105">**CreateItemType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7126e-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="7126e-106">Attributes and elements</span></span>

<span data-ttu-id="7126e-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7126e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7126e-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7126e-108">Attributes</span></span>

|<span data-ttu-id="7126e-109">Atributo</span><span class="sxs-lookup"><span data-stu-id="7126e-109">Attribute</span></span>|<span data-ttu-id="7126e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7126e-110">Description</span></span>|
|:-----|:-----|
|<span data-ttu-id="7126e-111">**MessageDisposition**</span><span class="sxs-lookup"><span data-stu-id="7126e-111">**MessageDisposition**</span></span> <br/> |<span data-ttu-id="7126e-112">Descreve como o item será manipulado após a criação.</span><span class="sxs-lookup"><span data-stu-id="7126e-112">Describes how the item will be handled after it is created.</span></span> <span data-ttu-id="7126e-113">O atributo é necessário para mensagens de email.</span><span class="sxs-lookup"><span data-stu-id="7126e-113">The attribute is required for e-mail messages.</span></span> <span data-ttu-id="7126e-114">Este atributo só é aplicável a mensagens de email.</span><span class="sxs-lookup"><span data-stu-id="7126e-114">This attribute is only applicable to e-mail messages.</span></span>  <br/> |
|<span data-ttu-id="7126e-115">**SendMeetingInvitations**</span><span class="sxs-lookup"><span data-stu-id="7126e-115">**SendMeetingInvitations**</span></span> <br/> |<span data-ttu-id="7126e-116">Descreve como as solicitações de reunião são tratadas após serem criadas.</span><span class="sxs-lookup"><span data-stu-id="7126e-116">Describes how meeting requests are handled after they are created.</span></span> <span data-ttu-id="7126e-117">Este atributo é obrigatório para itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="7126e-117">This attribute is required for calendar items.</span></span>  <br/> |
   
#### <a name="messagedisposition-attribute"></a><span data-ttu-id="7126e-118">Atributo MessageDisposition</span><span class="sxs-lookup"><span data-stu-id="7126e-118">MessageDisposition Attribute</span></span>

|<span data-ttu-id="7126e-119">Valor</span><span class="sxs-lookup"><span data-stu-id="7126e-119">Value</span></span>|<span data-ttu-id="7126e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="7126e-120">Description</span></span>|
|:-----|:-----|
|<span data-ttu-id="7126e-121">SaveOnly</span><span class="sxs-lookup"><span data-stu-id="7126e-121">SaveOnly</span></span>  <br/> |<span data-ttu-id="7126e-122">O item de mensagem é salvo na pasta que é especificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="7126e-122">The message item is saved in the folder that is specified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span> <span data-ttu-id="7126e-123">As mensagens podem ser enviadas posteriormente usando a [operação SendItem](senditem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="7126e-123">Messages can be sent later by using the [SendItem operation](senditem-operation.md).</span></span> <span data-ttu-id="7126e-124">Um identificador de item é retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="7126e-124">An item identifier is returned in the response.</span></span> <span data-ttu-id="7126e-125">Os identificadores de item não são retornados para qualquer tipo de item, exceto para itens de mensagem.</span><span class="sxs-lookup"><span data-stu-id="7126e-125">Item identifiers are not returned for any item types except for message items.</span></span> <span data-ttu-id="7126e-126">Isso inclui objetos Response.</span><span class="sxs-lookup"><span data-stu-id="7126e-126">This includes response objects.</span></span>  <br/> |
|<span data-ttu-id="7126e-127">SendOnly</span><span class="sxs-lookup"><span data-stu-id="7126e-127">SendOnly</span></span>  <br/> |<span data-ttu-id="7126e-128">O item é enviado, mas nenhuma cópia é salva na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="7126e-128">The item is sent but no copy is saved in the Sent Items folder.</span></span> <span data-ttu-id="7126e-129">Um identificador de item não é retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="7126e-129">An item identifier is not returned in the response.</span></span><br/><br/><span data-ttu-id="7126e-130">**Observação**: **CreateItem** não é compatível com o acesso de representante quando a opção SendOnly é usada porque uma pasta de destino não pode ser especificada com essa opção.</span><span class="sxs-lookup"><span data-stu-id="7126e-130">**NOTE**: **CreateItem** does not support delegate access when the SendOnly option is used because a destination folder cannot be specified with this option.</span></span> <span data-ttu-id="7126e-131">A solução alternativa é criar o item, obter o identificador de item e usar a operação SendItem para enviar o item.</span><span class="sxs-lookup"><span data-stu-id="7126e-131">The workaround is to create the item, get the item identifier, and then use the SendItem operation to send the item.</span></span>           |
|<span data-ttu-id="7126e-132">SendAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="7126e-132">SendAndSaveCopy</span></span>  <br/> |<span data-ttu-id="7126e-133">O item é enviado e uma cópia é salva na pasta identificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="7126e-133">The item is sent and a copy is saved in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span> <span data-ttu-id="7126e-134">Um identificador de item não é retornado na resposta.</span><span class="sxs-lookup"><span data-stu-id="7126e-134">An item identifier is not returned in the response.</span></span><br/><br/><span data-ttu-id="7126e-135">**Observação**: as solicitações de reunião não são salvas na pasta identificada pela propriedade [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="7126e-135">**NOTE**: Meeting requests are not saved to the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) property.</span></span> <span data-ttu-id="7126e-136">Para o calendário, somente o local de salvamento dos itens de calendário pode ser especificado pela propriedade **SavedItemFolderId** .</span><span class="sxs-lookup"><span data-stu-id="7126e-136">For calendaring, only the save location for calendar items can be specified by the **SavedItemFolderId** property.</span></span> <span data-ttu-id="7126e-137">Você não pode controlar onde um item de solicitação de reunião é salvo.</span><span class="sxs-lookup"><span data-stu-id="7126e-137">You cannot control where a meeting request item is saved.</span></span> <span data-ttu-id="7126e-138">Somente os itens de calendário associados são copiados e salvos na pasta identificada pela propriedade **SavedItemFolderId** .</span><span class="sxs-lookup"><span data-stu-id="7126e-138">Only the associated calendar items are copied and saved into the folder that is identified by the **SavedItemFolderId** property.</span></span>           |
   
#### <a name="sendmeetinginvitations-attribute"></a><span data-ttu-id="7126e-139">Atributo SendMeetingInvitations</span><span class="sxs-lookup"><span data-stu-id="7126e-139">SendMeetingInvitations Attribute</span></span>

|<span data-ttu-id="7126e-140">Valor</span><span class="sxs-lookup"><span data-stu-id="7126e-140">Value</span></span>|<span data-ttu-id="7126e-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="7126e-141">Description</span></span>|
|:-----|:-----|
|<span data-ttu-id="7126e-142">SendToNone</span><span class="sxs-lookup"><span data-stu-id="7126e-142">SendToNone</span></span>  <br/> |<span data-ttu-id="7126e-143">Se o item for uma solicitação de reunião, ele será salvo como um item de calendário, mas não será enviado.</span><span class="sxs-lookup"><span data-stu-id="7126e-143">If the item is a meeting request, it is saved as a calendar item but not sent.</span></span>  <br/> |
|<span data-ttu-id="7126e-144">SendOnlyToAll</span><span class="sxs-lookup"><span data-stu-id="7126e-144">SendOnlyToAll</span></span>  <br/> |<span data-ttu-id="7126e-145">A solicitação de reunião é enviada a todos os participantes, mas não é salva na pasta Itens enviados.</span><span class="sxs-lookup"><span data-stu-id="7126e-145">The meeting request is sent to all attendees but is not saved in the Sent Items folder.</span></span>  <br/> |
|<span data-ttu-id="7126e-146">SendToAllAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="7126e-146">SendToAllAndSaveCopy</span></span>  <br/> |<span data-ttu-id="7126e-147">A solicitação de reunião é enviada a todos os participantes e uma cópia é salva na pasta identificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="7126e-147">The meeting request is sent to all attendees and a copy is saved in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7126e-148">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7126e-148">Child elements</span></span>

|<span data-ttu-id="7126e-149">Elemento</span><span class="sxs-lookup"><span data-stu-id="7126e-149">Element</span></span>|<span data-ttu-id="7126e-150">Descrição</span><span class="sxs-lookup"><span data-stu-id="7126e-150">Description</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7126e-151">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="7126e-151">SavedItemFolderId</span></span>](saveditemfolderid.md) <br/> |<span data-ttu-id="7126e-152">Identifica a pasta de destino onde um novo item pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="7126e-152">Identifies the target folder where a new item can be created.</span></span> <span data-ttu-id="7126e-153">Se o atributo **MessageDisposition** for definido como SendOnly, uma mensagem criada será enviada apenas.</span><span class="sxs-lookup"><span data-stu-id="7126e-153">If the **MessageDisposition** attribute is set to SendOnly, a created message will only be sent.</span></span> <span data-ttu-id="7126e-154">A mensagem não será colocada na pasta que é identificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="7126e-154">The message will not be put in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
|[<span data-ttu-id="7126e-155">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="7126e-155">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md) <br/> |<span data-ttu-id="7126e-156">Contém uma matriz de itens a serem criados na pasta que é identificada pelo elemento [SavedItemFolderId](saveditemfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="7126e-156">Contains an array of items to create in the folder that is identified by the [SavedItemFolderId](saveditemfolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7126e-157">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7126e-157">Parent elements</span></span>

<span data-ttu-id="7126e-158">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7126e-158">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7126e-159">Comentários</span><span class="sxs-lookup"><span data-stu-id="7126e-159">Remarks</span></span>

<span data-ttu-id="7126e-160">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="7126e-160">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7126e-161">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="7126e-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7126e-162">Namespace</span><span class="sxs-lookup"><span data-stu-id="7126e-162">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7126e-163">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7126e-163">Schema Name</span></span>  <br/> |<span data-ttu-id="7126e-164">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="7126e-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7126e-165">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7126e-165">Validation File</span></span>  <br/> |<span data-ttu-id="7126e-166">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7126e-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7126e-167">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7126e-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="7126e-168">False</span><span class="sxs-lookup"><span data-stu-id="7126e-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7126e-169">Confira também</span><span class="sxs-lookup"><span data-stu-id="7126e-169">See also</span></span>

- [<span data-ttu-id="7126e-170">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="7126e-170">CreateItemResponse</span></span>](createitemresponse.md)  
- [<span data-ttu-id="7126e-171">Operação CreateItem</span><span class="sxs-lookup"><span data-stu-id="7126e-171">CreateItem operation</span></span>](createitem-operation.md)
- [<span data-ttu-id="7126e-172">Criar mensagens de email</span><span class="sxs-lookup"><span data-stu-id="7126e-172">Creating E-mail Messages</span></span>](https://msdn.microsoft.com/library/05bfb83c-2866-427d-a9fe-14ba3cb02793%28Office.15%29.aspx) 
- [<span data-ttu-id="7126e-173">Criando contatos (serviços Web do Exchange)</span><span class="sxs-lookup"><span data-stu-id="7126e-173">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [<span data-ttu-id="7126e-174">Criando tarefas</span><span class="sxs-lookup"><span data-stu-id="7126e-174">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx) 
- [<span data-ttu-id="7126e-175">Criar compromissos</span><span class="sxs-lookup"><span data-stu-id="7126e-175">Creating Appointments</span></span>](https://msdn.microsoft.com/library/2385391e-c9e7-4d45-b803-c4ff94d5c94e%28Office.15%29.aspx)

