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
description: A operação GetAttachment é usada para recuperar anexos existentes em itens no repositório do Exchange.
ms.openlocfilehash: ac7eafd61c62b077a8d20e5fd8d004924bf06cf1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461286"
---
# <a name="getattachment-operation"></a><span data-ttu-id="f9e0e-103">Operação GetAttachment</span><span class="sxs-lookup"><span data-stu-id="f9e0e-103">GetAttachment operation</span></span>

<span data-ttu-id="f9e0e-104">A operação GetAttachment é usada para recuperar anexos existentes em itens no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="f9e0e-104">The GetAttachment operation is used to retrieve existing attachments on items in the Exchange store.</span></span>
  
## <a name="getattachment-request-example"></a><span data-ttu-id="f9e0e-105">Exemplo de solicitação GetAttachment</span><span class="sxs-lookup"><span data-stu-id="f9e0e-105">GetAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="f9e0e-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9e0e-106">Description</span></span>

<span data-ttu-id="f9e0e-107">O exemplo a seguir de solicitação GetAttachment mostra como obter um anexo.</span><span class="sxs-lookup"><span data-stu-id="f9e0e-107">The following example of GetAttachment request shows how to get an attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="f9e0e-108">Código</span><span class="sxs-lookup"><span data-stu-id="f9e0e-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="f9e0e-109">Comentários</span><span class="sxs-lookup"><span data-stu-id="f9e0e-109">Comments</span></span>

<span data-ttu-id="f9e0e-110">O elemento [AttachmentShape](attachmentshape.md) permite que você especifique quais informações de anexo devem ser retornadas.</span><span class="sxs-lookup"><span data-stu-id="f9e0e-110">The [AttachmentShape](attachmentshape.md) element allows you to specify which attachment information should be returned.</span></span> <span data-ttu-id="f9e0e-111">Um elemento [AttachmentShape](attachmentshape.md) vazio é válido e renderizará seus anexos sem conteúdo MIME para anexos de item, com um tipo de corpo de texto e sem qualquer outra propriedade.</span><span class="sxs-lookup"><span data-stu-id="f9e0e-111">An empty [AttachmentShape](attachmentshape.md) element is valid and will render your attachments without MIME content for item attachments, with a text body type, and without any additional properties.</span></span> 
  
<span data-ttu-id="f9e0e-112">A coleção [AttachmentIds](attachmentids.md) permite que você especifique um ou mais identificadores de anexo a serem retornados.</span><span class="sxs-lookup"><span data-stu-id="f9e0e-112">The [AttachmentIds](attachmentids.md) collection allows you to specify one or more attachment identifiers to return.</span></span> <span data-ttu-id="f9e0e-113">Observe que eles são do tipo RequestAttachmentIdType, portanto, qualquer AttachmentIds que você receber de **CreateAttachment** deve ter os atributos **RootItemId** e **RootItemChangeKey** removidos antes de passá-los para **GetAttachment**.</span><span class="sxs-lookup"><span data-stu-id="f9e0e-113">Note that these are of type RequestAttachmentIdType, so any AttachmentIds that you receive from **CreateAttachment** must have the **RootItemId** and **RootItemChangeKey** attributes removed before passing them to **GetAttachment**.</span></span>
  
> [!NOTE]
> <span data-ttu-id="f9e0e-114">O identificador de anexo e a chave de alteração foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="f9e0e-114">The attachment identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="f9e0e-115">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="f9e0e-115">Request elements</span></span>

<span data-ttu-id="f9e0e-116">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="f9e0e-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="f9e0e-117">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="f9e0e-117">GetAttachment</span></span>](getattachment.md)
    
- [<span data-ttu-id="f9e0e-118">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="f9e0e-118">AttachmentShape</span></span>](attachmentshape.md)
    
- [<span data-ttu-id="f9e0e-119">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="f9e0e-119">AttachmentIds</span></span>](attachmentids.md)
    
- [<span data-ttu-id="f9e0e-120">Attachmentid (GetAttachment e DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="f9e0e-120">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md)
    
## <a name="getattachment-response-example"></a><span data-ttu-id="f9e0e-121">Exemplo de resposta de GetAttachment</span><span class="sxs-lookup"><span data-stu-id="f9e0e-121">GetAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="f9e0e-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f9e0e-122">Description</span></span>

<span data-ttu-id="f9e0e-123">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação GetAttachment.</span><span class="sxs-lookup"><span data-stu-id="f9e0e-123">The following example shows a successful response to a GetAttachment request.</span></span> <span data-ttu-id="f9e0e-124">Este exemplo retorna um anexo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="f9e0e-124">This example returns a file attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="f9e0e-125">Código</span><span class="sxs-lookup"><span data-stu-id="f9e0e-125">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="f9e0e-126">Comentários</span><span class="sxs-lookup"><span data-stu-id="f9e0e-126">Comments</span></span>

<span data-ttu-id="f9e0e-127">As mensagens de resposta para GetAttachment sempre conterão o anexo completo; ou seja, todas as propriedades serão sempre incluídas.</span><span class="sxs-lookup"><span data-stu-id="f9e0e-127">The response messages for GetAttachment will always contain the full attachment; that is, all properties will always be included.</span></span> <span data-ttu-id="f9e0e-128">Para anexos de arquivo, essas propriedades são [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md)e [Content](content.md).</span><span class="sxs-lookup"><span data-stu-id="f9e0e-128">For file attachments, those properties are [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md), and [Content](content.md).</span></span> <span data-ttu-id="f9e0e-129">Para anexos de item, essas propriedades são [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md) e todas as propriedades do item, como se a forma **myproperties** tivesse sido usada em uma chamada GetItem.</span><span class="sxs-lookup"><span data-stu-id="f9e0e-129">For item attachments, those properties are [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md) and all of the item's properties, as if the **AllProperties** shape had been used in a GetItem call.</span></span> <span data-ttu-id="f9e0e-130">O elemento [AttachmentShape](attachmentshape.md) , se presente, permitirá que um aplicativo de consumidor solicite propriedades estendidas adicionais para anexos de item.</span><span class="sxs-lookup"><span data-stu-id="f9e0e-130">The [AttachmentShape](attachmentshape.md) element, if present, will allow a consumer application to request additional extended properties for item attachments.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="f9e0e-131">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="f9e0e-131">Successful response elements</span></span>

<span data-ttu-id="f9e0e-132">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="f9e0e-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="f9e0e-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f9e0e-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="f9e0e-134">GetAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="f9e0e-134">GetAttachmentResponse</span></span>](getattachmentresponse.md)
    
- [<span data-ttu-id="f9e0e-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f9e0e-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="f9e0e-136">GetAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f9e0e-136">GetAttachmentResponseMessage</span></span>](getattachmentresponsemessage.md)
    
- [<span data-ttu-id="f9e0e-137">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f9e0e-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f9e0e-138">Anexos</span><span class="sxs-lookup"><span data-stu-id="f9e0e-138">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="f9e0e-139">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="f9e0e-139">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="f9e0e-140">Attachmentid (GetAttachment e DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="f9e0e-140">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md)
    
- [<span data-ttu-id="f9e0e-141">Nome (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="f9e0e-141">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="f9e0e-142">Conteúdo</span><span class="sxs-lookup"><span data-stu-id="f9e0e-142">Content</span></span>](content.md)
    
## <a name="see-also"></a><span data-ttu-id="f9e0e-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="f9e0e-143">See also</span></span>



[<span data-ttu-id="f9e0e-144">Operação CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="f9e0e-144">CreateAttachment operation</span></span>](createattachment-operation.md)
  
[<span data-ttu-id="f9e0e-145">Operação DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="f9e0e-145">DeleteAttachment operation</span></span>](deleteattachment-operation.md)

