---
title: Operação UpdateDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateDelegate
api_type:
- schema
ms.assetid: 03f618ac-ad1a-4772-9b81-c5bb0f12d6ab
description: A operação UpdateDelegate atualiza delegar permissões na caixa de correio da entidade de segurança.
ms.openlocfilehash: 9f69d784617d10d8902a260bbf6639703dd33b6d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19837877"
---
# <a name="updatedelegate-operation"></a><span data-ttu-id="03ead-103">Operação UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="03ead-103">UpdateDelegate operation</span></span>

<span data-ttu-id="03ead-104">A operação **UpdateDelegate** atualiza delegar permissões na caixa de correio da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="03ead-104">The **UpdateDelegate** operation updates delegate permissions on a principal's mailbox.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="03ead-105">Cabeçalhos SOAP</span><span class="sxs-lookup"><span data-stu-id="03ead-105">SOAP Headers</span></span>

<span data-ttu-id="03ead-106">A operação **UpdateDelegate** pode usar os cabeçalhos SOAP que estão listados e descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="03ead-106">The **UpdateDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="03ead-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="03ead-107">**Header**</span></span>|<span data-ttu-id="03ead-108">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="03ead-108">**Element**</span></span>|<span data-ttu-id="03ead-109">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="03ead-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="03ead-110">Representação</span><span class="sxs-lookup"><span data-stu-id="03ead-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="03ead-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="03ead-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="03ead-112">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="03ead-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="03ead-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="03ead-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="03ead-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="03ead-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="03ead-115">Identifica a cultura RFC3066 a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="03ead-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="03ead-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="03ead-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="03ead-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="03ead-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="03ead-118">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="03ead-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="03ead-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="03ead-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="03ead-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="03ead-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="03ead-121">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="03ead-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="updatedelegate-request-example"></a><span data-ttu-id="03ead-122">Exemplo de solicitação de UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="03ead-122">UpdateDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="03ead-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="03ead-123">Description</span></span>

<span data-ttu-id="03ead-124">O exemplo a seguir de uma solicitação de **UpdateDelegate** mostra como atualizar permissões delegadas na conta de user1.</span><span class="sxs-lookup"><span data-stu-id="03ead-124">The following example of an **UpdateDelegate** request shows you how to update delegate permissions on user1's account.</span></span> <span data-ttu-id="03ead-125">O Usuário2 recebe nenhuma permissão no nível da pasta de tarefas e é concedida a permissão para exibir itens particulares.</span><span class="sxs-lookup"><span data-stu-id="03ead-125">User2 is granted the None permission level for the Tasks folder and is granted permission to view private items.</span></span> <span data-ttu-id="03ead-126">User3 recebe permissões de revisor para a pasta diário.</span><span class="sxs-lookup"><span data-stu-id="03ead-126">User3 is granted Reviewer permissions for the Journal folder.</span></span> <span data-ttu-id="03ead-127">As solicitações de reunião sejam enviadas para os representantes e informações sobre a solicitação são enviadas ao User1.</span><span class="sxs-lookup"><span data-stu-id="03ead-127">Meeting requests are sent to the delegates, and information about the request is sent to User1.</span></span> 
  
### <a name="code"></a><span data-ttu-id="03ead-128">Código</span><span class="sxs-lookup"><span data-stu-id="03ead-128">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body>
    <UpdateDelegate xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
        <t:EmailAddress>user1@example.com</t:EmailAddress>
      </Mailbox>
      <DelegateUsers>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>user2@example.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:TasksFolderPermissionLevel>None</t:TasksFolderPermissionLevel>
          </t:DelegatePermissions>
          <t:ViewPrivateItems>true</t:ViewPrivateItems>
        </t:DelegateUser>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>user3@example.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:JournalFolderPermissionLevel>Reviewer</t:JournalFolderPermissionLevel>
          </t:DelegatePermissions>
        </t:DelegateUser>
      </DelegateUsers>
      <DeliverMeetingRequests>DelegatesAndSendInformationToMe</DeliverMeetingRequests>
    </UpdateDelegate>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="03ead-129">Comments</span><span class="sxs-lookup"><span data-stu-id="03ead-129">Comments</span></span>

<span data-ttu-id="03ead-130">A solicitação [UpdateDelegate](updatedelegate.md) não exige que as atualizações ser aplicadas aos delegados.</span><span class="sxs-lookup"><span data-stu-id="03ead-130">The [UpdateDelegate](updatedelegate.md) request does not require that updates be applied to delegates.</span></span> <span data-ttu-id="03ead-131">Os clientes podem alterar apenas a configuração de **DeliverMeetingMessage** .</span><span class="sxs-lookup"><span data-stu-id="03ead-131">Clients can change only the **DeliverMeetingMessage** setting.</span></span> 
  
## <a name="updatedelegate-response-example"></a><span data-ttu-id="03ead-132">Exemplo de resposta UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="03ead-132">UpdateDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="03ead-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="03ead-133">Description</span></span>

<span data-ttu-id="03ead-134">O exemplo a seguir mostra uma resposta bem-sucedida para uma operação de **UpdateDelegate** .</span><span class="sxs-lookup"><span data-stu-id="03ead-134">The following example shows a successful response to an **UpdateDelegate** operation.</span></span> 
  
### <a name="code"></a><span data-ttu-id="03ead-135">Código</span><span class="sxs-lookup"><span data-stu-id="03ead-135">Code</span></span>

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
    <m:UpdateDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                              ResponseClass="Success"
                              xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
            <t:UserId>
              <t:SID>S-1-5-21-1333220396-2200287332-232816053-1117</t:SID>
              <t:PrimarySmtpAddress>User2@example.com</t:PrimarySmtpAddress>
              <t:DisplayName>User2</t:DisplayName>
            </t:UserId>
            <t:ReceiveCopiesOfMeetingMessages>true</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>true</t:ViewPrivateItems>
          </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
            <t:UserId>
              <t:SID>S-1-5-21-1333220396-2200287332-232816053-1118</t:SID>
              <t:PrimarySmtpAddress>User3@example.com</t:PrimarySmtpAddress>
              <t:DisplayName>User3</t:DisplayName>
            </t:UserId>
            <t:ReceiveCopiesOfMeetingMessages>true</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
          </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
    </m:UpdateDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="updatedelegate-error-response-example"></a><span data-ttu-id="03ead-136">Exemplo de resposta de erro UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="03ead-136">UpdateDelegate Error response example</span></span>

### <a name="description"></a><span data-ttu-id="03ead-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="03ead-137">Description</span></span>

<span data-ttu-id="03ead-138">O exemplo a seguir mostra uma resposta de erro a uma solicitação **UpdateDelegate** .</span><span class="sxs-lookup"><span data-stu-id="03ead-138">The following example shows an error response to an **UpdateDelegate** request.</span></span> <span data-ttu-id="03ead-139">O erro foi gerado porque o representante não existir na lista de representantes do principal.</span><span class="sxs-lookup"><span data-stu-id="03ead-139">The error was generated because the delegate does not exist in the principal's delegate list.</span></span> 
  
### <a name="code"></a><span data-ttu-id="03ead-140">Código</span><span class="sxs-lookup"><span data-stu-id="03ead-140">Code</span></span>

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
    <m:UpdateDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
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
      </m:UpdateDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="03ead-141">Confira também</span><span class="sxs-lookup"><span data-stu-id="03ead-141">See also</span></span>



- [<span data-ttu-id="03ead-142">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="03ead-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

