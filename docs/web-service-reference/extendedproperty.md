---
title: ExtendedProperty
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExtendedProperty
api_type:
- schema
ms.assetid: f9701409-b620-4afe-b9ee-4c1e95507af7
description: O elemento ExtendedProperty identifica as propriedades estendidas de MAPI em pastas e itens.
ms.openlocfilehash: 6a0aecc732ef634c2258127fca89b19461e25762
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752177"
---
# <a name="extendedproperty"></a><span data-ttu-id="40d6a-103">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="40d6a-103">ExtendedProperty</span></span>

<span data-ttu-id="40d6a-104">O elemento **ExtendedProperty** identifica as propriedades estendidas de MAPI em pastas e itens.</span><span class="sxs-lookup"><span data-stu-id="40d6a-104">The **ExtendedProperty** element identifies extended MAPI properties on folders and items.</span></span> 
  
```xml
<ExtendedProperty>
   <ExtendedFieldURI/>
   <Values/>
</ExtendedProperty>
```

 <span data-ttu-id="40d6a-105">**ExtendedPropertyType**</span><span class="sxs-lookup"><span data-stu-id="40d6a-105">**ExtendedPropertyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="40d6a-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="40d6a-106">Attributes and elements</span></span>

<span data-ttu-id="40d6a-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="40d6a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="40d6a-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="40d6a-108">Attributes</span></span>

<span data-ttu-id="40d6a-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="40d6a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="40d6a-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="40d6a-110">Child elements</span></span>

|<span data-ttu-id="40d6a-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="40d6a-111">**Element**</span></span>|<span data-ttu-id="40d6a-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="40d6a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40d6a-113">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="40d6a-113">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="40d6a-114">Identifica uma propriedade MAPI estendida para obter, definir ou criar.</span><span class="sxs-lookup"><span data-stu-id="40d6a-114">Identifies an extended MAPI property to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="40d6a-115">Values</span><span class="sxs-lookup"><span data-stu-id="40d6a-115">Values</span></span>](values.md) <br/> |<span data-ttu-id="40d6a-116">Contém uma coleção de valores de uma propriedade MAPI estendida multivalorado.</span><span class="sxs-lookup"><span data-stu-id="40d6a-116">Contains a collection of values for a multivalued extended MAPI property.</span></span>  <br/> |
|[<span data-ttu-id="40d6a-117">Valor</span><span class="sxs-lookup"><span data-stu-id="40d6a-117">Value</span></span>](value.md) <br/> |<span data-ttu-id="40d6a-118">Contém o valor da propriedade estendida de MAPI valor único.</span><span class="sxs-lookup"><span data-stu-id="40d6a-118">Contains the value of single-valued MAPI extended property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="40d6a-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="40d6a-119">Parent elements</span></span>

|<span data-ttu-id="40d6a-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="40d6a-120">**Element**</span></span>|<span data-ttu-id="40d6a-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="40d6a-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="40d6a-122">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="40d6a-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="40d6a-123">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="40d6a-123">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="40d6a-124">Contato</span><span class="sxs-lookup"><span data-stu-id="40d6a-124">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="40d6a-125">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="40d6a-125">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="40d6a-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="40d6a-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="40d6a-127">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="40d6a-127">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="40d6a-128">1.1</span><span class="sxs-lookup"><span data-stu-id="40d6a-128">Item</span></span>](item.md) <br/> |<span data-ttu-id="40d6a-129">Representa um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="40d6a-129">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="40d6a-130">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="40d6a-130">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="40d6a-131">Representa o cancelamento da reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="40d6a-131">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="40d6a-132">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="40d6a-132">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="40d6a-133">Representa uma reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="40d6a-133">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="40d6a-134">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="40d6a-134">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="40d6a-135">Representa uma solicitação de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="40d6a-135">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="40d6a-136">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="40d6a-136">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="40d6a-137">Representa uma resposta de reunião no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="40d6a-137">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="40d6a-138">Mensagem</span><span class="sxs-lookup"><span data-stu-id="40d6a-138">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="40d6a-139">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="40d6a-139">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="40d6a-140">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="40d6a-140">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="40d6a-141">Remove um item de armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="40d6a-141">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="40d6a-142">Task</span><span class="sxs-lookup"><span data-stu-id="40d6a-142">Task</span></span>](task.md) <br/> |<span data-ttu-id="40d6a-143">Representa uma tarefa no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="40d6a-143">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="40d6a-144">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="40d6a-144">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="40d6a-145">Representa uma pasta que contém principalmente itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="40d6a-145">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="40d6a-146">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="40d6a-146">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="40d6a-147">Representa uma pasta de contatos em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="40d6a-147">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="40d6a-148">Folder</span><span class="sxs-lookup"><span data-stu-id="40d6a-148">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="40d6a-149">Representa uma pasta para criar, obter, encontre, sincronizar ou atualizar.</span><span class="sxs-lookup"><span data-stu-id="40d6a-149">Represents a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="40d6a-150">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="40d6a-150">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="40d6a-151">Representa uma pasta de pesquisa que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="40d6a-151">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="40d6a-152">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="40d6a-152">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="40d6a-153">Representa uma pasta de tarefas que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="40d6a-153">Represents a tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="40d6a-154">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="40d6a-154">Remarks</span></span>

<span data-ttu-id="40d6a-155">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="40d6a-155">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="40d6a-156">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="40d6a-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="40d6a-157">Namespace</span><span class="sxs-lookup"><span data-stu-id="40d6a-157">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="40d6a-158">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="40d6a-158">Schema Name</span></span>  <br/> |<span data-ttu-id="40d6a-159">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="40d6a-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="40d6a-160">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="40d6a-160">Validation File</span></span>  <br/> |<span data-ttu-id="40d6a-161">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="40d6a-161">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="40d6a-162">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="40d6a-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="40d6a-163">False</span><span class="sxs-lookup"><span data-stu-id="40d6a-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="40d6a-164">Ver também</span><span class="sxs-lookup"><span data-stu-id="40d6a-164">See also</span></span>



- [<span data-ttu-id="40d6a-165">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="40d6a-165">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

