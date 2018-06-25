---
title: Operação de GetFederationInformation (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c6666a42-a18f-4e4b-beb6-b25ff62cfcc5
description: A operação GetFederationInformation fornece informações sobre o status de Federação da organização, como o URI a ser usado ao solicitar tokens que são destinadas a esta organização e os outros domínios que a organização tem também de destino federados.
ms.openlocfilehash: bf38b2f2b3db3e38b9b0157d1677efe4fc274e1b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752502"
---
# <a name="getfederationinformation-operation-soap"></a><span data-ttu-id="d3d2c-103">Operação de GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3d2c-103">GetFederationInformation operation (SOAP)</span></span>

<span data-ttu-id="d3d2c-104">A operação **GetFederationInformation** fornece informações sobre o status de Federação da organização, como o destino URI a ser usado ao solicitar tokens que são destinadas a esta organização e os outros domínios que a organização também tem federados.</span><span class="sxs-lookup"><span data-stu-id="d3d2c-104">The **GetFederationInformation** operation provides information about the federation status of the organization, such as the target URI to be used when requesting tokens that are targeted at this organization, and the other domains that the organization has also federated.</span></span> 
  
<span data-ttu-id="d3d2c-105">Somente as organizações federadas podem compartilhar o calendário, contatos e mensagens para usuários externos.</span><span class="sxs-lookup"><span data-stu-id="d3d2c-105">Only federated organizations can share calendar, contacts, and messages to external users.</span></span>
  
## <a name="getfederationinformation-request-example"></a><span data-ttu-id="d3d2c-106">Exemplo de solicitação de GetFederationInformation</span><span class="sxs-lookup"><span data-stu-id="d3d2c-106">GetFederationInformation request example</span></span>

### <a name="description"></a><span data-ttu-id="d3d2c-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3d2c-107">Description</span></span>

<span data-ttu-id="d3d2c-108">O exemplo a seguir de uma solicitação de **GetFederationInformation** mostra uma solicitação de informações de federação de um usuário.</span><span class="sxs-lookup"><span data-stu-id="d3d2c-108">The following example of a **GetFederationInformation** request shows a request for a user's federation information.</span></span> <span data-ttu-id="d3d2c-109">O cliente envia essa solicitação ao servidor.</span><span class="sxs-lookup"><span data-stu-id="d3d2c-109">The client sends this request to the server.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d3d2c-110">Código</span><span class="sxs-lookup"><span data-stu-id="d3d2c-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?> 
<soap:Envelope xmlns:exm="http://schemas.microsoft.com/exchange/services/2006/messages"
           xmlns:ext="http://schemas.microsoft.com/exchange/services/2006/types"
           xmlns:a="http://www.w3.org/2005/08/addressing"
           xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema"> 
    <soap:Header> 
        <a:MessageID>urn:uuid:6389558d-9e05-465e-ade9-aae14c4bcd10</a:MessageID> 
        <a:Action soap:mustUnderstand="1">http://schemas.microsoft.com/
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
            xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Request> 
                <Domain>contoso.com</Domain> 
            </Request> 
        </GetFederationInformationRequestMessage>
    </soap:Body> 
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="d3d2c-111">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3d2c-111">Request elements</span></span>

<span data-ttu-id="d3d2c-112">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="d3d2c-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="d3d2c-113">GetFederationInformationRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3d2c-113">GetFederationInformationRequestMessage (SOAP)</span></span>](getfederationinformationrequestmessage-soap.md)
    
- [<span data-ttu-id="d3d2c-114">Solicitação (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3d2c-114">Request (SOAP)</span></span>](request-soap.md)
    
- [<span data-ttu-id="d3d2c-115">Domínio (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3d2c-115">Domain (SOAP)</span></span>](domain-soap.md)
    
## <a name="getfederationinformation-response-example"></a><span data-ttu-id="d3d2c-116">Exemplo de resposta GetFederationInformation</span><span class="sxs-lookup"><span data-stu-id="d3d2c-116">GetFederationInformation response example</span></span>

### <a name="description"></a><span data-ttu-id="d3d2c-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3d2c-117">Description</span></span>

<span data-ttu-id="d3d2c-118">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação de **GetFederationInformation** que o servidor envia para o cliente.</span><span class="sxs-lookup"><span data-stu-id="d3d2c-118">The following example shows a successful response to the **GetFederationInformation** request that the server sends to the client.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d3d2c-119">Código</span><span class="sxs-lookup"><span data-stu-id="d3d2c-119">Code</span></span>

```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
xmlns:a="http://www.w3.org/2005/08/addressing"> 
    <s:Header> 
        <a:Action s:mustUnderstand="1">
            http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetFederationInformationResponse
        </a:Action> 
        <a:RelatesTo>urn:uuid:6389558d-9e05-465e-ade9-aae14c4bcd10</a:RelatesTo> 
    </s:Header> 
    <s:Body> 
        <GetFederationInformationResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover"> 
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

### <a name="response-elements"></a><span data-ttu-id="d3d2c-120">Elementos de resposta</span><span class="sxs-lookup"><span data-stu-id="d3d2c-120">Response elements</span></span>

<span data-ttu-id="d3d2c-121">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="d3d2c-121">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="d3d2c-122">GetFederationInformationResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3d2c-122">GetFederationInformationResponseMessage (SOAP)</span></span>](getfederationinformationresponsemessage-soap.md)
    
- [<span data-ttu-id="d3d2c-123">Resposta SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3d2c-123">Response (SOAP)</span></span>](response-soap.md)
    
- [<span data-ttu-id="d3d2c-124">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3d2c-124">ErrorCode (SOAP)</span></span>](errorcode-soap.md)
    
- [<span data-ttu-id="d3d2c-125">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3d2c-125">ErrorMessage (SOAP)</span></span>](errormessage-soap.md)
    
- [<span data-ttu-id="d3d2c-126">ApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3d2c-126">ApplicationUri (SOAP)</span></span>](applicationuri-soap.md)
    
- [<span data-ttu-id="d3d2c-127">Domínios (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3d2c-127">Domains (SOAP)</span></span>](domains-soap.md)
    
- [<span data-ttu-id="d3d2c-128">Domínio (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3d2c-128">Domain (SOAP)</span></span>](domain-soap.md)
    
## <a name="see-also"></a><span data-ttu-id="d3d2c-129">Confira também</span><span class="sxs-lookup"><span data-stu-id="d3d2c-129">See also</span></span>

- [<span data-ttu-id="d3d2c-130">Operação de GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3d2c-130">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="d3d2c-131">Operação de GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3d2c-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

