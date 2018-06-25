---
title: Operação GetClientAccessToken
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 086876cc-e22c-4e89-89f9-19e78af51217
description: Encontre informações sobre o EWS GetClientAccessToken operação.
ms.openlocfilehash: afa9a315a8421f31c345c9547a5d80bed41e9fbc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752423"
---
# <a name="getclientaccesstoken-operation"></a><span data-ttu-id="44611-103">Operação GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="44611-103">GetClientAccessToken operation</span></span>

<span data-ttu-id="44611-104">Encontre informações sobre a operação de EWS **GetClientAccessToken** .</span><span class="sxs-lookup"><span data-stu-id="44611-104">Find information about the **GetClientAccessToken** EWS operation.</span></span> 
  
<span data-ttu-id="44611-105">A operação **GetClientAccessToken** obtém um acesso para cliente token para um aplicativo de email para Outlook.</span><span class="sxs-lookup"><span data-stu-id="44611-105">The **GetClientAccessToken** operation gets a client access token for a mail app for Outlook.</span></span> 
  
<span data-ttu-id="44611-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="44611-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getclientaccesstoken-operation"></a><span data-ttu-id="44611-107">Usando a operação GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="44611-107">Using the GetClientAccessToken operation</span></span>

<span data-ttu-id="44611-108">A solicitação de operação **GetClientAccessToken** leva dois argumentos obrigatórios: o identificador do aplicativo e o tipo de token.</span><span class="sxs-lookup"><span data-stu-id="44611-108">The **GetClientAccessToken** operation request takes two required arguments: the identifier of the app, and the token type.</span></span> <span data-ttu-id="44611-109">Você pode usar a [operação GetAppManifests](getappmanifests-operation.md) para solicitar o identificador de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="44611-109">You can use the [GetAppManifests operation](getappmanifests-operation.md) to request the app identifier.</span></span> 
  
### <a name="getclientaccesstoken-operation-soap-headers"></a><span data-ttu-id="44611-110">Cabeçalhos SOAP GetClientAccessToken operação</span><span class="sxs-lookup"><span data-stu-id="44611-110">GetClientAccessToken operation SOAP headers</span></span>

<span data-ttu-id="44611-111">A operação **GetClientAccessToken** pode usar os cabeçalhos SOAP que estão listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="44611-111">The **GetClientAccessToken** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="44611-112">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="44611-112">**Header name**</span></span>|<span data-ttu-id="44611-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="44611-113">**Element**</span></span>|<span data-ttu-id="44611-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="44611-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="44611-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="44611-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="44611-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="44611-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="44611-117">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="44611-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="44611-118">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="44611-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="44611-119">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="44611-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="44611-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="44611-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="44611-121">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="44611-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="44611-122">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="44611-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getclientaccesstoken-operation-request-example-get-a-caller-identity-token"></a><span data-ttu-id="44611-123">Exemplo de solicitação de operação GetClientAccessToken: Obtenha uma identidade de chamador token</span><span class="sxs-lookup"><span data-stu-id="44611-123">GetClientAccessToken operation request example: Get a caller identity token</span></span>

<span data-ttu-id="44611-124">O exemplo a seguir de uma solicitação de operação **GetClientAccessToken** mostra como obter uma identidade de chamador token para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="44611-124">The following example of a **GetClientAccessToken** operation request shows how to get a caller identity token for an app.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetClientAccessToken>
         <m:TokenRequests>
            <t:TokenRequest>
               <t:Id>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</t:Id>
               <t:TokenType>CallerIdentity</t:TokenType>
            </t:TokenRequest>
         </m:TokenRequests>
      </m:GetClientAccessToken>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="44611-125">A solicitação de corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="44611-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="44611-126">GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="44611-126">GetClientAccessToken</span></span>](getclientaccesstoken.md)
    
- [<span data-ttu-id="44611-127">TokenRequests</span><span class="sxs-lookup"><span data-stu-id="44611-127">TokenRequests</span></span>](tokenrequests.md)
    
- [<span data-ttu-id="44611-128">TokenRequest</span><span class="sxs-lookup"><span data-stu-id="44611-128">TokenRequest</span></span>](tokenrequest.md)
    
- [<span data-ttu-id="44611-129">ID (String)</span><span class="sxs-lookup"><span data-stu-id="44611-129">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="44611-130">TokenType</span><span class="sxs-lookup"><span data-stu-id="44611-130">TokenType</span></span>](tokentype.md)
    
## <a name="successful-getclientaccesstoken-operation-response"></a><span data-ttu-id="44611-131">Resposta de operação GetClientAccessToken bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="44611-131">Successful GetClientAccessToken operation response</span></span>

<span data-ttu-id="44611-132">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetClientAccessToken** para obter uma identidade de chamador token para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="44611-132">The following example shows a successful response to a **GetClientAccessToken** operation request to get a caller identity token for an app.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="44611-133">Os valores de tokens neste artigo foram diminuídos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="44611-133">The token values in this article have been shortened to preserve readability.</span></span> 
  
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
      <m:GetClientAccessTokenResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:GetClientAccessTokenResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Token>
                  <t:Id>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</t:Id>
                  <t:TokenType>CallerIdentity</t:TokenType>
                  <t:TokenValue>eyJ0eXAmv0QitaJg</t:TokenValue>
                  <t:TTL>479</t:TTL>
               </m:Token>
            </m:GetClientAccessTokenResponseMessage>
         </m:ResponseMessages>
      </m:GetClientAccessTokenResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="44611-134">A resposta SOAP body contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="44611-134">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="44611-135">GetClientAccessTokenResponse</span><span class="sxs-lookup"><span data-stu-id="44611-135">GetClientAccessTokenResponse</span></span>](getclientaccesstokenresponse.md)
    
- [<span data-ttu-id="44611-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="44611-136">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="44611-137">GetClientAccessTokenResponseMessage</span><span class="sxs-lookup"><span data-stu-id="44611-137">GetClientAccessTokenResponseMessage</span></span>](getclientaccesstokenresponsemessage.md)
    
- [<span data-ttu-id="44611-138">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="44611-138">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="44611-139">Token (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="44611-139">Token (ClientAccessTokenType)</span></span>](token-clientaccesstokentype.md)
    
- [<span data-ttu-id="44611-140">ID (String)</span><span class="sxs-lookup"><span data-stu-id="44611-140">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="44611-141">TokenType (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="44611-141">TokenType (ClientAccessTokenType)</span></span>](tokentype-clientaccesstokentype.md)
    
- [<span data-ttu-id="44611-142">TokenValue</span><span class="sxs-lookup"><span data-stu-id="44611-142">TokenValue</span></span>](tokenvalue.md)
    
- [<span data-ttu-id="44611-143">TTL (ClientAccessTokenTypeType)</span><span class="sxs-lookup"><span data-stu-id="44611-143">TTL (ClientAccessTokenTypeType)</span></span>](ttl-clientaccesstokentypetype.md)
    
## <a name="getclientaccesstoken-operation-error-response"></a><span data-ttu-id="44611-144">Resposta de erro de operação GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="44611-144">GetClientAccessToken operation error response</span></span>

<span data-ttu-id="44611-145">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **GetClientAccessToken** .</span><span class="sxs-lookup"><span data-stu-id="44611-145">The following example shows an error response to a **GetClientAccessToken** operation request.</span></span> <span data-ttu-id="44611-146">Esta é uma resposta a uma solicitação para obter um retorno de chamada de extensão token sem as permissões apropriadas.</span><span class="sxs-lookup"><span data-stu-id="44611-146">This is a response to a request to get an extension callback token without the appropriate permissions.</span></span> 
  
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
      <m:GetClientAccessTokenResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:GetClientAccessTokenResponseMessage ResponseClass="Error">
               <m:MessageText>The caller does not have enough permission for this token request.</m:MessageText>
               <m:ResponseCode>ErrorInvalidClientAccessTokenRequest</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
            </m:GetClientAccessTokenResponseMessage>
         </m:ResponseMessages>
      </m:GetClientAccessTokenResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="44611-147">A resposta de erro corpo SOAP contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="44611-147">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="44611-148">GetClientAccessTokenResponse</span><span class="sxs-lookup"><span data-stu-id="44611-148">GetClientAccessTokenResponse</span></span>](getclientaccesstokenresponse.md)
    
- [<span data-ttu-id="44611-149">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="44611-149">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="44611-150">GetClientAccessTokenResponseMessage</span><span class="sxs-lookup"><span data-stu-id="44611-150">GetClientAccessTokenResponseMessage</span></span>](getclientaccesstokenresponsemessage.md)
    
- [<span data-ttu-id="44611-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="44611-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="44611-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="44611-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="44611-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="44611-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="44611-154">Para códigos de erro adicionais que são genérica do EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="44611-154">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="44611-155">Confira também</span><span class="sxs-lookup"><span data-stu-id="44611-155">See also</span></span>

- [<span data-ttu-id="44611-156">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="44611-156">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="44611-157">Operação GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="44611-157">GetAppManifests operation</span></span>](getappmanifests-operation.md)
    
- <span data-ttu-id="44611-158">
  [Suplementos do Outlook](http://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="44611-158">[Outlook add-ins](http://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)</span></span>
    

