---
title: SetItemField
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
description: O elemento SetItemField representa uma atualização para uma única propriedade de um item em uma operação UpdateItem.
ms.openlocfilehash: 012e6ae21af653b4bf12588e5a97334a62884059
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825439"
---
# <a name="setitemfield"></a><span data-ttu-id="b23a7-103">SetItemField</span><span class="sxs-lookup"><span data-stu-id="b23a7-103">SetItemField</span></span>

<span data-ttu-id="b23a7-104">O elemento **SetItemField** representa uma atualização para uma única propriedade de um item em uma [operação UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="b23a7-104">The **SetItemField** element represents an update to a single property of an item in an [UpdateItem operation](updateitem-operation.md).</span></span>
  
```xml
<SetItemField>
   <FieldURI/>
   <Item/>
</SetItemField>
```

 <span data-ttu-id="b23a7-105">**SetItemFieldType**</span><span class="sxs-lookup"><span data-stu-id="b23a7-105">**SetItemFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b23a7-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="b23a7-106">Attributes and elements</span></span>

<span data-ttu-id="b23a7-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="b23a7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b23a7-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="b23a7-108">Attributes</span></span>

<span data-ttu-id="b23a7-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="b23a7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b23a7-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="b23a7-110">Child elements</span></span>

|<span data-ttu-id="b23a7-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b23a7-111">**Element**</span></span>|<span data-ttu-id="b23a7-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b23a7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b23a7-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="b23a7-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="b23a7-114">Identifica as propriedades frequentemente referenciadas pelo URI.</span><span class="sxs-lookup"><span data-stu-id="b23a7-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="b23a7-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="b23a7-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="b23a7-116">Identifica a membros individuais de um dicionário.</span><span class="sxs-lookup"><span data-stu-id="b23a7-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="b23a7-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="b23a7-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="b23a7-118">Identifica as propriedades estendidas de MAPI para definir.</span><span class="sxs-lookup"><span data-stu-id="b23a7-118">Identifies extended MAPI properties to set.</span></span>  <br/> |
|[<span data-ttu-id="b23a7-119">1.1</span><span class="sxs-lookup"><span data-stu-id="b23a7-119">Item</span></span>](item.md) <br/> |<span data-ttu-id="b23a7-120">Representa um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b23a7-120">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="b23a7-121">Mensagem</span><span class="sxs-lookup"><span data-stu-id="b23a7-121">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b23a7-122">Representa uma mensagem de email do Exchange para atualizar.</span><span class="sxs-lookup"><span data-stu-id="b23a7-122">Represents an Exchange e-mail message to update.</span></span>  <br/> |
|[<span data-ttu-id="b23a7-123">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="b23a7-123">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="b23a7-124">Representa um item de calendário do Exchange para atualizar.</span><span class="sxs-lookup"><span data-stu-id="b23a7-124">Represents an Exchange calendar item to update.</span></span>  <br/> |
|[<span data-ttu-id="b23a7-125">Contato</span><span class="sxs-lookup"><span data-stu-id="b23a7-125">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="b23a7-126">Representa um item de contato do Exchange para atualizar.</span><span class="sxs-lookup"><span data-stu-id="b23a7-126">Represents an Exchange contact item to update.</span></span>  <br/> |
|[<span data-ttu-id="b23a7-127">DistributionList</span><span class="sxs-lookup"><span data-stu-id="b23a7-127">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="b23a7-128">Representa uma lista de distribuição a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="b23a7-128">Represents a distribution list to update.</span></span>  <br/> |
|[<span data-ttu-id="b23a7-129">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="b23a7-129">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="b23a7-130">Representa uma mensagem de reunião a atualização.</span><span class="sxs-lookup"><span data-stu-id="b23a7-130">Represents a meeting message to update.</span></span>  <br/> |
|[<span data-ttu-id="b23a7-131">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="b23a7-131">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="b23a7-132">Representa uma solicitação de reunião para atualizar.</span><span class="sxs-lookup"><span data-stu-id="b23a7-132">Represents a meeting request to update.</span></span>  <br/> |
|[<span data-ttu-id="b23a7-133">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="b23a7-133">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="b23a7-134">Representa uma resposta de reunião para atualizar.</span><span class="sxs-lookup"><span data-stu-id="b23a7-134">Represents a meeting response to update.</span></span>  <br/> |
|[<span data-ttu-id="b23a7-135">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="b23a7-135">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="b23a7-136">Representa o cancelamento da reunião para atualizar.</span><span class="sxs-lookup"><span data-stu-id="b23a7-136">Represents a meeting cancellation to update.</span></span>  <br/> |
|[<span data-ttu-id="b23a7-137">Task</span><span class="sxs-lookup"><span data-stu-id="b23a7-137">Task</span></span>](task.md) <br/> |<span data-ttu-id="b23a7-138">Representa uma tarefa a ser atualizado.</span><span class="sxs-lookup"><span data-stu-id="b23a7-138">Represents a task to update.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b23a7-139">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="b23a7-139">Parent elements</span></span>

|<span data-ttu-id="b23a7-140">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="b23a7-140">**Element**</span></span>|<span data-ttu-id="b23a7-141">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="b23a7-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b23a7-142">Atualizações (Item)</span><span class="sxs-lookup"><span data-stu-id="b23a7-142">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="b23a7-143">Contém um conjunto de elementos que definem append, definir e excluir as alterações nas propriedades do item.</span><span class="sxs-lookup"><span data-stu-id="b23a7-143">Contains a set of elements that define append, set, and delete changes to item properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b23a7-144">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="b23a7-144">Remarks</span></span>

<span data-ttu-id="b23a7-145">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2007 que possui a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="b23a7-145">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b23a7-146">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="b23a7-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b23a7-147">Namespace</span><span class="sxs-lookup"><span data-stu-id="b23a7-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b23a7-148">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="b23a7-148">Schema Name</span></span>  <br/> |<span data-ttu-id="b23a7-149">Esquema de tipos</span><span class="sxs-lookup"><span data-stu-id="b23a7-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="b23a7-150">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="b23a7-150">Validation File</span></span>  <br/> |<span data-ttu-id="b23a7-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b23a7-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b23a7-152">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="b23a7-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="b23a7-153">False</span><span class="sxs-lookup"><span data-stu-id="b23a7-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b23a7-154">Ver também</span><span class="sxs-lookup"><span data-stu-id="b23a7-154">See also</span></span>



[<span data-ttu-id="b23a7-155">Operação UpdateItem</span><span class="sxs-lookup"><span data-stu-id="b23a7-155">UpdateItem operation</span></span>](updateitem-operation.md)

