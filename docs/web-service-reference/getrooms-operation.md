---
title: Operação GetRooms
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRooms
api_type:
- schema
ms.assetid: 5501ddc0-3bfa-4da6-8e15-4223ca5499a3
description: A operação GetRooms obtém as salas dentro da lista de sala especificado.
ms.openlocfilehash: 3718c476881ae8aa538646464e7c61845d849562
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752618"
---
# <a name="getrooms-operation"></a><span data-ttu-id="c689a-103">Operação GetRooms</span><span class="sxs-lookup"><span data-stu-id="c689a-103">GetRooms operation</span></span>

<span data-ttu-id="c689a-104">A operação **GetRooms** obtém as salas dentro da lista de sala especificado.</span><span class="sxs-lookup"><span data-stu-id="c689a-104">The **GetRooms** operation gets the rooms within the specified room list.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="c689a-105">Cabeçalhos SOAP</span><span class="sxs-lookup"><span data-stu-id="c689a-105">SOAP Headers</span></span>

<span data-ttu-id="c689a-106">A operação **GetRooms** pode usar os cabeçalhos SOAP que estão listados e descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="c689a-106">The **GetRooms** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="c689a-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="c689a-107">**Header**</span></span>|<span data-ttu-id="c689a-108">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="c689a-108">**Element**</span></span>|<span data-ttu-id="c689a-109">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="c689a-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c689a-110">Representação</span><span class="sxs-lookup"><span data-stu-id="c689a-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="c689a-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="c689a-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="c689a-112">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="c689a-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="c689a-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="c689a-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="c689a-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="c689a-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="c689a-115">Identifica a cultura RFC3066 a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="c689a-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="c689a-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="c689a-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="c689a-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="c689a-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="c689a-118">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="c689a-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="c689a-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="c689a-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="c689a-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c689a-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="c689a-121">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="c689a-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getrooms-request-example"></a><span data-ttu-id="c689a-122">Exemplo de solicitação de GetRooms</span><span class="sxs-lookup"><span data-stu-id="c689a-122">GetRooms request example</span></span>

### <a name="description"></a><span data-ttu-id="c689a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="c689a-123">Description</span></span>

<span data-ttu-id="c689a-124">O exemplo a seguir é um exemplo de uma solicitação de **GetRooms** que obtém as salas que estão associadas uma lista de salas.</span><span class="sxs-lookup"><span data-stu-id="c689a-124">The following is an example of a **GetRooms** request that gets the rooms that are associated with a room list.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c689a-125">Código</span><span class="sxs-lookup"><span data-stu-id="c689a-125">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
    <m:GetRooms>
      <m:RoomList>
        <t:EmailAddress>RoomList@contoso.com</t:EmailAddress>
      </m:RoomList>
    </m:GetRooms>
  </soap:Body>

```

### <a name="request-elements"></a><span data-ttu-id="c689a-126">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c689a-126">Request elements</span></span>

<span data-ttu-id="c689a-127">Os seguintes elementos são usados na solicitação:</span><span class="sxs-lookup"><span data-stu-id="c689a-127">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="c689a-128">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="c689a-128">RequestServerVersion</span></span>](requestserverversion.md)
    
- [<span data-ttu-id="c689a-129">GetRooms</span><span class="sxs-lookup"><span data-stu-id="c689a-129">GetRooms</span></span>](getrooms.md)
    
- [<span data-ttu-id="c689a-130">RoomList</span><span class="sxs-lookup"><span data-stu-id="c689a-130">RoomList</span></span>](roomlist.md)
    
- [<span data-ttu-id="c689a-131">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="c689a-131">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
## <a name="successful-getrooms-response-example"></a><span data-ttu-id="c689a-132">Exemplo de resposta bem-sucedida GetRooms</span><span class="sxs-lookup"><span data-stu-id="c689a-132">Successful GetRooms response example</span></span>

### <a name="description"></a><span data-ttu-id="c689a-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="c689a-133">Description</span></span>

<span data-ttu-id="c689a-134">A resposta a seguir mostra as informações de endereço de email para as salas que estão associados a lista de salas.</span><span class="sxs-lookup"><span data-stu-id="c689a-134">The following response shows the email address information for the rooms that are associated with the room list.</span></span>
  
### <a name="code"></a><span data-ttu-id="c689a-135">Código</span><span class="sxs-lookup"><span data-stu-id="c689a-135">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="1" MajorBuildNumber="164" MinorBuildNumber="0" Version="Exchange2010_SP1" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRoomsResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <m:Rooms xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
        <t:Room xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
          <t:Id>
            <t:Name>Room01</t:Name>
            <t:EmailAddress>Room01@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
        <t:Room xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
          <t:Id>
            <t:Name>Room02</t:Name>
            <t:EmailAddress>Room02@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
      </m:Rooms>
    </GetRoomsResponse>
  </s:Body>
</s:Envelope>
```

### <a name="successful-getrooms-response-elements"></a><span data-ttu-id="c689a-136">Elementos de resposta bem-sucedida GetRooms</span><span class="sxs-lookup"><span data-stu-id="c689a-136">Successful GetRooms response elements</span></span>

<span data-ttu-id="c689a-137">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="c689a-137">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="c689a-138">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c689a-138">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="c689a-139">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="c689a-139">GetRoomsResponse</span></span>](getroomsresponse.md)
    
- [<span data-ttu-id="c689a-140">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c689a-140">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c689a-141">Salas</span><span class="sxs-lookup"><span data-stu-id="c689a-141">Rooms</span></span>](rooms.md)
    
- [<span data-ttu-id="c689a-142">Sala</span><span class="sxs-lookup"><span data-stu-id="c689a-142">Room</span></span>](room.md)
    
- [<span data-ttu-id="c689a-143">Nome (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="c689a-143">Name (EmailAddress)</span></span>](name-emailaddress.md)
    
- [<span data-ttu-id="c689a-144">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="c689a-144">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="c689a-145">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="c689a-145">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md)
    
- [<span data-ttu-id="c689a-146">MailboxType</span><span class="sxs-lookup"><span data-stu-id="c689a-146">MailboxType</span></span>](mailboxtype.md)
    
## <a name="getrooms-error-response-example"></a><span data-ttu-id="c689a-147">Exemplo de resposta de erro GetRooms</span><span class="sxs-lookup"><span data-stu-id="c689a-147">GetRooms Error response example</span></span>

### <a name="description"></a><span data-ttu-id="c689a-148">Descrição</span><span class="sxs-lookup"><span data-stu-id="c689a-148">Description</span></span>

<span data-ttu-id="c689a-149">O exemplo a seguir mostra uma resposta de erro causada por uma tentativa de obter informações de sala para uma lista de salas inexistente.</span><span class="sxs-lookup"><span data-stu-id="c689a-149">The following example shows an error response caused by an attempt to get room information for a nonexistent room list.</span></span>
  
### <a name="code"></a><span data-ttu-id="c689a-150">Código</span><span class="sxs-lookup"><span data-stu-id="c689a-150">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="1" MajorBuildNumber="164" MinorBuildNumber="0" Version="Exchange2010_SP1" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRoomsResponse ResponseClass="Error" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>No results were found.</MessageText>
      <ResponseCode>ErrorNameResolutionNoResults</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetRoomsResponse>
  </s:Body>
</s:Envelope>
```

### <a name="getrooms-error-response-elements"></a><span data-ttu-id="c689a-151">Elementos de resposta de erro GetRooms</span><span class="sxs-lookup"><span data-stu-id="c689a-151">GetRooms Error response elements</span></span>

<span data-ttu-id="c689a-152">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="c689a-152">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="c689a-153">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c689a-153">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="c689a-154">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="c689a-154">GetRoomsResponse</span></span>](getroomsresponse.md)
    
- [<span data-ttu-id="c689a-155">MessageText</span><span class="sxs-lookup"><span data-stu-id="c689a-155">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="c689a-156">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c689a-156">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c689a-157">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c689a-157">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="c689a-158">Confira também</span><span class="sxs-lookup"><span data-stu-id="c689a-158">See also</span></span>

- [<span data-ttu-id="c689a-159">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c689a-159">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
- [<span data-ttu-id="c689a-160">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="c689a-160">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

