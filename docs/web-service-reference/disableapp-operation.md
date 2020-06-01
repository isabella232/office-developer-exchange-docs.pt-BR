---
title: Operação DisableApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 211731a3-2470-49af-bda3-1ddfc15a8e46
description: Encontre informações sobre a operação do EWS do DisableApp.
ms.openlocfilehash: 8e1f3a257a70c042a01ed70da97cfa0573a2d454
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462063"
---
# <a name="disableapp-operation"></a><span data-ttu-id="d7931-103">Operação DisableApp</span><span class="sxs-lookup"><span data-stu-id="d7931-103">DisableApp operation</span></span>

<span data-ttu-id="d7931-104">Encontre informações sobre a operação do EWS do **DisableApp** .</span><span class="sxs-lookup"><span data-stu-id="d7931-104">Find information about the **DisableApp** EWS operation.</span></span> 
  
<span data-ttu-id="d7931-105">A operação **DisableApp** desabilita um aplicativo de email para o Outlook.</span><span class="sxs-lookup"><span data-stu-id="d7931-105">The **DisableApp** operation disables a mail app for Outlook.</span></span> 
  
<span data-ttu-id="d7931-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d7931-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-disableapp-operation"></a><span data-ttu-id="d7931-107">Usando a operação DisableApp</span><span class="sxs-lookup"><span data-stu-id="d7931-107">Using the DisableApp operation</span></span>

<span data-ttu-id="d7931-108">A operação **DisableApp** leva dois argumentos na solicitação que identificam o aplicativo de email a ser desabilitado e o motivo pelo qual ele foi desabilitado.</span><span class="sxs-lookup"><span data-stu-id="d7931-108">The **DisableApp** operation takes two arguments in the request that identify the mail app to disable and the reason why it was disabled.</span></span> 
  
### <a name="disableapp-operation-soap-headers"></a><span data-ttu-id="d7931-109">Cabeçalhos SOAP de operação DisableApp</span><span class="sxs-lookup"><span data-stu-id="d7931-109">DisableApp operation SOAP headers</span></span>

<span data-ttu-id="d7931-110">A operação **DisableApp** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="d7931-110">The **DisableApp** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="d7931-111">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="d7931-111">**Header name**</span></span>|<span data-ttu-id="d7931-112">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d7931-112">**Element**</span></span>|<span data-ttu-id="d7931-113">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d7931-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d7931-114">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="d7931-114">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="d7931-115">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="d7931-115">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="d7931-116">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="d7931-116">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="d7931-117">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7931-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d7931-118">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="d7931-118">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="d7931-119">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d7931-119">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="d7931-120">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="d7931-120">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="d7931-121">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="d7931-121">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="disableapp-operation-request-example-disable-a-mail-app-installed-in-a-mailbox"></a><span data-ttu-id="d7931-122">Exemplo de solicitação de operação DisableApp: desabilitar um aplicativo de email instalado em uma caixa de correio</span><span class="sxs-lookup"><span data-stu-id="d7931-122">DisableApp operation request example: Disable a mail app installed in a mailbox</span></span>

<span data-ttu-id="d7931-123">O exemplo a seguir de uma solicitação de operação **DisableApp** mostra como um aplicativo de email desabilitado.</span><span class="sxs-lookup"><span data-stu-id="d7931-123">The following example of a **DisableApp** operation request shows how to a disable a mail app.</span></span> <span data-ttu-id="d7931-124">O identificador do aplicativo pode ser encontrado no manifesto do aplicativo que é retornado em uma resposta de [operação GetAppManifests](getappmanifests-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d7931-124">The app identifier can be found in the app manifest that is returned in a [GetAppManifests operation](getappmanifests-operation.md) response.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:DisableApp>
         <m:ID>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</m:ID>
         <m:DisableReason>NoReason</m:DisableReason>
      </m:DisableApp>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="d7931-125">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="d7931-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d7931-126">DisableApp</span><span class="sxs-lookup"><span data-stu-id="d7931-126">DisableApp</span></span>](disableapp.md)
    
- [<span data-ttu-id="d7931-127">ID (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="d7931-127">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="d7931-128">DisableReason</span><span class="sxs-lookup"><span data-stu-id="d7931-128">DisableReason</span></span>](disablereason.md)
    
## <a name="successful-disableapp-operation-response"></a><span data-ttu-id="d7931-129">Resposta de operação DisableApp bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="d7931-129">Successful DisableApp operation response</span></span>

<span data-ttu-id="d7931-130">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **DisableApp** para desabilitar um aplicativo de email.</span><span class="sxs-lookup"><span data-stu-id="d7931-130">The following example shows a successful response to a **DisableApp** operation request to disable a mail app.</span></span> 
  
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
      <DisableAppResponse ResponseClass="Success" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </DisableAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="d7931-131">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="d7931-131">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d7931-132">DisableAppResponse</span><span class="sxs-lookup"><span data-stu-id="d7931-132">DisableAppResponse</span></span>](disableappresponse.md)
    
- [<span data-ttu-id="d7931-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d7931-133">ResponseCode</span></span>](responsecode.md)
    
## <a name="disableapp-operation-error-response"></a><span data-ttu-id="d7931-134">Resposta de erro de operação DisableApp</span><span class="sxs-lookup"><span data-stu-id="d7931-134">DisableApp operation error response</span></span>

<span data-ttu-id="d7931-135">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **DisableApp** .</span><span class="sxs-lookup"><span data-stu-id="d7931-135">The following example shows an error response to a **DisableApp** operation request.</span></span> <span data-ttu-id="d7931-136">Esta é uma resposta a uma solicitação para desabilitar um aplicativo de email que não está instalado em uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d7931-136">This is a response to a request to disable a mail app that is not installed in a mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="556" MinorBuildNumber="14" Version="Exchange2013" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <DisableAppResponse ResponseClass="Error" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Extension ID 1C50226D-04B5-4AB2-9FCD-42E236B59E4A can't be found.</MessageText>
         <ResponseCode>ErrorExtensionNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </DisableAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="d7931-137">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="d7931-137">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d7931-138">DisableAppResponse</span><span class="sxs-lookup"><span data-stu-id="d7931-138">DisableAppResponse</span></span>](disableappresponse.md)
    
- [<span data-ttu-id="d7931-139">MessageText</span><span class="sxs-lookup"><span data-stu-id="d7931-139">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="d7931-140">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d7931-140">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d7931-141">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d7931-141">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="d7931-142">Para obter códigos de erro adicionais genéricos para o EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="d7931-142">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="d7931-143">Também consulte</span><span class="sxs-lookup"><span data-stu-id="d7931-143">See also</span></span>

- [<span data-ttu-id="d7931-144">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d7931-144">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)   
- [<span data-ttu-id="d7931-145">Operação InstallApp</span><span class="sxs-lookup"><span data-stu-id="d7931-145">InstallApp operation</span></span>](installapp-operation.md)   
- [<span data-ttu-id="d7931-146">Operação UninstallApp</span><span class="sxs-lookup"><span data-stu-id="d7931-146">UninstallApp operation</span></span>](uninstallapp-operation.md)   
- [<span data-ttu-id="d7931-147">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="d7931-147">GetAppManifests</span></span>](getappmanifests.md)   
- [<span data-ttu-id="d7931-148">Operação GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="d7931-148">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)   
- [<span data-ttu-id="d7931-149">Suplementos do Outlook</span><span class="sxs-lookup"><span data-stu-id="d7931-149">Outlook add-ins</span></span>](https://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)
    

