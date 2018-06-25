---
title: Operação UninstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7707aa6a-381d-43f7-a454-54f6343ed127
description: Encontre informações sobre o EWS UninstallApp operação.
ms.openlocfilehash: 4f44224651993023336eef5540ec29b7f6a6e32e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19837832"
---
# <a name="uninstallapp-operation"></a><span data-ttu-id="7d440-103">Operação UninstallApp</span><span class="sxs-lookup"><span data-stu-id="7d440-103">UninstallApp operation</span></span>

<span data-ttu-id="7d440-104">Encontre informações sobre a operação de EWS **UninstallApp** .</span><span class="sxs-lookup"><span data-stu-id="7d440-104">Find information about the **UninstallApp** EWS operation.</span></span> 
  
<span data-ttu-id="7d440-105">A operação **UninstallApp** desinstala um aplicativo de email para Outlook.</span><span class="sxs-lookup"><span data-stu-id="7d440-105">The **UninstallApp** operation uninstalls a mail app for Outlook.</span></span> 
  
<span data-ttu-id="7d440-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7d440-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-uninstallapp-operation"></a><span data-ttu-id="7d440-107">Usando a operação UninstallApp</span><span class="sxs-lookup"><span data-stu-id="7d440-107">Using the UninstallApp operation</span></span>

<span data-ttu-id="7d440-108">A operação **UninstallApp** tem um argumento na solicitação que identifica o aplicativo de email para desinstalar.</span><span class="sxs-lookup"><span data-stu-id="7d440-108">The **UninstallApp** operation takes one argument in the request that identifies the mail app to uninstall.</span></span> 
  
### <a name="uninstallapp-operation-soap-headers"></a><span data-ttu-id="7d440-109">Cabeçalhos SOAP UninstallApp operação</span><span class="sxs-lookup"><span data-stu-id="7d440-109">UninstallApp operation SOAP headers</span></span>

<span data-ttu-id="7d440-110">A operação **UninstallApp** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="7d440-110">The **UninstallApp** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="7d440-111">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="7d440-111">**Header name**</span></span>|<span data-ttu-id="7d440-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="7d440-112">**Element**</span></span>|<span data-ttu-id="7d440-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="7d440-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7d440-114">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="7d440-114">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="7d440-115">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="7d440-115">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="7d440-116">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="7d440-116">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="7d440-117">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d440-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="7d440-118">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="7d440-118">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="7d440-119">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7d440-119">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="7d440-120">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="7d440-120">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="7d440-121">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="7d440-121">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="uninstallapp-operation-request-example-uninstall-a-mail-app-in-a-mailbox"></a><span data-ttu-id="7d440-122">Exemplo de solicitação de operação UninstallApp: desinstalar um aplicativo de email em uma caixa de correio</span><span class="sxs-lookup"><span data-stu-id="7d440-122">UninstallApp operation request example: Uninstall a mail app in a mailbox</span></span>

<span data-ttu-id="7d440-123">O exemplo a seguir de uma operação **UninstallApp** solicitar mostra como a uma desinstalação de um aplicativo de email usando o identificador de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="7d440-123">The following example of an **UninstallApp** operation request shows how to a uninstall a mail app by using the app identifier.</span></span> <span data-ttu-id="7d440-124">O identificador de aplicativo pode ser encontrado no manifesto do aplicativo que é retornado pela [operação de GetAppManifests](getappmanifests-operation.md).</span><span class="sxs-lookup"><span data-stu-id="7d440-124">The app identifier can be found in the app manifest that is returned by the [GetAppManifests operation](getappmanifests-operation.md).</span></span>
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="7d440-125">A solicitação de corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="7d440-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7d440-126">UninstallApp</span><span class="sxs-lookup"><span data-stu-id="7d440-126">UninstallApp</span></span>](uninstallapp.md)
    
- [<span data-ttu-id="7d440-127">ID (String)</span><span class="sxs-lookup"><span data-stu-id="7d440-127">ID (String)</span></span>](id-string.md)
    
## <a name="successful-uninstallapp-operation-response"></a><span data-ttu-id="7d440-128">Resposta de operação UninstallApp bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="7d440-128">Successful UninstallApp operation response</span></span>

<span data-ttu-id="7d440-129">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **UninstallApp** para desinstalar um aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="7d440-129">The following example shows a successful response to an **UninstallApp** operation request to uninstall a mail app.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <UninstallAppResponse ResponseClass="Success" 
                            xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </UninstallAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="7d440-130">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="7d440-130">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7d440-131">UninstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="7d440-131">UninstallAppResponse</span></span>](uninstallappresponse.md)
    
- [<span data-ttu-id="7d440-132">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7d440-132">ResponseCode</span></span>](responsecode.md)
    
## <a name="uninstallapp-operation-error-response"></a><span data-ttu-id="7d440-133">Resposta de erro de operação UninstallApp</span><span class="sxs-lookup"><span data-stu-id="7d440-133">UninstallApp operation error response</span></span>

<span data-ttu-id="7d440-134">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **UninstallApp** .</span><span class="sxs-lookup"><span data-stu-id="7d440-134">The following example shows an error response to an **UninstallApp** operation request.</span></span> <span data-ttu-id="7d440-135">Esta é uma resposta a uma solicitação para desinstalar um aplicativo de email que já está desinstalado.</span><span class="sxs-lookup"><span data-stu-id="7d440-135">This is a response to a request to uninstall a mail app that has already been uninstalled.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <UninstallAppResponse ResponseClass="Error" 
                            xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Extension ID 1c50226d-04b5-4ab2-9fcd-42e236b59e4b can't be found.</MessageText>
         <ResponseCode>ErrorInternalServerError</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </UninstallAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="7d440-136">A resposta de erro corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="7d440-136">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7d440-137">UninstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="7d440-137">UninstallAppResponse</span></span>](uninstallappresponse.md)
    
- [<span data-ttu-id="7d440-138">MessageText</span><span class="sxs-lookup"><span data-stu-id="7d440-138">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="7d440-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7d440-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7d440-140">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7d440-140">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="7d440-141">Para códigos de erro adicionais que são genérica do EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="7d440-141">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="7d440-142">Confira também</span><span class="sxs-lookup"><span data-stu-id="7d440-142">See also</span></span>

- [<span data-ttu-id="7d440-143">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="7d440-143">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="7d440-144">Operação InstallApp</span><span class="sxs-lookup"><span data-stu-id="7d440-144">InstallApp operation</span></span>](installapp-operation.md)
    
- [<span data-ttu-id="7d440-145">Operação DisableApp</span><span class="sxs-lookup"><span data-stu-id="7d440-145">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="7d440-146">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="7d440-146">GetAppManifests</span></span>](getappmanifests.md)
    
- [<span data-ttu-id="7d440-147">Operação GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="7d440-147">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)
    

