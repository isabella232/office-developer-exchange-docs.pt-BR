---
title: Operação InstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 596eae95-3e78-489a-8bb2-d2dd4a026405
description: Encontre informações sobre a operação do EWS do InstallApp.
ms.openlocfilehash: ae6aab7f7176aa827bafa9abf1aa67d458d309d2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465685"
---
# <a name="installapp-operation"></a><span data-ttu-id="7b45c-103">Operação InstallApp</span><span class="sxs-lookup"><span data-stu-id="7b45c-103">InstallApp operation</span></span>

<span data-ttu-id="7b45c-104">Encontre informações sobre a operação do EWS do **InstallApp** .</span><span class="sxs-lookup"><span data-stu-id="7b45c-104">Find information about the **InstallApp** EWS operation.</span></span> 
  
<span data-ttu-id="7b45c-105">A operação **InstallApp** instala um aplicativo de email para o Outlook em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7b45c-105">The **InstallApp** operation installs a mail app for Outlook in a mailbox.</span></span> 
  
<span data-ttu-id="7b45c-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7b45c-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-installapp-operation"></a><span data-ttu-id="7b45c-107">Usando a operação InstallApp</span><span class="sxs-lookup"><span data-stu-id="7b45c-107">Using the InstallApp operation</span></span>

<span data-ttu-id="7b45c-108">A operação **InstallApp** aceita um único argumento que identifica um aplicativo de email para instalar.</span><span class="sxs-lookup"><span data-stu-id="7b45c-108">The **InstallApp** operation takes a single argument that identifies a mail app to install.</span></span> <span data-ttu-id="7b45c-109">O argumento contém o manifesto codificado em base64 para um aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="7b45c-109">The argument contains the base64-encoded manifest for a mail app.</span></span> 
  
### <a name="installapp-operation-soap-headers"></a><span data-ttu-id="7b45c-110">Cabeçalhos SOAP de operação InstallApp</span><span class="sxs-lookup"><span data-stu-id="7b45c-110">InstallApp operation SOAP headers</span></span>

<span data-ttu-id="7b45c-111">A operação **InstallApp** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="7b45c-111">The **InstallApp** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="7b45c-112">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="7b45c-112">**Header name**</span></span>|<span data-ttu-id="7b45c-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7b45c-113">**Element**</span></span>|<span data-ttu-id="7b45c-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7b45c-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7b45c-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="7b45c-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="7b45c-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="7b45c-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="7b45c-117">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="7b45c-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="7b45c-118">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b45c-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="7b45c-119">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="7b45c-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="7b45c-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7b45c-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="7b45c-121">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b45c-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="7b45c-122">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="7b45c-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="installapp-operation-request-example-install-a-mail-app-in-a-mailbox"></a><span data-ttu-id="7b45c-123">Exemplo de solicitação de operação InstallApp: instalar um aplicativo de email em uma caixa de correio</span><span class="sxs-lookup"><span data-stu-id="7b45c-123">InstallApp operation request example: Install a mail app in a mailbox</span></span>

<span data-ttu-id="7b45c-124">O exemplo a seguir de uma solicitação de operação do **InstallApp** mostra como instalar um aplicativo de email para o Outlook.</span><span class="sxs-lookup"><span data-stu-id="7b45c-124">The following example of an **InstallApp** operation request shows how to install a mail app for Outlook.</span></span> <span data-ttu-id="7b45c-125">O manifesto do aplicativo pode ser encontrado usando a [operação GetAppManifests](getappmanifests-operation.md).</span><span class="sxs-lookup"><span data-stu-id="7b45c-125">The app manifest can be found by using the [GetAppManifests operation](getappmanifests-operation.md).</span></span>
  
> [!NOTE]
> <span data-ttu-id="7b45c-126">O manifesto do aplicativo codificado em Base64 foi truncado arbitrariamente para preservar a legibilidade e não representa um manifesto válido.</span><span class="sxs-lookup"><span data-stu-id="7b45c-126">The base64-encoded app manifest has been arbitrarily truncated to preserve readability and does not represent a valid manifest.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:InstallApp>
         <m:Manifest>TUwiIC8+CiAgPC9SdWxlPgo8L09mZmljZUFwcD4=</m:Manifest>
      </m:InstallApp>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="7b45c-127">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="7b45c-127">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7b45c-128">InstallApp</span><span class="sxs-lookup"><span data-stu-id="7b45c-128">InstallApp</span></span>](installapp.md)
    
- [<span data-ttu-id="7b45c-129">Manifesto</span><span class="sxs-lookup"><span data-stu-id="7b45c-129">Manifest</span></span>](manifest.md)
    
## <a name="successful-installapp-operation-response"></a><span data-ttu-id="7b45c-130">Resposta de operação InstallApp bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="7b45c-130">Successful InstallApp operation response</span></span>

<span data-ttu-id="7b45c-131">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **InstallApp** para instalar um aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="7b45c-131">The following example shows a successful response to an **InstallApp** operation request to install a mail app.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <InstallAppResponse ResponseClass="Success" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="7b45c-132">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="7b45c-132">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7b45c-133">InstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="7b45c-133">InstallAppResponse</span></span>](installappresponse.md)
    
- [<span data-ttu-id="7b45c-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7b45c-134">ResponseCode</span></span>](responsecode.md)
    
## <a name="installapp-operation-error-response"></a><span data-ttu-id="7b45c-135">Resposta de erro de operação InstallApp</span><span class="sxs-lookup"><span data-stu-id="7b45c-135">InstallApp operation error response</span></span>

<span data-ttu-id="7b45c-136">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **InstallApp** .</span><span class="sxs-lookup"><span data-stu-id="7b45c-136">The following example shows an error response to an **InstallApp** operation request.</span></span> <span data-ttu-id="7b45c-137">Esta é uma resposta a uma solicitação que contém um manifesto inválido.</span><span class="sxs-lookup"><span data-stu-id="7b45c-137">This is a response to a request that contains an invalid manifest.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <InstallAppResponse ResponseClass="Error" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>This app can't be installed. Missing OfficeApp element.</MessageText>
         <ResponseCode>ErrorInternalServerError</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="7b45c-138">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="7b45c-138">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7b45c-139">InstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="7b45c-139">InstallAppResponse</span></span>](installappresponse.md)
    
- [<span data-ttu-id="7b45c-140">MessageText</span><span class="sxs-lookup"><span data-stu-id="7b45c-140">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="7b45c-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7b45c-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7b45c-142">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7b45c-142">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="7b45c-143">Confira também</span><span class="sxs-lookup"><span data-stu-id="7b45c-143">See also</span></span>

- [<span data-ttu-id="7b45c-144">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7b45c-144">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="7b45c-145">Operação DisableApp</span><span class="sxs-lookup"><span data-stu-id="7b45c-145">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="7b45c-146">Operação UninstallApp</span><span class="sxs-lookup"><span data-stu-id="7b45c-146">UninstallApp operation</span></span>](uninstallapp-operation.md)
    
- [<span data-ttu-id="7b45c-147">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="7b45c-147">GetAppManifests</span></span>](getappmanifests.md)
    
- [<span data-ttu-id="7b45c-148">Operação GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="7b45c-148">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)
    

