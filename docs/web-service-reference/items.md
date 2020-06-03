---
title: Itens
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Items
api_type:
- schema
ms.assetid: 0811a73e-bf1f-4889-9219-73902dd47639
description: O elemento items contém uma matriz de itens.
ms.openlocfilehash: 489e34ad0e4bcc2520febb3c213db970fa496051
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458128"
---
# <a name="items"></a><span data-ttu-id="77505-103">Itens</span><span class="sxs-lookup"><span data-stu-id="77505-103">Items</span></span>

<span data-ttu-id="77505-104">O elemento **Items** contém uma matriz de itens.</span><span class="sxs-lookup"><span data-stu-id="77505-104">The **Items** element contains an array of items.</span></span> 
  
```xml
<Items>
   <Item/>
   <Message/>
   <CalendarItem/>
   <Contact/>
   <DistributionList/>
   <MeetingMessage/>
   <MeetingRequest/>
   <MeetingResponse/>
   <MeetingCancellation/>
   <Task/>
   <PostItem/>
</Items>
```

 <span data-ttu-id="77505-105">**ArrayOfRealItemsType**</span><span class="sxs-lookup"><span data-stu-id="77505-105">**ArrayOfRealItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="77505-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="77505-106">Attributes and elements</span></span>

<span data-ttu-id="77505-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="77505-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="77505-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="77505-108">Attributes</span></span>

<span data-ttu-id="77505-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="77505-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="77505-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="77505-110">Child elements</span></span>

|<span data-ttu-id="77505-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="77505-111">**Element**</span></span>|<span data-ttu-id="77505-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="77505-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77505-113">Item</span><span class="sxs-lookup"><span data-stu-id="77505-113">Item</span></span>](item.md) <br/> |<span data-ttu-id="77505-114">Representa um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="77505-114">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="77505-115">Mensagem</span><span class="sxs-lookup"><span data-stu-id="77505-115">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="77505-116">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="77505-116">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="77505-117">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="77505-117">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="77505-118">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="77505-118">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="77505-119">Contato</span><span class="sxs-lookup"><span data-stu-id="77505-119">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="77505-120">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="77505-120">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="77505-121">DistributionList</span><span class="sxs-lookup"><span data-stu-id="77505-121">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="77505-122">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="77505-122">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="77505-123">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="77505-123">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="77505-124">Representa uma mensagem de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="77505-124">Represents a meeting message in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="77505-125">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="77505-125">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="77505-126">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="77505-126">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="77505-127">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="77505-127">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="77505-128">Representa uma resposta de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="77505-128">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="77505-129">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="77505-129">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="77505-130">Representa um cancelamento de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="77505-130">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="77505-131">Tarefa</span><span class="sxs-lookup"><span data-stu-id="77505-131">Task</span></span>](task.md) <br/> |<span data-ttu-id="77505-132">Representa uma tarefa no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="77505-132">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="77505-133">Item de postagem</span><span class="sxs-lookup"><span data-stu-id="77505-133">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="77505-134">Representa um item de postagem no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="77505-134">Represents a post item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="77505-135">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="77505-135">Parent elements</span></span>

|<span data-ttu-id="77505-136">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="77505-136">**Element**</span></span>|<span data-ttu-id="77505-137">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="77505-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="77505-138">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="77505-138">CopyItemResponseMessage</span></span>](copyitemresponsemessage.md) <br/> |<span data-ttu-id="77505-139">Contém o status e o resultado de uma solicitação de [operação CopyItem](copyitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="77505-139">Contains the status and result of a [CopyItem operation](copyitem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="77505-140">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="77505-140">CreateItemResponseMessage</span></span>](createitemresponsemessage.md) <br/> |<span data-ttu-id="77505-141">Contém o status e o resultado de uma solicitação de [operação CreateItem](createitem-operation.md) única.</span><span class="sxs-lookup"><span data-stu-id="77505-141">Contains the status and result of a single [CreateItem operation](createitem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="77505-142">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="77505-142">GetItemResponseMessage</span></span>](getitemresponsemessage.md) <br/> |<span data-ttu-id="77505-143">Contém o status e o resultado de uma solicitação de [operação GetItem](getitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="77505-143">Contains the status and result of a [GetItem operation](getitem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="77505-144">GroupedItems</span><span class="sxs-lookup"><span data-stu-id="77505-144">GroupedItems</span></span>](groupeditems.md) <br/> |<span data-ttu-id="77505-145">Representa uma coleção de itens que são o resultado de uma chamada de [operação FindItem](finditem-operation.md) agrupada.</span><span class="sxs-lookup"><span data-stu-id="77505-145">Represents a collection of items that are the result of a grouped [FindItem operation](finditem-operation.md) call.</span></span>  <br/> |
|[<span data-ttu-id="77505-146">MoveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="77505-146">MoveItemResponseMessage</span></span>](moveitemresponsemessage.md) <br/> |<span data-ttu-id="77505-147">Contém o status e o resultado de uma solicitação de [operação MoveItem](moveitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="77505-147">Contains the status and result of a [MoveItem operation](moveitem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="77505-148">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="77505-148">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md) <br/> |<span data-ttu-id="77505-149">Contém os resultados de uma pesquisa de uma única pasta raiz durante uma [operação FindItem](finditem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="77505-149">Contains the results of a search of a single root folder during a [FindItem operation](finditem-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="77505-150">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="77505-150">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md) <br/> |<span data-ttu-id="77505-151">Contém o status e o resultado de uma solicitação de [operação UpdateItem](updateitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="77505-151">Contains the status and result of an [UpdateItem operation](updateitem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="77505-152">Comentários</span><span class="sxs-lookup"><span data-stu-id="77505-152">Remarks</span></span>

<span data-ttu-id="77505-153">Para obter informações sobre o conjunto de itens em uma solicitação de [operação CreateItem](createitem-operation.md) , consulte [itens (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md).</span><span class="sxs-lookup"><span data-stu-id="77505-153">For information about the set of items in a [CreateItem operation](createitem-operation.md) request, see [Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md).</span></span>
  
<span data-ttu-id="77505-154">Os elementos da [mensagem](message-ex15websvcsotherref.md) representam mensagens de email e todos os outros itens que não são digitados com rigidez pelo esquema dos serviços Web do Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="77505-154">[Message](message-ex15websvcsotherref.md) elements represent e-mail messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="77505-155">Itens como IPM. O compartilhamento e o IPM. InfoPath são retornados como elementos de **mensagem** .</span><span class="sxs-lookup"><span data-stu-id="77505-155">Items such as IPM.Sharing and IPM.InfoPath are returned as **Message** elements.</span></span> <span data-ttu-id="77505-156">As versões do Exchange a partir do Exchange Server 2010 não retornam o elemento de [Item](item.md) base em respostas.</span><span class="sxs-lookup"><span data-stu-id="77505-156">Versions of Exchange starting with Exchange Server 2010 do not return the base [Item](item.md) element in responses.</span></span> 
  
<span data-ttu-id="77505-157">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Exchange que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="77505-157">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="77505-158">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="77505-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="77505-159">Namespace</span><span class="sxs-lookup"><span data-stu-id="77505-159">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="77505-160">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="77505-160">Schema Name</span></span>  <br/> |<span data-ttu-id="77505-161">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="77505-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="77505-162">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="77505-162">Validation File</span></span>  <br/> |<span data-ttu-id="77505-163">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="77505-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="77505-164">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="77505-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="77505-165">False</span><span class="sxs-lookup"><span data-stu-id="77505-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="77505-166">Confira também</span><span class="sxs-lookup"><span data-stu-id="77505-166">See also</span></span>



[<span data-ttu-id="77505-167">Referência do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="77505-167">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
  
- [<span data-ttu-id="77505-168">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="77505-168">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

