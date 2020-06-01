---
title: Operação UploadItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UploadItems
api_type:
- schema
ms.assetid: a88cbe99-7968-454d-a545-4f92c330909f
description: A operação UploadItems carrega um fluxo de itens em uma caixa de correio do Exchange.
ms.openlocfilehash: 57e722c7775baa090736875077781cee869c3b01
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468499"
---
# <a name="uploaditems-operation"></a><span data-ttu-id="b2592-103">Operação UploadItems</span><span class="sxs-lookup"><span data-stu-id="b2592-103">UploadItems operation</span></span>

<span data-ttu-id="b2592-104">A operação **UploadItems** carrega um fluxo de itens em uma caixa de correio do Exchange.</span><span class="sxs-lookup"><span data-stu-id="b2592-104">The **UploadItems** operation uploads a stream of items into an Exchange mailbox.</span></span> 
  
> [!IMPORTANT]
> <span data-ttu-id="b2592-105">A operação **UploadItems** é restrita no MicrosoftExchange Server 2010 Service Pack 1 (SP1) para uma carga de importação máxima de 25 MB de dados codificados em base64.</span><span class="sxs-lookup"><span data-stu-id="b2592-105">The **UploadItems** operation is restricted in MicrosoftExchange Server 2010 Service Pack 1 (SP1) to a maximum import payload of 25MB of base64 encoded data.</span></span> <span data-ttu-id="b2592-106">A configuração pode ser alterada no arquivo Web. config.</span><span class="sxs-lookup"><span data-stu-id="b2592-106">The setting can be altered in the web.config file.</span></span> 
  
## <a name="uploaditems-request-example"></a><span data-ttu-id="b2592-107">Exemplo de solicitação UploadItems</span><span class="sxs-lookup"><span data-stu-id="b2592-107">UploadItems request example</span></span>

### <a name="description"></a><span data-ttu-id="b2592-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2592-108">Description</span></span>

<span data-ttu-id="b2592-109">O exemplo a seguir de uma solicitação **UploadItems** mostra como carregar dois itens em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b2592-109">The following example of an **UploadItems** request shows how to upload two items into a mailbox.</span></span> <span data-ttu-id="b2592-110">O primeiro item é um novo item.</span><span class="sxs-lookup"><span data-stu-id="b2592-110">The first item is a new item.</span></span> <span data-ttu-id="b2592-111">O segundo item é uma versão atualizada de um item existente na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b2592-111">The second item is an updated version of an existing item in the mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b2592-112">Código</span><span class="sxs-lookup"><span data-stu-id="b2592-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UploadItems>
      <m:Items>
        <t:Item CreateAction="CreateNew">
          <t:ParentFolderId Id="AQMkADhhOGIgAAAA==" ChangeKey="AQAAAA=="/>
          <t:Data>
            AQAAAAgAAAAAAAAAAQAAAAMAAAAYAAAAAQAAAAcDAgAAAAAAwAAAAA
            AAAEYAJACABAAAAAYAAAABDqSAAAACAAAAcSMAAOSECEBbAAAAL089
            RklSU1QgT1JHQU5JWkFUSU9OL09VPUVYQ0hBTkdFIEFETUlOSVNUUk
            FUSVZFIEdST1VQIChGWURJQk9IRjIzU1BETFQpL0NOPVJFQ0lQSUVO
            VFMvQ049AAMAFwABAAAAsIQaABIAAABJAFAATQAuAE4AbwB0AGUAAA
            ALACMAAAADACYAAAAAAAsAKQAAAAMALgAAAAAAAwA2AAAAAACwhw4=
          </t:Data>
        </t:Item>
        <t:Item CreateAction="Update">
          <t:ParentFolderId Id="AQMkADhhOGIgAAAB==" ChangeKey="AQAAAA=="/>
          <t:ItemId Id="AAMkADhhOGU0MGM7AAA=" ChangeKey="CQAAAA=="/>
          <t:Data>
            AQAAAAgAAAAAAAAAAQAAAAMAAAAYAAAAAQAAAAcDAgAAAAAAwAAAAA
            AAAEYAJACABAAAAAYAAAABDqSAAAACAAAANiAAAOSECEBbAAAAL089
            RklSU1QgT1JHQU5JWkFUSU9OL09VPUVYQ0hBTkdFIEFETUlOSVNUUk
            FUSVZFIEdST1VQIChGWURJQk9IRjIzU1BETFQpL0NOPVJFQ0lQSUVO
            VFMvQ049AAMAFwABAAAAsIQaABIAAABJAFAATQAuAE4AbwB0AGUAAA
            ALACMAAAALACkAAAADADYAAAAAALCENwAyAAAASQBuAHQAZQByAGUA
            cwB0AGkAbgBnACAALQAgAGYAcgBvAG0AIABFAFcAUwBNAEEAAABAAD
            kAgJ2chyHuygECATsAZQAAAEVYOi9PPUZJUlNUIE9SR0FOSVpBVBMO
          </t:Data>
        </t:Item>
      </m:Items>
    </m:UploadItems>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="b2592-113">Comentários</span><span class="sxs-lookup"><span data-stu-id="b2592-113">Comments</span></span>

<span data-ttu-id="b2592-114">Os identificadores e os dados de item foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b2592-114">Identifiers and the item data have been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="b2592-115">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="b2592-115">Request elements</span></span>

<span data-ttu-id="b2592-116">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="b2592-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="b2592-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="b2592-117">RequestServerVersion</span></span>](requestserverversion.md)
    
- [<span data-ttu-id="b2592-118">UploadItems</span><span class="sxs-lookup"><span data-stu-id="b2592-118">UploadItems</span></span>](uploaditems.md)
    
- [<span data-ttu-id="b2592-119">Itens (NonEmptyArrayOfUploadItemsType)</span><span class="sxs-lookup"><span data-stu-id="b2592-119">Items (NonEmptyArrayOfUploadItemsType)</span></span>](items-nonemptyarrayofuploaditemstype.md)
    
- [<span data-ttu-id="b2592-120">Item (UploadItemType)</span><span class="sxs-lookup"><span data-stu-id="b2592-120">Item (UploadItemType)</span></span>](item-uploaditemtype.md)
    
- [<span data-ttu-id="b2592-121">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="b2592-121">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="b2592-122">Dados (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="b2592-122">Data (base64Binary)</span></span>](data-base64binary.md)
    
- [<span data-ttu-id="b2592-123">ItemId</span><span class="sxs-lookup"><span data-stu-id="b2592-123">ItemId</span></span>](itemid.md)
    
## <a name="successful-uploaditems-response-example"></a><span data-ttu-id="b2592-124">Exemplo de resposta UploadItems bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="b2592-124">Successful UploadItems response example</span></span>

### <a name="description"></a><span data-ttu-id="b2592-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2592-125">Description</span></span>

<span data-ttu-id="b2592-126">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação **UploadItems** .</span><span class="sxs-lookup"><span data-stu-id="b2592-126">The following example shows a successful response to the **UploadItems** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b2592-127">Código</span><span class="sxs-lookup"><span data-stu-id="b2592-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14"
                         MinorVersion="1"
                         MajorBuildNumber="164"
                         MinorBuildNumber="0"
                         Version="Exchange2010_SP1"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:UploadItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                           xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:UploadItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ItemId Id="AAMkADhhUFZ/AAA=" ChangeKey="CQAAABYAAABsMBS3hrihS7voMf0GPIQeAAAAULQm"/>
        </m:UploadItemsResponseMessage>
        <m:UploadItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ItemId Id="AAMkADhhOGZ7AAA=" ChangeKey="CQAAABYAAABsMBS3hrihS7voMf0GPIQeAAAAULQn"/>
        </m:UploadItemsResponseMessage>
      </m:ResponseMessages>
    </m:UploadItemsResponse>
  </s:Body>
</s:Envelope>
```

### <a name="comments"></a><span data-ttu-id="b2592-128">Comentários</span><span class="sxs-lookup"><span data-stu-id="b2592-128">Comments</span></span>

<span data-ttu-id="b2592-129">Os identificadores de item foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="b2592-129">Item identifiers have been shortened to preserve readability.</span></span>
  
### <a name="response-elements"></a><span data-ttu-id="b2592-130">Elementos de resposta</span><span class="sxs-lookup"><span data-stu-id="b2592-130">Response elements</span></span>

<span data-ttu-id="b2592-131">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="b2592-131">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="b2592-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b2592-132">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="b2592-133">UploadItemsResponse</span><span class="sxs-lookup"><span data-stu-id="b2592-133">UploadItemsResponse</span></span>](uploaditemsresponse.md)
    
- [<span data-ttu-id="b2592-134">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b2592-134">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b2592-135">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b2592-135">UploadItemsResponseMessage</span></span>](uploaditemsresponsemessage.md)
    
- [<span data-ttu-id="b2592-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b2592-136">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b2592-137">ItemId</span><span class="sxs-lookup"><span data-stu-id="b2592-137">ItemId</span></span>](itemid.md)
    
## <a name="uploaditems-error-response-example"></a><span data-ttu-id="b2592-138">Exemplo de resposta de erro UploadItems</span><span class="sxs-lookup"><span data-stu-id="b2592-138">UploadItems Error response example</span></span>

### <a name="description"></a><span data-ttu-id="b2592-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="b2592-139">Description</span></span>

<span data-ttu-id="b2592-140">O exemplo a seguir mostra uma resposta para a solicitação **UploadItems** que contém um erro causado por uma tentativa de atualizar um item que não pode ser encontrado na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="b2592-140">The following example shows a response to the **UploadItems** request that contains an error caused by an attempt to update an item that cannot be found in the mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b2592-141">Código</span><span class="sxs-lookup"><span data-stu-id="b2592-141">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="164" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:UploadItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:UploadItemsResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:UploadItemsResponseMessage>
      </m:ResponseMessages>
    </m:UploadItemsResponse>
  </s:Body>
</s:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="b2592-142">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="b2592-142">Error response elements</span></span>

<span data-ttu-id="b2592-143">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="b2592-143">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="b2592-144">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b2592-144">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="b2592-145">UploadItemsResponse</span><span class="sxs-lookup"><span data-stu-id="b2592-145">UploadItemsResponse</span></span>](uploaditemsresponse.md)
    
- [<span data-ttu-id="b2592-146">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b2592-146">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b2592-147">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b2592-147">UploadItemsResponseMessage</span></span>](uploaditemsresponsemessage.md)
    
- [<span data-ttu-id="b2592-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="b2592-148">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="b2592-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b2592-149">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b2592-150">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b2592-150">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="b2592-151">Também consulte</span><span class="sxs-lookup"><span data-stu-id="b2592-151">See also</span></span>



[<span data-ttu-id="b2592-152">Operação ExportItems</span><span class="sxs-lookup"><span data-stu-id="b2592-152">ExportItems operation</span></span>](exportitems-operation.md)


[<span data-ttu-id="b2592-153">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b2592-153">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="b2592-154">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="b2592-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

