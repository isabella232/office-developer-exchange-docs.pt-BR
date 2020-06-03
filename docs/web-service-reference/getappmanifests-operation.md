---
title: Operação GetAppManifests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 21a4987c-c24d-4a6e-ace4-e81edcda6303
description: Encontre informações sobre a operação do EWS do GetAppManifests.
ms.openlocfilehash: 4d4c1d32f14cf144335ddfdf8c9cd4c88a4421d0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463003"
---
# <a name="getappmanifests-operation"></a><span data-ttu-id="81835-103">Operação GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="81835-103">GetAppManifests operation</span></span>

<span data-ttu-id="81835-104">Encontre informações sobre a operação do EWS do **GetAppManifests** .</span><span class="sxs-lookup"><span data-stu-id="81835-104">Find information about the **GetAppManifests** EWS operation.</span></span> 
  
<span data-ttu-id="81835-105">A operação **GetAppManifests** recupera manifestos de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="81835-105">The **GetAppManifests** operation retrieves app manifests.</span></span> 
  
<span data-ttu-id="81835-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="81835-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getappmanifests-operation"></a><span data-ttu-id="81835-107">Usando a operação GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="81835-107">Using the GetAppManifests operation</span></span>

<span data-ttu-id="81835-108">A operação **GetAppManifests** não usa argumentos para solicitar os manifestos de aplicativo para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="81835-108">The **GetAppManifests** operation does not take any arguments to request the app manifests for a mailbox.</span></span> <span data-ttu-id="81835-109">A resposta conterá arquivos de manifesto XML codificados em base64 para cada aplicativo instalado em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="81835-109">The response will contain base64-encoded XML manifest files for each app that is installed in a mailbox.</span></span> 
  
### <a name="getappmanifests-operation-soap-headers"></a><span data-ttu-id="81835-110">Cabeçalhos SOAP de operação GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="81835-110">GetAppManifests operation SOAP headers</span></span>

<span data-ttu-id="81835-111">A operação **GetAppManifests** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="81835-111">The **GetAppManifests** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="81835-112">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="81835-112">**Header name**</span></span>|<span data-ttu-id="81835-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="81835-113">**Element**</span></span>|<span data-ttu-id="81835-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="81835-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="81835-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="81835-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="81835-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="81835-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="81835-117">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="81835-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="81835-118">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="81835-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="81835-119">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="81835-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="81835-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="81835-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="81835-121">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="81835-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="81835-122">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="81835-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getappmanifests-operation-request-example-get-the-app-manifests-for-a-mailbox"></a><span data-ttu-id="81835-123">Exemplo de solicitação de operação GetAppManifests: obter os manifestos de aplicativo para uma caixa de correio</span><span class="sxs-lookup"><span data-stu-id="81835-123">GetAppManifests operation request example: Get the app manifests for a mailbox</span></span>

<span data-ttu-id="81835-124">O exemplo a seguir de uma solicitação de operação **GetAppManifests** mostra como obter os manifestos de aplicativo para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="81835-124">The following example of a **GetAppManifests** operation request shows how to get the app manifests for a mailbox.</span></span> <span data-ttu-id="81835-125">O elemento [ApiVersionSupported](apiversionsupported.md) e o elemento [SchemaVersionSupported](schemaversionsupported.md) são opcionais.</span><span class="sxs-lookup"><span data-stu-id="81835-125">The [ApiVersionSupported](apiversionsupported.md) element and the [SchemaVersionSupported](schemaversionsupported.md) element are optional.</span></span> 
  
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
      <m:GetAppManifests>
        <m:ApiVersionSupported>1.1</m:ApiVersionSupported>
        <m:SchemaVersionSupported>1.1</m:SchemaVersionSupported>
      </m:GetAppManifests>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="81835-126">O corpo SOAP de solicitação contém o seguinte elemento:</span><span class="sxs-lookup"><span data-stu-id="81835-126">The request SOAP body contains the following element:</span></span>
  
- [<span data-ttu-id="81835-127">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="81835-127">GetAppManifests</span></span>](getappmanifests.md)
    
- [<span data-ttu-id="81835-128">ApiVersionSupported</span><span class="sxs-lookup"><span data-stu-id="81835-128">ApiVersionSupported</span></span>](apiversionsupported.md)
    
- [<span data-ttu-id="81835-129">SchemaVersionSupported</span><span class="sxs-lookup"><span data-stu-id="81835-129">SchemaVersionSupported</span></span>](schemaversionsupported.md)
    
## <a name="successful-getappmanifests-operation-response"></a><span data-ttu-id="81835-130">Resposta de operação GetAppManifests bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="81835-130">Successful GetAppManifests operation response</span></span>

<span data-ttu-id="81835-131">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetAppManifests** para obter os manifestos de aplicativo para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="81835-131">The following example shows a successful response to a **GetAppManifests** operation request to get the app manifests for a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="81835-132">Todos os manifestos de aplicativos Base64 foram truncados arbitrariamente para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="81835-132">All base64 app manifests have been arbitrarily truncated to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="07" 
                           Version="V2_10" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppManifestsResponse ResponseClass="Success" 
                               xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <m:Apps xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
          <t:App xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
            <t:Manifest>WNlQXBwPg==</t:Manifest>
          </t:App>
         </m:Apps>
      </GetAppManifestsResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="81835-133">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="81835-133">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="81835-134">GetAppManifestsResponse</span><span class="sxs-lookup"><span data-stu-id="81835-134">GetAppManifestsResponse</span></span>](getappmanifestsresponse.md)
    
- [<span data-ttu-id="81835-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="81835-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="81835-136">Apps</span><span class="sxs-lookup"><span data-stu-id="81835-136">Apps</span></span>](apps.md)
    
- [<span data-ttu-id="81835-137">App</span><span class="sxs-lookup"><span data-stu-id="81835-137">App</span></span>](app.md)
    
- [<span data-ttu-id="81835-138">Manifesto</span><span class="sxs-lookup"><span data-stu-id="81835-138">Manifest</span></span>](manifest.md)
    
<span data-ttu-id="81835-139">O corpo SOAP de resposta também pode conter o seguinte elemento:</span><span class="sxs-lookup"><span data-stu-id="81835-139">The response SOAP body can also contain the following element:</span></span>
  
- [<span data-ttu-id="81835-140">Manifestos</span><span class="sxs-lookup"><span data-stu-id="81835-140">Manifests</span></span>](manifests.md)
    
## <a name="getappmanifests-operation-error-response"></a><span data-ttu-id="81835-141">Resposta de erro de operação GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="81835-141">GetAppManifests operation error response</span></span>

<span data-ttu-id="81835-142">Os erros retornados para esta operação estão relacionados a um formato inválido dos parâmetros de entrada ou são erros genéricos do EWS.</span><span class="sxs-lookup"><span data-stu-id="81835-142">Errors returned for this operation are related to an invalid format of the input parameters or are generic EWS errors.</span></span> <span data-ttu-id="81835-143">Para códigos de erro genéricos para EWS e específicos para esta operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="81835-143">For error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="07"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetAppManifestsResponse ResponseClass="Error"
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>The apiVersionSupported parameter is invalid. 
                   It should be in the form of major version, minor 
                   version, separated by '.', for example '2.34'.</MessageText>
      <ResponseCode>ErrorInvalidRequest</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetAppManifestsResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a><span data-ttu-id="81835-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="81835-144">See also</span></span>

- [<span data-ttu-id="81835-145">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="81835-145">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="81835-146">Operação DisableApp</span><span class="sxs-lookup"><span data-stu-id="81835-146">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="81835-147">Operação InstallApp</span><span class="sxs-lookup"><span data-stu-id="81835-147">InstallApp operation</span></span>](installapp-operation.md)
    
- [<span data-ttu-id="81835-148">Operação UninstallApp</span><span class="sxs-lookup"><span data-stu-id="81835-148">UninstallApp operation</span></span>](uninstallapp-operation.md)
    
- [<span data-ttu-id="81835-149">Operação GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="81835-149">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)
    

