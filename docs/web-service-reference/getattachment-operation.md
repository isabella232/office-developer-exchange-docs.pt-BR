---
title: Operação GetAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetAttachment
api_type:
- schema
ms.assetid: 24d10a15-b942-415e-9024-a6375708f326
description: A operação GetAttachment é usada para recuperar os anexos existentes em itens no armazenamento do Exchange.
ms.openlocfilehash: c260033208bf49c60463c09041d8ffcc52a8f5c2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752411"
---
# <a name="getattachment-operation"></a><span data-ttu-id="ee18f-103">Operação GetAttachment</span><span class="sxs-lookup"><span data-stu-id="ee18f-103">GetAttachment operation</span></span>

<span data-ttu-id="ee18f-104">A operação GetAttachment é usada para recuperar os anexos existentes em itens no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="ee18f-104">The GetAttachment operation is used to retrieve existing attachments on items in the Exchange store.</span></span>
  
## <a name="getattachment-request-example"></a><span data-ttu-id="ee18f-105">Exemplo de solicitação GetAttachment</span><span class="sxs-lookup"><span data-stu-id="ee18f-105">GetAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="ee18f-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee18f-106">Description</span></span>

<span data-ttu-id="ee18f-107">O exemplo a seguir de solicitação GetAttachment mostra como obter um anexo.</span><span class="sxs-lookup"><span data-stu-id="ee18f-107">The following example of GetAttachment request shows how to get an attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="ee18f-108">Código</span><span class="sxs-lookup"><span data-stu-id="ee18f-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="ee18f-109">Comments</span><span class="sxs-lookup"><span data-stu-id="ee18f-109">Comments</span></span>

<span data-ttu-id="ee18f-110">O elemento [AttachmentShape](attachmentshape.md) permite que você especifique quais informações do anexo devem ser retornadas.</span><span class="sxs-lookup"><span data-stu-id="ee18f-110">The [AttachmentShape](attachmentshape.md) element allows you to specify which attachment information should be returned.</span></span> <span data-ttu-id="ee18f-111">Um elemento [AttachmentShape](attachmentshape.md) vazio é válido e será renderizado anexos sem conteúdo MIME para anexos de item, com um tipo de corpo de texto e sem qualquer propriedades adicionais.</span><span class="sxs-lookup"><span data-stu-id="ee18f-111">An empty [AttachmentShape](attachmentshape.md) element is valid and will render your attachments without MIME content for item attachments, with a text body type, and without any additional properties.</span></span> 
  
<span data-ttu-id="ee18f-112">A coleção [AttachmentIds](attachmentids.md) permite que você especifique um ou mais identificadores de anexo para retornar.</span><span class="sxs-lookup"><span data-stu-id="ee18f-112">The [AttachmentIds](attachmentids.md) collection allows you to specify one or more attachment identifiers to return.</span></span> <span data-ttu-id="ee18f-113">Observe que esses são do tipo RequestAttachmentIdType, portanto, qualquer AttachmentIds recebidos de **CreateAttachment** deve ter os atributos **RootItemId** e **RootItemChangeKey** removido antes de passar os mesmos para **GetAttachment**.</span><span class="sxs-lookup"><span data-stu-id="ee18f-113">Note that these are of type RequestAttachmentIdType, so any AttachmentIds that you receive from **CreateAttachment** must have the **RootItemId** and **RootItemChangeKey** attributes removed before passing them to **GetAttachment**.</span></span>
  
> [!NOTE]
> <span data-ttu-id="ee18f-114">O identificador de anexo e alterar chave foram diminuídas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="ee18f-114">The attachment identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="ee18f-115">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ee18f-115">Request elements</span></span>

<span data-ttu-id="ee18f-116">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="ee18f-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="ee18f-117">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="ee18f-117">GetAttachment</span></span>](getattachment.md)
    
- [<span data-ttu-id="ee18f-118">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="ee18f-118">AttachmentShape</span></span>](attachmentshape.md)
    
- [<span data-ttu-id="ee18f-119">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="ee18f-119">AttachmentIds</span></span>](attachmentids.md)
    
- [<span data-ttu-id="ee18f-120">AttachmentId (GetAttachment e DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="ee18f-120">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md)
    
## <a name="getattachment-response-example"></a><span data-ttu-id="ee18f-121">Exemplo de resposta GetAttachment</span><span class="sxs-lookup"><span data-stu-id="ee18f-121">GetAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="ee18f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee18f-122">Description</span></span>

<span data-ttu-id="ee18f-123">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de GetAttachment.</span><span class="sxs-lookup"><span data-stu-id="ee18f-123">The following example shows a successful response to a GetAttachment request.</span></span> <span data-ttu-id="ee18f-124">Este exemplo retorna um anexo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="ee18f-124">This example returns a file attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="ee18f-125">Código</span><span class="sxs-lookup"><span data-stu-id="ee18f-125">Code</span></span>

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
    <GetAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
              <t:Name>SomeFile</t:Name>
              <t:Content>AQIDBAU=</t:Content>
            </t:FileAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </GetAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="ee18f-126">Comments</span><span class="sxs-lookup"><span data-stu-id="ee18f-126">Comments</span></span>

<span data-ttu-id="ee18f-127">As mensagens de resposta para GetAttachment sempre conterá o anexo completo; ou seja, todas as propriedades sempre serão incluídas.</span><span class="sxs-lookup"><span data-stu-id="ee18f-127">The response messages for GetAttachment will always contain the full attachment; that is, all properties will always be included.</span></span> <span data-ttu-id="ee18f-128">Anexos de arquivo, essas propriedades são [nome (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md)e [conteúdo](content.md).</span><span class="sxs-lookup"><span data-stu-id="ee18f-128">For file attachments, those properties are [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md), and [Content](content.md).</span></span> <span data-ttu-id="ee18f-129">Anexos de item, essas propriedades são [nome (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md) e todas as propriedades do item, como se a forma **AllProperties** tenha sido usada em uma chamada de GetItem.</span><span class="sxs-lookup"><span data-stu-id="ee18f-129">For item attachments, those properties are [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md) and all of the item's properties, as if the **AllProperties** shape had been used in a GetItem call.</span></span> <span data-ttu-id="ee18f-130">O elemento [AttachmentShape](attachmentshape.md) , se houver, permitirá que um aplicativo de consumidor solicitar as propriedades estendidas adicionais para anexos do item.</span><span class="sxs-lookup"><span data-stu-id="ee18f-130">The [AttachmentShape](attachmentshape.md) element, if present, will allow a consumer application to request additional extended properties for item attachments.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="ee18f-131">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="ee18f-131">Successful response elements</span></span>

<span data-ttu-id="ee18f-132">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="ee18f-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="ee18f-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ee18f-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ee18f-134">GetAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="ee18f-134">GetAttachmentResponse</span></span>](getattachmentresponse.md)
    
- [<span data-ttu-id="ee18f-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ee18f-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ee18f-136">GetAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ee18f-136">GetAttachmentResponseMessage</span></span>](getattachmentresponsemessage.md)
    
- [<span data-ttu-id="ee18f-137">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ee18f-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ee18f-138">Anexos</span><span class="sxs-lookup"><span data-stu-id="ee18f-138">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="ee18f-139">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="ee18f-139">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="ee18f-140">AttachmentId (GetAttachment e DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="ee18f-140">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md)
    
- [<span data-ttu-id="ee18f-141">Nome (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="ee18f-141">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="ee18f-142">Conteúdo</span><span class="sxs-lookup"><span data-stu-id="ee18f-142">Content</span></span>](content.md)
    
## <a name="see-also"></a><span data-ttu-id="ee18f-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="ee18f-143">See also</span></span>



[<span data-ttu-id="ee18f-144">Operação CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="ee18f-144">CreateAttachment operation</span></span>](createattachment-operation.md)
  
[<span data-ttu-id="ee18f-145">Operação DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="ee18f-145">DeleteAttachment operation</span></span>](deleteattachment-operation.md)

