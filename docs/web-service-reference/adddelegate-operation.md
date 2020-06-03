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
description: A operação AddDelegate adiciona um ou mais representantes à caixa de correio de uma entidade de segurança e define permissões de acesso específicas.
ms.openlocfilehash: 80adbe71d69be1025dc9593c6a9002bc68fdcb76
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466511"
---
# <a name="adddelegate-operation"></a><span data-ttu-id="a6a03-103">Operação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="a6a03-103">AddDelegate operation</span></span>

<span data-ttu-id="a6a03-104">A operação **AddDelegate** adiciona um ou mais representantes à caixa de correio de uma entidade de segurança e define permissões de acesso específicas.</span><span class="sxs-lookup"><span data-stu-id="a6a03-104">The **AddDelegate** operation adds one or more delegates to a principal's mailbox and sets specific access permissions.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="a6a03-105">Cabeçalhos SOAP</span><span class="sxs-lookup"><span data-stu-id="a6a03-105">SOAP headers</span></span>

<span data-ttu-id="a6a03-106">A operação **AddDelegate** pode usar os cabeçalhos SOAP listados e descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="a6a03-106">The **AddDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="a6a03-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="a6a03-107">**Header**</span></span>|<span data-ttu-id="a6a03-108">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="a6a03-108">**Element**</span></span>|<span data-ttu-id="a6a03-109">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a6a03-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a6a03-110">Representação</span><span class="sxs-lookup"><span data-stu-id="a6a03-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="a6a03-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="a6a03-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="a6a03-112">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="a6a03-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="a6a03-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="a6a03-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="a6a03-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="a6a03-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="a6a03-115">Identifica a cultura RFC3066 a ser usada para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="a6a03-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="a6a03-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="a6a03-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="a6a03-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="a6a03-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="a6a03-118">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="a6a03-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="a6a03-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="a6a03-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="a6a03-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a6a03-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="a6a03-121">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6a03-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="adddelegate-request-example"></a><span data-ttu-id="a6a03-122">Exemplo de solicitação AddDelegate</span><span class="sxs-lookup"><span data-stu-id="a6a03-122">AddDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="a6a03-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6a03-123">Description</span></span>

<span data-ttu-id="a6a03-124">O exemplo a seguir de uma solicitação **AddDelegate** mostra uma tentativa de conceder as permissões de representante Usuário1 em pastas pertencentes a Usuário2.</span><span class="sxs-lookup"><span data-stu-id="a6a03-124">The following example of an **AddDelegate** request shows an attempt to give user1 delegate permissions on folders that are owned by user2.</span></span> <span data-ttu-id="a6a03-125">O Usuário1 recebe permissões no nível do autor para a pasta calendário do user2's e permissões no nível do revisor para a pasta contatos do user2's.</span><span class="sxs-lookup"><span data-stu-id="a6a03-125">User1 is given Author-level permissions to user2's Calendar folder and Reviewer-level permissions to user2's Contacts folder.</span></span> <span data-ttu-id="a6a03-126">Usuário1 não receberá cópias de mensagens de reunião e não poderá exibir itens privados na caixa de correio do user2's.</span><span class="sxs-lookup"><span data-stu-id="a6a03-126">User1 will not receive copies of meeting messages and will be unable to view private items in user2's mailbox.</span></span> <span data-ttu-id="a6a03-127">As solicitações de reunião serão enviadas para usuário1 e Usuário2.</span><span class="sxs-lookup"><span data-stu-id="a6a03-127">Meeting requests will be sent to both user1 and user2.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a6a03-128">Código</span><span class="sxs-lookup"><span data-stu-id="a6a03-128">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="adddelegate-response-example"></a><span data-ttu-id="a6a03-129">Exemplo de resposta AddDelegate</span><span class="sxs-lookup"><span data-stu-id="a6a03-129">AddDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="a6a03-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6a03-130">Description</span></span>

<span data-ttu-id="a6a03-131">O exemplo a seguir de uma resposta **AddDelegate** mostra uma resposta bem-sucedida a uma solicitação **adddelegar** .</span><span class="sxs-lookup"><span data-stu-id="a6a03-131">The following example of an **AddDelegate** response shows a successful response to an **AddDelegate** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a6a03-132">Código</span><span class="sxs-lookup"><span data-stu-id="a6a03-132">Code</span></span>

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
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:AddDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                           ResponseClass="Success" 
                           xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="adddelegate-error-response-example"></a><span data-ttu-id="a6a03-133">Exemplo de resposta de erro AddDelegate</span><span class="sxs-lookup"><span data-stu-id="a6a03-133">AddDelegate error response example</span></span>

### <a name="description"></a><span data-ttu-id="a6a03-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6a03-134">Description</span></span>

<span data-ttu-id="a6a03-135">O exemplo a seguir mostra a resposta a uma solicitação para adicionar um representante que já foi adicionado à caixa de correio da entidade de segurança.</span><span class="sxs-lookup"><span data-stu-id="a6a03-135">The following example shows the response to a request to add a delegate who has already been added to the principal's mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="a6a03-136">Código</span><span class="sxs-lookup"><span data-stu-id="a6a03-136">Code</span></span>

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
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:AddDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                           ResponseClass="Success"
                           xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="a6a03-137">Comentários</span><span class="sxs-lookup"><span data-stu-id="a6a03-137">Comments</span></span>

<span data-ttu-id="a6a03-138">Se o código de resposta ErrorDelegateAlreadyExists for retornado quando você tentar adicionar um representante, use a [operação getdelegate](getdelegate-operation.md) para obter todas as permissões atuais para o representante e, em seguida, use a [operação UpdateDelegate](updatedelegate-operation.md) para definir as novas permissões.</span><span class="sxs-lookup"><span data-stu-id="a6a03-138">If the ErrorDelegateAlreadyExists response code is returned when you try to add a delegate, use the [GetDelegate operation](getdelegate-operation.md) to get all the current permissions for the delegate, and then use the [UpdateDelegate operation](updatedelegate-operation.md) to set the new permissions.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="a6a03-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="a6a03-139">See also</span></span>

- [<span data-ttu-id="a6a03-140">Adicionar representantes</span><span class="sxs-lookup"><span data-stu-id="a6a03-140">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

