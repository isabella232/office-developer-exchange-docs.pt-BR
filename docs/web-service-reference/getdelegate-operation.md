---
title: Operação getdelegate
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
description: A operação getdelegation recupera as configurações de representante de uma caixa de correio especificada.
ms.openlocfilehash: 400bf5d1cafcbb789aaa749c62c7a908622d4ddb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461062"
---
# <a name="getdelegate-operation"></a><span data-ttu-id="4a590-103">Operação getdelegate</span><span class="sxs-lookup"><span data-stu-id="4a590-103">GetDelegate operation</span></span>

<span data-ttu-id="4a590-104">A operação **Getdelegation** recupera as configurações de representante de uma caixa de correio especificada.</span><span class="sxs-lookup"><span data-stu-id="4a590-104">The **GetDelegate** operation retrieves the delegate settings for a specified mailbox.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="4a590-105">Cabeçalhos SOAP</span><span class="sxs-lookup"><span data-stu-id="4a590-105">SOAP Headers</span></span>

<span data-ttu-id="4a590-106">A operação **Getdelegate** pode usar os cabeçalhos SOAP listados e descritos na tabela a seguir.</span><span class="sxs-lookup"><span data-stu-id="4a590-106">The **GetDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="4a590-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="4a590-107">**Header**</span></span>|<span data-ttu-id="4a590-108">**Elemento**</span><span class="sxs-lookup"><span data-stu-id="4a590-108">**Element**</span></span>|<span data-ttu-id="4a590-109">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="4a590-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4a590-110">Representação</span><span class="sxs-lookup"><span data-stu-id="4a590-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="4a590-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="4a590-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="4a590-112">Identifica o usuário que o aplicativo cliente está representando.</span><span class="sxs-lookup"><span data-stu-id="4a590-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="4a590-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="4a590-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="4a590-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="4a590-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="4a590-115">Identifica a cultura RFC3066 a ser usada para acessar a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4a590-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="4a590-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="4a590-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="4a590-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="4a590-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="4a590-118">Identifica a versão do esquema para a solicitação de operação.</span><span class="sxs-lookup"><span data-stu-id="4a590-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="4a590-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="4a590-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="4a590-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4a590-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="4a590-121">Identifica a versão do servidor que respondeu à solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a590-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getdelegate-request-example"></a><span data-ttu-id="4a590-122">Exemplo de solicitação getdelegate</span><span class="sxs-lookup"><span data-stu-id="4a590-122">GetDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="4a590-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a590-123">Description</span></span>

<span data-ttu-id="4a590-124">O exemplo de código a seguir mostra como recuperar as configurações de representante de todos os representantes definidos na caixa de correio do user3's.</span><span class="sxs-lookup"><span data-stu-id="4a590-124">The following code example shows how to retrieve the delegate settings for all the delegates that are set on user3's mailbox.</span></span> <span data-ttu-id="4a590-125">Todas as permissões para cada usuário são retornadas na resposta.</span><span class="sxs-lookup"><span data-stu-id="4a590-125">All the permissions for each user are returned in the response.</span></span>
  
### <a name="code"></a><span data-ttu-id="4a590-126">Código</span><span class="sxs-lookup"><span data-stu-id="4a590-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body>
    <GetDelegate xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                 IncludePermissions="true">
      <Mailbox>
        <t:EmailAddress>user3@example.com</t:EmailAddress>
      </Mailbox>
    </GetDelegate>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="4a590-127">Comentários</span><span class="sxs-lookup"><span data-stu-id="4a590-127">Comments</span></span>

<span data-ttu-id="4a590-128">Você pode usar o elemento [userid](userid.md) para especificar usuários individuais, em vez de retornar todos os usuários que têm permissões de acesso de representante na caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="4a590-128">You can use the [UserId](userid.md) element to specify individual users instead of returning all users who have delegate access permissions on the mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="4a590-129">Os serviços Web do Exchange (EWS) não dão suporte ao gerenciamento de delegados de grupo.</span><span class="sxs-lookup"><span data-stu-id="4a590-129">Exchange Web Services (EWS) does not support managing group delegates.</span></span> <span data-ttu-id="4a590-130">O EWS retornará um erro se a operação **Getdelegar** for chamada para uma entidade que tenha um representante de grupo de segurança.</span><span class="sxs-lookup"><span data-stu-id="4a590-130">EWS will return an error if the **GetDelegate** operation is called for a principal that has a security group delegate.</span></span> 
  
## <a name="getdelegate-response-example"></a><span data-ttu-id="4a590-131">Exemplo de resposta getdelegate</span><span class="sxs-lookup"><span data-stu-id="4a590-131">GetDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="4a590-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a590-132">Description</span></span>

<span data-ttu-id="4a590-133">O exemplo a seguir de uma resposta **Getdelegate** mostra uma resposta bem-sucedida a uma solicitação **getdelegate** .</span><span class="sxs-lookup"><span data-stu-id="4a590-133">The following example of a **GetDelegate** response shows a successful response to a **GetDelegate** request.</span></span> <span data-ttu-id="4a590-134">A resposta contém informações sobre as permissões de acesso de representante, se o representante pode exibir itens particulares, se o representante recebe cópias de mensagens de reunião e para quem as solicitações de reunião foram entregues.</span><span class="sxs-lookup"><span data-stu-id="4a590-134">The response contains information about the delegate access permissions, whether the delegate can view private items, whether the delegate receives copies of meeting messages, and to whom meeting requests were delivered.</span></span> 
  
### <a name="code"></a><span data-ttu-id="4a590-135">Código</span><span class="sxs-lookup"><span data-stu-id="4a590-135">Code</span></span>

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
    <m:GetDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
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

## <a name="see-also"></a><span data-ttu-id="4a590-136">Também consulte</span><span class="sxs-lookup"><span data-stu-id="4a590-136">See also</span></span>



- [<span data-ttu-id="4a590-137">Elementos XML do EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="4a590-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

