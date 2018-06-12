---
title: Operação RefreshSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RefreshSharingFolder
api_type:
- schema
ms.assetid: 1b047e34-40f0-459f-ac9e-e9f8e7349479
description: A operação RefreshSharingFolder atualiza a pasta local especificada com os dados mais recentes da pasta que está sendo compartilhado.
ms.openlocfilehash: 0037de28f0720b97cd51c58a6ee7e3c06e84d642
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825041"
---
# <a name="refreshsharingfolder-operation"></a><span data-ttu-id="f349f-103">Operação RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="f349f-103">RefreshSharingFolder operation</span></span>

<span data-ttu-id="f349f-104">A operação **RefreshSharingFolder** atualiza a pasta local especificada com os dados mais recentes da pasta que está sendo compartilhado.</span><span class="sxs-lookup"><span data-stu-id="f349f-104">The **RefreshSharingFolder** operation refreshes the specified local folder with the latest data from the folder that is being shared.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="f349f-105">Cabeçalhos SOAP</span><span class="sxs-lookup"><span data-stu-id="f349f-105">SOAP Headers</span></span>

<span data-ttu-id="f349f-106">A operação **RefreshSharingFolder** pode usar os cabeçalhos SOAP que estão listados e descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="f349f-106">The **RefreshSharingFolder** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="f349f-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="f349f-107">**Header**</span></span>|<span data-ttu-id="f349f-108">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="f349f-108">**Element**</span></span>|<span data-ttu-id="f349f-109">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="f349f-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f349f-110">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="f349f-110">RequestVersion</span></span>  <br/> |[<span data-ttu-id="f349f-111">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="f349f-111">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="f349f-112">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="f349f-112">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="f349f-113">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="f349f-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="f349f-114">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f349f-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="f349f-115">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="f349f-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="refreshsharingfolder-request-example"></a><span data-ttu-id="f349f-116">Exemplo de solicitação de RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="f349f-116">RefreshSharingFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="f349f-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="f349f-117">Description</span></span>

<span data-ttu-id="f349f-118">O exemplo a seguir mostra como formar uma solicitação para atualizar a pasta local especificada com os dados mais recentes da pasta que está sendo compartilhado.</span><span class="sxs-lookup"><span data-stu-id="f349f-118">The following example shows how to form a request to refresh the specified local folder with the latest data from the folder that is being shared.</span></span> <span data-ttu-id="f349f-119">O elemento [SharingFolderId](sharingfolderid.md) Especifica o identificador da pasta local a ser atualizada.</span><span class="sxs-lookup"><span data-stu-id="f349f-119">The [SharingFolderId](sharingfolderid.md) element specifies the identifier of the local folder to be refreshed.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f349f-120">Código</span><span class="sxs-lookup"><span data-stu-id="f349f-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <RefreshSharingFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:SharingFolderId Id="AAMkAD=" ChangeKey="AwAAA=" />
    </RefreshSharingFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="f349f-121">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f349f-121">Request elements</span></span>

<span data-ttu-id="f349f-122">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="f349f-122">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="f349f-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="f349f-123">RequestServerVersion</span></span>](requestserverversion.md)
    
- [<span data-ttu-id="f349f-124">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="f349f-124">RefreshSharingFolder</span></span>](refreshsharingfolder.md)
    
- [<span data-ttu-id="f349f-125">SharingFolderId</span><span class="sxs-lookup"><span data-stu-id="f349f-125">SharingFolderId</span></span>](sharingfolderid.md)
    
## <a name="successful-refreshsharingfolder-response"></a><span data-ttu-id="f349f-126">RefreshSharingFolder de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="f349f-126">Successful RefreshSharingFolder Response</span></span>

### <a name="description"></a><span data-ttu-id="f349f-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="f349f-127">Description</span></span>

<span data-ttu-id="f349f-128">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação **RefreshSharingFolder** .</span><span class="sxs-lookup"><span data-stu-id="f349f-128">The following example shows a successful response to a **RefreshSharingFolder** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f349f-129">Código</span><span class="sxs-lookup"><span data-stu-id="f349f-129">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <RefreshSharingFolderResponseMessage ResponseClass="Success"
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
    </RefreshSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="f349f-130">Elementos de resposta bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="f349f-130">Successful response elements</span></span>

<span data-ttu-id="f349f-131">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="f349f-131">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="f349f-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f349f-132">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="f349f-133">RefreshSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f349f-133">RefreshSharingFolderResponseMessage</span></span>](refreshsharingfolderresponsemessage.md)
    
- [<span data-ttu-id="f349f-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f349f-134">ResponseCode</span></span>](responsecode.md)
    
## <a name="refreshsharingfolder-error-response"></a><span data-ttu-id="f349f-135">Resposta de erro RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="f349f-135">RefreshSharingFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="f349f-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="f349f-136">Description</span></span>

<span data-ttu-id="f349f-137">O exemplo a seguir mostra uma resposta de erro a uma solicitação **RefreshSharingFolder** .</span><span class="sxs-lookup"><span data-stu-id="f349f-137">The following example shows an error response to a **RefreshSharingFolder** request.</span></span> <span data-ttu-id="f349f-138">Neste exemplo, a solicitação de **RefreshSharingFolder** falhou porque uma assinatura que corresponde à pasta local especificada não foi encontrada.</span><span class="sxs-lookup"><span data-stu-id="f349f-138">In this example, the **RefreshSharingFolder** request failed because a subscription that corresponds to the specified local folder was not found.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f349f-139">Código</span><span class="sxs-lookup"><span data-stu-id="f349f-139">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <RefreshSharingFolderResponseMessage ResponseClass="Error"
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:MessageText>Failed to synchronize the sharing folder.</m:MessageText>
      <m:ResponseCode>ErrorSharingSynchronizationFailed</m:ResponseCode>
      <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
      <m:MessageXml>
        <t:Value Name="ErrorDetails">Microsoft.Exchange.InfoWorker.Common.Sharing.SubscriptionNotFoundException: The subscription wasn't found.;</t:Value>
      </m:MessageXml>
    </RefreshSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="f349f-140">Elementos de resposta de erro</span><span class="sxs-lookup"><span data-stu-id="f349f-140">Error response elements</span></span>

<span data-ttu-id="f349f-141">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="f349f-141">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="f349f-142">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f349f-142">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="f349f-143">RefreshSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f349f-143">RefreshSharingFolderResponseMessage</span></span>](refreshsharingfolderresponsemessage.md)
    
- [<span data-ttu-id="f349f-144">MessageText</span><span class="sxs-lookup"><span data-stu-id="f349f-144">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="f349f-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f349f-145">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f349f-146">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f349f-146">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="f349f-147">MessageXml</span><span class="sxs-lookup"><span data-stu-id="f349f-147">MessageXml</span></span>](messagexml.md)
    
## <a name="see-also"></a><span data-ttu-id="f349f-148">Confira também</span><span class="sxs-lookup"><span data-stu-id="f349f-148">See also</span></span>



[<span data-ttu-id="f349f-149">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="f349f-149">RefreshSharingFolder</span></span>](refreshsharingfolder.md)
  
[<span data-ttu-id="f349f-150">RefreshSharingFolderType</span><span class="sxs-lookup"><span data-stu-id="f349f-150">RefreshSharingFolderType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.RefreshSharingFolderType.aspx)
  
[<span data-ttu-id="f349f-151">RefreshSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f349f-151">RefreshSharingFolderResponseMessage</span></span>](refreshsharingfolderresponsemessage.md)
  
[<span data-ttu-id="f349f-152">RefreshSharingFolderResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="f349f-152">RefreshSharingFolderResponseMessageType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.RefreshSharingFolderResponseMessageType.aspx)


[<span data-ttu-id="f349f-153">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f349f-153">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="f349f-154">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="f349f-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

