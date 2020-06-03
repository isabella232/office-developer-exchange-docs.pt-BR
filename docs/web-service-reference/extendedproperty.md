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
description: O elemento Extended identifica Propriedades de MAPI estendidas em pastas e itens.
ms.openlocfilehash: 99ede097d803d6fbf534cde0e77c08cec054bfa3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530604"
---
# <a name="extendedproperty"></a><span data-ttu-id="f7e92-103">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="f7e92-103">ExtendedProperty</span></span>

<span data-ttu-id="f7e92-104">O elemento **Extended** identifica Propriedades de MAPI estendidas em pastas e itens.</span><span class="sxs-lookup"><span data-stu-id="f7e92-104">The **ExtendedProperty** element identifies extended MAPI properties on folders and items.</span></span> 
  
```xml
<ExtendedProperty>
   <ExtendedFieldURI/>
   <Values/>
</ExtendedProperty>
```

```xml
<ExtendedProperty>
   <ExtendedFieldURI/>
   <Value/>
</ExtendedProperty>
```

<span data-ttu-id="f7e92-105">**ExtendedPropertyType**</span><span class="sxs-lookup"><span data-stu-id="f7e92-105">**ExtendedPropertyType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f7e92-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="f7e92-106">Attributes and elements</span></span>

<span data-ttu-id="f7e92-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="f7e92-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f7e92-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="f7e92-108">Attributes</span></span>

<span data-ttu-id="f7e92-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f7e92-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f7e92-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="f7e92-110">Child elements</span></span>

|<span data-ttu-id="f7e92-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f7e92-111">**Element**</span></span>|<span data-ttu-id="f7e92-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f7e92-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7e92-113">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="f7e92-113">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="f7e92-114">Identifica uma propriedade MAPI estendida a ser obtida, definida ou criada.</span><span class="sxs-lookup"><span data-stu-id="f7e92-114">Identifies an extended MAPI property to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="f7e92-115">Valores</span><span class="sxs-lookup"><span data-stu-id="f7e92-115">Values</span></span>](values.md) <br/> |<span data-ttu-id="f7e92-116">Contém uma coleção de valores para uma propriedade MAPI estendida com vários valores.</span><span class="sxs-lookup"><span data-stu-id="f7e92-116">Contains a collection of values for a multivalued extended MAPI property.</span></span>  <br/> |
|[<span data-ttu-id="f7e92-117">Valor</span><span class="sxs-lookup"><span data-stu-id="f7e92-117">Value</span></span>](value.md) <br/> |<span data-ttu-id="f7e92-118">Contém o valor da propriedade estendida MAPI de valor único.</span><span class="sxs-lookup"><span data-stu-id="f7e92-118">Contains the value of single-valued MAPI extended property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f7e92-119">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="f7e92-119">Parent elements</span></span>

|<span data-ttu-id="f7e92-120">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f7e92-120">**Element**</span></span>|<span data-ttu-id="f7e92-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f7e92-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7e92-122">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="f7e92-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="f7e92-123">Representa um item de calendário do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7e92-123">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="f7e92-124">Contato</span><span class="sxs-lookup"><span data-stu-id="f7e92-124">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="f7e92-125">Representa um item de contato do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7e92-125">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="f7e92-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="f7e92-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="f7e92-127">Representa uma lista de distribuição.</span><span class="sxs-lookup"><span data-stu-id="f7e92-127">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="f7e92-128">Item</span><span class="sxs-lookup"><span data-stu-id="f7e92-128">Item</span></span>](item.md) <br/> |<span data-ttu-id="f7e92-129">Representa um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7e92-129">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f7e92-130">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="f7e92-130">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="f7e92-131">Representa um cancelamento de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7e92-131">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f7e92-132">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="f7e92-132">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="f7e92-133">Representa uma reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7e92-133">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f7e92-134">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="f7e92-134">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="f7e92-135">Representa uma solicitação de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7e92-135">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f7e92-136">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="f7e92-136">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="f7e92-137">Representa uma resposta de reunião no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7e92-137">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f7e92-138">Mensagem</span><span class="sxs-lookup"><span data-stu-id="f7e92-138">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f7e92-139">Representa uma mensagem de email do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7e92-139">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="f7e92-140">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="f7e92-140">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="f7e92-141">Remove um item do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7e92-141">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f7e92-142">Tarefa</span><span class="sxs-lookup"><span data-stu-id="f7e92-142">Task</span></span>](task.md) <br/> |<span data-ttu-id="f7e92-143">Representa uma tarefa no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f7e92-143">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="f7e92-144">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="f7e92-144">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="f7e92-145">Representa uma pasta que contém principalmente itens de calendário.</span><span class="sxs-lookup"><span data-stu-id="f7e92-145">Represents a folder that primarily contains calendar items.</span></span>  <br/> |
|[<span data-ttu-id="f7e92-146">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="f7e92-146">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="f7e92-147">Representa uma pasta contatos em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f7e92-147">Represents a contacts folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f7e92-148">Folder</span><span class="sxs-lookup"><span data-stu-id="f7e92-148">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="f7e92-149">Representa uma pasta para criar, obter, localizar, sincronizar ou atualizar.</span><span class="sxs-lookup"><span data-stu-id="f7e92-149">Represents a folder to create, get, find, synchronize, or update.</span></span>  <br/> |
|[<span data-ttu-id="f7e92-150">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="f7e92-150">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="f7e92-151">Representa uma pasta de pesquisa que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f7e92-151">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f7e92-152">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="f7e92-152">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="f7e92-153">Representa uma pasta tarefas que está contida em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="f7e92-153">Represents a tasks folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f7e92-154">Comentários</span><span class="sxs-lookup"><span data-stu-id="f7e92-154">Remarks</span></span>

<span data-ttu-id="f7e92-155">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="f7e92-155">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f7e92-156">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="f7e92-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f7e92-157">Namespace</span><span class="sxs-lookup"><span data-stu-id="f7e92-157">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f7e92-158">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="f7e92-158">Schema Name</span></span>  <br/> |<span data-ttu-id="f7e92-159">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="f7e92-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="f7e92-160">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="f7e92-160">Validation File</span></span>  <br/> |<span data-ttu-id="f7e92-161">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f7e92-161">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f7e92-162">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="f7e92-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="f7e92-163">False</span><span class="sxs-lookup"><span data-stu-id="f7e92-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f7e92-164">Confira também</span><span class="sxs-lookup"><span data-stu-id="f7e92-164">See also</span></span>

- [<span data-ttu-id="f7e92-165">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f7e92-165">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

