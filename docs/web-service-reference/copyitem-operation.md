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
description: A operação CopyItem copia itens e coloca os itens em uma pasta diferente.
ms.openlocfilehash: ec07700a5ebbdc8774aa2134919634b8dfd02406
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462175"
---
# <a name="copyitem-operation"></a><span data-ttu-id="9b3ed-103">Operação CopyItem</span><span class="sxs-lookup"><span data-stu-id="9b3ed-103">CopyItem operation</span></span>

<span data-ttu-id="9b3ed-104">A operação **CopyItem** copia itens e coloca os itens em uma pasta diferente.</span><span class="sxs-lookup"><span data-stu-id="9b3ed-104">The **CopyItem** operation copies items and puts the items in a different folder.</span></span> 
  
## <a name="copyitem-request-example"></a><span data-ttu-id="9b3ed-105">Exemplo de solicitação CopyItem</span><span class="sxs-lookup"><span data-stu-id="9b3ed-105">CopyItem request example</span></span>

### <a name="description"></a><span data-ttu-id="9b3ed-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b3ed-106">Description</span></span>

<span data-ttu-id="9b3ed-107">O exemplo a seguir de uma solicitação **CopyItem** mostra como formar uma solicitação para copiar um item para a caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="9b3ed-107">The following example of a **CopyItem** request shows how to form a request to copy an item to the Inbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="9b3ed-108">Código</span><span class="sxs-lookup"><span data-stu-id="9b3ed-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CopyItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="9b3ed-109">Comentários</span><span class="sxs-lookup"><span data-stu-id="9b3ed-109">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="9b3ed-110">A ID da pasta e a chave de alteração foram reduzidas para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9b3ed-110">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="9b3ed-111">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="9b3ed-111">Request elements</span></span>

<span data-ttu-id="9b3ed-112">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="9b3ed-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="9b3ed-113">CopyItem</span><span class="sxs-lookup"><span data-stu-id="9b3ed-113">CopyItem</span></span>](copyitem.md)
    
- [<span data-ttu-id="9b3ed-114">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="9b3ed-114">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="9b3ed-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="9b3ed-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="9b3ed-116">ItemIds</span><span class="sxs-lookup"><span data-stu-id="9b3ed-116">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="9b3ed-117">ItemId</span><span class="sxs-lookup"><span data-stu-id="9b3ed-117">ItemId</span></span>](itemid.md)
    
> [!NOTE]
> <span data-ttu-id="9b3ed-118">O esquema que descreve este elemento está localizado no diretório virtual do EWS do computador que está executando o Microsoft Exchange Server 2010 que tem a função de servidor de acesso para Cliente instalada.</span><span class="sxs-lookup"><span data-stu-id="9b3ed-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="9b3ed-119">Para encontrar outras opções para a mensagem de solicitação da operação **CopyItem** , explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="9b3ed-119">To find other options for the request message of the **CopyItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="9b3ed-120">Inicie no elemento [CopyItem](copyitem.md) .</span><span class="sxs-lookup"><span data-stu-id="9b3ed-120">Start at the [CopyItem](copyitem.md) element.</span></span> 
  
## <a name="successful-copyitem-response"></a><span data-ttu-id="9b3ed-121">Resposta CopyItem bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="9b3ed-121">Successful CopyItem Response</span></span>

### <a name="description"></a><span data-ttu-id="9b3ed-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b3ed-122">Description</span></span>

<span data-ttu-id="9b3ed-123">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação **CopyItem** .</span><span class="sxs-lookup"><span data-stu-id="9b3ed-123">The following example shows a successful response to the **CopyItem** request.</span></span> 
  
<span data-ttu-id="9b3ed-124">O identificador de item do novo item é retornado na mensagem de resposta.</span><span class="sxs-lookup"><span data-stu-id="9b3ed-124">The item identifier of the new item is returned in the response message.</span></span> <span data-ttu-id="9b3ed-125">Os identificadores de item não são retornados em respostas para as operações de **CopyItem** de caixa de correio ou de caixa de correio de pasta pública.</span><span class="sxs-lookup"><span data-stu-id="9b3ed-125">Item identifiers are not returned in responses for cross-mailbox or mailbox to public folder **CopyItem** operations.</span></span> 
  
### <a name="code"></a><span data-ttu-id="9b3ed-126">Código</span><span class="sxs-lookup"><span data-stu-id="9b3ed-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a><span data-ttu-id="9b3ed-127">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="9b3ed-127">Successful response elements</span></span>

<span data-ttu-id="9b3ed-128">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="9b3ed-128">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="9b3ed-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="9b3ed-129">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="9b3ed-130">CopyItemResponse</span><span class="sxs-lookup"><span data-stu-id="9b3ed-130">CopyItemResponse</span></span>](copyitemresponse.md)
    
- [<span data-ttu-id="9b3ed-131">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9b3ed-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="9b3ed-132">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9b3ed-132">CopyItemResponseMessage</span></span>](copyitemresponsemessage.md)
    
- [<span data-ttu-id="9b3ed-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9b3ed-133">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="9b3ed-134">Itens</span><span class="sxs-lookup"><span data-stu-id="9b3ed-134">Items</span></span>](items.md)
    
<span data-ttu-id="9b3ed-135">Para encontrar outras opções para a mensagem de resposta da operação **CopyItem** , explore a hierarquia do esquema.</span><span class="sxs-lookup"><span data-stu-id="9b3ed-135">To find other options for the response message of the **CopyItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="9b3ed-136">Inicie no elemento [CopyItemResponse](copyitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="9b3ed-136">Start at the [CopyItemResponse](copyitemresponse.md) element.</span></span> 
  
## <a name="copyitem-error-response"></a><span data-ttu-id="9b3ed-137">Resposta de erro CopyItem</span><span class="sxs-lookup"><span data-stu-id="9b3ed-137">CopyItem error response</span></span>

### <a name="description"></a><span data-ttu-id="9b3ed-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b3ed-138">Description</span></span>

<span data-ttu-id="9b3ed-139">O exemplo a seguir mostra uma resposta de erro a uma solicitação **CopyItem** .</span><span class="sxs-lookup"><span data-stu-id="9b3ed-139">The following example shows an error response to a **CopyItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="9b3ed-140">Código</span><span class="sxs-lookup"><span data-stu-id="9b3ed-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="9b3ed-141">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="9b3ed-141">Error response elements</span></span>

<span data-ttu-id="9b3ed-142">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="9b3ed-142">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="9b3ed-143">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="9b3ed-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="9b3ed-144">CopyItemResponse</span><span class="sxs-lookup"><span data-stu-id="9b3ed-144">CopyItemResponse</span></span>](copyitemresponse.md)
    
- [<span data-ttu-id="9b3ed-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9b3ed-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="9b3ed-146">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9b3ed-146">CopyItemResponseMessage</span></span>](copyitemresponsemessage.md)
    
- [<span data-ttu-id="9b3ed-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="9b3ed-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="9b3ed-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9b3ed-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="9b3ed-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="9b3ed-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="9b3ed-150">Itens</span><span class="sxs-lookup"><span data-stu-id="9b3ed-150">Items</span></span>](items.md)
    
<span data-ttu-id="9b3ed-151">Para encontrar outras opções para a mensagem de resposta de erro da operação **CopyItem** , explore a hierarquia de esquema.</span><span class="sxs-lookup"><span data-stu-id="9b3ed-151">To find other options for the error response message of the **CopyItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="9b3ed-152">Inicie no elemento [CopyItemResponse](copyitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="9b3ed-152">Start at the [CopyItemResponse](copyitemresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="9b3ed-153">Também consulte</span><span class="sxs-lookup"><span data-stu-id="9b3ed-153">See also</span></span>



- [<span data-ttu-id="9b3ed-154">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9b3ed-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

