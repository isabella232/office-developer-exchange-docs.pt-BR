---
title: Operação GetDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetDelegate
api_type:
- schema
ms.assetid: 849b2c9e-4685-4bd1-9adb-aba0fcc52650
description: A operação GetDelegate recupera as configurações de representante para uma caixa de correio especificada.
ms.openlocfilehash: bd1a0add54ee5fd1c23b4ba09a921a9061afa394
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19752452"
---
# <a name="getdelegate-operation"></a><span data-ttu-id="fe3fa-103">Operação GetDelegate</span><span class="sxs-lookup"><span data-stu-id="fe3fa-103">GetDelegate operation</span></span>

<span data-ttu-id="fe3fa-104">A operação **GetDelegate** recupera as configurações de representante para uma caixa de correio especificada.</span><span class="sxs-lookup"><span data-stu-id="fe3fa-104">The **GetDelegate** operation retrieves the delegate settings for a specified mailbox.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="fe3fa-105">Cabeçalhos SOAP</span><span class="sxs-lookup"><span data-stu-id="fe3fa-105">SOAP Headers</span></span>

<span data-ttu-id="fe3fa-106">A operação **GetDelegate** pode usar os cabeçalhos SOAP que estão listados e descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="fe3fa-106">The **GetDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="fe3fa-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="fe3fa-107">**Header**</span></span>|<span data-ttu-id="fe3fa-108">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="fe3fa-108">**Element**</span></span>|<span data-ttu-id="fe3fa-109">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="fe3fa-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="fe3fa-110">Representação</span><span class="sxs-lookup"><span data-stu-id="fe3fa-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="fe3fa-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="fe3fa-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="fe3fa-112">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="fe3fa-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="fe3fa-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="fe3fa-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="fe3fa-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="fe3fa-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="fe3fa-115">Identifica a cultura RFC3066 a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fe3fa-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="fe3fa-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="fe3fa-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="fe3fa-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="fe3fa-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="fe3fa-118">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="fe3fa-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="fe3fa-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="fe3fa-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="fe3fa-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="fe3fa-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="fe3fa-121">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="fe3fa-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getdelegate-request-example"></a><span data-ttu-id="fe3fa-122">Exemplo de solicitação de GetDelegate</span><span class="sxs-lookup"><span data-stu-id="fe3fa-122">GetDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="fe3fa-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe3fa-123">Description</span></span>

<span data-ttu-id="fe3fa-124">O exemplo de código a seguir mostra como recuperar as configurações de representante para todos os representantes são definidos na caixa de correio do user3.</span><span class="sxs-lookup"><span data-stu-id="fe3fa-124">The following code example shows how to retrieve the delegate settings for all the delegates that are set on user3's mailbox.</span></span> <span data-ttu-id="fe3fa-125">Todas as permissões para cada usuário são retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="fe3fa-125">All the permissions for each user are returned in the response.</span></span>
  
### <a name="code"></a><span data-ttu-id="fe3fa-126">Código</span><span class="sxs-lookup"><span data-stu-id="fe3fa-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body>
    <GetDelegate xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                 IncludePermissions="true">
      <Mailbox>
        <t:EmailAddress>user3@example.com</t:EmailAddress>
      </Mailbox>
    </GetDelegate>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="fe3fa-127">Comments</span><span class="sxs-lookup"><span data-stu-id="fe3fa-127">Comments</span></span>

<span data-ttu-id="fe3fa-128">Você pode usar o elemento [UserId](userid.md) para especificar os usuários individuais em vez de retornar todos os usuários que têm permissões de acesso de representante na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="fe3fa-128">You can use the [UserId](userid.md) element to specify individual users instead of returning all users who have delegate access permissions on the mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="fe3fa-129">Serviços Web do Exchange (EWS) não oferece suporte para gerenciar representantes de grupo.</span><span class="sxs-lookup"><span data-stu-id="fe3fa-129">Exchange Web Services (EWS) does not support managing group delegates.</span></span> <span data-ttu-id="fe3fa-130">EWS retornará um erro se a operação **GetDelegate** é chamada para uma entidade que tenha um representante do grupo de segurança.</span><span class="sxs-lookup"><span data-stu-id="fe3fa-130">EWS will return an error if the **GetDelegate** operation is called for a principal that has a security group delegate.</span></span> 
  
## <a name="getdelegate-response-example"></a><span data-ttu-id="fe3fa-131">Exemplo de resposta GetDelegate</span><span class="sxs-lookup"><span data-stu-id="fe3fa-131">GetDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="fe3fa-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fe3fa-132">Description</span></span>

<span data-ttu-id="fe3fa-133">O exemplo a seguir de uma resposta **GetDelegate** mostra uma resposta bem-sucedida a uma solicitação **GetDelegate** .</span><span class="sxs-lookup"><span data-stu-id="fe3fa-133">The following example of a **GetDelegate** response shows a successful response to a **GetDelegate** request.</span></span> <span data-ttu-id="fe3fa-134">A resposta conterá informações sobre as permissões de acesso de representante, se o representante pode exibir itens particulares, se o representante recebe cópias de mensagens de reunião e a quem a reunião solicitações foram entregues.</span><span class="sxs-lookup"><span data-stu-id="fe3fa-134">The response contains information about the delegate access permissions, whether the delegate can view private items, whether the delegate receives copies of meeting messages, and to whom meeting requests were delivered.</span></span> 
  
### <a name="code"></a><span data-ttu-id="fe3fa-135">Código</span><span class="sxs-lookup"><span data-stu-id="fe3fa-135">Code</span></span>

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
    <m:GetDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                           ResponseClass="Success" 
                           xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
              <t:UserId>
                <t:SID>S-1-5-21-1333220396-2200287332-232816053-1116</t:SID>
                <t:PrimarySmtpAddress>User1@example.com</t:PrimarySmtpAddress>
                <t:DisplayName>User1</t:DisplayName>
              </t:UserId>
              <t:DelegatePermissions>
                <t:CalendarFolderPermissionLevel>Author</t:CalendarFolderPermissionLevel>
                <t:ContactsFolderPermissionLevel>Reviewer</t:ContactsFolderPermissionLevel>
              </t:DelegatePermissions>
              <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
            </m:DelegateUser>
          </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
      <m:DeliverMeetingRequests>DelegatesAndMe</m:DeliverMeetingRequests>
      </m:GetDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="fe3fa-136">Confira também</span><span class="sxs-lookup"><span data-stu-id="fe3fa-136">See also</span></span>



- [<span data-ttu-id="fe3fa-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="fe3fa-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

