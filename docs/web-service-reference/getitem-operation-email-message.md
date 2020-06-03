---
title: Operação GetItem (mensagem de email)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- GetItem
api_type:
- schema
ms.assetid: e8492e3b-1c8d-4b14-8070-9530f8306edd
description: A operação GetItem permite que o usuário acesse informações sobre mensagens de email.
localization_priority: Priority
ms.openlocfilehash: f8be01cad3d4c4534f66593cbe8bcee477726972
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459991"
---
# <a name="getitem-operation-email-message"></a><span data-ttu-id="c6808-103">Operação GetItem (mensagem de email)</span><span class="sxs-lookup"><span data-stu-id="c6808-103">GetItem operation (email message)</span></span>

<span data-ttu-id="c6808-104">A operação GetItem permite que o usuário acesse informações sobre mensagens de email.</span><span class="sxs-lookup"><span data-stu-id="c6808-104">The GetItem operation allows the user to access information about e-mail messages.</span></span>
  
## <a name="using-the-getitem-operation-for-messages"></a><span data-ttu-id="c6808-105">Usando a operação GetItem para mensagens</span><span class="sxs-lookup"><span data-stu-id="c6808-105">Using the GetItem Operation for Messages</span></span>

<span data-ttu-id="c6808-106">A solicitação GetItem deve ter as seguintes informações:</span><span class="sxs-lookup"><span data-stu-id="c6808-106">The GetItem request must have the following information:</span></span>
  
- <span data-ttu-id="c6808-107">O elemento [ItemId](itemid.md) para identificar as informações de item a serem retornadas.</span><span class="sxs-lookup"><span data-stu-id="c6808-107">The [ItemId](itemid.md) element to identify the item information to return.</span></span> 
    
- <span data-ttu-id="c6808-108">O elemento [myShape](itemshape.md) para identificar as propriedades do item a serem retornadas.</span><span class="sxs-lookup"><span data-stu-id="c6808-108">The [ItemShape](itemshape.md) element to identify the item properties to return.</span></span> 
    
## <a name="getitem-request-example"></a><span data-ttu-id="c6808-109">Exemplo de solicitação GetItem</span><span class="sxs-lookup"><span data-stu-id="c6808-109">GetItem request example</span></span>

### <a name="description"></a><span data-ttu-id="c6808-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6808-110">Description</span></span>

<span data-ttu-id="c6808-111">O exemplo a seguir de uma solicitação GetItem mostra como acessar informações sobre mensagens de email.</span><span class="sxs-lookup"><span data-stu-id="c6808-111">The following example of a GetItem request shows how to access information about e-mail messages.</span></span>
  
### <a name="code"></a><span data-ttu-id="c6808-112">Código</span><span class="sxs-lookup"><span data-stu-id="c6808-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope
  xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xmlns:xsd="http://www.w3.org/2001/XMLSchema"
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem
      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <ItemShape>
        <t:BaseShape>Default</t:BaseShape>
        <t:IncludeMimeContent>true</t:IncludeMimeContent>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAlAF" ChangeKey="CQAAAB" />
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="c6808-113">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="c6808-113">Request elements</span></span>

<span data-ttu-id="c6808-114">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="c6808-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="c6808-115">GetItem</span><span class="sxs-lookup"><span data-stu-id="c6808-115">GetItem</span></span>](getitem.md)
    
- [<span data-ttu-id="c6808-116">Shape</span><span class="sxs-lookup"><span data-stu-id="c6808-116">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="c6808-117">BaseShape</span><span class="sxs-lookup"><span data-stu-id="c6808-117">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="c6808-118">IncludeMimeContent</span><span class="sxs-lookup"><span data-stu-id="c6808-118">IncludeMimeContent</span></span>](includemimecontent.md)
    
- [<span data-ttu-id="c6808-119">ItemIds</span><span class="sxs-lookup"><span data-stu-id="c6808-119">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="c6808-120">ItemId</span><span class="sxs-lookup"><span data-stu-id="c6808-120">ItemId</span></span>](itemid.md)
    
## <a name="successful-getitem-e-mail-message-response-example"></a><span data-ttu-id="c6808-121">Exemplo de resposta de GetItem (mensagem de email) bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="c6808-121">Successful GetItem (E-mail Message) response example</span></span>

### <a name="description"></a><span data-ttu-id="c6808-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6808-122">Description</span></span>

<span data-ttu-id="c6808-123">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação GetItem.</span><span class="sxs-lookup"><span data-stu-id="c6808-123">The following example shows a successful response to the GetItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="c6808-124">Código</span><span class="sxs-lookup"><span data-stu-id="c6808-124">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:MimeContent CharacterSet="UTF-8">UmVjZWl</t:MimeContent>
              <t:ItemId Id="AAAlAFVz" ChangeKey="CQAAAB" />
              <t:Subject />
              <t:Sensitivity>Normal</t:Sensitivity>
              <t:Body BodyType="HTML">
                <html dir="ltr">
                  <head>
                    <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
                      <meta content="MSHTML 6.00.3790.2759" name="GENERATOR">
                        <style title="owaParaStyle">P { MARGIN-TOP: 0px; MARGIN-BOTTOM: 0px } </style>
                      </head>
                  <body ocsi="x">
                    <div dir="ltr">
                      <font face="Tahoma" color="#000000" size="2"></font>&amp;nbsp;
                    </div>
                  </body>
                </html>
              </t:Body>
              <t:Size>881</t:Size>
              <t:DateTimeSent>2006-10-28T01:37:06Z</t:DateTimeSent>
              <t:DateTimeCreated>2006-10-28T01:37:06Z</t:DateTimeCreated>
              <t:ResponseObjects>
                <t:ReplyToItem />
                <t:ReplyAllToItem />
                <t:ForwardItem />
              </t:ResponseObjects>
              <t:HasAttachments>false</t:HasAttachments>
              <t:ToRecipients>
                <t:Mailbox>
                  <t:Name>User1</t:Name>
                  <t:EmailAddress>User1@example.com</t:EmailAddress>
                  <t:RoutingType>SMTP</t:RoutingType>
                </t:Mailbox>
              </t:ToRecipients>
              <t:IsReadReceiptRequested>false</t:IsReadReceiptRequested>
              <t:IsDeliveryReceiptRequested>false</t:IsDeliveryReceiptRequested>
              <t:From>
                <t:Mailbox>
                  <t:Name>User2</t:Name>
                  <t:EmailAddress>User2@example.com</t:EmailAddress>
                  <t:RoutingType>SMTP</t:RoutingType>
                </t:Mailbox>
              </t:From>
              <t:IsRead>false</t:IsRead>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="c6808-125">Comentários</span><span class="sxs-lookup"><span data-stu-id="c6808-125">Comments</span></span>

<span data-ttu-id="c6808-126">O conteúdo MIME, a pasta e os identificadores de item foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c6808-126">The MIME content, folder, and item identifiers have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="c6808-127">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="c6808-127">Successful response elements</span></span>

<span data-ttu-id="c6808-128">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="c6808-128">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="c6808-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c6808-129">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="c6808-130">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="c6808-130">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="c6808-131">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c6808-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c6808-132">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c6808-132">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="c6808-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c6808-133">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c6808-134">Itens</span><span class="sxs-lookup"><span data-stu-id="c6808-134">Items</span></span>](items.md)
    
- [<span data-ttu-id="c6808-135">Mensagem</span><span class="sxs-lookup"><span data-stu-id="c6808-135">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="c6808-136">MimeContent</span><span class="sxs-lookup"><span data-stu-id="c6808-136">MimeContent</span></span>](mimecontent.md)
    
- [<span data-ttu-id="c6808-137">ItemId</span><span class="sxs-lookup"><span data-stu-id="c6808-137">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="c6808-138">Assunto</span><span class="sxs-lookup"><span data-stu-id="c6808-138">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="c6808-139">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="c6808-139">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="c6808-140">Body</span><span class="sxs-lookup"><span data-stu-id="c6808-140">Body</span></span>](body.md)
    
- [<span data-ttu-id="c6808-141">Tamanho</span><span class="sxs-lookup"><span data-stu-id="c6808-141">Size</span></span>](size.md)
    
- [<span data-ttu-id="c6808-142">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="c6808-142">DateTimeSent</span></span>](datetimesent.md)
    
- [<span data-ttu-id="c6808-143">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="c6808-143">DateTimeCreated</span></span>](datetimecreated.md)
    
- [<span data-ttu-id="c6808-144">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="c6808-144">ResponseObjects</span></span>](responseobjects.md)
    
- [<span data-ttu-id="c6808-145">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="c6808-145">ReplyToItem</span></span>](replytoitem.md)
    
- [<span data-ttu-id="c6808-146">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="c6808-146">ReplyAllToItem</span></span>](replyalltoitem.md)
    
- [<span data-ttu-id="c6808-147">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="c6808-147">ForwardItem</span></span>](forwarditem.md)
    
- [<span data-ttu-id="c6808-148">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="c6808-148">HasAttachments</span></span>](hasattachments.md)
    
- [<span data-ttu-id="c6808-149">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="c6808-149">ToRecipients</span></span>](torecipients.md)
    
- [<span data-ttu-id="c6808-150">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="c6808-150">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="c6808-151">Nome (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="c6808-151">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="c6808-152">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="c6808-152">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="c6808-153">RoutingType (EmailAddresstype)</span><span class="sxs-lookup"><span data-stu-id="c6808-153">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="c6808-154">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="c6808-154">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md)
    
- [<span data-ttu-id="c6808-155">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="c6808-155">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md)
    
- [<span data-ttu-id="c6808-156">De</span><span class="sxs-lookup"><span data-stu-id="c6808-156">From</span></span>](from.md)
    
- [<span data-ttu-id="c6808-157">IsRead</span><span class="sxs-lookup"><span data-stu-id="c6808-157">IsRead</span></span>](isread.md)
    
## <a name="getitem-e-mail-message-error-response-example"></a><span data-ttu-id="c6808-158">Exemplo de resposta de erro GetItem (mensagem de email)</span><span class="sxs-lookup"><span data-stu-id="c6808-158">GetItem (E-mail Message) Error response example</span></span>

### <a name="description"></a><span data-ttu-id="c6808-159">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6808-159">Description</span></span>

<span data-ttu-id="c6808-160">O exemplo a seguir mostra uma resposta de erro a uma solicitação GetItem.</span><span class="sxs-lookup"><span data-stu-id="c6808-160">The following example shows an error response to a GetItem request.</span></span> <span data-ttu-id="c6808-161">O erro foi causado por uma tentativa de obter uma propriedade adicional inválida.</span><span class="sxs-lookup"><span data-stu-id="c6808-161">The error was caused by an attempt to get an invalid additional property.</span></span>
  
### <a name="code"></a><span data-ttu-id="c6808-162">Código</span><span class="sxs-lookup"><span data-stu-id="c6808-162">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Error">
          <m:MessageText>Property is not valid for this object type.</m:MessageText>
          <m:ResponseCode>ErrorInvalidPropertyRequest</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:MessageXml>
            <t:FieldURI FieldURI="meeting:AssociatedCalendarItemId" />
          </m:MessageXml>
          <m:Items />
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="c6808-163">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="c6808-163">Error response elements</span></span>

<span data-ttu-id="c6808-164">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="c6808-164">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="c6808-165">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c6808-165">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="c6808-166">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="c6808-166">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="c6808-167">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c6808-167">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c6808-168">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c6808-168">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="c6808-169">MessageText</span><span class="sxs-lookup"><span data-stu-id="c6808-169">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="c6808-170">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c6808-170">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c6808-171">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c6808-171">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="c6808-172">MessageXml</span><span class="sxs-lookup"><span data-stu-id="c6808-172">MessageXml</span></span>](messagexml.md)
    
- [<span data-ttu-id="c6808-173">FieldURI</span><span class="sxs-lookup"><span data-stu-id="c6808-173">FieldURI</span></span>](fielduri.md)
    
## <a name="see-also"></a><span data-ttu-id="c6808-174">Confira também</span><span class="sxs-lookup"><span data-stu-id="c6808-174">See also</span></span>



[<span data-ttu-id="c6808-175">Operação GetItem</span><span class="sxs-lookup"><span data-stu-id="c6808-175">GetItem operation</span></span>](getitem-operation.md)

