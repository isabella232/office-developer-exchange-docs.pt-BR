---
title: Operação CreateAttachment
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
ms.assetid: e066db95-6963-4507-a8d0-8efad287f550
description: A operação CreateAttachment cria um item ou anexo de arquivo e anexa-o ao item especificado.
ms.openlocfilehash: 8028c56aa306774b54b39e5ee1ac0382b9113fa0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456567"
---
# <a name="createattachment-operation"></a><span data-ttu-id="d320c-103">Operação CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="d320c-103">CreateAttachment operation</span></span>

<span data-ttu-id="d320c-104">A operação CreateAttachment cria um item ou anexo de arquivo e anexa-o ao item especificado.</span><span class="sxs-lookup"><span data-stu-id="d320c-104">The CreateAttachment operation creates either an item or file attachment and attaches it to the specified item.</span></span>
  
## <a name="file-createattachment-request-example"></a><span data-ttu-id="d320c-105">Exemplo de solicitação de CreateAttachment de arquivo</span><span class="sxs-lookup"><span data-stu-id="d320c-105">File CreateAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="d320c-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="d320c-106">Description</span></span>

<span data-ttu-id="d320c-107">O exemplo a seguir de uma solicitação de CreateAttachment mostra como criar um anexo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="d320c-107">The following example of a CreateAttachment request shows how to create a file attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="d320c-108">Código</span><span class="sxs-lookup"><span data-stu-id="d320c-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
<soap:Body>
  <CreateAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
    <ParentItemId Id="AAAtAE..." ChangeKey="CQAAABYA..."/>
    <Attachments>
      <t:FileAttachment>
        <t:Name>SomeFile</t:Name>
        <t:Content>AQIDBAU=</t:Content>
      </t:FileAttachment>
    </Attachments>
  </CreateAttachment>
</soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="d320c-109">Comentário</span><span class="sxs-lookup"><span data-stu-id="d320c-109">Comment</span></span>

<span data-ttu-id="d320c-110">Deve ser fornecido um nome para o anexo.</span><span class="sxs-lookup"><span data-stu-id="d320c-110">A name for the attachment must be provided.</span></span>
  
> [!NOTE]
> <span data-ttu-id="d320c-111">O identificador de item pai e a chave de alteração foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d320c-111">The parent item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="d320c-112">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="d320c-112">Request elements</span></span>

<span data-ttu-id="d320c-113">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="d320c-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="d320c-114">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="d320c-114">CreateAttachment</span></span>](createattachment.md)
    
- [<span data-ttu-id="d320c-115">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="d320c-115">ParentItemId</span></span>](parentitemid.md)
    
- [<span data-ttu-id="d320c-116">Anexos</span><span class="sxs-lookup"><span data-stu-id="d320c-116">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="d320c-117">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="d320c-117">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="d320c-118">Nome (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="d320c-118">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="d320c-119">Conteúdo</span><span class="sxs-lookup"><span data-stu-id="d320c-119">Content</span></span>](content.md)
    
## <a name="successful-file-createattachment-response-example"></a><span data-ttu-id="d320c-120">Exemplo de resposta de CreateAttachment de arquivo bem-sucedido</span><span class="sxs-lookup"><span data-stu-id="d320c-120">Successful File CreateAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="d320c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="d320c-121">Description</span></span>

<span data-ttu-id="d320c-122">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="d320c-122">The following example shows a successful response to the CreateAttachment request.</span></span>
  
### <a name="code"></a><span data-ttu-id="d320c-123">Código</span><span class="sxs-lookup"><span data-stu-id="d320c-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="AAAtAE=" RootItemId="AAAtAEFk=" RootItemChangeKey="CQAAAB"/>
            </t:FileAttachment>
          </m:Attachments>
        </m:CreateAttachmentResponseMessage>
      </m:ResponseMessages>
    </CreateAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="d320c-124">Comentário</span><span class="sxs-lookup"><span data-stu-id="d320c-124">Comment</span></span>

<span data-ttu-id="d320c-125">A resposta contém o identificador do arquivo anexado.</span><span class="sxs-lookup"><span data-stu-id="d320c-125">The response contains the identifier of the attached file.</span></span> <span data-ttu-id="d320c-126">Ele também contém o identificador e a chave de alteração do item raiz.</span><span class="sxs-lookup"><span data-stu-id="d320c-126">It also contains the identifier and change key of the root item.</span></span> <span data-ttu-id="d320c-127">Os identificadores de item e a chave de alteração foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d320c-127">The item identifiers and change key have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="d320c-128">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="d320c-128">Successful response elements</span></span>

<span data-ttu-id="d320c-129">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="d320c-129">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="d320c-130">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d320c-130">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="d320c-131">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="d320c-131">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="d320c-132">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d320c-132">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="d320c-133">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d320c-133">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="d320c-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d320c-134">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d320c-135">Anexos</span><span class="sxs-lookup"><span data-stu-id="d320c-135">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="d320c-136">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="d320c-136">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="d320c-137">Attachmentid</span><span class="sxs-lookup"><span data-stu-id="d320c-137">AttachmentId</span></span>](attachmentid.md)
    
## <a name="item-createattachment-request-example"></a><span data-ttu-id="d320c-138">Exemplo de solicitação de CreateAttachment de item</span><span class="sxs-lookup"><span data-stu-id="d320c-138">Item CreateAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="d320c-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="d320c-139">Description</span></span>

<span data-ttu-id="d320c-140">O exemplo a seguir de uma solicitação de CreateAttachment mostra como criar um anexo de item.</span><span class="sxs-lookup"><span data-stu-id="d320c-140">The following example of a CreateAttachment request shows how to create an item attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="d320c-141">Código</span><span class="sxs-lookup"><span data-stu-id="d320c-141">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <ParentItemId Id="AAAtAE=" ChangeKey="CQAAABYA"/>
      <Attachments>
        <t:ItemAttachment>
          <t:Name>An item attachment</t:Name>
          <t:Message>
            <t:Subject>A message to attach</t:Subject>
          </t:Message>
        </t:ItemAttachment>
      </Attachments>
    </CreateAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="d320c-142">Comentário</span><span class="sxs-lookup"><span data-stu-id="d320c-142">Comment</span></span>

<span data-ttu-id="d320c-143">Deve ser fornecido um nome para o anexo.</span><span class="sxs-lookup"><span data-stu-id="d320c-143">A name for the attachment must be provided.</span></span>
  
 <span data-ttu-id="d320c-144">**Observação** O identificador de item pai e a chave de alteração foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d320c-144">**Note** The parent item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="d320c-145">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="d320c-145">Request elements</span></span>

<span data-ttu-id="d320c-146">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="d320c-146">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="d320c-147">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="d320c-147">CreateAttachment</span></span>](createattachment.md)
    
- [<span data-ttu-id="d320c-148">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="d320c-148">ParentItemId</span></span>](parentitemid.md)
    
- [<span data-ttu-id="d320c-149">Anexos</span><span class="sxs-lookup"><span data-stu-id="d320c-149">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="d320c-150">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="d320c-150">ItemAttachment</span></span>](itemattachment.md)
    
- [<span data-ttu-id="d320c-151">Nome (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="d320c-151">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="d320c-152">Mensagem</span><span class="sxs-lookup"><span data-stu-id="d320c-152">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="d320c-153">Assunto</span><span class="sxs-lookup"><span data-stu-id="d320c-153">Subject</span></span>](subject.md)
    
## <a name="successful-item-createattachment-response-example"></a><span data-ttu-id="d320c-154">Exemplo de resposta de CreateAttachment de item bem-sucedido</span><span class="sxs-lookup"><span data-stu-id="d320c-154">Successful Item CreateAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="d320c-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="d320c-155">Description</span></span>

<span data-ttu-id="d320c-156">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="d320c-156">The following example shows a successful response to the CreateAttachment request.</span></span>
  
### <a name="code"></a><span data-ttu-id="d320c-157">Código</span><span class="sxs-lookup"><span data-stu-id="d320c-157">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:ItemAttachment>
              <t:AttachmentId Id="AAAtAEFk=" RootItemId="AAAtAEFkb=" RootItemChangeKey="CQAAABYA"/>
            </t:ItemAttachment>
          </m:Attachments>
        </m:CreateAttachmentResponseMessage>
      </m:ResponseMessages>
    </CreateAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="d320c-158">Comentário</span><span class="sxs-lookup"><span data-stu-id="d320c-158">Comment</span></span>

<span data-ttu-id="d320c-159">A resposta contém o identificador do novo anexo.</span><span class="sxs-lookup"><span data-stu-id="d320c-159">The response contains the identifier of the new attachment.</span></span> <span data-ttu-id="d320c-160">Ele também contém o identificador e a chave de alteração do item raiz.</span><span class="sxs-lookup"><span data-stu-id="d320c-160">It also contains the identifier and change key of the root item.</span></span> <span data-ttu-id="d320c-161">O item raiz é o item que contém o anexo.</span><span class="sxs-lookup"><span data-stu-id="d320c-161">The root item is the item that contains the attachment.</span></span> <span data-ttu-id="d320c-162">Os identificadores de item e a chave de alteração foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="d320c-162">The item identifiers and change key have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="d320c-163">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="d320c-163">Successful response elements</span></span>

<span data-ttu-id="d320c-164">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="d320c-164">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="d320c-165">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d320c-165">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="d320c-166">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="d320c-166">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="d320c-167">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d320c-167">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="d320c-168">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d320c-168">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="d320c-169">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d320c-169">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d320c-170">Anexos</span><span class="sxs-lookup"><span data-stu-id="d320c-170">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="d320c-171">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="d320c-171">ItemAttachment</span></span>](itemattachment.md)
    
- [<span data-ttu-id="d320c-172">Attachmentid</span><span class="sxs-lookup"><span data-stu-id="d320c-172">AttachmentId</span></span>](attachmentid.md)
    
## <a name="createattachment-error-response-example"></a><span data-ttu-id="d320c-173">Exemplo de resposta de erro CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="d320c-173">CreateAttachment Error response example</span></span>

### <a name="description"></a><span data-ttu-id="d320c-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="d320c-174">Description</span></span>

<span data-ttu-id="d320c-175">O exemplo a seguir mostra uma resposta de erro para a solicitação de CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="d320c-175">The following example shows an error response to the CreateAttachment request.</span></span> <span data-ttu-id="d320c-176">O erro se deve ao fato de que o nome do anexo não foi especificado.</span><span class="sxs-lookup"><span data-stu-id="d320c-176">The error is due to the fact that the name of the attachment was not specified.</span></span>
  
### <a name="code"></a><span data-ttu-id="d320c-177">Código</span><span class="sxs-lookup"><span data-stu-id="d320c-177">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateAttachmentResponseMessage ResponseClass="Error">
          <m:MessageText>Required property is missing.</m:MessageText>
          <m:ResponseCode>ErrorRequiredPropertyMissing</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:MessageXml>
            <t:ExceptionFieldURI FieldURI="attachment:Name"/>
          </m:MessageXml>
          <m:Attachments/>
        </m:CreateAttachmentResponseMessage>
      </m:ResponseMessages>
    </CreateAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="d320c-178">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="d320c-178">Error response elements</span></span>

<span data-ttu-id="d320c-179">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="d320c-179">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="d320c-180">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d320c-180">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="d320c-181">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="d320c-181">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="d320c-182">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d320c-182">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="d320c-183">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d320c-183">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="d320c-184">MessageText</span><span class="sxs-lookup"><span data-stu-id="d320c-184">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="d320c-185">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d320c-185">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d320c-186">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d320c-186">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="d320c-187">MessageXml</span><span class="sxs-lookup"><span data-stu-id="d320c-187">MessageXml</span></span>](messagexml.md)
    
- [<span data-ttu-id="d320c-188">ExceptionFieldURI</span><span class="sxs-lookup"><span data-stu-id="d320c-188">ExceptionFieldURI</span></span>](exceptionfielduri.md)
    
- [<span data-ttu-id="d320c-189">Anexos</span><span class="sxs-lookup"><span data-stu-id="d320c-189">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
## <a name="remarks"></a><span data-ttu-id="d320c-190">Comentários</span><span class="sxs-lookup"><span data-stu-id="d320c-190">Remarks</span></span>

<span data-ttu-id="d320c-191">Se vários anexos estiverem anexados a um item em uma única viagem de ida e volta, o RootItemChangeKey na última mensagem de resposta será aquele que representa a nova chave de alteração do item que tem os anexos.</span><span class="sxs-lookup"><span data-stu-id="d320c-191">If multiple attachments are attached to an item in a single round trip, the RootItemChangeKey in the last response message is the one that represents the new change key of the item that has the attachments.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="d320c-192">Confira também</span><span class="sxs-lookup"><span data-stu-id="d320c-192">See also</span></span>



[<span data-ttu-id="d320c-193">Operação DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="d320c-193">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
  
[<span data-ttu-id="d320c-194">Operação GetAttachment</span><span class="sxs-lookup"><span data-stu-id="d320c-194">GetAttachment operation</span></span>](getattachment-operation.md)

