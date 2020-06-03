---
title: Operação GetUserOofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserOofSettings
api_type:
- schema
ms.assetid: 153e4440-495b-4972-9811-2fbea740142a
description: A operação GetUserOofSettings Obtém as configurações e mensagens de ausência temporária (OOF) de um usuário de caixa de correio.
ms.openlocfilehash: 622faa622b0ea231a6331ff62631885d4252c1f5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457694"
---
# <a name="getuseroofsettings-operation"></a><span data-ttu-id="821e5-103">Operação GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="821e5-103">GetUserOofSettings operation</span></span>

<span data-ttu-id="821e5-104">A operação **GetUserOofSettings** Obtém as configurações e mensagens de ausência temporária (OOF) de um usuário de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="821e5-104">The **GetUserOofSettings** operation gets a mailbox user's Out of Office (OOF) settings and messages.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="821e5-105">Cabeçalhos SOAP</span><span class="sxs-lookup"><span data-stu-id="821e5-105">SOAP Headers</span></span>

<span data-ttu-id="821e5-106">A operação **GetUserOofSettings** pode usar os cabeçalhos SOAP listados e descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="821e5-106">The **GetUserOofSettings** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="821e5-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="821e5-107">**Header**</span></span>|<span data-ttu-id="821e5-108">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="821e5-108">**Element**</span></span>|<span data-ttu-id="821e5-109">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="821e5-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="821e5-110">Representação</span><span class="sxs-lookup"><span data-stu-id="821e5-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="821e5-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="821e5-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="821e5-112">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="821e5-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="821e5-113">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="821e5-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="821e5-114">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="821e5-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="821e5-115">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="821e5-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="using-the-getuseroofsettings-operation"></a><span data-ttu-id="821e5-116">Usando a operação GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="821e5-116">Using the GetUserOofSettings Operation</span></span>

<span data-ttu-id="821e5-117">A operação **GetUserOofSettings** fornece acesso às configurações de ausência temporária de um usuário.</span><span class="sxs-lookup"><span data-stu-id="821e5-117">The **GetUserOofSettings** operation provides access to a user's OOF settings.</span></span> <span data-ttu-id="821e5-118">Um usuário é identificado pelo endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="821e5-118">A user is identified by the user's email address.</span></span> <span data-ttu-id="821e5-119">Se a mensagem OOF for nula e OOF estiver habilitada, nenhuma mensagem OOF será enviada.</span><span class="sxs-lookup"><span data-stu-id="821e5-119">If the OOF message is null and OOF is enabled, no OOF message is sent.</span></span> 
  
> [!IMPORTANT]
> <span data-ttu-id="821e5-120">Se as mensagens OOF forem definidas por MicrosoftOfficeOutlook, esta operação retornará as mensagens OOF no formato HTML.</span><span class="sxs-lookup"><span data-stu-id="821e5-120">If the OOF messages are set by MicrosoftOfficeOutlook, this operation will return the OOF messages in HTML format.</span></span> 
  
## <a name="getuseroofsettings-request-example"></a><span data-ttu-id="821e5-121">Exemplo de solicitação GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="821e5-121">GetUserOofSettings request example</span></span>

### <a name="description"></a><span data-ttu-id="821e5-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="821e5-122">Description</span></span>

<span data-ttu-id="821e5-123">O exemplo a seguir mostra uma solicitação **GetUserOofSettings** que obtém as informações de OOF de um único usuário.</span><span class="sxs-lookup"><span data-stu-id="821e5-123">The following example shows a **GetUserOofSettings** request that gets a single user's OOF information.</span></span> 
  
### <a name="code"></a><span data-ttu-id="821e5-124">Código</span><span class="sxs-lookup"><span data-stu-id="821e5-124">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns ="https://schemas.microsoft.com/exchange/services/2006/types">
        <Address>User1@example.com</Address>
      </Mailbox>
    </GetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="821e5-125">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="821e5-125">Request elements</span></span>

<span data-ttu-id="821e5-126">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="821e5-126">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="821e5-127">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="821e5-127">GetUserOofSettingsRequest</span></span>](getuseroofsettingsrequest.md)
    
- [<span data-ttu-id="821e5-128">Caixa de correio (disponibilidade)</span><span class="sxs-lookup"><span data-stu-id="821e5-128">Mailbox (Availability)</span></span>](mailbox-availability.md)
    
- [<span data-ttu-id="821e5-129">Endereço (cadeia de caracteres)</span><span class="sxs-lookup"><span data-stu-id="821e5-129">Address (string)</span></span>](address-string.md)
    
## <a name="successful-getuseroofsettings-response-example"></a><span data-ttu-id="821e5-130">Exemplo de resposta GetUserOofSettings bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="821e5-130">Successful GetUserOofSettings response example</span></span>

### <a name="description"></a><span data-ttu-id="821e5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="821e5-131">Description</span></span>

<span data-ttu-id="821e5-132">O exemplo a seguir mostra um estado de ausência temporária com mensagens de ausência temporária.</span><span class="sxs-lookup"><span data-stu-id="821e5-132">The following example shows a disabled OOF state with the OOF messages.</span></span>
  
### <a name="code"></a><span data-ttu-id="821e5-133">Código</span><span class="sxs-lookup"><span data-stu-id="821e5-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetUserOofSettingsResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessage ResponseClass="Success">
        <ResponseCode>NoError</ResponseCode>
      </ResponseMessage>
      <OofSettings xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Disabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2006-11-03T23:00:00</StartTime>
          <EndTime>2006-11-04T23:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office. This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
      </OofSettings>
      <AllowExternalOof>All</AllowExternalOof>
    </GetUserOofSettingsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-getuseroofsettings-response-elements"></a><span data-ttu-id="821e5-134">Elementos de resposta do GetUserOofSettings bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="821e5-134">Successful GetUserOofSettings response elements</span></span>

<span data-ttu-id="821e5-135">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="821e5-135">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="821e5-136">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="821e5-136">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="821e5-137">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="821e5-137">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md)
    
- [<span data-ttu-id="821e5-138">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="821e5-138">ResponseMessage</span></span>](responsemessage.md)
    
- [<span data-ttu-id="821e5-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="821e5-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="821e5-140">OofSettings</span><span class="sxs-lookup"><span data-stu-id="821e5-140">OofSettings</span></span>](oofsettings.md)
    
- [<span data-ttu-id="821e5-141">OofState</span><span class="sxs-lookup"><span data-stu-id="821e5-141">OofState</span></span>](oofstate.md)
    
- [<span data-ttu-id="821e5-142">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="821e5-142">ExternalAudience</span></span>](externalaudience.md)
    
- [<span data-ttu-id="821e5-143">Duração (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="821e5-143">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md)
    
- [<span data-ttu-id="821e5-144">StartTime</span><span class="sxs-lookup"><span data-stu-id="821e5-144">StartTime</span></span>](starttime.md)
    
- [<span data-ttu-id="821e5-145">EndTime</span><span class="sxs-lookup"><span data-stu-id="821e5-145">EndTime</span></span>](endtime.md)
    
- [<span data-ttu-id="821e5-146">InternalReply</span><span class="sxs-lookup"><span data-stu-id="821e5-146">InternalReply</span></span>](internalreply.md)
    
- [<span data-ttu-id="821e5-147">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="821e5-147">ExternalReply</span></span>](externalreply.md)
    
- [<span data-ttu-id="821e5-148">Mensagem</span><span class="sxs-lookup"><span data-stu-id="821e5-148">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="821e5-149">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="821e5-149">AllowExternalOof</span></span>](allowexternaloof.md)
    
## <a name="getuseroofsettings-error-response-example"></a><span data-ttu-id="821e5-150">Exemplo de resposta de erro GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="821e5-150">GetUserOofSettings Error response example</span></span>

### <a name="description"></a><span data-ttu-id="821e5-151">Descrição</span><span class="sxs-lookup"><span data-stu-id="821e5-151">Description</span></span>

<span data-ttu-id="821e5-152">O exemplo a seguir mostra uma resposta de erro causada por uma tentativa de acessar informações de ausência temporária de outro usuário.</span><span class="sxs-lookup"><span data-stu-id="821e5-152">The following example shows an error response caused by an attempt to access another user's OOF information.</span></span>
  
### <a name="code"></a><span data-ttu-id="821e5-153">Código</span><span class="sxs-lookup"><span data-stu-id="821e5-153">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <soap:Fault>
      <faultcode>soap:Client</faultcode>
      <faultstring>Microsoft.Exchange.Data.Storage.AccessDeniedException: User is not mailbox owner. User = S-1-5-21-3642464542-282065186-3871681729-1155, MailboxGuid = S-1-5-21-3642464542-282065186-3871681729-1156 ---> User is not mailbox owner. </faultstring>
      <faultactor>https://CAS01.example.com/EWS/Exchange.asmx</faultactor>
      <detail>
        <ErrorCode xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">-2146233088</ErrorCode>
      </detail>
    </soap:Fault>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="821e5-154">Confira também</span><span class="sxs-lookup"><span data-stu-id="821e5-154">See also</span></span>



- [<span data-ttu-id="821e5-155">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="821e5-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

