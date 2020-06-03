---
title: Create (issync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Create
api_type:
- schema
ms.assetid: cb5e64a2-66a5-4447-921e-7c13efb8f6bf
description: O elemento Create identifica um único item a ser criado no armazenamento do cliente local.
ms.openlocfilehash: b9c0f28333594a6c17ee9581a227fc4773874fd6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460796"
---
# <a name="create-itemsync"></a><span data-ttu-id="c7c5b-103">Create (issync)</span><span class="sxs-lookup"><span data-stu-id="c7c5b-103">Create (ItemSync)</span></span>

<span data-ttu-id="c7c5b-104">O elemento **Create** identifica um único item a ser criado no armazenamento do cliente local.</span><span class="sxs-lookup"><span data-stu-id="c7c5b-104">The **Create** element identifies a single item to create in the local client store.</span></span> 
  
- [<span data-ttu-id="c7c5b-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="c7c5b-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md) 
- [<span data-ttu-id="c7c5b-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c7c5b-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="c7c5b-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c7c5b-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) 
- [<span data-ttu-id="c7c5b-108">Alterações (itens)</span><span class="sxs-lookup"><span data-stu-id="c7c5b-108">Changes (Items)</span></span>](changes-items.md) 
- [<span data-ttu-id="c7c5b-109">Create (issync)</span><span class="sxs-lookup"><span data-stu-id="c7c5b-109">Create (ItemSync)</span></span>](create-itemsync.md)
  
```xml
<Create>
   <Item/>
</Create>
```

```xml
<Create>
   <Task/> 
</Create>
```

```xml
<Create>
   <MeetingResponse/>
</Create>
```

```xml
<Create>
   <CalendarItem/>
</Create>
```

```xml
<Create>
   <MeetingMessage/>
</Create>
```

```xml
<Create>
   <DistributionList/>
</Create>
```

```xml
<Create>
   <MeetingCancellation/>
</Create>
```

```xml
<Create>
   <MeetingRequest/> 
</Create>
```

```xml
<Create>
   <Message/> 
</Create>
```

```xml
<Create>
   <Contact/> 
</Create>
```

<span data-ttu-id="c7c5b-110">**SyncFolderItemsCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="c7c5b-110">**SyncFolderItemsCreateOrUpdateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c7c5b-111">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="c7c5b-111">Attributes and elements</span></span>

<span data-ttu-id="c7c5b-112">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c7c5b-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c7c5b-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="c7c5b-113">Attributes</span></span>

<span data-ttu-id="c7c5b-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c7c5b-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c7c5b-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c7c5b-115">Child elements</span></span>

|<span data-ttu-id="c7c5b-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c7c5b-116">**Element**</span></span>|<span data-ttu-id="c7c5b-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c7c5b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7c5b-118">Item</span><span class="sxs-lookup"><span data-stu-id="c7c5b-118">Item</span></span>](item.md) <br/> |<span data-ttu-id="c7c5b-119">Representa um item genérico do Exchange a ser criado.</span><span class="sxs-lookup"><span data-stu-id="c7c5b-119">Represents a generic Exchange item to create.</span></span>  <br/> |
|[<span data-ttu-id="c7c5b-120">Mensagem</span><span class="sxs-lookup"><span data-stu-id="c7c5b-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c7c5b-121">Representa uma mensagem de email do Exchange a ser criada.</span><span class="sxs-lookup"><span data-stu-id="c7c5b-121">Represents an Exchange e-mail message to create.</span></span>  <br/> |
|[<span data-ttu-id="c7c5b-122">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="c7c5b-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="c7c5b-123">Representa um item de calendário do Exchange a ser criado.</span><span class="sxs-lookup"><span data-stu-id="c7c5b-123">Represents an Exchange calendar item to create.</span></span>  <br/> |
|[<span data-ttu-id="c7c5b-124">Contato</span><span class="sxs-lookup"><span data-stu-id="c7c5b-124">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="c7c5b-125">Representa um item de contato do Exchange a ser criado.</span><span class="sxs-lookup"><span data-stu-id="c7c5b-125">Represents an Exchange contact item to create.</span></span>  <br/> |
|[<span data-ttu-id="c7c5b-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="c7c5b-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="c7c5b-127">Representa uma lista de distribuição a ser criada.</span><span class="sxs-lookup"><span data-stu-id="c7c5b-127">Represents a distribution list to create.</span></span>  <br/> |
|[<span data-ttu-id="c7c5b-128">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="c7c5b-128">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="c7c5b-129">Representa uma mensagem de reunião a ser criada.</span><span class="sxs-lookup"><span data-stu-id="c7c5b-129">Represents a meeting message to create.</span></span>  <br/> |
|[<span data-ttu-id="c7c5b-130">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="c7c5b-130">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="c7c5b-131">Representa uma solicitação de reunião a ser criada.</span><span class="sxs-lookup"><span data-stu-id="c7c5b-131">Represents a meeting request to create.</span></span>  <br/> |
|[<span data-ttu-id="c7c5b-132">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="c7c5b-132">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="c7c5b-133">Representa uma resposta de reunião a ser criada.</span><span class="sxs-lookup"><span data-stu-id="c7c5b-133">Represents a meeting response to create.</span></span>  <br/> |
|[<span data-ttu-id="c7c5b-134">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="c7c5b-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="c7c5b-135">Representa um cancelamento de reunião a ser criado.</span><span class="sxs-lookup"><span data-stu-id="c7c5b-135">Represents a meeting cancellation to create.</span></span>  <br/> |
|[<span data-ttu-id="c7c5b-136">Tarefa</span><span class="sxs-lookup"><span data-stu-id="c7c5b-136">Task</span></span>](task.md) <br/> |<span data-ttu-id="c7c5b-137">Representa uma tarefa a ser criada.</span><span class="sxs-lookup"><span data-stu-id="c7c5b-137">Represents a task to create.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c7c5b-138">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c7c5b-138">Parent elements</span></span>

|<span data-ttu-id="c7c5b-139">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c7c5b-139">**Element**</span></span>|<span data-ttu-id="c7c5b-140">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c7c5b-140">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7c5b-141">Alterações (itens)</span><span class="sxs-lookup"><span data-stu-id="c7c5b-141">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="c7c5b-142">Contém uma matriz de sequência de tipos de alteração que representam os tipos de diferenças entre os itens no cliente e os itens no servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="c7c5b-142">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c7c5b-143">Comentários</span><span class="sxs-lookup"><span data-stu-id="c7c5b-143">Remarks</span></span>

<span data-ttu-id="c7c5b-144">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="c7c5b-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c7c5b-145">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="c7c5b-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c7c5b-146">Namespace</span><span class="sxs-lookup"><span data-stu-id="c7c5b-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c7c5b-147">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c7c5b-147">Schema name</span></span>  <br/> |<span data-ttu-id="c7c5b-148">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="c7c5b-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="c7c5b-149">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c7c5b-149">Validation file</span></span>  <br/> |<span data-ttu-id="c7c5b-150">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c7c5b-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c7c5b-151">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="c7c5b-151">Can be empty</span></span>  <br/> |<span data-ttu-id="c7c5b-152">False</span><span class="sxs-lookup"><span data-stu-id="c7c5b-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c7c5b-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="c7c5b-153">See also</span></span>

- [<span data-ttu-id="c7c5b-154">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="c7c5b-154">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="c7c5b-155">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c7c5b-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

