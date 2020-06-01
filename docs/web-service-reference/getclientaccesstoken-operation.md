---
title: Operação GetClientAccessToken
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 086876cc-e22c-4e89-89f9-19e78af51217
description: Encontre informações sobre a operação do EWS do GetClientAccessToken.
ms.openlocfilehash: 2d49d675fcedb0e7e8312a9715f095c47fcf3d77
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462035"
---
# <a name="getclientaccesstoken-operation"></a><span data-ttu-id="68c9d-103">Operação GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="68c9d-103">GetClientAccessToken operation</span></span>

<span data-ttu-id="68c9d-104">Encontre informações sobre a operação do EWS do **GetClientAccessToken** .</span><span class="sxs-lookup"><span data-stu-id="68c9d-104">Find information about the **GetClientAccessToken** EWS operation.</span></span> 
  
<span data-ttu-id="68c9d-105">A operação **GetClientAccessToken** Obtém um token de acesso para cliente para um aplicativo de email para o Outlook.</span><span class="sxs-lookup"><span data-stu-id="68c9d-105">The **GetClientAccessToken** operation gets a client access token for a mail app for Outlook.</span></span> 
  
<span data-ttu-id="68c9d-106">This operation was introduced in Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="68c9d-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getclientaccesstoken-operation"></a><span data-ttu-id="68c9d-107">Usando a operação GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="68c9d-107">Using the GetClientAccessToken operation</span></span>

<span data-ttu-id="68c9d-108">A solicitação de operação **GetClientAccessToken** aceita dois argumentos obrigatórios: o identificador do aplicativo e o tipo de token.</span><span class="sxs-lookup"><span data-stu-id="68c9d-108">The **GetClientAccessToken** operation request takes two required arguments: the identifier of the app, and the token type.</span></span> <span data-ttu-id="68c9d-109">Você pode usar a [operação GetAppManifests](getappmanifests-operation.md) para solicitar o identificador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="68c9d-109">You can use the [GetAppManifests operation](getappmanifests-operation.md) to request the app identifier.</span></span> 
  
### <a name="getclientaccesstoken-operation-soap-headers"></a><span data-ttu-id="68c9d-110">Cabeçalhos SOAP de operação GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="68c9d-110">GetClientAccessToken operation SOAP headers</span></span>

<span data-ttu-id="68c9d-111">A operação **GetClientAccessToken** pode usar os cabeçalhos SOAP listados na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="68c9d-111">The **GetClientAccessToken** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="68c9d-112">**Nome de cabeçalho**</span><span class="sxs-lookup"><span data-stu-id="68c9d-112">**Header name**</span></span>|<span data-ttu-id="68c9d-113">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="68c9d-113">**Element**</span></span>|<span data-ttu-id="68c9d-114">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="68c9d-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="68c9d-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="68c9d-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="68c9d-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="68c9d-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="68c9d-117">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="68c9d-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="68c9d-118">Este cabeçalho é aplicável a uma solicitação.</span><span class="sxs-lookup"><span data-stu-id="68c9d-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="68c9d-119">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="68c9d-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="68c9d-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="68c9d-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="68c9d-121">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="68c9d-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="68c9d-122">Este cabeçalho é aplicável a uma resposta.</span><span class="sxs-lookup"><span data-stu-id="68c9d-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getclientaccesstoken-operation-request-example-get-a-caller-identity-token"></a><span data-ttu-id="68c9d-123">Exemplo de solicitação de operação GetClientAccessToken: obter um token de identidade de chamador</span><span class="sxs-lookup"><span data-stu-id="68c9d-123">GetClientAccessToken operation request example: Get a caller identity token</span></span>

<span data-ttu-id="68c9d-124">O exemplo a seguir de uma solicitação de operação **GetClientAccessToken** mostra como obter um token de identidade de chamador para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="68c9d-124">The following example of a **GetClientAccessToken** operation request shows how to get a caller identity token for an app.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="68c9d-125">O corpo SOAP de solicitação contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="68c9d-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="68c9d-126">GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="68c9d-126">GetClientAccessToken</span></span>](getclientaccesstoken.md)
    
- [<span data-ttu-id="68c9d-127">TokenRequests</span><span class="sxs-lookup"><span data-stu-id="68c9d-127">TokenRequests</span></span>](tokenrequests.md)
    
- [<span data-ttu-id="68c9d-128">TokenRequest</span><span class="sxs-lookup"><span data-stu-id="68c9d-128">TokenRequest</span></span>](tokenrequest.md)
    
- [<span data-ttu-id="68c9d-129">ID (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="68c9d-129">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="68c9d-130">TokenType</span><span class="sxs-lookup"><span data-stu-id="68c9d-130">TokenType</span></span>](tokentype.md)
    
## <a name="successful-getclientaccesstoken-operation-response"></a><span data-ttu-id="68c9d-131">Resposta de operação GetClientAccessToken bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="68c9d-131">Successful GetClientAccessToken operation response</span></span>

<span data-ttu-id="68c9d-132">O exemplo a seguir mostra uma resposta bem-sucedida a uma solicitação de operação **GetClientAccessToken** para obter um token de identidade de chamador para um aplicativo.</span><span class="sxs-lookup"><span data-stu-id="68c9d-132">The following example shows a successful response to a **GetClientAccessToken** operation request to get a caller identity token for an app.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="68c9d-133">Os valores de token neste artigo foram reduzidos para preservar a legibilidade.</span><span class="sxs-lookup"><span data-stu-id="68c9d-133">The token values in this article have been shortened to preserve readability.</span></span> 
  
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
      <m:GetClientAccessTokenResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="68c9d-134">O corpo SOAP de resposta contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="68c9d-134">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="68c9d-135">GetClientAccessTokenResponse</span><span class="sxs-lookup"><span data-stu-id="68c9d-135">GetClientAccessTokenResponse</span></span>](getclientaccesstokenresponse.md)
    
- [<span data-ttu-id="68c9d-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="68c9d-136">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="68c9d-137">GetClientAccessTokenResponseMessage</span><span class="sxs-lookup"><span data-stu-id="68c9d-137">GetClientAccessTokenResponseMessage</span></span>](getclientaccesstokenresponsemessage.md)
    
- [<span data-ttu-id="68c9d-138">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="68c9d-138">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="68c9d-139">Token (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="68c9d-139">Token (ClientAccessTokenType)</span></span>](token-clientaccesstokentype.md)
    
- [<span data-ttu-id="68c9d-140">ID (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="68c9d-140">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="68c9d-141">TokenType (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="68c9d-141">TokenType (ClientAccessTokenType)</span></span>](tokentype-clientaccesstokentype.md)
    
- [<span data-ttu-id="68c9d-142">TokenValue</span><span class="sxs-lookup"><span data-stu-id="68c9d-142">TokenValue</span></span>](tokenvalue.md)
    
- [<span data-ttu-id="68c9d-143">TTL (ClientAccessTokenTypeType)</span><span class="sxs-lookup"><span data-stu-id="68c9d-143">TTL (ClientAccessTokenTypeType)</span></span>](ttl-clientaccesstokentypetype.md)
    
## <a name="getclientaccesstoken-operation-error-response"></a><span data-ttu-id="68c9d-144">Resposta de erro de operação GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="68c9d-144">GetClientAccessToken operation error response</span></span>

<span data-ttu-id="68c9d-145">O exemplo a seguir mostra uma resposta de erro a uma solicitação de operação **GetClientAccessToken** .</span><span class="sxs-lookup"><span data-stu-id="68c9d-145">The following example shows an error response to a **GetClientAccessToken** operation request.</span></span> <span data-ttu-id="68c9d-146">Esta é uma resposta a uma solicitação para obter um token de retorno de chamada de extensão sem as permissões apropriadas.</span><span class="sxs-lookup"><span data-stu-id="68c9d-146">This is a response to a request to get an extension callback token without the appropriate permissions.</span></span> 
  
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
      <m:GetClientAccessTokenResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="68c9d-147">O corpo SOAP de resposta de erro contém os seguintes elementos:</span><span class="sxs-lookup"><span data-stu-id="68c9d-147">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="68c9d-148">GetClientAccessTokenResponse</span><span class="sxs-lookup"><span data-stu-id="68c9d-148">GetClientAccessTokenResponse</span></span>](getclientaccesstokenresponse.md)
    
- [<span data-ttu-id="68c9d-149">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="68c9d-149">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="68c9d-150">GetClientAccessTokenResponseMessage</span><span class="sxs-lookup"><span data-stu-id="68c9d-150">GetClientAccessTokenResponseMessage</span></span>](getclientaccesstokenresponsemessage.md)
    
- [<span data-ttu-id="68c9d-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="68c9d-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="68c9d-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="68c9d-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="68c9d-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="68c9d-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="68c9d-154">Para obter códigos de erro adicionais genéricos para o EWS e específicos para essa operação, consulte [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="68c9d-154">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="68c9d-155">Também consulte</span><span class="sxs-lookup"><span data-stu-id="68c9d-155">See also</span></span>

- [<span data-ttu-id="68c9d-156">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="68c9d-156">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="68c9d-157">Operação GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="68c9d-157">GetAppManifests operation</span></span>](getappmanifests-operation.md)
    
- [<span data-ttu-id="68c9d-158">Suplementos do Outlook</span><span class="sxs-lookup"><span data-stu-id="68c9d-158">Outlook add-ins</span></span>](https://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)
    

