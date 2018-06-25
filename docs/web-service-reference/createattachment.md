---
title: CreateAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAttachment
api_type:
- schema
ms.assetid: e33b403a-b7d3-48ee-8d24-6b7abf0d70bc
description: O elemento de CreateAttachment define uma solicitação para criar um anexo a um item no armazenamento do Exchange.
ms.openlocfilehash: d403eb5ca15623d3a973f7b224dbcde5529cf1bc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19751567"
---
# <a name="createattachment"></a><span data-ttu-id="c96fd-103">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="c96fd-103">CreateAttachment</span></span>

<span data-ttu-id="c96fd-104">O elemento de **CreateAttachment** define uma solicitação para criar um anexo a um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c96fd-104">The **CreateAttachment** element defines a request to create an attachment to an item in the Exchange store.</span></span> 
  
```xml
<CreateAttachment>
   <ParentItemId/>
   <Attachments/>
</CreateAttachment>
```

 <span data-ttu-id="c96fd-105">**CreateAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="c96fd-105">**CreateAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c96fd-106">Attributes and elements</span><span class="sxs-lookup"><span data-stu-id="c96fd-106">Attributes and elements</span></span>

<span data-ttu-id="c96fd-107">As seções a seguir descrevem os atributos e elementos filho elementos pai.</span><span class="sxs-lookup"><span data-stu-id="c96fd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c96fd-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="c96fd-108">Attributes</span></span>

<span data-ttu-id="c96fd-109">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c96fd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c96fd-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="c96fd-110">Child elements</span></span>

|<span data-ttu-id="c96fd-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c96fd-111">**Element**</span></span>|<span data-ttu-id="c96fd-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c96fd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c96fd-113">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="c96fd-113">ParentItemId</span></span>](parentitemid.md) <br/> |<span data-ttu-id="c96fd-114">Identifica o item pai Exchange repositório que contém o anexo criado.</span><span class="sxs-lookup"><span data-stu-id="c96fd-114">Identifies the parent Exchange store item that contains the created attachment.</span></span> <span data-ttu-id="c96fd-115">O elemento [ParentItemId](parentitemid.md) deve fornecer a identificação de uma troca real armazenam o item.</span><span class="sxs-lookup"><span data-stu-id="c96fd-115">The [ParentItemId](parentitemid.md) element must provide the ID of a real Exchange store item.</span></span> <span data-ttu-id="c96fd-116">Real de armazenar itens podem ser recuperadas usando a [operação GetItem](getitem-operation.md); anexos serão recuperados usando a [operação GetAttachment](getattachment-operation.md).</span><span class="sxs-lookup"><span data-stu-id="c96fd-116">Real store items can be retrieved by using the [GetItem operation](getitem-operation.md); attachments are retrieved by using the [GetAttachment operation](getattachment-operation.md).</span></span> <span data-ttu-id="c96fd-117">Ocorrerá um erro se o [ParentItemId](parentitemid.md) é passado a identificação de um anexo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="c96fd-117">An error occurs if the [ParentItemId](parentitemid.md) is passed the ID of a file attachment.</span></span> <span data-ttu-id="c96fd-118">Se o [ParentItemId](parentitemid.md) representar a identificação de um anexo de item existente, a [operação CreateAttachment](createattachment-operation.md) adiciona o novo anexo no anexo existente.</span><span class="sxs-lookup"><span data-stu-id="c96fd-118">If the [ParentItemId](parentitemid.md) represents the ID of an existing item attachment, the [CreateAttachment operation](createattachment-operation.md) adds the new attachment to the existing attachment.</span></span>  <br/> <span data-ttu-id="c96fd-119">Esse elemento é necessário para a [operação CreateAttachment](createattachment-operation.md).</span><span class="sxs-lookup"><span data-stu-id="c96fd-119">This element is required for the [CreateAttachment operation](createattachment-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="c96fd-120">Anexos</span><span class="sxs-lookup"><span data-stu-id="c96fd-120">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c96fd-121">Contém os itens ou arquivos a serem anexados a um item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c96fd-121">Contains the items or files to attach to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c96fd-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="c96fd-122">Parent elements</span></span>

<span data-ttu-id="c96fd-123">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="c96fd-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c96fd-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="c96fd-124">Remarks</span></span>

<span data-ttu-id="c96fd-125">Um anexo do item não existe como um item de armazenamento.</span><span class="sxs-lookup"><span data-stu-id="c96fd-125">An item attachment does not exist as a store item.</span></span> <span data-ttu-id="c96fd-126">Ele só existe como um anexo de um item ou outro.</span><span class="sxs-lookup"><span data-stu-id="c96fd-126">It only exists as an attachment to an item or another attachment.</span></span> <span data-ttu-id="c96fd-127">Anexos de item só podem ser recuperados usando-se a solicitação [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="c96fd-127">Item attachments can only be retrieved by using the [GetAttachment](getattachment.md) request.</span></span> 
  
<span data-ttu-id="c96fd-128">Os seguintes anexos de item podem ser criados:</span><span class="sxs-lookup"><span data-stu-id="c96fd-128">The following item attachments can be created:</span></span>
  
- <span data-ttu-id="c96fd-129">Item</span><span class="sxs-lookup"><span data-stu-id="c96fd-129">Item</span></span>
    
- <span data-ttu-id="c96fd-130">Message</span><span class="sxs-lookup"><span data-stu-id="c96fd-130">Message</span></span>
    
- <span data-ttu-id="c96fd-131">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="c96fd-131">CalendarItem</span></span>
    
- <span data-ttu-id="c96fd-132">Contato</span><span class="sxs-lookup"><span data-stu-id="c96fd-132">Contact</span></span>
    
- <span data-ttu-id="c96fd-133">Tarefa</span><span class="sxs-lookup"><span data-stu-id="c96fd-133">Task</span></span>
    
- <span data-ttu-id="c96fd-134">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="c96fd-134">MeetingMessage</span></span>
    
- <span data-ttu-id="c96fd-135">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="c96fd-135">MeetingRequest</span></span>
    
<span data-ttu-id="c96fd-136">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="c96fd-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="c96fd-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c96fd-137">Example</span></span>

<span data-ttu-id="c96fd-138">O exemplo a seguir mostra como criar e anexar um item a outro item no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c96fd-138">The following example shows how to create and attach an item to another item in the Exchange store.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <ParentItemId Id="ASkAS"/>
      <Attachments>
        <t:ItemAttachment>
          <t:Name>MyAttachment</t:Name>
          <t:Message>
            <t:ItemClass>IPM>Note</t:ItemClass>
            <t:Subject>My attachment subject</t:Subject>
            <t:Body BodyType="Text">My attachment body</t:Body>
          </t:Message>
        </t:ItemAttachment>
      </Attachments>
    </CreateAttachment>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="c96fd-139">Informações de elemento</span><span class="sxs-lookup"><span data-stu-id="c96fd-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c96fd-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="c96fd-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c96fd-141">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="c96fd-141">Schema Name</span></span>  <br/> |<span data-ttu-id="c96fd-142">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="c96fd-142">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c96fd-143">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="c96fd-143">Validation File</span></span>  <br/> |<span data-ttu-id="c96fd-144">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c96fd-144">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c96fd-145">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="c96fd-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="c96fd-146">False</span><span class="sxs-lookup"><span data-stu-id="c96fd-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c96fd-147">Ver também</span><span class="sxs-lookup"><span data-stu-id="c96fd-147">See also</span></span>



[<span data-ttu-id="c96fd-148">Operação CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="c96fd-148">CreateAttachment operation</span></span>](createattachment-operation.md)
  
[<span data-ttu-id="c96fd-149">Operação DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="c96fd-149">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
  
[<span data-ttu-id="c96fd-150">Operação GetAttachment</span><span class="sxs-lookup"><span data-stu-id="c96fd-150">GetAttachment operation</span></span>](getattachment-operation.md)

