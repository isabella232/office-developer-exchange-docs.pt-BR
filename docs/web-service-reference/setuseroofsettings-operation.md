---
title: Operação SetUserOofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetUserOofSettings
api_type:
- schema
ms.assetid: 36277ef0-18ee-4b35-9e6e-8c321d8f5433
description: O método Web SetUserOofSettings define as configurações e mensagens de ausência temporária (OOF) de um usuário de caixa de correio.
ms.openlocfilehash: 88b5475dd2f0fe6d334bad51a0fe8d0beb767634
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463150"
---
# <a name="setuseroofsettings-operation"></a><span data-ttu-id="d6833-103">Operação SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="d6833-103">SetUserOofSettings operation</span></span>

<span data-ttu-id="d6833-104">O método Web **SetUserOofSettings** define as configurações e mensagens de ausência temporária (OOF) de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="d6833-104">The **SetUserOofSettings** Web method sets a mailbox user's Out of Office (OOF) settings and message.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="d6833-105">Cabeçalhos SOAP</span><span class="sxs-lookup"><span data-stu-id="d6833-105">SOAP Headers</span></span>

<span data-ttu-id="d6833-106">A operação **SetUserOofSettings** pode usar os cabeçalhos SOAP listados e descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="d6833-106">The **SetUserOofSettings** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="d6833-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="d6833-107">**Header**</span></span>|<span data-ttu-id="d6833-108">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="d6833-108">**Element**</span></span>|<span data-ttu-id="d6833-109">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="d6833-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d6833-110">Representação</span><span class="sxs-lookup"><span data-stu-id="d6833-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="d6833-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="d6833-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="d6833-112">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="d6833-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="d6833-113">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="d6833-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="d6833-114">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d6833-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="d6833-115">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="d6833-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="setuseroofsettings-request-example"></a><span data-ttu-id="d6833-116">Exemplo de solicitação SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="d6833-116">SetUserOofSettings request example</span></span>

### <a name="description"></a><span data-ttu-id="d6833-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6833-117">Description</span></span>

<span data-ttu-id="d6833-118">O exemplo a seguir de uma solicitação **SetUserOofSettings** define uma configuração de ausência temporária por 10 dias.</span><span class="sxs-lookup"><span data-stu-id="d6833-118">The following example of a **SetUserOofSettings** request sets an OOF setting for 10 days.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d6833-119">Código</span><span class="sxs-lookup"><span data-stu-id="d6833-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <Name>User1</Name>
        <Address>user1@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Enabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2006-10-05T00:00:00</StartTime>
          <EndTime>2006-10-25T00:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office.  This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
      </UserOofSettings>
    </SetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="d6833-120">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="d6833-120">Request elements</span></span>

<span data-ttu-id="d6833-121">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="d6833-121">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="d6833-122">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="d6833-122">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md)
    
- [<span data-ttu-id="d6833-123">Caixa de correio (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="d6833-123">Mailbox (Availability)</span></span>](mailbox-availability.md)
    
- [<span data-ttu-id="d6833-124">Nome (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="d6833-124">Name (EmailAddress)</span></span>](name-emailaddress.md)
    
- [<span data-ttu-id="d6833-125">Endereço (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="d6833-125">Address (string)</span></span>](address-string.md)
    
- [<span data-ttu-id="d6833-126">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="d6833-126">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md)
    
- [<span data-ttu-id="d6833-127">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="d6833-127">UserOofSettings</span></span>](useroofsettings.md)
    
- [<span data-ttu-id="d6833-128">OofState</span><span class="sxs-lookup"><span data-stu-id="d6833-128">OofState</span></span>](oofstate.md)
    
- [<span data-ttu-id="d6833-129">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="d6833-129">ExternalAudience</span></span>](externalaudience.md)
    
- [<span data-ttu-id="d6833-130">Duração (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="d6833-130">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md)
    
- [<span data-ttu-id="d6833-131">StartTime</span><span class="sxs-lookup"><span data-stu-id="d6833-131">StartTime</span></span>](starttime.md)
    
- [<span data-ttu-id="d6833-132">EndTime</span><span class="sxs-lookup"><span data-stu-id="d6833-132">EndTime</span></span>](endtime.md)
    
- [<span data-ttu-id="d6833-133">InternalReply</span><span class="sxs-lookup"><span data-stu-id="d6833-133">InternalReply</span></span>](internalreply.md)
    
- [<span data-ttu-id="d6833-134">Mensagem (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="d6833-134">Message (Availability)</span></span>](message-availability.md)
    
- [<span data-ttu-id="d6833-135">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="d6833-135">ExternalReply</span></span>](externalreply.md)
    
## <a name="successful-setuseroofsettings-response-example"></a><span data-ttu-id="d6833-136">Exemplo de resposta SetUserOofSettings bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="d6833-136">Successful SetUserOofSettings response example</span></span>

### <a name="description"></a><span data-ttu-id="d6833-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="d6833-137">Description</span></span>

<span data-ttu-id="d6833-138">O exemplo a seguir mostra uma resposta bem-sucedida à solicitação **SetUserOofSettings** .</span><span class="sxs-lookup"><span data-stu-id="d6833-138">The following example shows a successful response to the **SetUserOofSettings** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d6833-139">Código</span><span class="sxs-lookup"><span data-stu-id="d6833-139">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" /> 
  </soap:Header>
  <soap:Body>
    <SetUserOofSettingsResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessage ResponseClass="Success">
        <ResponseCode>NoError</ResponseCode> 
      </ResponseMessage>
    </SetUserOofSettingsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="d6833-140">Elementos de resposta bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="d6833-140">Successful response elements</span></span>

<span data-ttu-id="d6833-141">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="d6833-141">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="d6833-142">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d6833-142">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="d6833-143">SetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="d6833-143">SetUserOofSettingsResponse</span></span>](setuseroofsettingsresponse.md)
    
- [<span data-ttu-id="d6833-144">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d6833-144">ResponseMessage</span></span>](responsemessage.md)
    
- [<span data-ttu-id="d6833-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d6833-145">ResponseCode</span></span>](responsecode.md)
    
## <a name="see-also"></a><span data-ttu-id="d6833-146">Também consulte</span><span class="sxs-lookup"><span data-stu-id="d6833-146">See also</span></span>



- [<span data-ttu-id="d6833-147">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="d6833-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

