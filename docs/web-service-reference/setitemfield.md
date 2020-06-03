---
title: Setitemfield
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetItemField
api_type:
- schema
ms.assetid: 85284fcb-bd1e-4fda-9dab-cb4cd637cd5b
description: O elemento setitemfield representa uma atualização para uma única propriedade de um item em uma operação UpdateItem.
ms.openlocfilehash: b4606eb7d94b9d0c4c5bcd5a2b56d73a4d4270cb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467421"
---
# <a name="setitemfield"></a><span data-ttu-id="9688b-103">Setitemfield</span><span class="sxs-lookup"><span data-stu-id="9688b-103">SetItemField</span></span>

<span data-ttu-id="9688b-104">O elemento **Setitemfield** representa uma atualização para uma única propriedade de um item em uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="9688b-104">The **SetItemField** element represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>
  
```xml
<SetItemField>
   <FieldURI/>
   <Item/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <Item/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <MeetingRequest/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <MeetingResponse/>
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <Contact/>
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <DistributionList/>
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <MeetingResponse/>
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <MeetingResponse/> 
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <MeetingRequest/> 
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <Contact/>
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <Message/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <CalendarItem/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <Task/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <Message/> 
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <MeetingCancellation/> 
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <Task/> 
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <MeetingRequest/>  
</SetItemField>
```

```xml
<SetItemField>
    <FieldURI/> 
    <CalendarItem/>
</SetItemField>
```

```xml
<SetItemField>
    <IndexedFieldURI/> 
    <Item/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <MeetingCancellation/>
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <DistributionList/> 
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <MeetingCancellation/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <MeetingMessage/>
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <Task/> 
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <CalendarItem/>
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <MeetingMessage/>
</SetItemField>
```

```xml
<SetItemField>
   <IndexedFieldURI/> 
   <MeetingMessage/>
</SetItemField>
```

```xml
<SetItemField>
   <FieldURI/> 
   <Message/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <DistributionList/>
</SetItemField>
```

```xml
<SetItemField>
   <ExtendedFieldURI/> 
   <Contact/> 
</SetItemField>
```


<span data-ttu-id="9688b-105">**SetItemFieldType**</span><span class="sxs-lookup"><span data-stu-id="9688b-105">**SetItemFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9688b-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="9688b-106">Attributes and elements</span></span>

<span data-ttu-id="9688b-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="9688b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9688b-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="9688b-108">Attributes</span></span>

<span data-ttu-id="9688b-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9688b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9688b-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="9688b-110">Child elements</span></span>

|<span data-ttu-id="9688b-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9688b-111">**Element**</span></span>|<span data-ttu-id="9688b-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9688b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9688b-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="9688b-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="9688b-114">Identifica as propriedades com frequência referenciadas por URI.</span><span class="sxs-lookup"><span data-stu-id="9688b-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="9688b-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="9688b-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="9688b-116">Identifica membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="9688b-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="9688b-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="9688b-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="9688b-118">Identifica as propriedades de MAPI estendidas a serem definidas.</span><span class="sxs-lookup"><span data-stu-id="9688b-118">Identifies extended MAPI properties to set.</span></span>  <br/> |
|[<span data-ttu-id="9688b-119">Item</span><span class="sxs-lookup"><span data-stu-id="9688b-119">Item</span></span>](item.md) <br/> |<span data-ttu-id="9688b-120">Representa um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9688b-120">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="9688b-121">Mensagem</span><span class="sxs-lookup"><span data-stu-id="9688b-121">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9688b-122">Representa uma mensagem de email do Exchange a ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="9688b-122">Represents an Exchange e-mail message to update.</span></span>  <br/> |
|[<span data-ttu-id="9688b-123">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="9688b-123">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="9688b-124">Representa um item de calendário do Exchange a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="9688b-124">Represents an Exchange calendar item to update.</span></span>  <br/> |
|[<span data-ttu-id="9688b-125">Contato</span><span class="sxs-lookup"><span data-stu-id="9688b-125">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="9688b-126">Representa um item de contato do Exchange a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="9688b-126">Represents an Exchange contact item to update.</span></span>  <br/> |
|[<span data-ttu-id="9688b-127">DistributionList</span><span class="sxs-lookup"><span data-stu-id="9688b-127">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="9688b-128">Representa uma lista de distribuição a ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="9688b-128">Represents a distribution list to update.</span></span>  <br/> |
|[<span data-ttu-id="9688b-129">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="9688b-129">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="9688b-130">Representa uma mensagem de reunião a ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="9688b-130">Represents a meeting message to update.</span></span>  <br/> |
|[<span data-ttu-id="9688b-131">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="9688b-131">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="9688b-132">Representa uma solicitação de reunião a ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="9688b-132">Represents a meeting request to update.</span></span>  <br/> |
|[<span data-ttu-id="9688b-133">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="9688b-133">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="9688b-134">Representa uma resposta de reunião a ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="9688b-134">Represents a meeting response to update.</span></span>  <br/> |
|[<span data-ttu-id="9688b-135">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="9688b-135">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="9688b-136">Representa um cancelamento de reunião a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="9688b-136">Represents a meeting cancellation to update.</span></span>  <br/> |
|[<span data-ttu-id="9688b-137">Tarefa</span><span class="sxs-lookup"><span data-stu-id="9688b-137">Task</span></span>](task.md) <br/> |<span data-ttu-id="9688b-138">Representa uma tarefa a ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="9688b-138">Represents a task to update.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9688b-139">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="9688b-139">Parent elements</span></span>

|<span data-ttu-id="9688b-140">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="9688b-140">**Element**</span></span>|<span data-ttu-id="9688b-141">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="9688b-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9688b-142">Atualizações (item)</span><span class="sxs-lookup"><span data-stu-id="9688b-142">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="9688b-143">Contém um conjunto de elementos que definem Append, set e Delete alterações nas propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="9688b-143">Contains a set of elements that define append, set, and delete changes to item properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9688b-144">Comentários</span><span class="sxs-lookup"><span data-stu-id="9688b-144">Remarks</span></span>

<span data-ttu-id="9688b-145">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2007 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="9688b-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9688b-146">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="9688b-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9688b-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="9688b-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9688b-148">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="9688b-148">Schema Name</span></span>  <br/> |<span data-ttu-id="9688b-149">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="9688b-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="9688b-150">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="9688b-150">Validation File</span></span>  <br/> |<span data-ttu-id="9688b-151">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9688b-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9688b-152">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="9688b-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="9688b-153">False</span><span class="sxs-lookup"><span data-stu-id="9688b-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9688b-154">Confira também</span><span class="sxs-lookup"><span data-stu-id="9688b-154">See also</span></span>

- [<span data-ttu-id="9688b-155">Operação UpdateItem</span><span class="sxs-lookup"><span data-stu-id="9688b-155">UpdateItem operation</span></span>](updateitem-operation.md)

