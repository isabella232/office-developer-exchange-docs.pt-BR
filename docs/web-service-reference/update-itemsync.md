---
title: Atualização (issync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Update
api_type:
- schema
ms.assetid: 4e204446-1c80-44f9-b93b-77ce630a01a5
description: O elemento Update identifica um único item a ser atualizado no repositório do cliente local.
ms.openlocfilehash: 12248cbbd5d47a19e36d49fcebe6d4753a2e162f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468884"
---
# <a name="update-itemsync"></a><span data-ttu-id="b2f4c-103">Atualização (issync)</span><span class="sxs-lookup"><span data-stu-id="b2f4c-103">Update (ItemSync)</span></span>

<span data-ttu-id="b2f4c-104">O elemento **Update** identifica um único item a ser atualizado no repositório do cliente local.</span><span class="sxs-lookup"><span data-stu-id="b2f4c-104">The **Update** element identifies a single item to update in the local client store.</span></span> 
  
- [<span data-ttu-id="b2f4c-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="b2f4c-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md) 
- [<span data-ttu-id="b2f4c-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b2f4c-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="b2f4c-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b2f4c-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)  
- [<span data-ttu-id="b2f4c-108">Alterações (itens)</span><span class="sxs-lookup"><span data-stu-id="b2f4c-108">Changes (Items)</span></span>](changes-items.md)  
- [<span data-ttu-id="b2f4c-109">Atualização (issync)</span><span class="sxs-lookup"><span data-stu-id="b2f4c-109">Update (ItemSync)</span></span>](update-itemsync.md)
  
```xml
<Update>
   <Item/>
</Update>
```

```xml
<Update>
   <MeetingRequest/>
</Update>
```

```xml
<Update>
   <MeetingCancellation/>
</Update>
```

```xml
<Update>
   <Task/>
</Update>
```

```xml
<Update>
   <CalendarItem/>
</Update>
```

```xml
<Update>
   <MeetingResponse/>
</Update>
```

```xml
<Update>
   <Message/>
</Update>
```

```xml
<Update>
   <DistributionList/>
</Update>
```

```xml
<Update>
   <MeetingMessage/>
</Update>
```

```xml
<Update>
   <Contact/> 
</Update>
```

<span data-ttu-id="b2f4c-110">**SyncFolderItemsCreateOrUpdateType**</span><span class="sxs-lookup"><span data-stu-id="b2f4c-110">**SyncFolderItemsCreateOrUpdateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b2f4c-111">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="b2f4c-111">Attributes and elements</span></span>

<span data-ttu-id="b2f4c-112">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b2f4c-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b2f4c-113">Atributos</span><span class="sxs-lookup"><span data-stu-id="b2f4c-113">Attributes</span></span>

<span data-ttu-id="b2f4c-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b2f4c-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b2f4c-115">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b2f4c-115">Child elements</span></span>

|<span data-ttu-id="b2f4c-116">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b2f4c-116">**Element**</span></span>|<span data-ttu-id="b2f4c-117">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b2f4c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b2f4c-118">Item</span><span class="sxs-lookup"><span data-stu-id="b2f4c-118">Item</span></span>](item.md) <br/> |<span data-ttu-id="b2f4c-119">Representa um item genérico do Exchange a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="b2f4c-119">Represents a generic Exchange item to update.</span></span>  <br/> |
|[<span data-ttu-id="b2f4c-120">Mensagem</span><span class="sxs-lookup"><span data-stu-id="b2f4c-120">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b2f4c-121">Representa uma mensagem de email do Exchange a ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="b2f4c-121">Represents an Exchange e-mail message to update.</span></span>  <br/> |
|[<span data-ttu-id="b2f4c-122">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="b2f4c-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="b2f4c-123">Representa um item de calendário do Exchange a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="b2f4c-123">Represents an Exchange calendar item to update.</span></span>  <br/> |
|[<span data-ttu-id="b2f4c-124">Contato</span><span class="sxs-lookup"><span data-stu-id="b2f4c-124">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="b2f4c-125">Representa um item de contato do Exchange a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="b2f4c-125">Represents an Exchange contact item to update.</span></span>  <br/> |
|[<span data-ttu-id="b2f4c-126">DistributionList</span><span class="sxs-lookup"><span data-stu-id="b2f4c-126">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="b2f4c-127">Representa uma lista de distribuição a ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="b2f4c-127">Represents a distribution list to update.</span></span>  <br/> |
|[<span data-ttu-id="b2f4c-128">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="b2f4c-128">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="b2f4c-129">Representa uma mensagem de reunião a ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="b2f4c-129">Represents a meeting message to update.</span></span>  <br/> |
|[<span data-ttu-id="b2f4c-130">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="b2f4c-130">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="b2f4c-131">Representa uma solicitação de reunião a ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="b2f4c-131">Represents a meeting request to update.</span></span>  <br/> |
|[<span data-ttu-id="b2f4c-132">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="b2f4c-132">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="b2f4c-133">Representa uma resposta de reunião a ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="b2f4c-133">Represents a meeting response to update.</span></span>  <br/> |
|[<span data-ttu-id="b2f4c-134">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="b2f4c-134">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="b2f4c-135">Representa um cancelamento de reunião a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="b2f4c-135">Represents a meeting cancellation to update.</span></span>  <br/> |
|[<span data-ttu-id="b2f4c-136">Tarefa</span><span class="sxs-lookup"><span data-stu-id="b2f4c-136">Task</span></span>](task.md) <br/> |<span data-ttu-id="b2f4c-137">Representa uma tarefa a ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="b2f4c-137">Represents a task to update.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b2f4c-138">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b2f4c-138">Parent elements</span></span>

|<span data-ttu-id="b2f4c-139">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b2f4c-139">**Element**</span></span>|<span data-ttu-id="b2f4c-140">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b2f4c-140">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b2f4c-141">Alterações (itens)</span><span class="sxs-lookup"><span data-stu-id="b2f4c-141">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="b2f4c-142">Contém uma matriz de sequência de tipos de alteração que representam o tipo de diferença entre os itens no cliente e os itens no servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="b2f4c-142">Contains a sequence array of change types that represent the type of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b2f4c-143">Comentários</span><span class="sxs-lookup"><span data-stu-id="b2f4c-143">Remarks</span></span>

<span data-ttu-id="b2f4c-144">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="b2f4c-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b2f4c-145">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="b2f4c-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b2f4c-146">Namespace</span><span class="sxs-lookup"><span data-stu-id="b2f4c-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b2f4c-147">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b2f4c-147">Schema name</span></span>  <br/> |<span data-ttu-id="b2f4c-148">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b2f4c-148">Types schema</span></span>  <br/> |
|<span data-ttu-id="b2f4c-149">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b2f4c-149">Validation file</span></span>  <br/> |<span data-ttu-id="b2f4c-150">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b2f4c-150">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b2f4c-151">Pode estar vazio</span><span class="sxs-lookup"><span data-stu-id="b2f4c-151">Can be empty</span></span>  <br/> |<span data-ttu-id="b2f4c-152">False</span><span class="sxs-lookup"><span data-stu-id="b2f4c-152">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b2f4c-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="b2f4c-153">See also</span></span>

- [<span data-ttu-id="b2f4c-154">Operação SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="b2f4c-154">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="b2f4c-155">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b2f4c-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

