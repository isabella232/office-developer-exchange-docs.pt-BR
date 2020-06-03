---
title: Operação SendItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItem
api_type:
- schema
ms.assetid: 337b89ef-e1b7-45ed-92f3-8abe4200e4c7
description: A operação SendItem é usada para enviar mensagens de email que estão localizadas no repositório do Exchange.
ms.openlocfilehash: 9136379e50723211fe5a483c7f113da4fa125fc1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530335"
---
# <a name="senditem-operation"></a><span data-ttu-id="9c380-103">Operação SendItem</span><span class="sxs-lookup"><span data-stu-id="9c380-103">SendItem operation</span></span>

<span data-ttu-id="9c380-104">A operação SendItem é usada para enviar mensagens de email que estão localizadas no repositório do Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c380-104">The SendItem operation is used to send e-mail messages that are located in the Exchange store.</span></span>
  
## <a name="senditem-e-mail-message-request-example"></a><span data-ttu-id="9c380-105">Exemplo de solicitação SendItem (mensagem de email)</span><span class="sxs-lookup"><span data-stu-id="9c380-105">SendItem (E-mail Message) request example</span></span>

### <a name="description"></a><span data-ttu-id="9c380-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c380-106">Description</span></span>

<span data-ttu-id="9c380-107">O exemplo a seguir mostra como enviar uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="9c380-107">The following example shows how to send an e-mail message.</span></span>
  
### <a name="code"></a><span data-ttu-id="9c380-108">Código</span><span class="sxs-lookup"><span data-stu-id="9c380-108">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SendItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
              SaveItemToFolder="true">
      <ItemIds>
        <t:ItemId Id="AAAtAEF=" ChangeKey="CQAAABY+T" />
      </ItemIds>
    </SendItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="9c380-109">Comentários</span><span class="sxs-lookup"><span data-stu-id="9c380-109">Comments</span></span>

<span data-ttu-id="9c380-110">O identificador de item foi reduzido para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9c380-110">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="9c380-111">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="9c380-111">Request elements</span></span>

<span data-ttu-id="9c380-112">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="9c380-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="9c380-113">SendItem</span><span class="sxs-lookup"><span data-stu-id="9c380-113">SendItem</span></span>](senditem.md)
    
- [<span data-ttu-id="9c380-114">ItemIds</span><span class="sxs-lookup"><span data-stu-id="9c380-114">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="9c380-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="9c380-115">ItemId</span></span>](itemid.md)
    
## <a name="successful-senditem-e-mail-message-response"></a><span data-ttu-id="9c380-116">Resposta SendItem (mensagem de email) bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="9c380-116">Successful SendItem (E-mail Message) Response</span></span>

### <a name="description"></a><span data-ttu-id="9c380-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c380-117">Description</span></span>

<span data-ttu-id="9c380-118">O exemplo a seguir mostra uma resposta SendItem bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="9c380-118">The following example shows a successful SendItem response.</span></span>
  
### <a name="code"></a><span data-ttu-id="9c380-119">Código</span><span class="sxs-lookup"><span data-stu-id="9c380-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SendItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </SendItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="9c380-120">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="9c380-120">Successful response elements</span></span>

<span data-ttu-id="9c380-121">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="9c380-121">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="9c380-122">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="9c380-122">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="9c380-123">SendItemResponse</span><span class="sxs-lookup"><span data-stu-id="9c380-123">SendItemResponse</span></span>](senditemresponse.md)
    
- [<span data-ttu-id="9c380-124">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9c380-124">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="9c380-125">SendItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9c380-125">SendItemResponseMessage</span></span>](senditemresponsemessage.md)
    
- [<span data-ttu-id="9c380-126">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9c380-126">ResponseCode</span></span>](responsecode.md)
    
### <a name="comments"></a><span data-ttu-id="9c380-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="9c380-127">Comments</span></span>

<span data-ttu-id="9c380-128">Um representante que tentar enviar uma mensagem de email que está localizado na pasta Rascunhos da entidade de segurança com a opção SendAndSaveCopy definida para salvar uma cópia na pasta distinta de itens enviados, falhará silenciosamente, para mover uma cópia do item enviado para a pasta distinta itens enviados.</span><span class="sxs-lookup"><span data-stu-id="9c380-128">A delegate who tries to send an e-mail message that is located in the principal's Drafts folder with the SendAndSaveCopy option set to save a copy in the Sent Items distinguished folder will silently fail to move a copy of the sent item to the Sent Items distinguished folder.</span></span> <span data-ttu-id="9c380-129">O item permanecerá na pasta Rascunhos da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="9c380-129">The item will remain in the principal's Drafts folder.</span></span> <span data-ttu-id="9c380-130">A solução alternativa para esse problema é especificar a caixa de correio da entidade de segurança no elemento [DistinguishedFolderId](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="9c380-130">The workaround for this issue is to specify the principal's mailbox in the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span> 
  
<span data-ttu-id="9c380-131">Um cenário adicional a ser considerado é quando um representante cria uma mensagem de email e a salva na pasta Rascunhos da caixa de correio do representante.</span><span class="sxs-lookup"><span data-stu-id="9c380-131">An additional scenario to consider is when a delegate creates an e-mail message and saves it to the Drafts folder of the delegate's mailbox.</span></span> <span data-ttu-id="9c380-132">Se o representante tentar enviar o item e salvar uma cópia na pasta distinta de itens enviados da entidade de segurança, a mensagem será enviada corretamente, a mensagem de rascunho permanecerá na pasta Rascunhos do representante, a mensagem enviada não aparecerá na pasta Itens enviados do representante ou da entidade de segurança e a resposta será um êxito.</span><span class="sxs-lookup"><span data-stu-id="9c380-132">If the delegate tries to send the item and save a copy to the principal's Sent Items distinguished folder, the message is sent correctly, the draft message remains in the delegate's Drafts folder, the sent message does not appear in either the delegate's or principal's Sent Items folder, and the response is a success.</span></span>
  
## <a name="invalid-senditem-e-mail-message-request-example"></a><span data-ttu-id="9c380-133">Exemplo de solicitação SendItem (mensagem de email) inválida</span><span class="sxs-lookup"><span data-stu-id="9c380-133">Invalid SendItem (E-mail Message) request example</span></span>

### <a name="description"></a><span data-ttu-id="9c380-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c380-134">Description</span></span>

<span data-ttu-id="9c380-135">O exemplo de código a seguir mostra um exemplo de uma solicitação com um identificador inválido.</span><span class="sxs-lookup"><span data-stu-id="9c380-135">The following code sample shows an example of a request with an invalid identifier.</span></span>
  
### <a name="code"></a><span data-ttu-id="9c380-136">Código</span><span class="sxs-lookup"><span data-stu-id="9c380-136">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SendItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
              SaveItemToFolder="true">
      <ItemIds>
        <t:ItemId Id="%BadItemId%" ChangeKey="CQAAABYAAA" />
      </ItemIds>
    </SendItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="senditem-e-mail-message-error-response"></a><span data-ttu-id="9c380-137">Resposta de erro SendItem (mensagem de email)</span><span class="sxs-lookup"><span data-stu-id="9c380-137">SendItem (E-mail Message) error response</span></span>

### <a name="description"></a><span data-ttu-id="9c380-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c380-138">Description</span></span>

<span data-ttu-id="9c380-139">O exemplo a seguir mostra uma resposta de erro a uma solicitação de SendItem que contém um identificador inválido.</span><span class="sxs-lookup"><span data-stu-id="9c380-139">The following example shows an error response to a SendItem request that contains an invalid identifier.</span></span>
  
### <a name="code"></a><span data-ttu-id="9c380-140">Código</span><span class="sxs-lookup"><span data-stu-id="9c380-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SendItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </SendItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="9c380-141">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="9c380-141">Error response elements</span></span>

<span data-ttu-id="9c380-142">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="9c380-142">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="9c380-143">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="9c380-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="9c380-144">SendItemResponse</span><span class="sxs-lookup"><span data-stu-id="9c380-144">SendItemResponse</span></span>](senditemresponse.md)
    
- [<span data-ttu-id="9c380-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9c380-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="9c380-146">SendItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9c380-146">SendItemResponseMessage</span></span>](senditemresponsemessage.md)
    
- [<span data-ttu-id="9c380-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="9c380-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="9c380-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9c380-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="9c380-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="9c380-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="9c380-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="9c380-150">See also</span></span>



[<span data-ttu-id="9c380-151">Operação SendItem</span><span class="sxs-lookup"><span data-stu-id="9c380-151">SendItem operation</span></span>](senditem-operation.md)
  
 <span data-ttu-id="9c380-152">**SendItemType**</span><span class="sxs-lookup"><span data-stu-id="9c380-152">**SendItemType**</span></span>


- [<span data-ttu-id="9c380-153">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9c380-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

