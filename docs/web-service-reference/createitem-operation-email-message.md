---
title: Operação CreateItem (mensagem de email)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1
description: A operação CreateItem é usada para criar mensagens de email.
ms.openlocfilehash: 384ed8ff653029c2b7db0b36986d85842b0a06cf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457113"
---
# <a name="createitem-operation-email-message"></a><span data-ttu-id="f3bd3-103">Operação CreateItem (mensagem de email)</span><span class="sxs-lookup"><span data-stu-id="f3bd3-103">CreateItem operation (email message)</span></span>

<span data-ttu-id="f3bd3-104">A operação CreateItem é usada para criar mensagens de email.</span><span class="sxs-lookup"><span data-stu-id="f3bd3-104">The CreateItem operation is used to create e-mail messages.</span></span>
  
## <a name="createitem-request-example"></a><span data-ttu-id="f3bd3-105">Exemplo de solicitação CreateItem</span><span class="sxs-lookup"><span data-stu-id="f3bd3-105">CreateItem request example</span></span>

### <a name="description"></a><span data-ttu-id="f3bd3-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3bd3-106">Description</span></span>

<span data-ttu-id="f3bd3-107">O exemplo a seguir de uma solicitação CreateItem mostra como criar uma nova mensagem de email, enviar a mensagem e salvar uma cópia dela na pasta Rascunhos.</span><span class="sxs-lookup"><span data-stu-id="f3bd3-107">The following example of a CreateItem request shows how to create a new e-mail message, send the message, and save a copy of it in the drafts folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="f3bd3-108">Código</span><span class="sxs-lookup"><span data-stu-id="f3bd3-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem MessageDisposition="SendAndSaveCopy" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts" />
      </SavedItemFolderId>
      <Items>
        <t:Message>
          <t:ItemClass>IPM.Note</t:ItemClass>
          <t:Subject>Project Action</t:Subject>
          <t:Body BodyType="Text">Priority - Update specification</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sschmidt@example.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
          <t:IsRead>false</t:IsRead>
        </t:Message>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="f3bd3-109">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="f3bd3-109">Request elements</span></span>

<span data-ttu-id="f3bd3-110">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="f3bd3-110">The following elements are used in the request:</span></span> 
  
- [<span data-ttu-id="f3bd3-111">CreateItem</span><span class="sxs-lookup"><span data-stu-id="f3bd3-111">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="f3bd3-112">SavedItemFolderId</span><span class="sxs-lookup"><span data-stu-id="f3bd3-112">SavedItemFolderId</span></span>](saveditemfolderid.md)
    
- [<span data-ttu-id="f3bd3-113">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="f3bd3-113">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="f3bd3-114">Message</span><span class="sxs-lookup"><span data-stu-id="f3bd3-114">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="f3bd3-115">ItemClass</span><span class="sxs-lookup"><span data-stu-id="f3bd3-115">ItemClass</span></span>](itemclass.md)
    
- [<span data-ttu-id="f3bd3-116">Assunto</span><span class="sxs-lookup"><span data-stu-id="f3bd3-116">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="f3bd3-117">Body</span><span class="sxs-lookup"><span data-stu-id="f3bd3-117">Body</span></span>](body.md)
    
- [<span data-ttu-id="f3bd3-118">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="f3bd3-118">ToRecipients</span></span>](torecipients.md)
    
- [<span data-ttu-id="f3bd3-119">Caixa de Correio</span><span class="sxs-lookup"><span data-stu-id="f3bd3-119">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="f3bd3-120">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="f3bd3-120">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="f3bd3-121">IsRead</span><span class="sxs-lookup"><span data-stu-id="f3bd3-121">IsRead</span></span>](isread.md)
    
<span data-ttu-id="f3bd3-122">Para encontrar outras opções para a mensagem de solicitação da operação CreateItem, explore a hierarquia do esquema.</span><span class="sxs-lookup"><span data-stu-id="f3bd3-122">To find other options for the request message of the CreateItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="f3bd3-123">Inicie no elemento [CreateItem](createitem.md) .</span><span class="sxs-lookup"><span data-stu-id="f3bd3-123">Start at the [CreateItem](createitem.md) element.</span></span> 
  
## <a name="successful-createitem-response"></a><span data-ttu-id="f3bd3-124">Resposta CreateItem bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="f3bd3-124">Successful CreateItem Response</span></span>

### <a name="description"></a><span data-ttu-id="f3bd3-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3bd3-125">Description</span></span>

<span data-ttu-id="f3bd3-126">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação CreateItem.</span><span class="sxs-lookup"><span data-stu-id="f3bd3-126">The following example shows a successful response to the CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="f3bd3-127">Código</span><span class="sxs-lookup"><span data-stu-id="f3bd3-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="f3bd3-128">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="f3bd3-128">Successful response elements</span></span>

<span data-ttu-id="f3bd3-129">Os seguintes elementos estão incluídos na resposta:</span><span class="sxs-lookup"><span data-stu-id="f3bd3-129">The following elements are included in the response:</span></span> 
  
- [<span data-ttu-id="f3bd3-130">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="f3bd3-130">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="f3bd3-131">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f3bd3-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="f3bd3-132">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f3bd3-132">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="f3bd3-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f3bd3-133">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f3bd3-134">Itens</span><span class="sxs-lookup"><span data-stu-id="f3bd3-134">Items</span></span>](items.md)
    
<span data-ttu-id="f3bd3-135">Para encontrar outras opções para a mensagem de resposta da operação CreateItem, explore a hierarquia do esquema.</span><span class="sxs-lookup"><span data-stu-id="f3bd3-135">To find other options for the response message of the CreateItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="f3bd3-136">Inicie no elemento [CreateItemResponse](createitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="f3bd3-136">Start at the [CreateItemResponse](createitemresponse.md) element.</span></span> 
  
## <a name="error-createitem-response"></a><span data-ttu-id="f3bd3-137">Resposta de erro CreateItem</span><span class="sxs-lookup"><span data-stu-id="f3bd3-137">Error CreateItem Response</span></span>

### <a name="description"></a><span data-ttu-id="f3bd3-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3bd3-138">Description</span></span>

<span data-ttu-id="f3bd3-139">O exemplo a seguir mostra uma resposta de erro a uma solicitação CreateItem.</span><span class="sxs-lookup"><span data-stu-id="f3bd3-139">The following example shows an error response to a CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="f3bd3-140">Código</span><span class="sxs-lookup"><span data-stu-id="f3bd3-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Error">
          <m:MessageText>The user account which was used to submit this request does not have the right to send mail on behalf of the specified sending account.</m:MessageText>
          <m:ResponseCode>ErrorSendAsDenied</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="f3bd3-141">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="f3bd3-141">Error response elements</span></span>

<span data-ttu-id="f3bd3-142">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="f3bd3-142">The following elements are used in the error response:</span></span> 
  
- [<span data-ttu-id="f3bd3-143">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="f3bd3-143">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="f3bd3-144">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f3bd3-144">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="f3bd3-145">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f3bd3-145">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="f3bd3-146">MessageText</span><span class="sxs-lookup"><span data-stu-id="f3bd3-146">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="f3bd3-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f3bd3-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f3bd3-148">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f3bd3-148">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="f3bd3-149">Itens</span><span class="sxs-lookup"><span data-stu-id="f3bd3-149">Items</span></span>](items.md)
    
<span data-ttu-id="f3bd3-150">Para encontrar outras opções para a mensagem de resposta de erro da operação CreateItem, explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="f3bd3-150">To find other options for the error response message of the CreateItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="f3bd3-151">Inicie no elemento [CreateItemResponse](createitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="f3bd3-151">Start at the [CreateItemResponse](createitemresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="f3bd3-152">Também consulte</span><span class="sxs-lookup"><span data-stu-id="f3bd3-152">See also</span></span>



[<span data-ttu-id="f3bd3-153">Operação CreateItem</span><span class="sxs-lookup"><span data-stu-id="f3bd3-153">CreateItem operation</span></span>](createitem-operation.md)

