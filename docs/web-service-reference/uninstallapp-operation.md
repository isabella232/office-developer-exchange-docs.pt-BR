---
title: Operação UninstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7707aa6a-381d-43f7-a454-54f6343ed127
description: Encontre informações sobre a operação do EWS do UninstallApp.
ms.openlocfilehash: 27931636ee13a251fb03fe804987d7b01a325230
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467148"
---
# <a name="uninstallapp-operation"></a><span data-ttu-id="6f0e1-103">Operação UninstallApp</span><span class="sxs-lookup"><span data-stu-id="6f0e1-103">UninstallApp operation</span></span>

<span data-ttu-id="6f0e1-104">Encontre informações sobre a operação do EWS do **UninstallApp** .</span><span class="sxs-lookup"><span data-stu-id="6f0e1-104">Find information about the **UninstallApp** EWS operation.</span></span> 
  
<span data-ttu-id="6f0e1-105">A operação **UninstallApp** desinstala um aplicativo de email para o Outlook.</span><span class="sxs-lookup"><span data-stu-id="6f0e1-105">The **UninstallApp** operation uninstalls a mail app for Outlook.</span></span> 
  
<span data-ttu-id="6f0e1-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6f0e1-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-uninstallapp-operation"></a><span data-ttu-id="6f0e1-107">Usando a operação UninstallApp</span><span class="sxs-lookup"><span data-stu-id="6f0e1-107">Using the UninstallApp operation</span></span>

<span data-ttu-id="6f0e1-108">A operação **UninstallApp** aceita um argumento na solicitação que identifica o aplicativo de email a ser desinstalado.</span><span class="sxs-lookup"><span data-stu-id="6f0e1-108">The **UninstallApp** operation takes one argument in the request that identifies the mail app to uninstall.</span></span> 
  
### <a name="uninstallapp-operation-soap-headers"></a><span data-ttu-id="6f0e1-109">Cabeçalhos SOAP de operação UninstallApp</span><span class="sxs-lookup"><span data-stu-id="6f0e1-109">UninstallApp operation SOAP headers</span></span>

<span data-ttu-id="6f0e1-110">A operação **UninstallApp** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="6f0e1-110">The **UninstallApp** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="6f0e1-111">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="6f0e1-111">**Header name**</span></span>|<span data-ttu-id="6f0e1-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="6f0e1-112">**Element**</span></span>|<span data-ttu-id="6f0e1-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="6f0e1-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6f0e1-114">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="6f0e1-114">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="6f0e1-115">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="6f0e1-115">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="6f0e1-116">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="6f0e1-116">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="6f0e1-117">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f0e1-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="6f0e1-118">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="6f0e1-118">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="6f0e1-119">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="6f0e1-119">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="6f0e1-120">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f0e1-120">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="6f0e1-121">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="6f0e1-121">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="uninstallapp-operation-request-example-uninstall-a-mail-app-in-a-mailbox"></a><span data-ttu-id="6f0e1-122">Exemplo de solicitação de operação UninstallApp: desinstalar um aplicativo de email em uma caixa de correio</span><span class="sxs-lookup"><span data-stu-id="6f0e1-122">UninstallApp operation request example: Uninstall a mail app in a mailbox</span></span>

<span data-ttu-id="6f0e1-123">O exemplo a seguir de uma solicitação de operação do **UninstallApp** mostra como um aplicativo de email é desinstalado usando o identificador de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6f0e1-123">The following example of an **UninstallApp** operation request shows how to a uninstall a mail app by using the app identifier.</span></span> <span data-ttu-id="6f0e1-124">O identificador do aplicativo pode ser encontrado no manifesto do aplicativo que é retornado pela [operação GetAppManifests](getappmanifests-operation.md).</span><span class="sxs-lookup"><span data-stu-id="6f0e1-124">The app identifier can be found in the app manifest that is returned by the [GetAppManifests operation](getappmanifests-operation.md).</span></span>
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:UninstallApp>
         <m:ID>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</m:ID>
      </m:UninstallApp>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="6f0e1-125">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="6f0e1-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="6f0e1-126">UninstallApp</span><span class="sxs-lookup"><span data-stu-id="6f0e1-126">UninstallApp</span></span>](uninstallapp.md)
    
- [<span data-ttu-id="6f0e1-127">ID (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="6f0e1-127">ID (String)</span></span>](id-string.md)
    
## <a name="successful-uninstallapp-operation-response"></a><span data-ttu-id="6f0e1-128">Resposta de operação UninstallApp bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="6f0e1-128">Successful UninstallApp operation response</span></span>

<span data-ttu-id="6f0e1-129">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação do **UninstallApp** para desinstalar um aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="6f0e1-129">The following example shows a successful response to an **UninstallApp** operation request to uninstall a mail app.</span></span> 
  
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
      <UninstallAppResponse ResponseClass="Success" 
                            xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </UninstallAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="6f0e1-130">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="6f0e1-130">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="6f0e1-131">UninstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="6f0e1-131">UninstallAppResponse</span></span>](uninstallappresponse.md)
    
- [<span data-ttu-id="6f0e1-132">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="6f0e1-132">ResponseCode</span></span>](responsecode.md)
    
## <a name="uninstallapp-operation-error-response"></a><span data-ttu-id="6f0e1-133">Resposta de erro de operação UninstallApp</span><span class="sxs-lookup"><span data-stu-id="6f0e1-133">UninstallApp operation error response</span></span>

<span data-ttu-id="6f0e1-134">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **UninstallApp** .</span><span class="sxs-lookup"><span data-stu-id="6f0e1-134">The following example shows an error response to an **UninstallApp** operation request.</span></span> <span data-ttu-id="6f0e1-135">Esta é uma resposta a uma solicitação para desinstalar um aplicativo de email que já foi desinstalado.</span><span class="sxs-lookup"><span data-stu-id="6f0e1-135">This is a response to a request to uninstall a mail app that has already been uninstalled.</span></span> 
  
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
      <UninstallAppResponse ResponseClass="Error" 
                            xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Extension ID 1c50226d-04b5-4ab2-9fcd-42e236b59e4b can't be found.</MessageText>
         <ResponseCode>ErrorInternalServerError</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </UninstallAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="6f0e1-136">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="6f0e1-136">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="6f0e1-137">UninstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="6f0e1-137">UninstallAppResponse</span></span>](uninstallappresponse.md)
    
- [<span data-ttu-id="6f0e1-138">MessageText</span><span class="sxs-lookup"><span data-stu-id="6f0e1-138">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="6f0e1-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="6f0e1-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="6f0e1-140">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="6f0e1-140">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="6f0e1-141">Para obter códigos de erro adicionais genéricos para o EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="6f0e1-141">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="6f0e1-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="6f0e1-142">See also</span></span>

- [<span data-ttu-id="6f0e1-143">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="6f0e1-143">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="6f0e1-144">Operação InstallApp</span><span class="sxs-lookup"><span data-stu-id="6f0e1-144">InstallApp operation</span></span>](installapp-operation.md)
    
- [<span data-ttu-id="6f0e1-145">Operação DisableApp</span><span class="sxs-lookup"><span data-stu-id="6f0e1-145">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="6f0e1-146">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="6f0e1-146">GetAppManifests</span></span>](getappmanifests.md)
    
- [<span data-ttu-id="6f0e1-147">Operação GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="6f0e1-147">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)
    

