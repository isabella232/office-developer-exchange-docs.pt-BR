---
title: Operação GetAppManifests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 21a4987c-c24d-4a6e-ace4-e81edcda6303
description: Encontre informações sobre o EWS GetAppManifests operação.
ms.openlocfilehash: 9c919bac9ac0042890d1c439454b37e6b7c60876
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752393"
---
# <a name="getappmanifests-operation"></a><span data-ttu-id="0047e-103">Operação GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="0047e-103">GetAppManifests operation</span></span>

<span data-ttu-id="0047e-104">Encontre informações sobre a operação de EWS **GetAppManifests** .</span><span class="sxs-lookup"><span data-stu-id="0047e-104">Find information about the **GetAppManifests** EWS operation.</span></span> 
  
<span data-ttu-id="0047e-105">A operação **GetAppManifests** recupera manifestos de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="0047e-105">The **GetAppManifests** operation retrieves app manifests.</span></span> 
  
<span data-ttu-id="0047e-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0047e-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getappmanifests-operation"></a><span data-ttu-id="0047e-107">Usando a operação GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="0047e-107">Using the GetAppManifests operation</span></span>

<span data-ttu-id="0047e-108">A operação **GetAppManifests** não usa argumentos para solicitar os manifestos de aplicativos para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0047e-108">The **GetAppManifests** operation does not take any arguments to request the app manifests for a mailbox.</span></span> <span data-ttu-id="0047e-109">A resposta conterá codificado na base64 arquivos de manifesto XML para cada aplicativo que está instalado em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0047e-109">The response will contain base64-encoded XML manifest files for each app that is installed in a mailbox.</span></span> 
  
### <a name="getappmanifests-operation-soap-headers"></a><span data-ttu-id="0047e-110">Cabeçalhos SOAP GetAppManifests operação</span><span class="sxs-lookup"><span data-stu-id="0047e-110">GetAppManifests operation SOAP headers</span></span>

<span data-ttu-id="0047e-111">A operação **GetAppManifests** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="0047e-111">The **GetAppManifests** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="0047e-112">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="0047e-112">**Header name**</span></span>|<span data-ttu-id="0047e-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="0047e-113">**Element**</span></span>|<span data-ttu-id="0047e-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="0047e-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0047e-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="0047e-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="0047e-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="0047e-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="0047e-117">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="0047e-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="0047e-118">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="0047e-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0047e-119">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="0047e-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="0047e-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0047e-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="0047e-121">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="0047e-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="0047e-122">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="0047e-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getappmanifests-operation-request-example-get-the-app-manifests-for-a-mailbox"></a><span data-ttu-id="0047e-123">Exemplo de solicitação de operação GetAppManifests: obter os manifestos de aplicativos para uma caixa de correio</span><span class="sxs-lookup"><span data-stu-id="0047e-123">GetAppManifests operation request example: Get the app manifests for a mailbox</span></span>

<span data-ttu-id="0047e-124">O exemplo a seguir de uma solicitação de operação **GetAppManifests** mostra como obter os manifestos de aplicativos para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0047e-124">The following example of a **GetAppManifests** operation request shows how to get the app manifests for a mailbox.</span></span> <span data-ttu-id="0047e-125">O elemento [ApiVersionSupported](apiversionsupported.md) e o elemento [SchemaVersionSupported](schemaversionsupported.md) são opcionais.</span><span class="sxs-lookup"><span data-stu-id="0047e-125">The [ApiVersionSupported](apiversionsupported.md) element and the [SchemaVersionSupported](schemaversionsupported.md) element are optional.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="0047e-126">A solicitação de corpo SOAP contém o elemento a seguir:</span><span class="sxs-lookup"><span data-stu-id="0047e-126">The request SOAP body contains the following element:</span></span>
  
- [<span data-ttu-id="0047e-127">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="0047e-127">GetAppManifests</span></span>](getappmanifests.md)
    
- [<span data-ttu-id="0047e-128">ApiVersionSupported</span><span class="sxs-lookup"><span data-stu-id="0047e-128">ApiVersionSupported</span></span>](apiversionsupported.md)
    
- [<span data-ttu-id="0047e-129">SchemaVersionSupported</span><span class="sxs-lookup"><span data-stu-id="0047e-129">SchemaVersionSupported</span></span>](schemaversionsupported.md)
    
## <a name="successful-getappmanifests-operation-response"></a><span data-ttu-id="0047e-130">Resposta de operação GetAppManifests bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="0047e-130">Successful GetAppManifests operation response</span></span>

<span data-ttu-id="0047e-131">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetAppManifests** para obter os manifestos de aplicativos para uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="0047e-131">The following example shows a successful response to a **GetAppManifests** operation request to get the app manifests for a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="0047e-132">Todos os manifestos de app base64 tem sido truncados arbitrariamente para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="0047e-132">All base64 app manifests have been arbitrarily truncated to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="07" 
                           Version="V2_10" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppManifestsResponse ResponseClass="Success" 
                               xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <m:Apps xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
          <t:App xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
            <t:Manifest>WNlQXBwPg==</t:Manifest>
          </t:App>
         </m:Apps>
      </GetAppManifestsResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="0047e-133">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="0047e-133">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0047e-134">GetAppManifestsResponse</span><span class="sxs-lookup"><span data-stu-id="0047e-134">GetAppManifestsResponse</span></span>](getappmanifestsresponse.md)
    
- [<span data-ttu-id="0047e-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0047e-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0047e-136">Aplicativos</span><span class="sxs-lookup"><span data-stu-id="0047e-136">Apps</span></span>](apps.md)
    
- [<span data-ttu-id="0047e-137">App</span><span class="sxs-lookup"><span data-stu-id="0047e-137">App</span></span>](app.md)
    
- [<span data-ttu-id="0047e-138">Manifesto</span><span class="sxs-lookup"><span data-stu-id="0047e-138">Manifest</span></span>](manifest.md)
    
<span data-ttu-id="0047e-139">A resposta SOAP body também pode conter o seguinte elemento:</span><span class="sxs-lookup"><span data-stu-id="0047e-139">The response SOAP body can also contain the following element:</span></span>
  
- [<span data-ttu-id="0047e-140">Manifestos</span><span class="sxs-lookup"><span data-stu-id="0047e-140">Manifests</span></span>](manifests.md)
    
## <a name="getappmanifests-operation-error-response"></a><span data-ttu-id="0047e-141">Resposta de erro de operação GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="0047e-141">GetAppManifests operation error response</span></span>

<span data-ttu-id="0047e-142">Erros retornados para esta operação estão relacionados ao formato inválido de parâmetros de entrada ou erros de EWS genérico.</span><span class="sxs-lookup"><span data-stu-id="0047e-142">Errors returned for this operation are related to an invalid format of the input parameters or are generic EWS errors.</span></span> <span data-ttu-id="0047e-143">Para códigos de erro genérica do EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="0047e-143">For error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="07"
                       Version="V2_10"
                       xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetAppManifestsResponse ResponseClass="Error"
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>The apiVersionSupported parameter is invalid. 
                   It should be in the form of major version, minor 
                   version, separated by '.', for example '2.34'.</MessageText>
      <ResponseCode>ErrorInvalidRequest</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetAppManifestsResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a><span data-ttu-id="0047e-144">Confira também</span><span class="sxs-lookup"><span data-stu-id="0047e-144">See also</span></span>

- [<span data-ttu-id="0047e-145">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="0047e-145">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="0047e-146">Operação DisableApp</span><span class="sxs-lookup"><span data-stu-id="0047e-146">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="0047e-147">Operação InstallApp</span><span class="sxs-lookup"><span data-stu-id="0047e-147">InstallApp operation</span></span>](installapp-operation.md)
    
- [<span data-ttu-id="0047e-148">Operação UninstallApp</span><span class="sxs-lookup"><span data-stu-id="0047e-148">UninstallApp operation</span></span>](uninstallapp-operation.md)
    
- [<span data-ttu-id="0047e-149">Operação GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="0047e-149">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)
    

