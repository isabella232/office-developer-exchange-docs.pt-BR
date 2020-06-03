---
title: Operação GetFederationInformation (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c6666a42-a18f-4e4b-beb6-b25ff62cfcc5
description: A operação GetFederationInformation fornece informações sobre o status de Federação da organização, como o URI de destino a ser usado ao solicitar tokens direcionados a essa organização e os outros domínios que a organização também tenha federado.
ms.openlocfilehash: 533b2f6d282e3287f4945df56b169f5bc93ff445
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455622"
---
# <a name="getfederationinformation-operation-soap"></a><span data-ttu-id="fcb5b-103">Operação GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fcb5b-103">GetFederationInformation operation (SOAP)</span></span>

<span data-ttu-id="fcb5b-104">A operação **GetFederationInformation** fornece informações sobre o status de Federação da organização, como o URI de destino a ser usado ao solicitar tokens direcionados a essa organização e os outros domínios que a organização também tenha federado.</span><span class="sxs-lookup"><span data-stu-id="fcb5b-104">The **GetFederationInformation** operation provides information about the federation status of the organization, such as the target URI to be used when requesting tokens that are targeted at this organization, and the other domains that the organization has also federated.</span></span> 
  
<span data-ttu-id="fcb5b-105">Somente organizações federadas podem compartilhar calendário, contatos e mensagens para usuários externos.</span><span class="sxs-lookup"><span data-stu-id="fcb5b-105">Only federated organizations can share calendar, contacts, and messages to external users.</span></span>
  
## <a name="getfederationinformation-request-example"></a><span data-ttu-id="fcb5b-106">Exemplo de solicitação GetFederationInformation</span><span class="sxs-lookup"><span data-stu-id="fcb5b-106">GetFederationInformation request example</span></span>

### <a name="description"></a><span data-ttu-id="fcb5b-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcb5b-107">Description</span></span>

<span data-ttu-id="fcb5b-108">O exemplo a seguir de uma solicitação **GetFederationInformation** mostra uma solicitação para as informações de Federação de um usuário.</span><span class="sxs-lookup"><span data-stu-id="fcb5b-108">The following example of a **GetFederationInformation** request shows a request for a user's federation information.</span></span> <span data-ttu-id="fcb5b-109">O cliente envia essa solicitação para o servidor.</span><span class="sxs-lookup"><span data-stu-id="fcb5b-109">The client sends this request to the server.</span></span> 
  
### <a name="code"></a><span data-ttu-id="fcb5b-110">Código</span><span class="sxs-lookup"><span data-stu-id="fcb5b-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?> 
<soap:Envelope xmlns:exm="https://schemas.microsoft.com/exchange/services/2006/messages"
           xmlns:ext="https://schemas.microsoft.com/exchange/services/2006/types"
           xmlns:a="http://www.w3.org/2005/08/addressing"
           xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema"> 
    <soap:Header> 
        <a:MessageID>urn:uuid:6389558d-9e05-465e-ade9-aae14c4bcd10</a:MessageID> 
        <a:Action soap:mustUnderstand="1">https://schemas.microsoft.com/
            exchange/2010/Autodiscover/Autodiscover/GetFederationInformation
        </a:Action> 
        <a:To soap:mustUnderstand="1">https://autodiscover.byfcxu-
            dom.extest.microsoft.com/autodiscover/autodiscover.svc</a:To> 
        <a:ReplyTo>
            <a:Address>http://www.w3.org/2005/08/addressing/anonymous</a:Address> 
        </a:ReplyTo> 
    </soap:Header> 
    <soap:Body> 
        <GetFederationInformationRequestMessage 
            xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Request> 
                <Domain>contoso.com</Domain> 
            </Request> 
        </GetFederationInformationRequestMessage>
    </soap:Body> 
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="fcb5b-111">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="fcb5b-111">Request elements</span></span>

<span data-ttu-id="fcb5b-112">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="fcb5b-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="fcb5b-113">GetFederationInformationRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fcb5b-113">GetFederationInformationRequestMessage (SOAP)</span></span>](getfederationinformationrequestmessage-soap.md)
    
- [<span data-ttu-id="fcb5b-114">Solicitação (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fcb5b-114">Request (SOAP)</span></span>](request-soap.md)
    
- [<span data-ttu-id="fcb5b-115">Domínio (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fcb5b-115">Domain (SOAP)</span></span>](domain-soap.md)
    
## <a name="getfederationinformation-response-example"></a><span data-ttu-id="fcb5b-116">Exemplo de resposta GetFederationInformation</span><span class="sxs-lookup"><span data-stu-id="fcb5b-116">GetFederationInformation response example</span></span>

### <a name="description"></a><span data-ttu-id="fcb5b-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="fcb5b-117">Description</span></span>

<span data-ttu-id="fcb5b-118">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação **GetFederationInformation** que o servidor envia para o cliente.</span><span class="sxs-lookup"><span data-stu-id="fcb5b-118">The following example shows a successful response to the **GetFederationInformation** request that the server sends to the client.</span></span> 
  
### <a name="code"></a><span data-ttu-id="fcb5b-119">Código</span><span class="sxs-lookup"><span data-stu-id="fcb5b-119">Code</span></span>

```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
xmlns:a="http://www.w3.org/2005/08/addressing"> 
    <s:Header> 
        <a:Action s:mustUnderstand="1">
            https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetFederationInformationResponse
        </a:Action> 
        <a:RelatesTo>urn:uuid:6389558d-9e05-465e-ade9-aae14c4bcd10</a:RelatesTo> 
    </s:Header> 
    <s:Body> 
        <GetFederationInformationResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance"> 
                <ErrorCode>NoError</ErrorCode> 
                <ErrorMessage/> 
                <ApplicationUri>BYFCXU-DOM.EXTEST.MICROSOFT.COM</ApplicationUri> 
                <Domains> 
                    <Domain>contoso.com</Domain> 
                    <Domain>europe.contoso.com</Domain> 
                    <Domain>americas.contoso.com</Domain> 
                    <Domain>contosolive.com</Domain> 
                </Domains> 
            </Response> 
        </GetFederationInformationResponseMessage> 
    </s:Body> 
</s:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="fcb5b-120">Elementos de resposta</span><span class="sxs-lookup"><span data-stu-id="fcb5b-120">Response elements</span></span>

<span data-ttu-id="fcb5b-121">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="fcb5b-121">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="fcb5b-122">GetFederationInformationResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fcb5b-122">GetFederationInformationResponseMessage (SOAP)</span></span>](getfederationinformationresponsemessage-soap.md)
    
- [<span data-ttu-id="fcb5b-123">Resposta (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fcb5b-123">Response (SOAP)</span></span>](response-soap.md)
    
- [<span data-ttu-id="fcb5b-124">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fcb5b-124">ErrorCode (SOAP)</span></span>](errorcode-soap.md)
    
- [<span data-ttu-id="fcb5b-125">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fcb5b-125">ErrorMessage (SOAP)</span></span>](errormessage-soap.md)
    
- [<span data-ttu-id="fcb5b-126">ApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fcb5b-126">ApplicationUri (SOAP)</span></span>](applicationuri-soap.md)
    
- [<span data-ttu-id="fcb5b-127">Domínios (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fcb5b-127">Domains (SOAP)</span></span>](domains-soap.md)
    
- [<span data-ttu-id="fcb5b-128">Domínio (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fcb5b-128">Domain (SOAP)</span></span>](domain-soap.md)
    
## <a name="see-also"></a><span data-ttu-id="fcb5b-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="fcb5b-129">See also</span></span>

- [<span data-ttu-id="fcb5b-130">Operação GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fcb5b-130">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="fcb5b-131">Operação GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fcb5b-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

