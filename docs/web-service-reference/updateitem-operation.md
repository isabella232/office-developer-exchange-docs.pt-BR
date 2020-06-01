---
title: Operação UpdateItem
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
ms.assetid: 5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4
description: A operação UpdateItem é usada para modificar as propriedades de um item existente no repositório do Exchange.
ms.openlocfilehash: c001b7656862144023e9704cb04e6b4c0030f9df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459388"
---
# <a name="updateitem-operation"></a><span data-ttu-id="d06f6-103">Operação UpdateItem</span><span class="sxs-lookup"><span data-stu-id="d06f6-103">UpdateItem operation</span></span>

<span data-ttu-id="d06f6-104">A operação **UpdateItem** é usada para modificar as propriedades de um item existente no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d06f6-104">The **UpdateItem** operation is used to modify the properties of an existing item in the Exchange store.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d06f6-105">Comentários</span><span class="sxs-lookup"><span data-stu-id="d06f6-105">Remarks</span></span>

<span data-ttu-id="d06f6-106">Você pode executar três ações básicas de atualização em um item.</span><span class="sxs-lookup"><span data-stu-id="d06f6-106">You can perform three basic update actions on an item.</span></span> <span data-ttu-id="d06f6-107">A tabela a seguir lista as ações que você pode executar.</span><span class="sxs-lookup"><span data-stu-id="d06f6-107">The following table lists the actions that you can perform.</span></span>
  
|<span data-ttu-id="d06f6-108">**Action**</span><span class="sxs-lookup"><span data-stu-id="d06f6-108">**Action**</span></span>|<span data-ttu-id="d06f6-109">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d06f6-109">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d06f6-110">Append</span><span class="sxs-lookup"><span data-stu-id="d06f6-110">Append</span></span>  <br/> |<span data-ttu-id="d06f6-111">Adiciona dados a uma propriedade existente.</span><span class="sxs-lookup"><span data-stu-id="d06f6-111">Adds data to an existing property.</span></span> <span data-ttu-id="d06f6-112">Esta ação preserva os dados atuais.</span><span class="sxs-lookup"><span data-stu-id="d06f6-112">This action preserves the current data.</span></span> <span data-ttu-id="d06f6-113">Append não se aplica a todas as propriedades.</span><span class="sxs-lookup"><span data-stu-id="d06f6-113">Append does not apply to all properties.</span></span>  <br/> |
|<span data-ttu-id="d06f6-114">Set</span><span class="sxs-lookup"><span data-stu-id="d06f6-114">Set</span></span>  <br/> |<span data-ttu-id="d06f6-115">Substitui dados de uma propriedade se a propriedade contiver dados ou criar a propriedade e define seu valor se a propriedade não existir.</span><span class="sxs-lookup"><span data-stu-id="d06f6-115">Replaces data for a property if the property contains data, or creates the property and sets its value if the property does not exist.</span></span> <span data-ttu-id="d06f6-116">A ação Set só é aplicável a propriedades graváveis.</span><span class="sxs-lookup"><span data-stu-id="d06f6-116">The set action is only applicable to writable properties.</span></span>  <br/> |
|<span data-ttu-id="d06f6-117">Excluir</span><span class="sxs-lookup"><span data-stu-id="d06f6-117">Delete</span></span>  <br/> |<span data-ttu-id="d06f6-118">Remove uma propriedade de um item.</span><span class="sxs-lookup"><span data-stu-id="d06f6-118">Removes a property from an item.</span></span> <span data-ttu-id="d06f6-119">Isso difere da definição de uma propriedade para um valor vazio.</span><span class="sxs-lookup"><span data-stu-id="d06f6-119">This differs from setting a property to an empty value.</span></span> <span data-ttu-id="d06f6-120">Quando essa ação é concluída, a propriedade não existe para o item.</span><span class="sxs-lookup"><span data-stu-id="d06f6-120">When this action is finished, the property does not exist for the item.</span></span> <span data-ttu-id="d06f6-121">Delete só é aplicável a propriedades graváveis.</span><span class="sxs-lookup"><span data-stu-id="d06f6-121">Delete is only applicable to writable properties.</span></span>  <br/> |
   
<span data-ttu-id="d06f6-122">Uma chamada **UpdateItem** pode ser usada para modificar um ou mais itens e uma ou mais propriedades em cada item.</span><span class="sxs-lookup"><span data-stu-id="d06f6-122">An **UpdateItem** call can be used to modify one or more items, and one or more properties on each item.</span></span> <span data-ttu-id="d06f6-123">O elemento [Mychanges](itemchanges.md) contém todas as modificações que devem ser realizadas como parte desta chamada.</span><span class="sxs-lookup"><span data-stu-id="d06f6-123">The [ItemChanges](itemchanges.md) element contains all the modifications that are to be performed as part of this call.</span></span> <span data-ttu-id="d06f6-124">O elemento [ItemChange](itemchange.md) , um filho [do elemento items](itemchanges.md) , representa as modificações a serem realizadas em um único item.</span><span class="sxs-lookup"><span data-stu-id="d06f6-124">The [ItemChange](itemchange.md) element, a child of the [ItemChanges](itemchanges.md) element, represents the modifications to be performed on a single item.</span></span> <span data-ttu-id="d06f6-125">O elemento [ItemChange](itemchange.md) contém um conjunto de ações de atualização que podem ser executadas em um único item.</span><span class="sxs-lookup"><span data-stu-id="d06f6-125">The [ItemChange](itemchange.md) element contains a set of update actions that can be performed on a single item.</span></span> <span data-ttu-id="d06f6-126">Essas alterações estão contidas no elemento [Updates (item)](updates-item.md) .</span><span class="sxs-lookup"><span data-stu-id="d06f6-126">These changes are contained in the [Updates (Item)](updates-item.md) element.</span></span> <span data-ttu-id="d06f6-127">O elemento [ItemId](itemid.md) identifica o item a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="d06f6-127">The [ItemId](itemid.md) element identifies the item to update.</span></span> <span data-ttu-id="d06f6-128">Para atualizar mais de uma propriedade em um item, um [Setitemfield](setitemfield.md), [AppendToItemField](appendtoitemfield.md)ou [DeleteItemField](deleteitemfield.md) deve ser fornecido para cada propriedade que requer a atualização.</span><span class="sxs-lookup"><span data-stu-id="d06f6-128">To update more than one property on an item, a [SetItemField](setitemfield.md), [AppendToItemField](appendtoitemfield.md), or [DeleteItemField](deleteitemfield.md) must be provided for each property that requires the update.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="d06f6-129">As ações de atualização são aplicadas na ordem em que são especificadas.</span><span class="sxs-lookup"><span data-stu-id="d06f6-129">Update actions are applied in the order in which they are specified.</span></span> 
  
<span data-ttu-id="d06f6-130">Para cada alteração, você precisa especificar o caminho da propriedade a ser alterada e uma representação desse item com o novo valor.</span><span class="sxs-lookup"><span data-stu-id="d06f6-130">For each change, you have to specify the path of the property to change and a representation of that item with its new value.</span></span> <span data-ttu-id="d06f6-131">A ação de exclusão é ligeiramente diferente, pois apenas o caminho da propriedade que deve ser excluído é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d06f6-131">The delete action is slightly different in that only the path of the property that should be deleted is required.</span></span> <span data-ttu-id="d06f6-132">Para ações set e Append, o caminho especificado deve se referir à mesma propriedade que está sendo definida na representação do item.</span><span class="sxs-lookup"><span data-stu-id="d06f6-132">For set and append actions, the path that is specified must refer to the same property that is being set in the item representation.</span></span> <span data-ttu-id="d06f6-133">Se forem diferentes, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="d06f6-133">If these differ, an error will be returned.</span></span>
  
<span data-ttu-id="d06f6-134">A operação **UpdateItem** pode definir a hora de [início](start.md) e de [término](end-ex15websvcsotherref.md) de um item do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d06f6-134">The **UpdateItem** operation can set the [Start](start.md) and [End ](end-ex15websvcsotherref.md) time of an Exchange store item.</span></span> <span data-ttu-id="d06f6-135">Em uma solicitação **UpdateItem** , a hora de [início](start.md) pode ser definida sem definir também a hora de [término](end-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="d06f6-135">In an **UpdateItem** request, the [Start](start.md) time can be set without also setting the [End ](end-ex15websvcsotherref.md) time.</span></span> <span data-ttu-id="d06f6-136">Isso pode causar um erro se a hora de [início](start.md) for posterior à hora de [término](end-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="d06f6-136">This can cause an error if the [Start](start.md) time is later than the [End ](end-ex15websvcsotherref.md) time.</span></span> <span data-ttu-id="d06f6-137">Lembre-se de que os aplicativos cliente devem ajustar a hora de [término](end-ex15websvcsotherref.md) quando a hora de [início](start.md) é alterada para preservar a duração.</span><span class="sxs-lookup"><span data-stu-id="d06f6-137">Be aware that client applications must adjust the [End ](end-ex15websvcsotherref.md) time when the [Start](start.md) time is changed in order to preserve the duration.</span></span> 
  
<span data-ttu-id="d06f6-138">Quando um único item de calendário é atualizado para se tornar um item de calendário mestre recorrente, a propriedade [MeetingTimeZone](meetingtimezone.md) deve ser definida pela operação **UpdateItem** para preservar o fuso horário original do item do calendário.</span><span class="sxs-lookup"><span data-stu-id="d06f6-138">When a single calendar item is updated to become a recurring master calendar item, the [MeetingTimeZone](meetingtimezone.md) property must be set by the **UpdateItem** operation in order to preserve the calendar item's original time zone.</span></span> 
  
## <a name="setitemfield-request-example"></a><span data-ttu-id="d06f6-139">Exemplo de solicitação setitemfield</span><span class="sxs-lookup"><span data-stu-id="d06f6-139">SetItemField request example</span></span>

### <a name="description"></a><span data-ttu-id="d06f6-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="d06f6-140">Description</span></span>

<span data-ttu-id="d06f6-141">O exemplo a seguir de uma solicitação **UpdateItem** mostra como definir a propriedade sensibilidade em um item.</span><span class="sxs-lookup"><span data-stu-id="d06f6-141">The following example of an **UpdateItem** request shows how to set the sensitivity property on an item.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d06f6-142">Código</span><span class="sxs-lookup"><span data-stu-id="d06f6-142">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkb..." ChangeKey="CQAAABYAAAB..."/>
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Sensitivity"/>
              <t:Message>
                <t:Sensitivity>Normal</t:Sensitivity>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="d06f6-143">Comentários</span><span class="sxs-lookup"><span data-stu-id="d06f6-143">Comments</span></span>

<span data-ttu-id="d06f6-144">O identificador de item e a chave de alteração foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d06f6-144">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="setitemfield-request-elements"></a><span data-ttu-id="d06f6-145">Elementos de solicitação setitemfield</span><span class="sxs-lookup"><span data-stu-id="d06f6-145">SetItemField Request Elements</span></span>

<span data-ttu-id="d06f6-146">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="d06f6-146">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="d06f6-147">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="d06f6-147">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="d06f6-148">Alterações</span><span class="sxs-lookup"><span data-stu-id="d06f6-148">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="d06f6-149">ItemChange</span><span class="sxs-lookup"><span data-stu-id="d06f6-149">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="d06f6-150">ItemId</span><span class="sxs-lookup"><span data-stu-id="d06f6-150">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="d06f6-151">Atualizações (item)</span><span class="sxs-lookup"><span data-stu-id="d06f6-151">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="d06f6-152">Setitemfield</span><span class="sxs-lookup"><span data-stu-id="d06f6-152">SetItemField</span></span>](setitemfield.md)
    
- [<span data-ttu-id="d06f6-153">FieldURI</span><span class="sxs-lookup"><span data-stu-id="d06f6-153">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="d06f6-154">Message</span><span class="sxs-lookup"><span data-stu-id="d06f6-154">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="d06f6-155">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="d06f6-155">Sensitivity</span></span>](sensitivity.md)
    
## <a name="appendtoitemfield-request-example"></a><span data-ttu-id="d06f6-156">Exemplo de solicitação AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="d06f6-156">AppendToItemField request example</span></span>

### <a name="description"></a><span data-ttu-id="d06f6-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="d06f6-157">Description</span></span>

<span data-ttu-id="d06f6-158">O exemplo a seguir de uma solicitação **UpdateItem** mostra como acrescentar texto à Propriedade Body em um item.</span><span class="sxs-lookup"><span data-stu-id="d06f6-158">The following example of an **UpdateItem** request shows how to append text to the body property on an item.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d06f6-159">Código</span><span class="sxs-lookup"><span data-stu-id="d06f6-159">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkbW..." ChangeKey="CQAAABYA..."/>
          <t:Updates>
            <t:AppendToItemField>
              <t:FieldURI FieldURI="item:Body"/>
              <t:Message>
                <t:Body BodyType="Text">Some additional text to append</t:Body>
              </t:Message>
            </t:AppendToItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="d06f6-160">Comentários</span><span class="sxs-lookup"><span data-stu-id="d06f6-160">Comments</span></span>

<span data-ttu-id="d06f6-161">As propriedades a seguir dão suporte à ação Append:</span><span class="sxs-lookup"><span data-stu-id="d06f6-161">The following properties support the append action:</span></span>
  
- <span data-ttu-id="d06f6-162">**mensagem: ReplyTo**</span><span class="sxs-lookup"><span data-stu-id="d06f6-162">**message:ReplyTo**</span></span>
    
- <span data-ttu-id="d06f6-163">**item: Body**</span><span class="sxs-lookup"><span data-stu-id="d06f6-163">**item:Body**</span></span>
    
- <span data-ttu-id="d06f6-164">Todas as propriedades de coleção Recipient e participante</span><span class="sxs-lookup"><span data-stu-id="d06f6-164">All the recipient and attendee collection properties</span></span>
    
<span data-ttu-id="d06f6-165">O identificador de item e a chave de alteração foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d06f6-165">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="appendtoitemfield-request-elements"></a><span data-ttu-id="d06f6-166">Elementos de solicitação AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="d06f6-166">AppendToItemField Request Elements</span></span>

<span data-ttu-id="d06f6-167">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="d06f6-167">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="d06f6-168">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="d06f6-168">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="d06f6-169">Alterações</span><span class="sxs-lookup"><span data-stu-id="d06f6-169">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="d06f6-170">ItemChange</span><span class="sxs-lookup"><span data-stu-id="d06f6-170">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="d06f6-171">ItemId</span><span class="sxs-lookup"><span data-stu-id="d06f6-171">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="d06f6-172">Atualizações (item)</span><span class="sxs-lookup"><span data-stu-id="d06f6-172">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="d06f6-173">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="d06f6-173">AppendToItemField</span></span>](appendtoitemfield.md)
    
- [<span data-ttu-id="d06f6-174">FieldURI</span><span class="sxs-lookup"><span data-stu-id="d06f6-174">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="d06f6-175">Message</span><span class="sxs-lookup"><span data-stu-id="d06f6-175">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="d06f6-176">Body</span><span class="sxs-lookup"><span data-stu-id="d06f6-176">Body</span></span>](body.md)
    
## <a name="deleteitemfield-request-example"></a><span data-ttu-id="d06f6-177">Exemplo de solicitação DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="d06f6-177">DeleteItemField request example</span></span>

### <a name="description"></a><span data-ttu-id="d06f6-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="d06f6-178">Description</span></span>

<span data-ttu-id="d06f6-179">O exemplo a seguir de uma solicitação **UpdateItem** mostra como excluir uma propriedade em um item.</span><span class="sxs-lookup"><span data-stu-id="d06f6-179">The following example of an **UpdateItem** request shows how to delete a property on an item.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d06f6-180">Código</span><span class="sxs-lookup"><span data-stu-id="d06f6-180">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkbWluaXN0cm..." ChangeKey="CQAAABYAA..."/>
          <t:Updates>
            <t:DeleteItemField>
              <t:FieldURI FieldURI="item:Body"/>
            </t:DeleteItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="d06f6-181">Comentários</span><span class="sxs-lookup"><span data-stu-id="d06f6-181">Comments</span></span>

<span data-ttu-id="d06f6-182">O identificador de item e a chave de alteração foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d06f6-182">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="deleteitemfield-request-elements"></a><span data-ttu-id="d06f6-183">Elementos de solicitação DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="d06f6-183">DeleteItemField Request Elements</span></span>

<span data-ttu-id="d06f6-184">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="d06f6-184">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="d06f6-185">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="d06f6-185">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="d06f6-186">Alterações</span><span class="sxs-lookup"><span data-stu-id="d06f6-186">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="d06f6-187">ItemChange</span><span class="sxs-lookup"><span data-stu-id="d06f6-187">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="d06f6-188">ItemId</span><span class="sxs-lookup"><span data-stu-id="d06f6-188">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="d06f6-189">Atualizações (item)</span><span class="sxs-lookup"><span data-stu-id="d06f6-189">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="d06f6-190">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="d06f6-190">DeleteItemField</span></span>](deleteitemfield.md)
    
- [<span data-ttu-id="d06f6-191">FieldURI</span><span class="sxs-lookup"><span data-stu-id="d06f6-191">FieldURI</span></span>](fielduri.md)
    
## <a name="successful-response-example"></a><span data-ttu-id="d06f6-192">Exemplo de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="d06f6-192">Successful response example</span></span>

### <a name="description"></a><span data-ttu-id="d06f6-193">Descrição</span><span class="sxs-lookup"><span data-stu-id="d06f6-193">Description</span></span>

<span data-ttu-id="d06f6-194">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação **UpdateItem** .</span><span class="sxs-lookup"><span data-stu-id="d06f6-194">The following example shows a successful response to an **UpdateItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d06f6-195">Código</span><span class="sxs-lookup"><span data-stu-id="d06f6-195">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
  xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="664" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <UpdateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="AAAtAEFkbW..." ChangeKey="CQAAABYAAA..."/>
            </t:Message>
          </m:Items>
        </m:UpdateItemResponseMessage>
      </m:ResponseMessages>
    </UpdateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="d06f6-196">Comentários</span><span class="sxs-lookup"><span data-stu-id="d06f6-196">Comments</span></span>

<span data-ttu-id="d06f6-197">O identificador de item e a chave de alteração foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d06f6-197">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="d06f6-198">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="d06f6-198">Successful response elements</span></span>

<span data-ttu-id="d06f6-199">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="d06f6-199">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="d06f6-200">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d06f6-200">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="d06f6-201">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="d06f6-201">UpdateItemResponse</span></span>](updateitemresponse.md)
    
- [<span data-ttu-id="d06f6-202">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d06f6-202">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="d06f6-203">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d06f6-203">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
    
- [<span data-ttu-id="d06f6-204">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d06f6-204">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d06f6-205">Itens</span><span class="sxs-lookup"><span data-stu-id="d06f6-205">Items</span></span>](items.md)
    
- [<span data-ttu-id="d06f6-206">Message</span><span class="sxs-lookup"><span data-stu-id="d06f6-206">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="d06f6-207">ItemId</span><span class="sxs-lookup"><span data-stu-id="d06f6-207">ItemId</span></span>](itemid.md)
    
## <a name="see-also"></a><span data-ttu-id="d06f6-208">Também consulte</span><span class="sxs-lookup"><span data-stu-id="d06f6-208">See also</span></span>



[<span data-ttu-id="d06f6-209">Operação UpdateItem (tarefa)</span><span class="sxs-lookup"><span data-stu-id="d06f6-209">UpdateItem operation (task)</span></span>](updateitem-operation-task.md)
  
[<span data-ttu-id="d06f6-210">Operação UpdateItem (contato)</span><span class="sxs-lookup"><span data-stu-id="d06f6-210">UpdateItem operation (contact)</span></span>](updateitem-operation-contact.md)


- [<span data-ttu-id="d06f6-211">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d06f6-211">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="d06f6-212">Atualizando contatos</span><span class="sxs-lookup"><span data-stu-id="d06f6-212">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="d06f6-213">Atualizando tarefas</span><span class="sxs-lookup"><span data-stu-id="d06f6-213">Updating Tasks</span></span>](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

