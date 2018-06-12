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
description: A operação UpdateItem é usada para modificar as propriedades de um item existente no armazenamento do Exchange.
ms.openlocfilehash: 009ba16315017c4418fbd71d49744015c4d6d1b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837913"
---
# <a name="updateitem-operation"></a><span data-ttu-id="adc22-103">Operação UpdateItem</span><span class="sxs-lookup"><span data-stu-id="adc22-103">UpdateItem operation</span></span>

<span data-ttu-id="adc22-104">A operação **UpdateItem** é usada para modificar as propriedades de um item existente no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="adc22-104">The **UpdateItem** operation is used to modify the properties of an existing item in the Exchange store.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="adc22-105">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="adc22-105">Remarks</span></span>

<span data-ttu-id="adc22-106">Você pode executar três ações de atualização básica em um item.</span><span class="sxs-lookup"><span data-stu-id="adc22-106">You can perform three basic update actions on an item.</span></span> <span data-ttu-id="adc22-107">A tabela a seguir lista as ações que podem ser executadas.</span><span class="sxs-lookup"><span data-stu-id="adc22-107">The following table lists the actions that you can perform.</span></span>
  
|<span data-ttu-id="adc22-108">**Action**</span><span class="sxs-lookup"><span data-stu-id="adc22-108">**Action**</span></span>|<span data-ttu-id="adc22-109">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="adc22-109">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="adc22-110">Acréscimo</span><span class="sxs-lookup"><span data-stu-id="adc22-110">Append</span></span>  <br/> |<span data-ttu-id="adc22-111">Adiciona dados a uma propriedade existente.</span><span class="sxs-lookup"><span data-stu-id="adc22-111">Adds data to an existing property.</span></span> <span data-ttu-id="adc22-112">Essa ação preserva os dados atuais.</span><span class="sxs-lookup"><span data-stu-id="adc22-112">This action preserves the current data.</span></span> <span data-ttu-id="adc22-113">Acrescentar não se aplica a todas as propriedades.</span><span class="sxs-lookup"><span data-stu-id="adc22-113">Append does not apply to all properties.</span></span>  <br/> |
|<span data-ttu-id="adc22-114">Conjunto</span><span class="sxs-lookup"><span data-stu-id="adc22-114">Set</span></span>  <br/> |<span data-ttu-id="adc22-115">Substitui os dados de uma propriedade se a propriedade contém dados, ou cria a propriedade e define seu valor se a propriedade não existir.</span><span class="sxs-lookup"><span data-stu-id="adc22-115">Replaces data for a property if the property contains data, or creates the property and sets its value if the property does not exist.</span></span> <span data-ttu-id="adc22-116">A ação set só é aplicável às propriedades graváveis.</span><span class="sxs-lookup"><span data-stu-id="adc22-116">The set action is only applicable to writable properties.</span></span>  <br/> |
|<span data-ttu-id="adc22-117">Excluir</span><span class="sxs-lookup"><span data-stu-id="adc22-117">Delete</span></span>  <br/> |<span data-ttu-id="adc22-118">Remove uma propriedade de um item.</span><span class="sxs-lookup"><span data-stu-id="adc22-118">Removes a property from an item.</span></span> <span data-ttu-id="adc22-119">Isso é diferente da configuração de uma propriedade para um valor vazio.</span><span class="sxs-lookup"><span data-stu-id="adc22-119">This differs from setting a property to an empty value.</span></span> <span data-ttu-id="adc22-120">Quando essa ação for concluída, a propriedade não existe para o item.</span><span class="sxs-lookup"><span data-stu-id="adc22-120">When this action is finished, the property does not exist for the item.</span></span> <span data-ttu-id="adc22-121">Excluir só é aplicável às propriedades graváveis.</span><span class="sxs-lookup"><span data-stu-id="adc22-121">Delete is only applicable to writable properties.</span></span>  <br/> |
   
<span data-ttu-id="adc22-122">Uma chamada **UpdateItem** pode ser usada para modificar um ou mais itens e uma ou mais propriedades em cada item.</span><span class="sxs-lookup"><span data-stu-id="adc22-122">An **UpdateItem** call can be used to modify one or more items, and one or more properties on each item.</span></span> <span data-ttu-id="adc22-123">O elemento [ItemChanges](itemchanges.md) contém todas as modificações que devem ser executadas como parte desta chamada.</span><span class="sxs-lookup"><span data-stu-id="adc22-123">The [ItemChanges](itemchanges.md) element contains all the modifications that are to be performed as part of this call.</span></span> <span data-ttu-id="adc22-124">O elemento [ItemChange](itemchange.md) , um filho do elemento [ItemChanges](itemchanges.md) , representa as modificações para ser executado em um único item.</span><span class="sxs-lookup"><span data-stu-id="adc22-124">The [ItemChange](itemchange.md) element, a child of the [ItemChanges](itemchanges.md) element, represents the modifications to be performed on a single item.</span></span> <span data-ttu-id="adc22-125">O elemento de [ItemChange](itemchange.md) contém um conjunto de ações de atualização que podem ser executadas em um único item.</span><span class="sxs-lookup"><span data-stu-id="adc22-125">The [ItemChange](itemchange.md) element contains a set of update actions that can be performed on a single item.</span></span> <span data-ttu-id="adc22-126">Essas alterações estão contidas no elemento [atualizações (Item)](updates-item.md) .</span><span class="sxs-lookup"><span data-stu-id="adc22-126">These changes are contained in the [Updates (Item)](updates-item.md) element.</span></span> <span data-ttu-id="adc22-127">O elemento [ItemId](itemid.md) identifica o item a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="adc22-127">The [ItemId](itemid.md) element identifies the item to update.</span></span> <span data-ttu-id="adc22-128">Para atualizar mais de uma propriedade em um item, um [SetItemField](setitemfield.md), [AppendToItemField](appendtoitemfield.md)ou [DeleteItemField](deleteitemfield.md) deve ser fornecido para cada propriedade que requer a atualização.</span><span class="sxs-lookup"><span data-stu-id="adc22-128">To update more than one property on an item, a [SetItemField](setitemfield.md), [AppendToItemField](appendtoitemfield.md), or [DeleteItemField](deleteitemfield.md) must be provided for each property that requires the update.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="adc22-129">Ações de atualização são aplicadas na ordem na qual foram especificados.</span><span class="sxs-lookup"><span data-stu-id="adc22-129">Update actions are applied in the order in which they are specified.</span></span> 
  
<span data-ttu-id="adc22-130">Para cada alteração, você precisará especificar o caminho da propriedade para alterar e uma representação de um item com o seu novo valor.</span><span class="sxs-lookup"><span data-stu-id="adc22-130">For each change, you have to specify the path of the property to change and a representation of that item with its new value.</span></span> <span data-ttu-id="adc22-131">A ação Excluir é ligeiramente diferente apenas o caminho da propriedade que deve ser excluído é necessário.</span><span class="sxs-lookup"><span data-stu-id="adc22-131">The delete action is slightly different in that only the path of the property that should be deleted is required.</span></span> <span data-ttu-id="adc22-132">Para definir e acrescentar ações, o caminho especificado deve se referir a mesma propriedade que está sendo definida na representação do item.</span><span class="sxs-lookup"><span data-stu-id="adc22-132">For set and append actions, the path that is specified must refer to the same property that is being set in the item representation.</span></span> <span data-ttu-id="adc22-133">Se eles forem diferentes, um erro será retornado.</span><span class="sxs-lookup"><span data-stu-id="adc22-133">If these differ, an error will be returned.</span></span>
  
<span data-ttu-id="adc22-134">A operação **UpdateItem** pode definir a hora de [início](start.md) e [término](end-ex15websvcsotherref.md) de um item de armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="adc22-134">The **UpdateItem** operation can set the [Start](start.md) and [End ](end-ex15websvcsotherref.md) time of an Exchange store item.</span></span> <span data-ttu-id="adc22-135">Em uma solicitação de **UpdateItem** , a hora de [início](start.md) pode ser definida sem também definir a hora de [término](end-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="adc22-135">In an **UpdateItem** request, the [Start](start.md) time can be set without also setting the [End ](end-ex15websvcsotherref.md) time.</span></span> <span data-ttu-id="adc22-136">Isso pode causar um erro se a hora de [início](start.md) é posterior à hora de [término](end-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="adc22-136">This can cause an error if the [Start](start.md) time is later than the [End ](end-ex15websvcsotherref.md) time.</span></span> <span data-ttu-id="adc22-137">Lembre-se de que os aplicativos cliente devem ajustar a hora de [término](end-ex15websvcsotherref.md) quando a hora de [início](start.md) for alterada para preservar a duração.</span><span class="sxs-lookup"><span data-stu-id="adc22-137">Be aware that client applications must adjust the [End ](end-ex15websvcsotherref.md) time when the [Start](start.md) time is changed in order to preserve the duration.</span></span> 
  
<span data-ttu-id="adc22-138">Quando um item de calendário único é atualizado para se tornar um item de calendário mestre recorrente, a propriedade [MeetingTimeZone](meetingtimezone.md) deve ser definida pela operação de **UpdateItem** para preservar o fuso horário original do item de calendário.</span><span class="sxs-lookup"><span data-stu-id="adc22-138">When a single calendar item is updated to become a recurring master calendar item, the [MeetingTimeZone](meetingtimezone.md) property must be set by the **UpdateItem** operation in order to preserve the calendar item's original time zone.</span></span> 
  
## <a name="setitemfield-request-example"></a><span data-ttu-id="adc22-139">Exemplo de solicitação de SetItemField</span><span class="sxs-lookup"><span data-stu-id="adc22-139">SetItemField request example</span></span>

### <a name="description"></a><span data-ttu-id="adc22-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="adc22-140">Description</span></span>

<span data-ttu-id="adc22-141">O exemplo a seguir de uma solicitação de **UpdateItem** mostra como definir a propriedade sensitivity em um item.</span><span class="sxs-lookup"><span data-stu-id="adc22-141">The following example of an **UpdateItem** request shows how to set the sensitivity property on an item.</span></span> 
  
### <a name="code"></a><span data-ttu-id="adc22-142">Código</span><span class="sxs-lookup"><span data-stu-id="adc22-142">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="adc22-143">Comments</span><span class="sxs-lookup"><span data-stu-id="adc22-143">Comments</span></span>

<span data-ttu-id="adc22-144">O identificador do item e alterar chave foram diminuídas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="adc22-144">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="setitemfield-request-elements"></a><span data-ttu-id="adc22-145">Elementos de solicitação de SetItemField</span><span class="sxs-lookup"><span data-stu-id="adc22-145">SetItemField Request Elements</span></span>

<span data-ttu-id="adc22-146">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="adc22-146">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="adc22-147">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="adc22-147">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="adc22-148">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="adc22-148">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="adc22-149">ItemChange</span><span class="sxs-lookup"><span data-stu-id="adc22-149">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="adc22-150">ItemId</span><span class="sxs-lookup"><span data-stu-id="adc22-150">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="adc22-151">Atualizações (Item)</span><span class="sxs-lookup"><span data-stu-id="adc22-151">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="adc22-152">SetItemField</span><span class="sxs-lookup"><span data-stu-id="adc22-152">SetItemField</span></span>](setitemfield.md)
    
- [<span data-ttu-id="adc22-153">FieldURI</span><span class="sxs-lookup"><span data-stu-id="adc22-153">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="adc22-154">Mensagem</span><span class="sxs-lookup"><span data-stu-id="adc22-154">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="adc22-155">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="adc22-155">Sensitivity</span></span>](sensitivity.md)
    
## <a name="appendtoitemfield-request-example"></a><span data-ttu-id="adc22-156">Exemplo de solicitação de AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="adc22-156">AppendToItemField request example</span></span>

### <a name="description"></a><span data-ttu-id="adc22-157">Descrição</span><span class="sxs-lookup"><span data-stu-id="adc22-157">Description</span></span>

<span data-ttu-id="adc22-158">O exemplo a seguir de uma solicitação de **UpdateItem** mostra como acrescentar texto a propriedade body em um item.</span><span class="sxs-lookup"><span data-stu-id="adc22-158">The following example of an **UpdateItem** request shows how to append text to the body property on an item.</span></span> 
  
### <a name="code"></a><span data-ttu-id="adc22-159">Código</span><span class="sxs-lookup"><span data-stu-id="adc22-159">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="adc22-160">Comments</span><span class="sxs-lookup"><span data-stu-id="adc22-160">Comments</span></span>

<span data-ttu-id="adc22-161">As propriedades a seguir oferecem suporte à ação de append:</span><span class="sxs-lookup"><span data-stu-id="adc22-161">The following properties support the append action:</span></span>
  
- <span data-ttu-id="adc22-162">**mensagem: ReplyTo**</span><span class="sxs-lookup"><span data-stu-id="adc22-162">**message:ReplyTo**</span></span>
    
- <span data-ttu-id="adc22-163">**Corpo do item:**</span><span class="sxs-lookup"><span data-stu-id="adc22-163">**item:Body**</span></span>
    
- <span data-ttu-id="adc22-164">Todas as participante e destinatário coleção propriedades</span><span class="sxs-lookup"><span data-stu-id="adc22-164">All the recipient and attendee collection properties</span></span>
    
<span data-ttu-id="adc22-165">O identificador do item e alterar chave foram diminuídas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="adc22-165">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="appendtoitemfield-request-elements"></a><span data-ttu-id="adc22-166">Elementos de solicitação de AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="adc22-166">AppendToItemField Request Elements</span></span>

<span data-ttu-id="adc22-167">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="adc22-167">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="adc22-168">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="adc22-168">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="adc22-169">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="adc22-169">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="adc22-170">ItemChange</span><span class="sxs-lookup"><span data-stu-id="adc22-170">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="adc22-171">ItemId</span><span class="sxs-lookup"><span data-stu-id="adc22-171">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="adc22-172">Atualizações (Item)</span><span class="sxs-lookup"><span data-stu-id="adc22-172">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="adc22-173">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="adc22-173">AppendToItemField</span></span>](appendtoitemfield.md)
    
- [<span data-ttu-id="adc22-174">FieldURI</span><span class="sxs-lookup"><span data-stu-id="adc22-174">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="adc22-175">Mensagem</span><span class="sxs-lookup"><span data-stu-id="adc22-175">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="adc22-176">Corpo</span><span class="sxs-lookup"><span data-stu-id="adc22-176">Body</span></span>](body.md)
    
## <a name="deleteitemfield-request-example"></a><span data-ttu-id="adc22-177">Exemplo de solicitação de DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="adc22-177">DeleteItemField request example</span></span>

### <a name="description"></a><span data-ttu-id="adc22-178">Descrição</span><span class="sxs-lookup"><span data-stu-id="adc22-178">Description</span></span>

<span data-ttu-id="adc22-179">O exemplo a seguir de uma solicitação de **UpdateItem** mostra como excluir uma propriedade em um item.</span><span class="sxs-lookup"><span data-stu-id="adc22-179">The following example of an **UpdateItem** request shows how to delete a property on an item.</span></span> 
  
### <a name="code"></a><span data-ttu-id="adc22-180">Código</span><span class="sxs-lookup"><span data-stu-id="adc22-180">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="adc22-181">Comments</span><span class="sxs-lookup"><span data-stu-id="adc22-181">Comments</span></span>

<span data-ttu-id="adc22-182">O identificador do item e alterar chave foram diminuídas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="adc22-182">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="deleteitemfield-request-elements"></a><span data-ttu-id="adc22-183">Elementos de solicitação de DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="adc22-183">DeleteItemField Request Elements</span></span>

<span data-ttu-id="adc22-184">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="adc22-184">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="adc22-185">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="adc22-185">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="adc22-186">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="adc22-186">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="adc22-187">ItemChange</span><span class="sxs-lookup"><span data-stu-id="adc22-187">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="adc22-188">ItemId</span><span class="sxs-lookup"><span data-stu-id="adc22-188">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="adc22-189">Atualizações (Item)</span><span class="sxs-lookup"><span data-stu-id="adc22-189">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="adc22-190">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="adc22-190">DeleteItemField</span></span>](deleteitemfield.md)
    
- [<span data-ttu-id="adc22-191">FieldURI</span><span class="sxs-lookup"><span data-stu-id="adc22-191">FieldURI</span></span>](fielduri.md)
    
## <a name="successful-response-example"></a><span data-ttu-id="adc22-192">Exemplo de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="adc22-192">Successful response example</span></span>

### <a name="description"></a><span data-ttu-id="adc22-193">Descrição</span><span class="sxs-lookup"><span data-stu-id="adc22-193">Description</span></span>

<span data-ttu-id="adc22-194">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de **UpdateItem** .</span><span class="sxs-lookup"><span data-stu-id="adc22-194">The following example shows a successful response to an **UpdateItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="adc22-195">Código</span><span class="sxs-lookup"><span data-stu-id="adc22-195">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
  xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="664" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <UpdateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="adc22-196">Comments</span><span class="sxs-lookup"><span data-stu-id="adc22-196">Comments</span></span>

<span data-ttu-id="adc22-197">O identificador do item e alterar chave foram diminuídas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="adc22-197">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="adc22-198">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="adc22-198">Successful response elements</span></span>

<span data-ttu-id="adc22-199">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="adc22-199">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="adc22-200">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="adc22-200">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="adc22-201">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="adc22-201">UpdateItemResponse</span></span>](updateitemresponse.md)
    
- [<span data-ttu-id="adc22-202">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="adc22-202">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="adc22-203">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="adc22-203">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
    
- [<span data-ttu-id="adc22-204">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="adc22-204">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="adc22-205">Items</span><span class="sxs-lookup"><span data-stu-id="adc22-205">Items</span></span>](items.md)
    
- [<span data-ttu-id="adc22-206">Mensagem</span><span class="sxs-lookup"><span data-stu-id="adc22-206">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="adc22-207">ItemId</span><span class="sxs-lookup"><span data-stu-id="adc22-207">ItemId</span></span>](itemid.md)
    
## <a name="see-also"></a><span data-ttu-id="adc22-208">Confira também</span><span class="sxs-lookup"><span data-stu-id="adc22-208">See also</span></span>



[<span data-ttu-id="adc22-209">Operação UpdateItem (tarefa)</span><span class="sxs-lookup"><span data-stu-id="adc22-209">UpdateItem operation (task)</span></span>](updateitem-operation-task.md)
  
[<span data-ttu-id="adc22-210">Operação UpdateItem (contato)</span><span class="sxs-lookup"><span data-stu-id="adc22-210">UpdateItem operation (contact)</span></span>](updateitem-operation-contact.md)


- [<span data-ttu-id="adc22-211">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="adc22-211">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="adc22-212">Atualizar contatos</span><span class="sxs-lookup"><span data-stu-id="adc22-212">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="adc22-213">Atualizar as tarefas</span><span class="sxs-lookup"><span data-stu-id="adc22-213">Updating Tasks</span></span>](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

