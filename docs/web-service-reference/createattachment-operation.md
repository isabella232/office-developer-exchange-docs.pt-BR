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
description: A operação CreateAttachment cria um item ou o arquivo de anexo e o anexa ao item especificado.
ms.openlocfilehash: fed60275a007f2796c60d936def7a937e4982f29
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751565"
---
# <a name="createattachment-operation"></a><span data-ttu-id="0b86c-103">Operação CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="0b86c-103">CreateAttachment operation</span></span>

<span data-ttu-id="0b86c-104">A operação CreateAttachment cria um item ou o arquivo de anexo e o anexa ao item especificado.</span><span class="sxs-lookup"><span data-stu-id="0b86c-104">The CreateAttachment operation creates either an item or file attachment and attaches it to the specified item.</span></span>
  
## <a name="file-createattachment-request-example"></a><span data-ttu-id="0b86c-105">Exemplo de arquivo de solicitação CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="0b86c-105">File CreateAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="0b86c-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b86c-106">Description</span></span>

<span data-ttu-id="0b86c-107">O exemplo a seguir de uma solicitação de CreateAttachment mostra como criar um anexo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="0b86c-107">The following example of a CreateAttachment request shows how to create a file attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="0b86c-108">Código</span><span class="sxs-lookup"><span data-stu-id="0b86c-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
<soap:Body>
  <CreateAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comment"></a><span data-ttu-id="0b86c-109">Comment</span><span class="sxs-lookup"><span data-stu-id="0b86c-109">Comment</span></span>

<span data-ttu-id="0b86c-110">Um nome para o anexo deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="0b86c-110">A name for the attachment must be provided.</span></span>
  
> [!NOTE]
> <span data-ttu-id="0b86c-111">O identificador do item pai e alterar chave foram diminuídas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0b86c-111">The parent item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="0b86c-112">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b86c-112">Request elements</span></span>

<span data-ttu-id="0b86c-113">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="0b86c-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="0b86c-114">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="0b86c-114">CreateAttachment</span></span>](createattachment.md)
    
- [<span data-ttu-id="0b86c-115">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="0b86c-115">ParentItemId</span></span>](parentitemid.md)
    
- [<span data-ttu-id="0b86c-116">Anexos</span><span class="sxs-lookup"><span data-stu-id="0b86c-116">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="0b86c-117">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="0b86c-117">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="0b86c-118">Nome (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="0b86c-118">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="0b86c-119">Conteúdo</span><span class="sxs-lookup"><span data-stu-id="0b86c-119">Content</span></span>](content.md)
    
## <a name="successful-file-createattachment-response-example"></a><span data-ttu-id="0b86c-120">Exemplo de resposta bem-sucedida CreateAttachment de arquivo</span><span class="sxs-lookup"><span data-stu-id="0b86c-120">Successful File CreateAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="0b86c-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b86c-121">Description</span></span>

<span data-ttu-id="0b86c-122">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="0b86c-122">The following example shows a successful response to the CreateAttachment request.</span></span>
  
### <a name="code"></a><span data-ttu-id="0b86c-123">Código</span><span class="sxs-lookup"><span data-stu-id="0b86c-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comment"></a><span data-ttu-id="0b86c-124">Comment</span><span class="sxs-lookup"><span data-stu-id="0b86c-124">Comment</span></span>

<span data-ttu-id="0b86c-125">A resposta conterá o identificador do arquivo anexado.</span><span class="sxs-lookup"><span data-stu-id="0b86c-125">The response contains the identifier of the attached file.</span></span> <span data-ttu-id="0b86c-126">Ele também contém o identificador e alterar a chave do item raiz.</span><span class="sxs-lookup"><span data-stu-id="0b86c-126">It also contains the identifier and change key of the root item.</span></span> <span data-ttu-id="0b86c-127">Os identificadores de item e alterar chave foram diminuídas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0b86c-127">The item identifiers and change key have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="0b86c-128">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="0b86c-128">Successful response elements</span></span>

<span data-ttu-id="0b86c-129">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="0b86c-129">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="0b86c-130">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0b86c-130">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="0b86c-131">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="0b86c-131">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="0b86c-132">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0b86c-132">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="0b86c-133">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0b86c-133">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="0b86c-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0b86c-134">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0b86c-135">Anexos</span><span class="sxs-lookup"><span data-stu-id="0b86c-135">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="0b86c-136">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="0b86c-136">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="0b86c-137">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="0b86c-137">AttachmentId</span></span>](attachmentid.md)
    
## <a name="item-createattachment-request-example"></a><span data-ttu-id="0b86c-138">Exemplo de solicitação do item CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="0b86c-138">Item CreateAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="0b86c-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b86c-139">Description</span></span>

<span data-ttu-id="0b86c-140">O exemplo a seguir de uma solicitação de CreateAttachment mostra como criar um anexo do item.</span><span class="sxs-lookup"><span data-stu-id="0b86c-140">The following example of a CreateAttachment request shows how to create an item attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="0b86c-141">Código</span><span class="sxs-lookup"><span data-stu-id="0b86c-141">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comment"></a><span data-ttu-id="0b86c-142">Comment</span><span class="sxs-lookup"><span data-stu-id="0b86c-142">Comment</span></span>

<span data-ttu-id="0b86c-143">Um nome para o anexo deve ser fornecido.</span><span class="sxs-lookup"><span data-stu-id="0b86c-143">A name for the attachment must be provided.</span></span>
  
 <span data-ttu-id="0b86c-144">**Observação** O identificador do item pai e alterar chave foram diminuídas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0b86c-144">**Note** The parent item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="0b86c-145">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0b86c-145">Request elements</span></span>

<span data-ttu-id="0b86c-146">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="0b86c-146">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="0b86c-147">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="0b86c-147">CreateAttachment</span></span>](createattachment.md)
    
- [<span data-ttu-id="0b86c-148">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="0b86c-148">ParentItemId</span></span>](parentitemid.md)
    
- [<span data-ttu-id="0b86c-149">Anexos</span><span class="sxs-lookup"><span data-stu-id="0b86c-149">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="0b86c-150">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="0b86c-150">ItemAttachment</span></span>](itemattachment.md)
    
- [<span data-ttu-id="0b86c-151">Nome (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="0b86c-151">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="0b86c-152">Mensagem</span><span class="sxs-lookup"><span data-stu-id="0b86c-152">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="0b86c-153">Assunto</span><span class="sxs-lookup"><span data-stu-id="0b86c-153">Subject</span></span>](subject.md)
    
## <a name="successful-item-createattachment-response-example"></a><span data-ttu-id="0b86c-154">Exemplo de resposta bem-sucedida CreateAttachment de Item</span><span class="sxs-lookup"><span data-stu-id="0b86c-154">Successful Item CreateAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="0b86c-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b86c-155">Description</span></span>

<span data-ttu-id="0b86c-156">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="0b86c-156">The following example shows a successful response to the CreateAttachment request.</span></span>
  
### <a name="code"></a><span data-ttu-id="0b86c-157">Código</span><span class="sxs-lookup"><span data-stu-id="0b86c-157">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comment"></a><span data-ttu-id="0b86c-158">Comment</span><span class="sxs-lookup"><span data-stu-id="0b86c-158">Comment</span></span>

<span data-ttu-id="0b86c-159">A resposta conterá o identificador do novo anexo.</span><span class="sxs-lookup"><span data-stu-id="0b86c-159">The response contains the identifier of the new attachment.</span></span> <span data-ttu-id="0b86c-160">Ele também contém o identificador e alterar a chave do item raiz.</span><span class="sxs-lookup"><span data-stu-id="0b86c-160">It also contains the identifier and change key of the root item.</span></span> <span data-ttu-id="0b86c-161">O item raiz é o item que contém o anexo.</span><span class="sxs-lookup"><span data-stu-id="0b86c-161">The root item is the item that contains the attachment.</span></span> <span data-ttu-id="0b86c-162">Os identificadores de item e alterar chave foram diminuídas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0b86c-162">The item identifiers and change key have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="0b86c-163">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="0b86c-163">Successful response elements</span></span>

<span data-ttu-id="0b86c-164">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="0b86c-164">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="0b86c-165">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0b86c-165">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="0b86c-166">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="0b86c-166">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="0b86c-167">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0b86c-167">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="0b86c-168">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0b86c-168">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="0b86c-169">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0b86c-169">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0b86c-170">Anexos</span><span class="sxs-lookup"><span data-stu-id="0b86c-170">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="0b86c-171">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="0b86c-171">ItemAttachment</span></span>](itemattachment.md)
    
- [<span data-ttu-id="0b86c-172">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="0b86c-172">AttachmentId</span></span>](attachmentid.md)
    
## <a name="createattachment-error-response-example"></a><span data-ttu-id="0b86c-173">Exemplo de resposta de erro CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="0b86c-173">CreateAttachment Error response example</span></span>

### <a name="description"></a><span data-ttu-id="0b86c-174">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b86c-174">Description</span></span>

<span data-ttu-id="0b86c-175">O exemplo a seguir mostra uma resposta de erro à solicitação CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="0b86c-175">The following example shows an error response to the CreateAttachment request.</span></span> <span data-ttu-id="0b86c-176">O erro é devido ao fato de que o nome do anexo não foi especificado.</span><span class="sxs-lookup"><span data-stu-id="0b86c-176">The error is due to the fact that the name of the attachment was not specified.</span></span>
  
### <a name="code"></a><span data-ttu-id="0b86c-177">Código</span><span class="sxs-lookup"><span data-stu-id="0b86c-177">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="0b86c-178">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="0b86c-178">Error response elements</span></span>

<span data-ttu-id="0b86c-179">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="0b86c-179">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="0b86c-180">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0b86c-180">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="0b86c-181">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="0b86c-181">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="0b86c-182">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0b86c-182">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="0b86c-183">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0b86c-183">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="0b86c-184">MessageText</span><span class="sxs-lookup"><span data-stu-id="0b86c-184">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="0b86c-185">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0b86c-185">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0b86c-186">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0b86c-186">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="0b86c-187">MessageXml</span><span class="sxs-lookup"><span data-stu-id="0b86c-187">MessageXml</span></span>](messagexml.md)
    
- [<span data-ttu-id="0b86c-188">ExceptionFieldURI</span><span class="sxs-lookup"><span data-stu-id="0b86c-188">ExceptionFieldURI</span></span>](exceptionfielduri.md)
    
- [<span data-ttu-id="0b86c-189">Anexos</span><span class="sxs-lookup"><span data-stu-id="0b86c-189">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
## <a name="remarks"></a><span data-ttu-id="0b86c-190">Coment�rios</span><span class="sxs-lookup"><span data-stu-id="0b86c-190">Remarks</span></span>

<span data-ttu-id="0b86c-191">Se vários anexos anexados a um item em uma única ida e volta, o RootItemChangeKey na última mensagem de resposta é aquela que representa a nova chave de alteração do item que tenha os anexos.</span><span class="sxs-lookup"><span data-stu-id="0b86c-191">If multiple attachments are attached to an item in a single round trip, the RootItemChangeKey in the last response message is the one that represents the new change key of the item that has the attachments.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="0b86c-192">Confira também</span><span class="sxs-lookup"><span data-stu-id="0b86c-192">See also</span></span>



[<span data-ttu-id="0b86c-193">Operação DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="0b86c-193">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
  
[<span data-ttu-id="0b86c-194">Operação GetAttachment</span><span class="sxs-lookup"><span data-stu-id="0b86c-194">GetAttachment operation</span></span>](getattachment-operation.md)
