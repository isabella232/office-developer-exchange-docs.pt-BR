---
title: Operação CopyItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyItem
api_type:
- schema
ms.assetid: bcc68f9e-d511-4c29-bba6-ed535524624a
description: A operação CopyItem copia os itens e coloca os itens em uma pasta diferente.
ms.openlocfilehash: 95d2371e9185aa25f40eaec37dda54276a54d321
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751551"
---
# <a name="copyitem-operation"></a><span data-ttu-id="e4dfa-103">Operação CopyItem</span><span class="sxs-lookup"><span data-stu-id="e4dfa-103">CopyItem operation</span></span>

<span data-ttu-id="e4dfa-104">A operação **CopyItem** copia os itens e coloca os itens em uma pasta diferente.</span><span class="sxs-lookup"><span data-stu-id="e4dfa-104">The **CopyItem** operation copies items and puts the items in a different folder.</span></span> 
  
## <a name="copyitem-request-example"></a><span data-ttu-id="e4dfa-105">Exemplo de solicitação de CopyItem</span><span class="sxs-lookup"><span data-stu-id="e4dfa-105">CopyItem request example</span></span>

### <a name="description"></a><span data-ttu-id="e4dfa-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4dfa-106">Description</span></span>

<span data-ttu-id="e4dfa-107">O exemplo a seguir de uma solicitação de **CopyItem** mostra como uma solicitação para copiar um item para a caixa de entrada de formulário.</span><span class="sxs-lookup"><span data-stu-id="e4dfa-107">The following example of a **CopyItem** request shows how to form a request to copy an item to the Inbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="e4dfa-108">Código</span><span class="sxs-lookup"><span data-stu-id="e4dfa-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CopyItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </ToFolderId>
      <ItemIds>
        <t:ItemId Id="AS4AUnV="/>
      </ItemIds>
    </CopyItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="e4dfa-109">Comments</span><span class="sxs-lookup"><span data-stu-id="e4dfa-109">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="e4dfa-110">A ID de pasta e a chave de alteração tem sido reduzidas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e4dfa-110">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="e4dfa-111">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e4dfa-111">Request elements</span></span>

<span data-ttu-id="e4dfa-112">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="e4dfa-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="e4dfa-113">CopyItem</span><span class="sxs-lookup"><span data-stu-id="e4dfa-113">CopyItem</span></span>](copyitem.md)
    
- [<span data-ttu-id="e4dfa-114">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="e4dfa-114">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="e4dfa-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="e4dfa-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="e4dfa-116">ItemIds</span><span class="sxs-lookup"><span data-stu-id="e4dfa-116">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="e4dfa-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="e4dfa-117">ItemId</span></span>](itemid.md)
    
> [!NOTE]
> <span data-ttu-id="e4dfa-118">O esquema que descreve este elemento está localizado no diretório virtual EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor acesso para cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="e4dfa-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="e4dfa-119">Para localizar outras opções para a mensagem de solicitação da operação **CopyItem** , explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="e4dfa-119">To find other options for the request message of the **CopyItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="e4dfa-120">Inicie o elemento [CopyItem](copyitem.md) .</span><span class="sxs-lookup"><span data-stu-id="e4dfa-120">Start at the [CopyItem](copyitem.md) element.</span></span> 
  
## <a name="successful-copyitem-response"></a><span data-ttu-id="e4dfa-121">Resposta de CopyItem bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="e4dfa-121">Successful CopyItem Response</span></span>

### <a name="description"></a><span data-ttu-id="e4dfa-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4dfa-122">Description</span></span>

<span data-ttu-id="e4dfa-123">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação de **CopyItem** .</span><span class="sxs-lookup"><span data-stu-id="e4dfa-123">The following example shows a successful response to the **CopyItem** request.</span></span> 
  
<span data-ttu-id="e4dfa-124">O identificador do item do novo item será retornado na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="e4dfa-124">The item identifier of the new item is returned in the response message.</span></span> <span data-ttu-id="e4dfa-125">Identificadores de item não são retornados em respostas em entre caixas de correio ou de caixa de correio para operações de **CopyItem** de pasta pública.</span><span class="sxs-lookup"><span data-stu-id="e4dfa-125">Item identifiers are not returned in responses for cross-mailbox or mailbox to public folder **CopyItem** operations.</span></span> 
  
### <a name="code"></a><span data-ttu-id="e4dfa-126">Código</span><span class="sxs-lookup"><span data-stu-id="e4dfa-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemID Id="AAMkAd" ChangeKey="FwAAABY" />
            </t:Message>
          </m:Items>
        </m:CopyItemResponseMessage>
      </m:ResponseMessages>
    </CopyItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="e4dfa-127">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="e4dfa-127">Successful response elements</span></span>

<span data-ttu-id="e4dfa-128">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="e4dfa-128">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="e4dfa-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e4dfa-129">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="e4dfa-130">CopyItemResponse</span><span class="sxs-lookup"><span data-stu-id="e4dfa-130">CopyItemResponse</span></span>](copyitemresponse.md)
    
- [<span data-ttu-id="e4dfa-131">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e4dfa-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e4dfa-132">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e4dfa-132">CopyItemResponseMessage</span></span>](copyitemresponsemessage.md)
    
- [<span data-ttu-id="e4dfa-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e4dfa-133">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e4dfa-134">Items</span><span class="sxs-lookup"><span data-stu-id="e4dfa-134">Items</span></span>](items.md)
    
<span data-ttu-id="e4dfa-135">Para localizar outras opções para a mensagem de resposta da operação **CopyItem** , explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="e4dfa-135">To find other options for the response message of the **CopyItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="e4dfa-136">Inicie o elemento [CopyItemResponse](copyitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="e4dfa-136">Start at the [CopyItemResponse](copyitemresponse.md) element.</span></span> 
  
## <a name="copyitem-error-response"></a><span data-ttu-id="e4dfa-137">Resposta de erro CopyItem</span><span class="sxs-lookup"><span data-stu-id="e4dfa-137">CopyItem error response</span></span>

### <a name="description"></a><span data-ttu-id="e4dfa-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4dfa-138">Description</span></span>

<span data-ttu-id="e4dfa-139">O exemplo a seguir mostra uma resposta de erro a uma solicitação de **CopyItem** .</span><span class="sxs-lookup"><span data-stu-id="e4dfa-139">The following example shows an error response to a **CopyItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="e4dfa-140">Código</span><span class="sxs-lookup"><span data-stu-id="e4dfa-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CopyItemResponseMessage>
      </m:ResponseMessages>
    </CopyItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="e4dfa-141">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="e4dfa-141">Error response elements</span></span>

<span data-ttu-id="e4dfa-142">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="e4dfa-142">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="e4dfa-143">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e4dfa-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="e4dfa-144">CopyItemResponse</span><span class="sxs-lookup"><span data-stu-id="e4dfa-144">CopyItemResponse</span></span>](copyitemresponse.md)
    
- [<span data-ttu-id="e4dfa-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e4dfa-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e4dfa-146">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e4dfa-146">CopyItemResponseMessage</span></span>](copyitemresponsemessage.md)
    
- [<span data-ttu-id="e4dfa-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="e4dfa-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="e4dfa-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e4dfa-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e4dfa-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e4dfa-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="e4dfa-150">Items</span><span class="sxs-lookup"><span data-stu-id="e4dfa-150">Items</span></span>](items.md)
    
<span data-ttu-id="e4dfa-151">Para localizar outras opções para a mensagem de resposta de erro da operação **CopyItem** , explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="e4dfa-151">To find other options for the error response message of the **CopyItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="e4dfa-152">Inicie o elemento [CopyItemResponse](copyitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="e4dfa-152">Start at the [CopyItemResponse](copyitemresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="e4dfa-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="e4dfa-153">See also</span></span>



- [<span data-ttu-id="e4dfa-154">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="e4dfa-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

