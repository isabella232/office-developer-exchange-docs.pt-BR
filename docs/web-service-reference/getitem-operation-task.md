---
title: Operação GetItem (tarefa)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: 8265dd06-1752-4470-8074-5f0e3e970f52
description: A operação GetItem é usada para obter as tarefas do Exchange store.
ms.openlocfilehash: 412710f32ed8702e1a28a596833c3a7e47e3ed76
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752550"
---
# <a name="getitem-operation-task"></a><span data-ttu-id="e46b6-103">Operação GetItem (tarefa)</span><span class="sxs-lookup"><span data-stu-id="e46b6-103">GetItem operation (task)</span></span>

<span data-ttu-id="e46b6-104">A operação GetItem é usada para obter as tarefas do Exchange store.</span><span class="sxs-lookup"><span data-stu-id="e46b6-104">The GetItem operation is used to get tasks from the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e46b6-105">Comentários</span><span class="sxs-lookup"><span data-stu-id="e46b6-105">Remarks</span></span>

<span data-ttu-id="e46b6-106">O formato da solicitação GetItem para tarefas é igual ao GetItem para qualquer outro tipo de item.</span><span class="sxs-lookup"><span data-stu-id="e46b6-106">The format of the GetItem request for tasks is the same as GetItem for any other item type.</span></span> <span data-ttu-id="e46b6-107">A única diferença é que em que as propriedades adicionais podem ser solicitadas dentro da forma de resposta.</span><span class="sxs-lookup"><span data-stu-id="e46b6-107">The only difference is in which additional properties can be requested within the response shape.</span></span> <span data-ttu-id="e46b6-108">Essas propriedades adicionais devem ser propriedades relacionadas a tarefa ou propriedades estendidas.</span><span class="sxs-lookup"><span data-stu-id="e46b6-108">Such additional properties must either be task-related properties or extended properties.</span></span>
  
## <a name="task-getitem-request-example"></a><span data-ttu-id="e46b6-109">Exemplo de solicitação de GetItem de tarefa</span><span class="sxs-lookup"><span data-stu-id="e46b6-109">Task GetItem request example</span></span>

### <a name="description"></a><span data-ttu-id="e46b6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e46b6-110">Description</span></span>

<span data-ttu-id="e46b6-111">O exemplo a seguir de uma solicitação de GetItem mostra como obter um item de tarefa.</span><span class="sxs-lookup"><span data-stu-id="e46b6-111">The following example of a GetItem request shows how to get a task item.</span></span>
  
### <a name="code"></a><span data-ttu-id="e46b6-112">Código</span><span class="sxs-lookup"><span data-stu-id="e46b6-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAtAEFkb..."/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="e46b6-113">Comments</span><span class="sxs-lookup"><span data-stu-id="e46b6-113">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="e46b6-114">O identificador do item e alterar chave foram diminuídas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e46b6-114">The item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="e46b6-115">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e46b6-115">Request elements</span></span>

<span data-ttu-id="e46b6-116">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="e46b6-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="e46b6-117">GetItem</span><span class="sxs-lookup"><span data-stu-id="e46b6-117">GetItem</span></span>](getitem.md)
    
- [<span data-ttu-id="e46b6-118">ItemShape</span><span class="sxs-lookup"><span data-stu-id="e46b6-118">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="e46b6-119">BaseShape</span><span class="sxs-lookup"><span data-stu-id="e46b6-119">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="e46b6-120">ItemIds</span><span class="sxs-lookup"><span data-stu-id="e46b6-120">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="e46b6-121">ItemId</span><span class="sxs-lookup"><span data-stu-id="e46b6-121">ItemId</span></span>](itemid.md)
    
## <a name="task-getitem-response-example"></a><span data-ttu-id="e46b6-122">Exemplo de resposta GetItem da tarefa</span><span class="sxs-lookup"><span data-stu-id="e46b6-122">Task GetItem response example</span></span>

### <a name="description"></a><span data-ttu-id="e46b6-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e46b6-123">Description</span></span>

<span data-ttu-id="e46b6-124">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de GetItem.</span><span class="sxs-lookup"><span data-stu-id="e46b6-124">The following example shows a successful response to a GetItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="e46b6-125">Código</span><span class="sxs-lookup"><span data-stu-id="e46b6-125">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Task>
              <t:ItemId Id="AAAtAEA=" ChangeKey="EwAAAB"/>
              <t:ParentFolderId Id="AAAtAEFkbWl=" ChangeKey="AQAAAA=="/>
              <t:ItemClass>IPM.Task</t:ItemClass>
              <t:Subject>Buy new shoes</t:Subject>
              <t:Sensitivity>Normal</t:Sensitivity>
              <t:Body BodyType="Text"/>
              <t:DateTimeReceived>2006-09-15T15:23:08Z</t:DateTimeReceived>
              <t:Size>153</t:Size>
              <t:Importance>Normal</t:Importance>
              <t:IsSubmitted>false</t:IsSubmitted>
              <t:IsDraft>true</t:IsDraft>
              <t:IsFromMe>false</t:IsFromMe>
              <t:IsResend>false</t:IsResend>
              <t:IsUnmodified>false</t:IsUnmodified>
              <t:DateTimeSent>2006-09-15T15:23:08Z</t:DateTimeSent>
              <t:DateTimeCreated>2006-09-15T15:23:08Z</t:DateTimeCreated>
              <t:HasAttachments>false</t:HasAttachments>
              <t:Culture>en-US</t:Culture>
              <t:ChangeCount>1</t:ChangeCount>
              <t:IsComplete>false</t:IsComplete>
              <t:IsRecurring>false</t:IsRecurring>
              <t:PercentComplete>0</t:PercentComplete>
              <t:Status>NotStarted</t:Status>
              <t:StatusDescription>Not Started</t:StatusDescription>
            </t:Task>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="e46b6-126">Comments</span><span class="sxs-lookup"><span data-stu-id="e46b6-126">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="e46b6-127">Os identificadores de item e pasta e chaves de alteração tem sido reduzidas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e46b6-127">The item and folder identifiers and change keys have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="e46b6-128">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="e46b6-128">Successful response elements</span></span>

<span data-ttu-id="e46b6-129">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="e46b6-129">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="e46b6-130">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e46b6-130">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="e46b6-131">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="e46b6-131">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="e46b6-132">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e46b6-132">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e46b6-133">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e46b6-133">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="e46b6-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e46b6-134">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e46b6-135">Items</span><span class="sxs-lookup"><span data-stu-id="e46b6-135">Items</span></span>](items.md)
    
- [<span data-ttu-id="e46b6-136">Task</span><span class="sxs-lookup"><span data-stu-id="e46b6-136">Task</span></span>](task.md)
    
- [<span data-ttu-id="e46b6-137">ItemId</span><span class="sxs-lookup"><span data-stu-id="e46b6-137">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="e46b6-138">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="e46b6-138">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="e46b6-139">ItemClass</span><span class="sxs-lookup"><span data-stu-id="e46b6-139">ItemClass</span></span>](itemclass.md)
    
- [<span data-ttu-id="e46b6-140">Assunto</span><span class="sxs-lookup"><span data-stu-id="e46b6-140">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="e46b6-141">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="e46b6-141">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="e46b6-142">Corpo</span><span class="sxs-lookup"><span data-stu-id="e46b6-142">Body</span></span>](body.md)
    
- [<span data-ttu-id="e46b6-143">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="e46b6-143">DateTimeReceived</span></span>](datetimereceived.md)
    
- [<span data-ttu-id="e46b6-144">Size</span><span class="sxs-lookup"><span data-stu-id="e46b6-144">Size</span></span>](size.md)
    
- [<span data-ttu-id="e46b6-145">Importância</span><span class="sxs-lookup"><span data-stu-id="e46b6-145">Importance</span></span>](importance.md)
    
- [<span data-ttu-id="e46b6-146">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="e46b6-146">IsSubmitted</span></span>](issubmitted.md)
    
- [<span data-ttu-id="e46b6-147">IsDraft</span><span class="sxs-lookup"><span data-stu-id="e46b6-147">IsDraft</span></span>](isdraft.md)
    
- [<span data-ttu-id="e46b6-148">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="e46b6-148">IsFromMe</span></span>](isfromme.md)
    
- [<span data-ttu-id="e46b6-149">IsResend</span><span class="sxs-lookup"><span data-stu-id="e46b6-149">IsResend</span></span>](isresend.md)
    
- [<span data-ttu-id="e46b6-150">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="e46b6-150">IsUnmodified</span></span>](isunmodified.md)
    
- [<span data-ttu-id="e46b6-151">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="e46b6-151">DateTimeSent</span></span>](datetimesent.md)
    
- [<span data-ttu-id="e46b6-152">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="e46b6-152">DateTimeCreated</span></span>](datetimecreated.md)
    
- [<span data-ttu-id="e46b6-153">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="e46b6-153">HasAttachments</span></span>](hasattachments.md)
    
- [<span data-ttu-id="e46b6-154">Cultura</span><span class="sxs-lookup"><span data-stu-id="e46b6-154">Culture</span></span>](culture.md)
    
- [<span data-ttu-id="e46b6-155">ChangeCount</span><span class="sxs-lookup"><span data-stu-id="e46b6-155">ChangeCount</span></span>](changecount.md)
    
- [<span data-ttu-id="e46b6-156">IsComplete</span><span class="sxs-lookup"><span data-stu-id="e46b6-156">IsComplete</span></span>](iscomplete.md)
    
- [<span data-ttu-id="e46b6-157">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="e46b6-157">IsRecurring</span></span>](isrecurring.md)
    
- [<span data-ttu-id="e46b6-158">PercentComplete</span><span class="sxs-lookup"><span data-stu-id="e46b6-158">PercentComplete</span></span>](percentcomplete.md)
    
- [<span data-ttu-id="e46b6-159">Status</span><span class="sxs-lookup"><span data-stu-id="e46b6-159">Status</span></span>](status.md)
    
- [<span data-ttu-id="e46b6-160">StatusDescription</span><span class="sxs-lookup"><span data-stu-id="e46b6-160">StatusDescription</span></span>](statusdescription.md)
    
## <a name="see-also"></a><span data-ttu-id="e46b6-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="e46b6-161">See also</span></span>



[<span data-ttu-id="e46b6-162">Operação GetItem</span><span class="sxs-lookup"><span data-stu-id="e46b6-162">GetItem operation</span></span>](getitem-operation.md)


[<span data-ttu-id="e46b6-163">Criação de tarefas</span><span class="sxs-lookup"><span data-stu-id="e46b6-163">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="e46b6-164">Atualizar as tarefas</span><span class="sxs-lookup"><span data-stu-id="e46b6-164">Updating Tasks</span></span>](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)
  
[<span data-ttu-id="e46b6-165">A exclusão de tarefas</span><span class="sxs-lookup"><span data-stu-id="e46b6-165">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

