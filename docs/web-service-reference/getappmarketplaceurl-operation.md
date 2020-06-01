---
title: Operação GetAppMarketplaceUrl
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2c016fc3-0e13-4624-9a5b-d3e84577a860
description: Encontre informações sobre a operação do EWS do GetAppMarketplaceUrl.
ms.openlocfilehash: 6797af44c3aaa6653c440b3d53a282d8c90a4381
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459522"
---
# <a name="getappmarketplaceurl-operation"></a><span data-ttu-id="782f8-103">Operação GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="782f8-103">GetAppMarketplaceUrl operation</span></span>

<span data-ttu-id="782f8-104">Encontre informações sobre a operação do EWS do **GetAppMarketplaceUrl** .</span><span class="sxs-lookup"><span data-stu-id="782f8-104">Find information about the **GetAppMarketplaceUrl** EWS operation.</span></span> 
  
<span data-ttu-id="782f8-105">A operação **GetAppMarketplaceUrl** recupera a URL para o Marketplace do aplicativo que um cliente pode acessar para adquirir aplicativos para instalar em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="782f8-105">The **GetAppMarketplaceUrl** operation retrieves the URL for the app marketplace that a client can visit to acquire apps to install in a mailbox.</span></span> 
  
<span data-ttu-id="782f8-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="782f8-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getappmarketplaceurl-operation"></a><span data-ttu-id="782f8-107">Usando a operação GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="782f8-107">Using the GetAppMarketplaceUrl operation</span></span>

<span data-ttu-id="782f8-108">A operação **GetAppMarketplaceUrl** não usa argumentos para solicitar a URL para o Marketplace a partir do qual um cliente pode instalar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="782f8-108">The **GetAppMarketplaceUrl** operation does not take any arguments to request the URL for the marketplace from which a client can install apps.</span></span> <span data-ttu-id="782f8-109">A resposta conterá uma URL para o Marketplace de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="782f8-109">The response will contain a URL to the app marketplace.</span></span> 
  
### <a name="getappmarketplaceurl-operation-soap-headers"></a><span data-ttu-id="782f8-110">Cabeçalhos SOAP de operação GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="782f8-110">GetAppMarketplaceUrl operation SOAP headers</span></span>

<span data-ttu-id="782f8-111">A operação **GetAppMarketplaceUrl** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="782f8-111">The **GetAppMarketplaceUrl** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="782f8-112">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="782f8-112">**Header name**</span></span>|<span data-ttu-id="782f8-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="782f8-113">**Element**</span></span>|<span data-ttu-id="782f8-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="782f8-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="782f8-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="782f8-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="782f8-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="782f8-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="782f8-117">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="782f8-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="782f8-118">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="782f8-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="782f8-119">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="782f8-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="782f8-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="782f8-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="782f8-121">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="782f8-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="782f8-122">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="782f8-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getappmarketplaceurl-operation-request-example-get-the-app-marketplace-url-for-a-mailbox"></a><span data-ttu-id="782f8-123">Exemplo de solicitação de operação GetAppMarketplaceUrl: obter a URL do App Marketplace para uma caixa de correio</span><span class="sxs-lookup"><span data-stu-id="782f8-123">GetAppMarketplaceUrl operation request example: Get the app marketplace URL for a mailbox</span></span>

<span data-ttu-id="782f8-124">O exemplo a seguir de uma solicitação de operação **GetAppMarketplaceUrl** mostra como obter a URL do App Marketplace para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="782f8-124">The following example of a **GetAppMarketplaceUrl** operation request shows how to get the app marketplace URL for a mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013_SP1" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:GetAppMarketplaceUrl>
        <m:ApiVersionSupported>1.0</m:ApiVersionSupported>
        <m:SchemaVersionSupported>1.0</m:SchemaVersionSupported>
      </m:GetAppMarketplaceUrl>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="782f8-125">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="782f8-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="782f8-126">GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="782f8-126">GetAppMarketplaceUrl</span></span>](getappmarketplaceurl.md)
    
- [<span data-ttu-id="782f8-127">ApiVersionSupported</span><span class="sxs-lookup"><span data-stu-id="782f8-127">ApiVersionSupported</span></span>](apiversionsupported.md)
    
- [<span data-ttu-id="782f8-128">SchemaVersionSupported</span><span class="sxs-lookup"><span data-stu-id="782f8-128">SchemaVersionSupported</span></span>](schemaversionsupported.md)
    
## <a name="successful-getappmarketplaceurl-operation-response"></a><span data-ttu-id="782f8-129">Resposta de operação GetAppMarketplaceUrl bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="782f8-129">Successful GetAppMarketplaceUrl operation response</span></span>

<span data-ttu-id="782f8-130">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetAppMarketplaceUrl** para obter a URL do App Marketplace para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="782f8-130">The following example shows a successful response to a **GetAppMarketplaceUrl** operation request to get the app marketplace URL for a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="782f8-131">A URL do Marketplace de aplicativos foi alterada para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="782f8-131">The app marketplace URL has been altered to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="7" 
                           Version="V2_10" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppMarketplaceUrlResponse ResponseClass="Success" 
                                    xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <AppMarketplaceUrl>http://marketplace.contoso.com</AppMarketplaceUrl>
      </GetAppMarketplaceUrlResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="782f8-132">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="782f8-132">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="782f8-133">GetAppMarketplaceUrlResponse</span><span class="sxs-lookup"><span data-stu-id="782f8-133">GetAppMarketplaceUrlResponse</span></span>](getappmarketplaceurlresponse.md)
    
- [<span data-ttu-id="782f8-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="782f8-134">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="782f8-135">AppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="782f8-135">AppMarketplaceUrl</span></span>](appmarketplaceurl.md)
    
## <a name="getappmarketplaceurl-operation-error-response"></a><span data-ttu-id="782f8-136">Resposta de erro de operação GetAppMarketPlaceUrl</span><span class="sxs-lookup"><span data-stu-id="782f8-136">GetAppMarketPlaceUrl operation error response</span></span>

<span data-ttu-id="782f8-137">Os erros retornados para esta operação estão relacionados a uma configuração de serviço incorreta ou são erros de EWS genéricos.</span><span class="sxs-lookup"><span data-stu-id="782f8-137">Errors returned for this operation are either related to an incorrect service configuration or are generic EWS errors.</span></span> <span data-ttu-id="782f8-138">Para códigos de erro genéricos para EWS e específicos para esta operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="782f8-138">For error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span> 
  
<span data-ttu-id="782f8-139">O exemplo a seguir mostra uma resposta de erro que é retornada quando o painel de controle externo do Exchange (ECP) não é configurado.</span><span class="sxs-lookup"><span data-stu-id="782f8-139">The following example shows an error response that is returned when external Exchange Control Panel (ECP) is not configured.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="7" 
                           Version="V2_10" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppMarketplaceUrlResponse ResponseClass="Error" 
                                    xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Cannot get external ECP URL. This might happen if external ECP URL isn't configured.</MessageText>
         <ResponseCode>ErrorCannotGetExternalEcpUrl</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetAppMarketplaceUrlResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="782f8-140">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="782f8-140">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="782f8-141">GetAppMarketplaceUrlResponse</span><span class="sxs-lookup"><span data-stu-id="782f8-141">GetAppMarketplaceUrlResponse</span></span>](getappmarketplaceurlresponse.md)
    
- [<span data-ttu-id="782f8-142">MessageText</span><span class="sxs-lookup"><span data-stu-id="782f8-142">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="782f8-143">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="782f8-143">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="782f8-144">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="782f8-144">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="782f8-145">Também consulte</span><span class="sxs-lookup"><span data-stu-id="782f8-145">See also</span></span>

- [<span data-ttu-id="782f8-146">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="782f8-146">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="782f8-147">Operação DisableApp</span><span class="sxs-lookup"><span data-stu-id="782f8-147">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="782f8-148">Operação InstallApp</span><span class="sxs-lookup"><span data-stu-id="782f8-148">InstallApp operation</span></span>](installapp-operation.md)
    
- [<span data-ttu-id="782f8-149">Operação UninstallApp</span><span class="sxs-lookup"><span data-stu-id="782f8-149">UninstallApp operation</span></span>](uninstallapp-operation.md)
    
- [<span data-ttu-id="782f8-150">Operação GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="782f8-150">GetAppManifests operation</span></span>](getappmanifests-operation.md)
    

