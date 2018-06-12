---
title: Operação UpdateItem (contato)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 298fdd71-a83d-4407-9728-4f0a8e2d857c
description: A operação UpdateItem é usada para atualizar as propriedades de item de contato no armazenamento do Exchange.
ms.openlocfilehash: f2a501ce8e69068cd30b58011adf4defc68ce365
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837908"
---
# <a name="updateitem-operation-contact"></a><span data-ttu-id="5694c-103">Operação UpdateItem (contato)</span><span class="sxs-lookup"><span data-stu-id="5694c-103">UpdateItem operation (contact)</span></span>

<span data-ttu-id="5694c-104">A operação UpdateItem é usada para atualizar as propriedades de item de contato no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="5694c-104">The UpdateItem operation is used to update contact item properties in the Exchange store.</span></span>
  
## <a name="updateitem-contact-request-example"></a><span data-ttu-id="5694c-105">Exemplo de solicitação UpdateItem (contato)</span><span class="sxs-lookup"><span data-stu-id="5694c-105">UpdateItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="5694c-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="5694c-106">Description</span></span>

<span data-ttu-id="5694c-107">O exemplo de código a seguir mostra como atualizar o endereço de email de um contato.</span><span class="sxs-lookup"><span data-stu-id="5694c-107">The following code example shows how to update the e-mail address of a contact.</span></span>
  
### <a name="code"></a><span data-ttu-id="5694c-108">Código</span><span class="sxs-lookup"><span data-stu-id="5694c-108">Code</span></span>

```XML
<soap:Envelope
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                ConflictResolution="AlwaysOverwrite">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAA=" ChangeKey="EQAAABYi" />
          <t:Updates>
            <t:SetItemField>
              <t:IndexedFieldURI FieldURI="contacts:EmailAddress" FieldIndex="EmailAddress1"/>
              <t:Contact>
                <t:EmailAddresses>
                  <t:Entry Key="EmailAddress1">changedemail@example.com</t:Entry>
                </t:EmailAddresses>
              </t:Contact>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="5694c-109">Comments</span><span class="sxs-lookup"><span data-stu-id="5694c-109">Comments</span></span>

<span data-ttu-id="5694c-110">O identificador do item foi reduzido para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5694c-110">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="5694c-111">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5694c-111">Request elements</span></span>

<span data-ttu-id="5694c-112">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="5694c-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="5694c-113">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="5694c-113">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="5694c-114">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="5694c-114">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="5694c-115">ItemChange</span><span class="sxs-lookup"><span data-stu-id="5694c-115">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="5694c-116">ItemId</span><span class="sxs-lookup"><span data-stu-id="5694c-116">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="5694c-117">Atualizações (Item)</span><span class="sxs-lookup"><span data-stu-id="5694c-117">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="5694c-118">SetItemField</span><span class="sxs-lookup"><span data-stu-id="5694c-118">SetItemField</span></span>](setitemfield.md)
    
- [<span data-ttu-id="5694c-119">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="5694c-119">IndexedFieldURI</span></span>](indexedfielduri.md)
    
- [<span data-ttu-id="5694c-120">Contato</span><span class="sxs-lookup"><span data-stu-id="5694c-120">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="5694c-121">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="5694c-121">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="5694c-122">Entrada (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="5694c-122">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
## <a name="successful-updateitem-contact-response"></a><span data-ttu-id="5694c-123">Resposta bem-sucedida UpdateItem (contato)</span><span class="sxs-lookup"><span data-stu-id="5694c-123">Successful UpdateItem (Contact) Response</span></span>

### <a name="description"></a><span data-ttu-id="5694c-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5694c-124">Description</span></span>

<span data-ttu-id="5694c-125">O exemplo de código a seguir mostra uma resposta UpdateItem bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="5694c-125">The following code example shows a successful UpdateItem response.</span></span>
  
### <a name="code"></a><span data-ttu-id="5694c-126">Código</span><span class="sxs-lookup"><span data-stu-id="5694c-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UpdateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAtAE=" ChangeKey="EQAAABYx" />
            </t:Contact>
          </m:Items>
        </m:UpdateItemResponseMessage>
      </m:ResponseMessages>
    </UpdateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="5694c-127">Comments</span><span class="sxs-lookup"><span data-stu-id="5694c-127">Comments</span></span>

<span data-ttu-id="5694c-128">O identificador do item foi reduzido para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5694c-128">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="5694c-129">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="5694c-129">Successful response elements</span></span>

<span data-ttu-id="5694c-130">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="5694c-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="5694c-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5694c-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5694c-132">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="5694c-132">UpdateItemResponse</span></span>](updateitemresponse.md)
    
- [<span data-ttu-id="5694c-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5694c-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5694c-134">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5694c-134">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
    
- [<span data-ttu-id="5694c-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5694c-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5694c-136">Itens (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="5694c-136">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="5694c-137">Contato</span><span class="sxs-lookup"><span data-stu-id="5694c-137">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="5694c-138">ItemId</span><span class="sxs-lookup"><span data-stu-id="5694c-138">ItemId</span></span>](itemid.md)
    
## <a name="invalid-updateitem-contact-request-example"></a><span data-ttu-id="5694c-139">Exemplo de solicitação inválido UpdateItem (contato)</span><span class="sxs-lookup"><span data-stu-id="5694c-139">Invalid UpdateItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="5694c-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="5694c-140">Description</span></span>

<span data-ttu-id="5694c-141">O exemplo de código a seguir mostra uma solicitação inválida.</span><span class="sxs-lookup"><span data-stu-id="5694c-141">The following code example shows an invalid request.</span></span>
  
### <a name="code"></a><span data-ttu-id="5694c-142">Código</span><span class="sxs-lookup"><span data-stu-id="5694c-142">Code</span></span>

```XML
<soap:Envelope
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                ConflictResolution="AlwaysOverwrite">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEF=" ChangeKey="EQAAABYi" />
          <t:Updates>
            <t:SetItemField>
              <t:IndexedFieldURI FieldURI="contacts:EmailAddress" FieldIndex="EmailAddress4"/>
              <t:Contact>
                <t:EmailAddresses>
                  <t:Entry Key="EmailAddress4">changedemail2@example.com</t:Entry>
                </t:EmailAddresses>
              </t:Contact>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="5694c-143">Comments</span><span class="sxs-lookup"><span data-stu-id="5694c-143">Comments</span></span>

<span data-ttu-id="5694c-144">O identificador do item foi reduzido para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="5694c-144">The item identifier has been shortened to preserve readability.</span></span>
  
## <a name="updateitem-contact-error-response"></a><span data-ttu-id="5694c-145">Resposta de erro UpdateItem (contato)</span><span class="sxs-lookup"><span data-stu-id="5694c-145">UpdateItem (Contact) error response</span></span>

### <a name="description"></a><span data-ttu-id="5694c-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="5694c-146">Description</span></span>

<span data-ttu-id="5694c-147">O exemplo de código a seguir mostra uma resposta de erro a uma solicitação de UpdateItem (contato).</span><span class="sxs-lookup"><span data-stu-id="5694c-147">The following code example shows an error response to an UpdateItem (Contact) request.</span></span>
  
### <a name="code"></a><span data-ttu-id="5694c-148">Código</span><span class="sxs-lookup"><span data-stu-id="5694c-148">Code</span></span>

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <soap:Fault>
      <soap:faultcode>Client</soap:faultcode>
      <soap:faultstring>The request failed schema validation.</soap:faultstring>
      <detail>
        <e:ResponseCode xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
        <e:Message xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">The 'Key' attribute is invalid - The value 'EmailAddress4' is invalid according to its data type 'http://schemas.microsoft.com/exchange/services/2006/types:EmailAddressKeyType' - The Enumeration constraint failed.</e:Message>
        <e:Line xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">17</e:Line>
        <e:Position xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">19</e:Position>
      </detail>
    </soap:Fault>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="5694c-149">Comments</span><span class="sxs-lookup"><span data-stu-id="5694c-149">Comments</span></span>

<span data-ttu-id="5694c-150">Alguns elementos que são usados no corpo SOAP de uma resposta de erro é gerado por um erro de validação de esquema não estão definidos em esquemas de mensagens ou tipos.</span><span class="sxs-lookup"><span data-stu-id="5694c-150">Some elements that are used in the SOAP body of an error response that is caused by a schema validation error are not defined in the messages or types schemas.</span></span> <span data-ttu-id="5694c-151">O elemento de **detalhe** contém informações sobre o erro.</span><span class="sxs-lookup"><span data-stu-id="5694c-151">The **detail** element contains information about the error.</span></span> <span data-ttu-id="5694c-152">O elemento [ResponseCode](responsecode.md) contém o código de erro.</span><span class="sxs-lookup"><span data-stu-id="5694c-152">The [ResponseCode](responsecode.md) element contains the error code.</span></span> <span data-ttu-id="5694c-153">O elemento de [mensagem](message-ex15websvcsotherref.md) contém uma explicação para o erro, caso alguma esteja disponível.</span><span class="sxs-lookup"><span data-stu-id="5694c-153">The [Message](message-ex15websvcsotherref.md) element contains an explanation for the error, if one is available.</span></span> <span data-ttu-id="5694c-154">O elemento de **linha** descreve o número da linha onde ocorreu o erro de validação de esquema.</span><span class="sxs-lookup"><span data-stu-id="5694c-154">The **Line** element describes the line number where the schema validation error occurred.</span></span> <span data-ttu-id="5694c-155">O elemento de **posição** descreve a posição do caractere mais à esquerda do documento XML.</span><span class="sxs-lookup"><span data-stu-id="5694c-155">The **Position** element describes the position from the leftmost character of the XML document.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="5694c-156">Confira também</span><span class="sxs-lookup"><span data-stu-id="5694c-156">See also</span></span>



[<span data-ttu-id="5694c-157">Operação UpdateItem</span><span class="sxs-lookup"><span data-stu-id="5694c-157">UpdateItem operation</span></span>](updateitem-operation.md)

