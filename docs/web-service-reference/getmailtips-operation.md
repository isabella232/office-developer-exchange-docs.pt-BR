---
title: Operação
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMailTips
api_type:
- schema
ms.assetid: 025483ec-a9f3-4735-8a95-d26e30ea7974
description: A operação condicas de email Obtém as informações de dicas de email da caixa de correio especificada.
ms.openlocfilehash: 41a4bb99ee7ae4e416ec8a106968bb7869e60345
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458653"
---
# <a name="getmailtips-operation"></a><span data-ttu-id="a3fe1-103">Operação</span><span class="sxs-lookup"><span data-stu-id="a3fe1-103">GetMailTips operation</span></span>

<span data-ttu-id="a3fe1-104">A operação **condicas** de email Obtém as informações de dicas de email da caixa de correio especificada.</span><span class="sxs-lookup"><span data-stu-id="a3fe1-104">The **GetMailTips** operation gets the mail tips information for the specified mailbox.</span></span> 
  
## <a name="getmailtips-request-example"></a><span data-ttu-id="a3fe1-105">Exemplo de solicitação de getquers</span><span class="sxs-lookup"><span data-stu-id="a3fe1-105">GetMailTips request example</span></span>

### <a name="description"></a><span data-ttu-id="a3fe1-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3fe1-106">Description</span></span>

<span data-ttu-id="a3fe1-107">O cliente cria a solicitação XML e a envia para o servidor.</span><span class="sxs-lookup"><span data-stu-id="a3fe1-107">The client constructs the request XML and sends it to the server.</span></span> <span data-ttu-id="a3fe1-108">A solicitação identifica quem o cliente está enviando como, a caixa de correio para recuperar as dicas de email e quais dicas de email são solicitadas.</span><span class="sxs-lookup"><span data-stu-id="a3fe1-108">The request identifies who the client is sending as, the mailbox to retrieve the mail tips for, and what mail tips are requested.</span></span> <span data-ttu-id="a3fe1-109">Neste exemplo, o cliente solicita que todas as dicas de email sejam retornadas para a caixa de correio selecionada.</span><span class="sxs-lookup"><span data-stu-id="a3fe1-109">In this example, the client requests that all mail tips be returned for the selected mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="a3fe1-110">Código</span><span class="sxs-lookup"><span data-stu-id="a3fe1-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"> 
  <soap:Header> 
    <t:RequestServerVersion Version="Exchange2010" /> 
  </soap:Header> 
  <soap:Body> 
    <GetMailTips xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"> 
      <SendingAs> 
        <t:EmailAddress> user1@contoso.com </t:EmailAddress> 
        <t:RoutingType>SMTP</t:RoutingType> 
      </SendingAs> 
      <Recipients> 
        <t:Mailbox> 
          <t:EmailAddress> user2@contoso.com </t:EmailAddress> 
          <t:RoutingType>SMTP</t:RoutingType> 
        </t:Mailbox> 
      </Recipients> 
      <MailTipsRequested>All</MailTipsRequested> 
    </GetMailTips> 
  </soap:Body> 
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="a3fe1-111">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="a3fe1-111">Request elements</span></span>

<span data-ttu-id="a3fe1-112">Os seguintes elementos estão incluídos na solicitação:</span><span class="sxs-lookup"><span data-stu-id="a3fe1-112">The following elements are included in the request:</span></span>
  
- [<span data-ttu-id="a3fe1-113">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="a3fe1-113">GetMailTips</span></span>](getmailtips.md)
    
- [<span data-ttu-id="a3fe1-114">Envios</span><span class="sxs-lookup"><span data-stu-id="a3fe1-114">SendingAs</span></span>](sendingas.md)
    
- [<span data-ttu-id="a3fe1-115">Destinatários (ArrayOfRecipientsType)</span><span class="sxs-lookup"><span data-stu-id="a3fe1-115">Recipients (ArrayOfRecipientsType)</span></span>](recipients-arrayofrecipientstype.md)
    
- [<span data-ttu-id="a3fe1-116">MailTipsRequested</span><span class="sxs-lookup"><span data-stu-id="a3fe1-116">MailTipsRequested</span></span>](mailtipsrequested.md)
    
## <a name="successful-getmailtips-response-example"></a><span data-ttu-id="a3fe1-117">Exemplo de resposta de getdicas de respostas bem-sucedida</span><span class="sxs-lookup"><span data-stu-id="a3fe1-117">Successful GetMailTips response example</span></span>

### <a name="description"></a><span data-ttu-id="a3fe1-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3fe1-118">Description</span></span>

<span data-ttu-id="a3fe1-119">O exemplo a seguir do corpo SOAP (Simple Object Access Protocol) mostra uma resposta bem-sucedida **à solicitação** getquers.</span><span class="sxs-lookup"><span data-stu-id="a3fe1-119">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **GetMailTips** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a3fe1-120">Código</span><span class="sxs-lookup"><span data-stu-id="a3fe1-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?> 
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"> 
  <s:Header> 
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="0" MajorBuildNumber="536" MinorBuildNumber="0" Version="Exchange2010" 
xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xmlns:xsd="http://www.w3.org/2001/XMLSchema"/> 
  </s:Header> 
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"> 
    <GetMailTipsResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"> 
      <ResponseCode>NoError</ResponseCode> 
      <ResponseMessages> 
        <MailTipsResponseMessageType ResponseClass="Success"> 
        <ResponseCode>NoError</ResponseCode> 
        <m:MailTips xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"> 20 / 29 [MS-OXWMT] — v20100517 Mail Tips Web Service Extensions Copyright © 2010 Microsoft Corporation. Release: Monday, May 17, 2010 
          <t:RecipientAddress xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"> 
          <t:Name/> 
          <t:EmailAddress>user2@contoso.com</t:EmailAddress> 
          <t:RoutingType>SMTP</t:RoutingType> 
          </t:RecipientAddress> 
          <t:PendingMailTips xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/> 
          <t:OutOfOffice xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"> 
            <t:ReplyBody> 
              <t:Message/> 
            </t:ReplyBody> 
          </t:OutOfOffice> 
          <t:MailboxFull xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">false</t:MailboxFull> 
          <t:CustomMailTip xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">Hello World Mailtips</t:CustomMailTip> 
          <t:TotalMemberCount xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">1</t:TotalMemberCount> 
          <t:ExternalMemberCount xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">0</t:ExternalMemberCount> 
          <t:MaxMessageSize xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">10485760</t:MaxMessageSize> 
          <t:DeliveryRestricted xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">false</t:DeliveryRestricted> 
          <t:IsModerated xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">false</t:IsModerated> 
          <t:InvalidRecipient xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">false</t:InvalidRecipient> 
        </m:MailTips> 
        </MailTipsResponseMessageType> 
      </ResponseMessages> 
    </GetMailTipsResponse> 
  </s:Body> 
</s:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="a3fe1-121">Elementos de resposta</span><span class="sxs-lookup"><span data-stu-id="a3fe1-121">Response elements</span></span>

<span data-ttu-id="a3fe1-122">Os seguintes elementos estão incluídos na resposta:</span><span class="sxs-lookup"><span data-stu-id="a3fe1-122">The following elements are included in the response:</span></span>
  
- [<span data-ttu-id="a3fe1-123">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a3fe1-123">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a3fe1-124">Dicas de Email</span><span class="sxs-lookup"><span data-stu-id="a3fe1-124">MailTips</span></span>](mailtips.md)
    
## <a name="see-also"></a><span data-ttu-id="a3fe1-125">Confira também</span><span class="sxs-lookup"><span data-stu-id="a3fe1-125">See also</span></span>



[<span data-ttu-id="a3fe1-126">Operações do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a3fe1-126">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="a3fe1-127">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="a3fe1-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

