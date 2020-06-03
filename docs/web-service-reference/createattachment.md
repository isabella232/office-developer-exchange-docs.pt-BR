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
description: O elemento CreateAttachment define uma solicitação para criar um anexo a um item no repositório do Exchange.
ms.openlocfilehash: 4cba1b8865dae5da58b9617b249a29314c67331a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466434"
---
# <a name="createattachment"></a><span data-ttu-id="7370f-103">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="7370f-103">CreateAttachment</span></span>

<span data-ttu-id="7370f-104">O elemento **CreateAttachment** define uma solicitação para criar um anexo a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7370f-104">The **CreateAttachment** element defines a request to create an attachment to an item in the Exchange store.</span></span> 
  
```xml
<CreateAttachment>
   <ParentItemId/>
   <Attachments/>
</CreateAttachment>
```

 <span data-ttu-id="7370f-105">**CreateAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="7370f-105">**CreateAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7370f-106">Atributos e elementos</span><span class="sxs-lookup"><span data-stu-id="7370f-106">Attributes and elements</span></span>

<span data-ttu-id="7370f-107">As seções a seguir descrevem os atributos, os elementos filhos e os elementos pai.</span><span class="sxs-lookup"><span data-stu-id="7370f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7370f-108">Atributos</span><span class="sxs-lookup"><span data-stu-id="7370f-108">Attributes</span></span>

<span data-ttu-id="7370f-109">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7370f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7370f-110">Elementos filho</span><span class="sxs-lookup"><span data-stu-id="7370f-110">Child elements</span></span>

|<span data-ttu-id="7370f-111">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7370f-111">**Element**</span></span>|<span data-ttu-id="7370f-112">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7370f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7370f-113">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="7370f-113">ParentItemId</span></span>](parentitemid.md) <br/> |<span data-ttu-id="7370f-114">Identifica o item do repositório pai do Exchange que contém o anexo criado.</span><span class="sxs-lookup"><span data-stu-id="7370f-114">Identifies the parent Exchange store item that contains the created attachment.</span></span> <span data-ttu-id="7370f-115">O elemento [ParentItemId](parentitemid.md) deve fornecer a ID de um item real do repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7370f-115">The [ParentItemId](parentitemid.md) element must provide the ID of a real Exchange store item.</span></span> <span data-ttu-id="7370f-116">Os itens do repositório real podem ser recuperados usando a [operação GetItem](getitem-operation.md); os anexos são recuperados usando a [operação GetAttachment](getattachment-operation.md).</span><span class="sxs-lookup"><span data-stu-id="7370f-116">Real store items can be retrieved by using the [GetItem operation](getitem-operation.md); attachments are retrieved by using the [GetAttachment operation](getattachment-operation.md).</span></span> <span data-ttu-id="7370f-117">Ocorrerá um erro se [ParentItemId](parentitemid.md) for passado a ID de um anexo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="7370f-117">An error occurs if the [ParentItemId](parentitemid.md) is passed the ID of a file attachment.</span></span> <span data-ttu-id="7370f-118">Se [ParentItemId](parentitemid.md) representar a ID de um anexo de item existente, a [operação CreateAttachment](createattachment-operation.md) adicionará o novo anexo ao anexo existente.</span><span class="sxs-lookup"><span data-stu-id="7370f-118">If the [ParentItemId](parentitemid.md) represents the ID of an existing item attachment, the [CreateAttachment operation](createattachment-operation.md) adds the new attachment to the existing attachment.</span></span>  <br/> <span data-ttu-id="7370f-119">Este elemento é necessário para a [operação CreateAttachment](createattachment-operation.md).</span><span class="sxs-lookup"><span data-stu-id="7370f-119">This element is required for the [CreateAttachment operation](createattachment-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="7370f-120">Anexos</span><span class="sxs-lookup"><span data-stu-id="7370f-120">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="7370f-121">Contém os itens ou arquivos a serem anexados a um item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7370f-121">Contains the items or files to attach to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7370f-122">Elementos pai</span><span class="sxs-lookup"><span data-stu-id="7370f-122">Parent elements</span></span>

<span data-ttu-id="7370f-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7370f-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7370f-124">Comentários</span><span class="sxs-lookup"><span data-stu-id="7370f-124">Remarks</span></span>

<span data-ttu-id="7370f-125">Um anexo de item não existe como um item de repositório.</span><span class="sxs-lookup"><span data-stu-id="7370f-125">An item attachment does not exist as a store item.</span></span> <span data-ttu-id="7370f-126">Ela só existe como um anexo a um item ou outro anexo.</span><span class="sxs-lookup"><span data-stu-id="7370f-126">It only exists as an attachment to an item or another attachment.</span></span> <span data-ttu-id="7370f-127">Os anexos de item só podem ser recuperados usando a solicitação [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="7370f-127">Item attachments can only be retrieved by using the [GetAttachment](getattachment.md) request.</span></span> 
  
<span data-ttu-id="7370f-128">Os seguintes anexos de item podem ser criados:</span><span class="sxs-lookup"><span data-stu-id="7370f-128">The following item attachments can be created:</span></span>
  
- <span data-ttu-id="7370f-129">Item</span><span class="sxs-lookup"><span data-stu-id="7370f-129">Item</span></span>
    
- <span data-ttu-id="7370f-130">Mensagem</span><span class="sxs-lookup"><span data-stu-id="7370f-130">Message</span></span>
    
- <span data-ttu-id="7370f-131">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="7370f-131">CalendarItem</span></span>
    
- <span data-ttu-id="7370f-132">Contato</span><span class="sxs-lookup"><span data-stu-id="7370f-132">Contact</span></span>
    
- <span data-ttu-id="7370f-133">Tarefa</span><span class="sxs-lookup"><span data-stu-id="7370f-133">Task</span></span>
    
- <span data-ttu-id="7370f-134">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="7370f-134">MeetingMessage</span></span>
    
- <span data-ttu-id="7370f-135">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="7370f-135">MeetingRequest</span></span>
    
<span data-ttu-id="7370f-136">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o MicrosoftExchange Server 2007 que tem instalada a função de servidor de Acesso para Cliente.</span><span class="sxs-lookup"><span data-stu-id="7370f-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="7370f-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7370f-137">Example</span></span>

<span data-ttu-id="7370f-138">O exemplo a seguir mostra como criar e anexar um item a outro item no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="7370f-138">The following example shows how to create and attach an item to another item in the Exchange store.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="7370f-139">Elemento de informações</span><span class="sxs-lookup"><span data-stu-id="7370f-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7370f-140">Namespace</span><span class="sxs-lookup"><span data-stu-id="7370f-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7370f-141">Nome do esquema</span><span class="sxs-lookup"><span data-stu-id="7370f-141">Schema Name</span></span>  <br/> |<span data-ttu-id="7370f-142">Esquema de mensagens</span><span class="sxs-lookup"><span data-stu-id="7370f-142">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7370f-143">Arquivo de validação</span><span class="sxs-lookup"><span data-stu-id="7370f-143">Validation File</span></span>  <br/> |<span data-ttu-id="7370f-144">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7370f-144">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7370f-145">Pode ser vazio</span><span class="sxs-lookup"><span data-stu-id="7370f-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="7370f-146">False</span><span class="sxs-lookup"><span data-stu-id="7370f-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7370f-147">Confira também</span><span class="sxs-lookup"><span data-stu-id="7370f-147">See also</span></span>



[<span data-ttu-id="7370f-148">Operação CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="7370f-148">CreateAttachment operation</span></span>](createattachment-operation.md)
  
[<span data-ttu-id="7370f-149">Operação DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="7370f-149">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
  
[<span data-ttu-id="7370f-150">Operação GetAttachment</span><span class="sxs-lookup"><span data-stu-id="7370f-150">GetAttachment operation</span></span>](getattachment-operation.md)

