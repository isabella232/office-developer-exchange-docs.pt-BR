---
title: Operação AddDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AddDelegate
api_type:
- schema
ms.assetid: 012d8cc5-648c-4ba0-a155-15c422b1e994
description: A operação AddDelegate adiciona um ou mais representantes à caixa de correio da entidade de segurança e define as permissões de acesso específico.
ms.openlocfilehash: 28d4ded2625efc3d6eade44f5fafc06c2ffca7ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19751043"
---
# <a name="adddelegate-operation"></a><span data-ttu-id="2596a-103">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="2596a-103">AddDelegate operation</span></span>

<span data-ttu-id="2596a-104">A operação **AddDelegate** adiciona um ou mais representantes à caixa de correio da entidade de segurança e define as permissões de acesso específico.</span><span class="sxs-lookup"><span data-stu-id="2596a-104">The **AddDelegate** operation adds one or more delegates to a principal's mailbox and sets specific access permissions.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="2596a-105">Cabeçalhos SOAP</span><span class="sxs-lookup"><span data-stu-id="2596a-105">SOAP headers</span></span>

<span data-ttu-id="2596a-106">A operação **AddDelegate** pode usar os cabeçalhos SOAP que estão listados e descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="2596a-106">The **AddDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="2596a-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="2596a-107">**Header**</span></span>|<span data-ttu-id="2596a-108">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="2596a-108">**Element**</span></span>|<span data-ttu-id="2596a-109">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2596a-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2596a-110">Representação</span><span class="sxs-lookup"><span data-stu-id="2596a-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="2596a-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="2596a-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="2596a-112">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="2596a-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="2596a-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="2596a-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="2596a-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="2596a-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="2596a-115">Identifica a cultura RFC3066 a ser usado para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2596a-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="2596a-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="2596a-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="2596a-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="2596a-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="2596a-118">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="2596a-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="2596a-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="2596a-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="2596a-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="2596a-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="2596a-121">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="2596a-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="adddelegate-request-example"></a><span data-ttu-id="2596a-122">Exemplo de solicitação de AddDelegate</span><span class="sxs-lookup"><span data-stu-id="2596a-122">AddDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="2596a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="2596a-123">Description</span></span>

<span data-ttu-id="2596a-124">O exemplo a seguir de uma solicitação de **AddDelegate** mostra uma tentativa de dar user1 delegar permissões de pastas pertencentes Usuário2.</span><span class="sxs-lookup"><span data-stu-id="2596a-124">The following example of an **AddDelegate** request shows an attempt to give user1 delegate permissions on folders that are owned by user2.</span></span> <span data-ttu-id="2596a-125">O Usuário1 recebe permissões no nível do autor a pasta de calendário e permissões no nível do revisor à pasta de contatos do Usuário2 do Usuário2.</span><span class="sxs-lookup"><span data-stu-id="2596a-125">User1 is given Author-level permissions to user2's Calendar folder and Reviewer-level permissions to user2's Contacts folder.</span></span> <span data-ttu-id="2596a-126">Usuário1 não receberá cópias de mensagens de reunião e poderão exibir itens particulares na caixa de correio do Usuário2.</span><span class="sxs-lookup"><span data-stu-id="2596a-126">User1 will not receive copies of meeting messages and will be unable to view private items in user2's mailbox.</span></span> <span data-ttu-id="2596a-127">Solicitações de reunião serão enviadas para user1 e user2.</span><span class="sxs-lookup"><span data-stu-id="2596a-127">Meeting requests will be sent to both user1 and user2.</span></span> 
  
### <a name="code"></a><span data-ttu-id="2596a-128">Código</span><span class="sxs-lookup"><span data-stu-id="2596a-128">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <AddDelegate>
      <Mailbox>
        <t:EmailAddress>user2@example.com</t:EmailAddress>
      </Mailbox>
      <DelegateUsers>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>user1@example.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:CalendarFolderPermissionLevel>Author</t:CalendarFolderPermissionLevel>
            <t:ContactsFolderPermissionLevel>Reviewer</t:ContactsFolderPermissionLevel>
          </t:DelegatePermissions>
          <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
          <t:ViewPrivateItems>false</t:ViewPrivateItems>
        </t:DelegateUser>
      </DelegateUsers>
      <DeliverMeetingRequests>DelegatesAndMe</DeliverMeetingRequests>
    </AddDelegate>
  </soap:Body>
</soap:Envelope>
```

## <a name="adddelegate-response-example"></a><span data-ttu-id="2596a-129">Exemplo de resposta AddDelegate</span><span class="sxs-lookup"><span data-stu-id="2596a-129">AddDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="2596a-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="2596a-130">Description</span></span>

<span data-ttu-id="2596a-131">O exemplo a seguir de uma resposta **AddDelegate** mostra uma resposta bem-sucedida a uma solicitação **AddDelegate** .</span><span class="sxs-lookup"><span data-stu-id="2596a-131">The following example of an **AddDelegate** response shows a successful response to an **AddDelegate** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="2596a-132">Código</span><span class="sxs-lookup"><span data-stu-id="2596a-132">Code</span></span>

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
    <m:AddDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
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
              <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
            </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
    </m:AddDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="adddelegate-error-response-example"></a><span data-ttu-id="2596a-133">Exemplo de resposta de erro AddDelegate</span><span class="sxs-lookup"><span data-stu-id="2596a-133">AddDelegate error response example</span></span>

### <a name="description"></a><span data-ttu-id="2596a-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="2596a-134">Description</span></span>

<span data-ttu-id="2596a-135">O exemplo a seguir mostra a resposta a uma solicitação para adicionar um delegado que já foi adicionado à caixa de correio do principal.</span><span class="sxs-lookup"><span data-stu-id="2596a-135">The following example shows the response to a request to add a delegate who has already been added to the principal's mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="2596a-136">Código</span><span class="sxs-lookup"><span data-stu-id="2596a-136">Code</span></span>

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
    <m:AddDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                           ResponseClass="Success"
                           xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Error">
          <m:MessageText>The user is already a delegate for the mailbox.</m:MessageText>
          <m:ResponseCode>ErrorDelegateAlreadyExists</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
      </m:AddDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="2596a-137">Comments</span><span class="sxs-lookup"><span data-stu-id="2596a-137">Comments</span></span>

<span data-ttu-id="2596a-138">Se o código de resposta ErrorDelegateAlreadyExists é retornado ao tentar adicionar um representante, use a [operação GetDelegate](getdelegate-operation.md) para obter todas as permissões atuais para o representante e, em seguida, use a [operação UpdateDelegate](updatedelegate-operation.md) para definir as novas permissões.</span><span class="sxs-lookup"><span data-stu-id="2596a-138">If the ErrorDelegateAlreadyExists response code is returned when you try to add a delegate, use the [GetDelegate operation](getdelegate-operation.md) to get all the current permissions for the delegate, and then use the [UpdateDelegate operation](updatedelegate-operation.md) to set the new permissions.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="2596a-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="2596a-139">See also</span></span>

- [<span data-ttu-id="2596a-140">Adicionando representantes</span><span class="sxs-lookup"><span data-stu-id="2596a-140">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

