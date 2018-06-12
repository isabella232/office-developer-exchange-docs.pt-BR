---
title: Operação RemoveDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveDelegate
api_type:
- schema
ms.assetid: 1d42d5ff-8fde-4f8a-b18d-57b1ef7a946a
description: A operação RemoveDelegate remove um ou mais representantes da caixa de correio de um usuário.
ms.openlocfilehash: 6f3371d19bd8a7fd967d4959d85037ae6b51f6aa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19825088"
---
# <a name="removedelegate-operation"></a><span data-ttu-id="4318a-103">Operação RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="4318a-103">RemoveDelegate operation</span></span>

<span data-ttu-id="4318a-104">A operação **RemoveDelegate** remove um ou mais representantes da caixa de correio de um usuário.</span><span class="sxs-lookup"><span data-stu-id="4318a-104">The **RemoveDelegate** operation removes one or more delegates from a user's mailbox.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="4318a-105">Cabeçalhos SOAP</span><span class="sxs-lookup"><span data-stu-id="4318a-105">SOAP Headers</span></span>

<span data-ttu-id="4318a-106">A operação **RemoveDelegate** pode usar os cabeçalhos SOAP que estão listados e descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="4318a-106">The **RemoveDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="4318a-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="4318a-107">**Header**</span></span>|<span data-ttu-id="4318a-108">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4318a-108">**Element**</span></span>|<span data-ttu-id="4318a-109">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4318a-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4318a-110">Representação</span><span class="sxs-lookup"><span data-stu-id="4318a-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="4318a-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="4318a-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="4318a-112">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="4318a-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="4318a-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="4318a-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="4318a-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="4318a-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="4318a-115">Identifica a cultura RFC3066 a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4318a-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="4318a-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="4318a-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="4318a-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="4318a-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="4318a-118">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="4318a-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="4318a-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="4318a-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="4318a-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4318a-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="4318a-121">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="4318a-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="removedelegate-request-example"></a><span data-ttu-id="4318a-122">Exemplo de solicitação de RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="4318a-122">RemoveDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="4318a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4318a-123">Description</span></span>

<span data-ttu-id="4318a-124">O exemplo de código a seguir mostra como remover dois delegados de caixa de correio do user1.</span><span class="sxs-lookup"><span data-stu-id="4318a-124">The following code example shows how to remove two delegates from user1's mailbox.</span></span> <span data-ttu-id="4318a-125">Neste exemplo, um delegado é removido usando o endereço de SMTP primário do representante, e outro é removido usando o identificador de segurança (SID) do representante.</span><span class="sxs-lookup"><span data-stu-id="4318a-125">In this example, one delegate is removed by using the delegate's primary SMTP address, and the other one is removed by using the delegate's security identifier (SID).</span></span>
  
### <a name="code"></a><span data-ttu-id="4318a-126">Código</span><span class="sxs-lookup"><span data-stu-id="4318a-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body>
    <RemoveDelegate xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
        <t:EmailAddress>user1@example.com</t:EmailAddress>
      </Mailbox>
      <UserIds>
        <t:UserId>
          <t:PrimarySmtpAddress>user2@example.com</t:PrimarySmtpAddress>
        </t:UserId>
        <t:UserId>
          <t:SID>S-1-5-21-1333220396-2200287332-232816053-1118</t:SID>
        </t:UserId>
      </UserIds>
    </RemoveDelegate>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="4318a-127">Comments</span><span class="sxs-lookup"><span data-stu-id="4318a-127">Comments</span></span>

<span data-ttu-id="4318a-128">A operação **RemoveDelegate** requer que o usuário delegado especificado para ter uma caixa de correio ou existir no serviço de diretório do Active Directory.</span><span class="sxs-lookup"><span data-stu-id="4318a-128">The **RemoveDelegate** operation does not require the specified delegate user to have a mailbox or to exist in the Active Directory directory service.</span></span> <span data-ttu-id="4318a-129">A operação **RemoveDelegate** terá êxito se a entrada de representante for órfão.</span><span class="sxs-lookup"><span data-stu-id="4318a-129">The **RemoveDelegate** operation will succeed if the delegate entry is orphaned.</span></span> 
  
## <a name="removedelegate-response-example"></a><span data-ttu-id="4318a-130">Exemplo de resposta RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="4318a-130">RemoveDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="4318a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="4318a-131">Description</span></span>

<span data-ttu-id="4318a-132">O exemplo a seguir de uma resposta **RemoveDelegate** mostra uma resposta bem-sucedida a uma solicitação **RemoveDelegate** .</span><span class="sxs-lookup"><span data-stu-id="4318a-132">The following example of a **RemoveDelegate** response shows a successful response to a **RemoveDelegate** request.</span></span> <span data-ttu-id="4318a-133">A resposta conterá um elemento **DelegateUserResponseMessageType** para cada delegado que é removido da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4318a-133">The response contains a **DelegateUserResponseMessageType** element for each delegate that is removed from the mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="4318a-134">Código</span><span class="sxs-lookup"><span data-stu-id="4318a-134">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" 
                         MinorVersion="1" 
                         MajorBuildNumber="206" 
                         MinorBuildNumber="0" 
                         Version="Exchange2007_SP1" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:RemoveDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              ResponseClass="Success" 
                              xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DelegateUserResponseMessageType>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
      </m:RemoveDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="removedelegate-error-response-example"></a><span data-ttu-id="4318a-135">Exemplo de resposta de erro RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="4318a-135">RemoveDelegate Error response example</span></span>

### <a name="description"></a><span data-ttu-id="4318a-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="4318a-136">Description</span></span>

<span data-ttu-id="4318a-137">O exemplo a seguir de uma resposta de erro **RemoveDelegate** mostra os resultados de uma solicitação para remover um representante que não existe.</span><span class="sxs-lookup"><span data-stu-id="4318a-137">The following example of a **RemoveDelegate** error response shows the results of a request to remove a delegate that does not exist.</span></span> 
  
### <a name="code"></a><span data-ttu-id="4318a-138">Código</span><span class="sxs-lookup"><span data-stu-id="4318a-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8"
                         MinorVersion="1"
                         MajorBuildNumber="206"
                         MinorBuildNumber="0"
                         Version="Exchange2007_SP1"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:RemoveDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                              ResponseClass="Success"
                              xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Error">
          <m:MessageText>The user is not a delegate for the mailbox.</m:MessageText>
          <m:ResponseCode>ErrorNotDelegate</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
    </m:RemoveDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="4318a-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="4318a-139">See also</span></span>



- [<span data-ttu-id="4318a-140">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4318a-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

