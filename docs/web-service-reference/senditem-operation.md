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
description: A operação SendItem é usada para enviar mensagens de email que estão localizadas no armazenamento do Exchange.
ms.openlocfilehash: 780778b1599d0d5e5f4b6e5b58b67773bbe18cda
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19825336"
---
# <a name="senditem-operation"></a><span data-ttu-id="c4434-103">Operação SendItem</span><span class="sxs-lookup"><span data-stu-id="c4434-103">SendItem operation</span></span>

<span data-ttu-id="c4434-104">A operação SendItem é usada para enviar mensagens de email que estão localizadas no armazenamento do Exchange.</span><span class="sxs-lookup"><span data-stu-id="c4434-104">The SendItem operation is used to send e-mail messages that are located in the Exchange store.</span></span>
  
## <a name="senditem-e-mail-message-request-example"></a><span data-ttu-id="c4434-105">Exemplo de solicitação SendItem (mensagem de email)</span><span class="sxs-lookup"><span data-stu-id="c4434-105">SendItem (E-mail Message) request example</span></span>

### <a name="description"></a><span data-ttu-id="c4434-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4434-106">Description</span></span>

<span data-ttu-id="c4434-107">O exemplo a seguir mostra como enviar uma mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="c4434-107">The following example shows how to send an e-mail message.</span></span>
  
### <a name="code"></a><span data-ttu-id="c4434-108">Código</span><span class="sxs-lookup"><span data-stu-id="c4434-108">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SendItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
              SaveItemToFolder="true">
      <ItemIds>
        <t:ItemId Id="AAAtAEF=" ChangeKey="CQAAABY+T" />
      </ItemIds>
    </SendItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="c4434-109">Comments</span><span class="sxs-lookup"><span data-stu-id="c4434-109">Comments</span></span>

<span data-ttu-id="c4434-110">O identificador do item foi reduzido para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="c4434-110">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="c4434-111">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c4434-111">Request elements</span></span>

<span data-ttu-id="c4434-112">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="c4434-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="c4434-113">SendItem</span><span class="sxs-lookup"><span data-stu-id="c4434-113">SendItem</span></span>](senditem.md)
    
- [<span data-ttu-id="c4434-114">ItemIds</span><span class="sxs-lookup"><span data-stu-id="c4434-114">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="c4434-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="c4434-115">ItemId</span></span>](itemid.md)
    
## <a name="successful-senditem-e-mail-message-response"></a><span data-ttu-id="c4434-116">Resposta bem-sucedida SendItem (mensagem de email)</span><span class="sxs-lookup"><span data-stu-id="c4434-116">Successful SendItem (E-mail Message) Response</span></span>

### <a name="description"></a><span data-ttu-id="c4434-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4434-117">Description</span></span>

<span data-ttu-id="c4434-118">O exemplo a seguir mostra uma resposta SendItem bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="c4434-118">The following example shows a successful SendItem response.</span></span>
  
### <a name="code"></a><span data-ttu-id="c4434-119">Código</span><span class="sxs-lookup"><span data-stu-id="c4434-119">Code</span></span>

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
    <SendItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </SendItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="c4434-120">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="c4434-120">Successful response elements</span></span>

<span data-ttu-id="c4434-121">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="c4434-121">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="c4434-122">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c4434-122">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="c4434-123">SendItemResponse</span><span class="sxs-lookup"><span data-stu-id="c4434-123">SendItemResponse</span></span>](senditemresponse.md)
    
- [<span data-ttu-id="c4434-124">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c4434-124">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c4434-125">SendItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c4434-125">SendItemResponseMessage</span></span>](senditemresponsemessage.md)
    
- [<span data-ttu-id="c4434-126">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c4434-126">ResponseCode</span></span>](responsecode.md)
    
### <a name="comments"></a><span data-ttu-id="c4434-127">Comments</span><span class="sxs-lookup"><span data-stu-id="c4434-127">Comments</span></span>

<span data-ttu-id="c4434-128">Um delegado que tenta enviar uma mensagem de email que está localizada na pasta Rascunhos da entidade de segurança com a opção de SendAndSaveCopy definida para salvar uma cópia na pasta distinta falhará silenciosamente para mover uma cópia do item enviado para itens enviados diferenciado enviadas itens pasta.</span><span class="sxs-lookup"><span data-stu-id="c4434-128">A delegate who tries to send an e-mail message that is located in the principal's Drafts folder with the SendAndSaveCopy option set to save a copy in the Sent Items distinguished folder will silently fail to move a copy of the sent item to the Sent Items distinguished folder.</span></span> <span data-ttu-id="c4434-129">O item permanecerá na pasta Rascunhos do principal.</span><span class="sxs-lookup"><span data-stu-id="c4434-129">The item will remain in the principal's Drafts folder.</span></span> <span data-ttu-id="c4434-130">A solução alternativa para esse problema é especificar a caixa de correio da entidade de segurança no elemento [DistinguishedFolderId](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="c4434-130">The workaround for this issue is to specify the principal's mailbox in the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span> 
  
<span data-ttu-id="c4434-131">Um cenário adicional a serem considerados é quando um delegado cria uma mensagem de email e o salva na pasta Rascunhos da caixa de correio do representante.</span><span class="sxs-lookup"><span data-stu-id="c4434-131">An additional scenario to consider is when a delegate creates an e-mail message and saves it to the Drafts folder of the delegate's mailbox.</span></span> <span data-ttu-id="c4434-132">Se o representante tenta enviar o item e salvar uma cópia para pasta distinto de itens enviados do principal, a mensagem é enviada corretamente, que a mensagem de rascunho permanece na pasta Rascunhos do representante, a mensagem enviada não aparecem do representante ou da entidade de segurança Pasta Itens enviados e a resposta é um sucesso.</span><span class="sxs-lookup"><span data-stu-id="c4434-132">If the delegate tries to send the item and save a copy to the principal's Sent Items distinguished folder, the message is sent correctly, the draft message remains in the delegate's Drafts folder, the sent message does not appear in either the delegate's or principal's Sent Items folder, and the response is a success.</span></span>
  
## <a name="invalid-senditem-e-mail-message-request-example"></a><span data-ttu-id="c4434-133">Exemplo de solicitação inválido SendItem (mensagem de email)</span><span class="sxs-lookup"><span data-stu-id="c4434-133">Invalid SendItem (E-mail Message) request example</span></span>

### <a name="description"></a><span data-ttu-id="c4434-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4434-134">Description</span></span>

<span data-ttu-id="c4434-135">O exemplo de código a seguir mostra um exemplo de uma solicitação com um identificador inválido.</span><span class="sxs-lookup"><span data-stu-id="c4434-135">The following code sample shows an example of a request with an invalid identifier.</span></span>
  
### <a name="code"></a><span data-ttu-id="c4434-136">Código</span><span class="sxs-lookup"><span data-stu-id="c4434-136">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SendItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
              SaveItemToFolder="true">
      <ItemIds>
        <t:ItemId Id="%BadItemId%" ChangeKey="CQAAABYAAA" />
      </ItemIds>
    </SendItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="senditem-e-mail-message-error-response"></a><span data-ttu-id="c4434-137">Resposta de erro SendItem (mensagem de email)</span><span class="sxs-lookup"><span data-stu-id="c4434-137">SendItem (E-mail Message) error response</span></span>

### <a name="description"></a><span data-ttu-id="c4434-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4434-138">Description</span></span>

<span data-ttu-id="c4434-139">O exemplo a seguir mostra uma resposta de erro a uma solicitação de SendItem que contém um identificador inválido.</span><span class="sxs-lookup"><span data-stu-id="c4434-139">The following example shows an error response to a SendItem request that contains an invalid identifier.</span></span>
  
### <a name="code"></a><span data-ttu-id="c4434-140">Código</span><span class="sxs-lookup"><span data-stu-id="c4434-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SendItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="c4434-141">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="c4434-141">Error response elements</span></span>

<span data-ttu-id="c4434-142">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="c4434-142">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="c4434-143">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c4434-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="c4434-144">SendItemResponse</span><span class="sxs-lookup"><span data-stu-id="c4434-144">SendItemResponse</span></span>](senditemresponse.md)
    
- [<span data-ttu-id="c4434-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c4434-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c4434-146">SendItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c4434-146">SendItemResponseMessage</span></span>](senditemresponsemessage.md)
    
- [<span data-ttu-id="c4434-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="c4434-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="c4434-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c4434-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c4434-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c4434-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="c4434-150">Confira também</span><span class="sxs-lookup"><span data-stu-id="c4434-150">See also</span></span>



[<span data-ttu-id="c4434-151">Operação SendItem</span><span class="sxs-lookup"><span data-stu-id="c4434-151">SendItem operation</span></span>](senditem-operation.md)
  
 <span data-ttu-id="c4434-152">**SendItemType**</span><span class="sxs-lookup"><span data-stu-id="c4434-152">**SendItemType**</span></span>


- [<span data-ttu-id="c4434-153">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c4434-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

