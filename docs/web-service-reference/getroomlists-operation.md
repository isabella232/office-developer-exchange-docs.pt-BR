---
title: Operação GetRoomLists
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRoomLists
api_type:
- schema
ms.assetid: 55d451f9-547f-44ac-872e-9cb220ea7b7c
description: A operação GetRoomLists Obtém as listas de salas que estão disponíveis na organização do Exchange.
ms.openlocfilehash: d1393a6a5e99b7e0a7e354d2b7dd035d04356ec2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458275"
---
# <a name="getroomlists-operation"></a><span data-ttu-id="037dc-103">Operação GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="037dc-103">GetRoomLists operation</span></span>

<span data-ttu-id="037dc-104">A operação **GetRoomLists** Obtém as listas de salas que estão disponíveis na organização do Exchange.</span><span class="sxs-lookup"><span data-stu-id="037dc-104">The **GetRoomLists** operation gets the room lists that are available within the Exchange organization.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="037dc-105">Cabeçalhos SOAP</span><span class="sxs-lookup"><span data-stu-id="037dc-105">SOAP Headers</span></span>

<span data-ttu-id="037dc-106">A operação **GetRoomLists** pode usar os cabeçalhos SOAP listados e descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="037dc-106">The **GetRoomLists** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="037dc-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="037dc-107">**Header**</span></span>|<span data-ttu-id="037dc-108">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="037dc-108">**Element**</span></span>|<span data-ttu-id="037dc-109">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="037dc-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="037dc-110">Representação</span><span class="sxs-lookup"><span data-stu-id="037dc-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="037dc-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="037dc-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="037dc-112">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="037dc-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="037dc-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="037dc-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="037dc-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="037dc-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="037dc-115">Identifica a cultura RFC3066 a ser usada para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="037dc-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="037dc-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="037dc-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="037dc-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="037dc-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="037dc-118">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="037dc-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="037dc-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="037dc-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="037dc-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="037dc-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="037dc-121">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="037dc-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getroomlists-request-example"></a><span data-ttu-id="037dc-122">Exemplo de solicitação GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="037dc-122">GetRoomLists request example</span></span>

### <a name="description"></a><span data-ttu-id="037dc-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="037dc-123">Description</span></span>

<span data-ttu-id="037dc-124">Veja a seguir um exemplo de uma solicitação **GetRoomLists** que retorna as listas de salas disponíveis no servidor.</span><span class="sxs-lookup"><span data-stu-id="037dc-124">The following is an example of a **GetRoomLists** request that returns the room lists that are available on the server.</span></span> 
  
### <a name="code"></a><span data-ttu-id="037dc-125">Código</span><span class="sxs-lookup"><span data-stu-id="037dc-125">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
    <m:GetRoomLists />
  </soap:Body>
</soap:Envelope>

```

### <a name="request-elements"></a><span data-ttu-id="037dc-126">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="037dc-126">Request elements</span></span>

<span data-ttu-id="037dc-127">O elemento a seguir é usado na solicitação:</span><span class="sxs-lookup"><span data-stu-id="037dc-127">The following element is used in the request:</span></span>
  
- [<span data-ttu-id="037dc-128">GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="037dc-128">GetRoomLists</span></span>](getroomlists.md)
    
## <a name="successful-getroomlists-response-example"></a><span data-ttu-id="037dc-129">Exemplo de resposta GetRoomLists bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="037dc-129">Successful GetRoomLists response example</span></span>

### <a name="description"></a><span data-ttu-id="037dc-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="037dc-130">Description</span></span>

<span data-ttu-id="037dc-131">Veja a seguir um exemplo de uma resposta a uma solicitação **GetRoomLists** .</span><span class="sxs-lookup"><span data-stu-id="037dc-131">The following is an example of a response to a **GetRoomLists** request.</span></span> <span data-ttu-id="037dc-132">Essa resposta mostra uma lista de salas no servidor.</span><span class="sxs-lookup"><span data-stu-id="037dc-132">This response shows one room list on the server.</span></span> 
  
### <a name="code"></a><span data-ttu-id="037dc-133">Código</span><span class="sxs-lookup"><span data-stu-id="037dc-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="1" MajorBuildNumber="164" MinorBuildNumber="0" Version="Exchange2010_SP1" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRoomListsResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <m:RoomLists xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
        <t:Address xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
          <t:Name>Room List</t:Name>
          <t:EmailAddress>RoomList@contoso.com</t:EmailAddress>
          <t:RoutingType>SMTP</t:RoutingType>
          <t:MailboxType>PublicDL</t:MailboxType>
        </t:Address>
      </m:RoomLists>
    </GetRoomListsResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-getroomlists-response-elements"></a><span data-ttu-id="037dc-134">Elementos de resposta do GetRoomLists bem-sucedidos</span><span class="sxs-lookup"><span data-stu-id="037dc-134">Successful GetRoomLists response elements</span></span>

<span data-ttu-id="037dc-135">Os seguintes elementos são usados na resposta:</span><span class="sxs-lookup"><span data-stu-id="037dc-135">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="037dc-136">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="037dc-136">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="037dc-137">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="037dc-137">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
    
- [<span data-ttu-id="037dc-138">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="037dc-138">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="037dc-139">RoomLists</span><span class="sxs-lookup"><span data-stu-id="037dc-139">RoomLists</span></span>](roomlists.md)
    
- [<span data-ttu-id="037dc-140">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="037dc-140">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="037dc-141">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="037dc-141">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md)
    
- [<span data-ttu-id="037dc-142">MailboxType</span><span class="sxs-lookup"><span data-stu-id="037dc-142">MailboxType</span></span>](mailboxtype.md)
    
### <a name="getroomlists-error-response-example"></a><span data-ttu-id="037dc-143">Exemplo de resposta de erro GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="037dc-143">GetRoomLists Error response example</span></span>

#### <a name="description"></a><span data-ttu-id="037dc-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="037dc-144">Description</span></span>

<span data-ttu-id="037dc-145">O exemplo a seguir mostra a resposta a uma tentativa de obter listas de salas de um servidor que não tenha nenhuma lista de salas definida.</span><span class="sxs-lookup"><span data-stu-id="037dc-145">The following example shows the response to an attempt to get room lists from a server that does not have any room lists defined.</span></span>
  
#### <a name="code"></a><span data-ttu-id="037dc-146">Código</span><span class="sxs-lookup"><span data-stu-id="037dc-146">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="1" MajorBuildNumber="164" MinorBuildNumber="0" Version="Exchange2010_SP1" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRoomListsResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <m:RoomLists xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"/>
    </GetRoomListsResponse>
  </s:Body>
</s:Envelope>

```

#### <a name="getroomlists-error-response-elements"></a><span data-ttu-id="037dc-147">Elementos de resposta de erro GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="037dc-147">GetRoomLists Error response elements</span></span>

<span data-ttu-id="037dc-148">Os seguintes elementos são usados na resposta de erro:</span><span class="sxs-lookup"><span data-stu-id="037dc-148">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="037dc-149">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="037dc-149">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="037dc-150">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="037dc-150">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
    
- [<span data-ttu-id="037dc-151">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="037dc-151">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="037dc-152">RoomLists</span><span class="sxs-lookup"><span data-stu-id="037dc-152">RoomLists</span></span>](roomlists.md)
    
## <a name="see-also"></a><span data-ttu-id="037dc-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="037dc-153">See also</span></span>



[<span data-ttu-id="037dc-154">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="037dc-154">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="037dc-155">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="037dc-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

