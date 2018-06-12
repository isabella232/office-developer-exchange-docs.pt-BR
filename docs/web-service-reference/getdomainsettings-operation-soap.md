---
title: Operação de GetDomainSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a6f4a53d-d7f6-4ad1-8afb-78745c500eaa
description: A operação GetDomainSettings recupera as configurações especificadas do domínio para o usuário. Descoberta automática retorna os domínios que devem ser descobertos e as configurações solicitadas desses domínios.
ms.openlocfilehash: 09b1d610cd415d2d9d7d0098354521ece86f5184
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19752475"
---
# <a name="getdomainsettings-operation-soap"></a><span data-ttu-id="c64f2-104">Operação de GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c64f2-104">GetDomainSettings operation (SOAP)</span></span>

<span data-ttu-id="c64f2-105">A operação **GetDomainSettings** recupera as configurações especificadas do domínio para o usuário.</span><span class="sxs-lookup"><span data-stu-id="c64f2-105">The **GetDomainSettings** operation retrieves the specified settings of the domain for the user.</span></span> <span data-ttu-id="c64f2-106">Descoberta automática retorna os domínios que devem ser descobertos e as configurações solicitadas desses domínios.</span><span class="sxs-lookup"><span data-stu-id="c64f2-106">Autodiscover returns the domains that are to be discovered and the requested settings of those domains.</span></span> 
  
## <a name="getdomainsettings-request-example"></a><span data-ttu-id="c64f2-107">Exemplo de solicitação de GetDomainSettings</span><span class="sxs-lookup"><span data-stu-id="c64f2-107">GetDomainSettings request example</span></span>

### <a name="description"></a><span data-ttu-id="c64f2-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="c64f2-108">Description</span></span>

<span data-ttu-id="c64f2-109">O exemplo a seguir de uma solicitação de **GetDomainSettings** mostra uma solicitação para configurações de um usuário de domínio **ExternalEWSUrl** .</span><span class="sxs-lookup"><span data-stu-id="c64f2-109">The following example of a **GetDomainSettings** request shows a request for a user's **ExternalEWSUrl** domain settings.</span></span> <span data-ttu-id="c64f2-110">O cliente envia essa solicitação ao servidor.</span><span class="sxs-lookup"><span data-stu-id="c64f2-110">The client sends this request to the server.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c64f2-111">Código</span><span class="sxs-lookup"><span data-stu-id="c64f2-111">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?> 
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover"
               xmlns:wsa="http://www.w3.org/2005/08/addressing"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"> 
    <soap:Header> 
        <a:RequestedServerVersion>Exchange2010</a:RequestedServerVersion>
        <wsa:Action>http://schemas.microsoft.com/exchange/2010/
            Autodiscover/Autodiscover/GetDomainSettings</wsa:Action>
        <wsa:To>
            https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc
        </wsa:To>
    </soap:Header> 
    <soap:Body> 
        <a:GetDomainSettingsRequestMessage xmlns:a="http://schemas.microsoft.com
            /exchange/2010/Autodiscover"> 
            <a:Request> 
                <a:Domains> 
                    <a:Domain>contoso.com<</a:Domain> 
                </a:Domains> 
                <a:RequestedSettings> 
                    <a:Setting>ExternalEwsUrl</a:Setting> 
                </a:RequestedSettings> 
            </a:Request> 
        </a:GetDomainSettingsRequestMessage> 
    </soap:Body> 
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="c64f2-112">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c64f2-112">Request elements</span></span>

<span data-ttu-id="c64f2-113">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="c64f2-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="c64f2-114">GetDomainSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c64f2-114">GetDomainSettingsRequestMessage (SOAP)</span></span>](getdomainsettingsrequestmessage-soap.md)
    
- [<span data-ttu-id="c64f2-115">Solicitação (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c64f2-115">Request (SOAP)</span></span>](request-soap.md)
    
- [<span data-ttu-id="c64f2-116">Domínios (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c64f2-116">Domains (SOAP)</span></span>](domains-soap.md)
    
- [<span data-ttu-id="c64f2-117">Domínio (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c64f2-117">Domain (SOAP)</span></span>](domain-soap.md)
    
- [<span data-ttu-id="c64f2-118">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c64f2-118">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md)
    
- [<span data-ttu-id="c64f2-119">Configuração (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c64f2-119">Setting (SOAP)</span></span>](setting-soap.md)
    
## <a name="getdomainsettings-response-example"></a><span data-ttu-id="c64f2-120">Exemplo de resposta GetDomainSettings</span><span class="sxs-lookup"><span data-stu-id="c64f2-120">GetDomainSettings response example</span></span>

### <a name="description"></a><span data-ttu-id="c64f2-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="c64f2-121">Description</span></span>

<span data-ttu-id="c64f2-122">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação de **GetDomainSettings** que o servidor envia para o cliente.</span><span class="sxs-lookup"><span data-stu-id="c64f2-122">The following example shows a successful response to the **GetDomainSettings** request that the server sends to the client.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c64f2-123">Código</span><span class="sxs-lookup"><span data-stu-id="c64f2-123">Code</span></span>

```XML
//www.w3.org/2005/08/addressing"> 
    <s:Header> 
        <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/ 
            Autodiscover/Autodiscover/GetDomainSettingsResponse
        </a:Action> 
        <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
            xmlns:i="http://www.w3.org/2001/XMLSchema-instance"> 
        <h:MajorVersion>14</h:MajorVersion> 
        <h:MinorVersion>0</h:MinorVersion> 
        <h:MajorBuildNumber>639</h:MajorBuildNumber> 
        <h:MinorBuildNumber>20</h:MinorBuildNumber> 
        <h:Version>Exchange2010</h:Version> 
        </h:ServerVersionInfo>
    </s:Header> 
    <s:Body> 
        <GetDomainSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance"> 
                <ErrorCode>NoError</ErrorCode> 
                <ErrorMessage /> 
                <DomainResponses> 
                    <DomainResponse> 
                        <ErrorCode>NoError</ErrorCode> 
                        <ErrorMessage>No error.</ErrorMessage> 
                        <DomainSettingErrors /> 
                        <DomainSettings> 
                            <DomainSetting i:type="DomainStringSetting"> 
                                <Name>ExternalEwsUrl</Name> 
                                <Value>https://emea.mail.microsoft.com/EWS/Exchange.asmx</Value> 
                            </DomainSetting> 
                        </DomainSettings> 
                        <RedirectTarget i:nil="true" /> 
                    </DomainResponse> 
                </DomainResponses> 
            </Response> 
        </GetDomainSettingsResponseMessage> 
    </s:Body> 
</s:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="c64f2-124">Elementos de resposta</span><span class="sxs-lookup"><span data-stu-id="c64f2-124">Response elements</span></span>

<span data-ttu-id="c64f2-125">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="c64f2-125">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="c64f2-126">GetDomainSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c64f2-126">GetDomainSettingsResponseMessage (SOAP)</span></span>](getdomainsettingsresponsemessage-soap.md)
    
- [<span data-ttu-id="c64f2-127">Resposta SOAP)</span><span class="sxs-lookup"><span data-stu-id="c64f2-127">Response (SOAP)</span></span>](response-soap.md)
    
- [<span data-ttu-id="c64f2-128">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c64f2-128">ErrorCode (SOAP)</span></span>](errorcode-soap.md)
    
- [<span data-ttu-id="c64f2-129">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c64f2-129">ErrorMessage (SOAP)</span></span>](errormessage-soap.md)
    
- [<span data-ttu-id="c64f2-130">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c64f2-130">DomainResponses (SOAP)</span></span>](domainresponses-soap.md)
    
- [<span data-ttu-id="c64f2-131">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c64f2-131">DomainResponse (SOAP)</span></span>](domainresponse-soap.md)
    
- [<span data-ttu-id="c64f2-132">DomainSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c64f2-132">DomainSettingErrors (SOAP)</span></span>](domainsettingerrors-soap.md)
    
- [<span data-ttu-id="c64f2-133">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c64f2-133">DomainSettings (SOAP)</span></span>](domainsettings-soap.md)
    
- [<span data-ttu-id="c64f2-134">DomainSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c64f2-134">DomainSetting (SOAP)</span></span>](domainsetting-soap.md)
    
- [<span data-ttu-id="c64f2-135">Nome (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c64f2-135">Name (SOAP)</span></span>](name-soap.md)
    
- [<span data-ttu-id="c64f2-136">Valor (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c64f2-136">Value (SOAP)</span></span>](value-soap.md)
    
- [<span data-ttu-id="c64f2-137">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c64f2-137">RedirectTarget (SOAP)</span></span>](redirecttarget-soap.md)
    
## <a name="see-also"></a><span data-ttu-id="c64f2-138">Confira também</span><span class="sxs-lookup"><span data-stu-id="c64f2-138">See also</span></span>



[<span data-ttu-id="c64f2-139">Operação de GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c64f2-139">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="c64f2-140">Operação de GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c64f2-140">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

