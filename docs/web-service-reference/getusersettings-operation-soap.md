---
title: Operação GetUserSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 758d965c-ef63-4de4-9120-e293abf14ff8
description: A operação GetUserSettings contém uma consulta para a configuração de acesso para cliente dos usuários.
ms.openlocfilehash: e274fd4e1ca954ea25ea91a52e363c9a434b290a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466140"
---
# <a name="getusersettings-operation-soap"></a><span data-ttu-id="d4007-103">Operação GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4007-103">GetUserSettings operation (SOAP)</span></span>

<span data-ttu-id="d4007-104">A operação **GetUserSettings** contém uma consulta para a configuração de acesso para cliente dos usuários.</span><span class="sxs-lookup"><span data-stu-id="d4007-104">The **GetUserSettings** operation contains a query for users' client access configuration.</span></span> 
  
## <a name="getusersettings-request-example"></a><span data-ttu-id="d4007-105">Exemplo de solicitação GetUserSettings</span><span class="sxs-lookup"><span data-stu-id="d4007-105">GetUserSettings request example</span></span>

### <a name="description"></a><span data-ttu-id="d4007-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4007-106">Description</span></span>

<span data-ttu-id="d4007-107">O exemplo de XML a seguir mostra um corpo de solicitação de descoberta automática que solicita o nome de exibição de um usuário, o nome diferenciado, a ID de implantação, o servidor de caixa de correio, o nome diferenciado da caixa de correio, o servidor do Active Directory, a versão do servidor de acesso para cliente e os esquemas</span><span class="sxs-lookup"><span data-stu-id="d4007-107">The following XML example shows an Autodiscover request body that requests a user's display name, distinguished name, deployment ID, mailbox server, mailbox distinguished name, Active Directory server, Client Access server version, and supported Exchange Web Services schemas.</span></span>
  
### <a name="code"></a><span data-ttu-id="d4007-108">Código</span><span class="sxs-lookup"><span data-stu-id="d4007-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover"      
               xmlns:wsa="http://www.w3.org/2005/08/addressing" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"      
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2010</a:RequestedServerVersion>
    <wsa:Action>https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://myserver.contoso.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>UserName@domain.contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>UserDisplayName</a:Setting>
          <a:Setting>UserDN</a:Setting>
          <a:Setting>UserDeploymentId</a:Setting>
          <a:Setting>InternalMailboxServer</a:Setting>
          <a:Setting>MailboxDN</a:Setting>
          <a:Setting>ActiveDirectoryServer</a:Setting>
          <a:Setting>CasVersion</a:Setting>
          <a:Setting>EwsSupportedSchemas</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>

```

### <a name="request-elements"></a><span data-ttu-id="d4007-109">Elementos Request</span><span class="sxs-lookup"><span data-stu-id="d4007-109">Request elements</span></span>

<span data-ttu-id="d4007-110">Os seguintes elementos são usados no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="d4007-110">The following elements are used in the request body:</span></span>
  
- [<span data-ttu-id="d4007-111">GetUserSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4007-111">GetUserSettingsRequestMessage (SOAP)</span></span>](getusersettingsrequestmessage-soap.md)
    
- [<span data-ttu-id="d4007-112">Caixa de correio (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4007-112">Mailbox (SOAP)</span></span>](mailbox-soap.md)
    
- [<span data-ttu-id="d4007-113">Solicitação (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4007-113">Request (SOAP)</span></span>](request-soap.md)
    
- [<span data-ttu-id="d4007-114">RequestedServerVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4007-114">RequestedServerVersion (SOAP)</span></span>](requestedserverversion-soap.md)
    
- [<span data-ttu-id="d4007-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4007-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md)
    
- [<span data-ttu-id="d4007-116">Configuração (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4007-116">Setting (SOAP)</span></span>](setting-soap.md)
    
- [<span data-ttu-id="d4007-117">Usuário (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4007-117">User (SOAP)</span></span>](user-soap.md)
    
- [<span data-ttu-id="d4007-118">Usuários (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4007-118">Users (SOAP)</span></span>](users-soap.md)
    
## <a name="getusersettings-response-example"></a><span data-ttu-id="d4007-119">Exemplo de resposta GetUserSettings</span><span class="sxs-lookup"><span data-stu-id="d4007-119">GetUserSettings response example</span></span>

### <a name="description"></a><span data-ttu-id="d4007-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4007-120">Description</span></span>

<span data-ttu-id="d4007-121">O exemplo a seguir mostra uma resposta **GetUserSettings** bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="d4007-121">The following example shows a successful **GetUserSettings** response.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d4007-122">Código</span><span class="sxs-lookup"><span data-stu-id="d4007-122">Code</span></span>

```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
  </s:Header>
  <s:Body>
  <GetUserSettingsResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>NoError</ErrorCode>
            <ErrorMessage>No error.</ErrorMessage>
            <RedirectTarget i:nil="true" />
            <UserSettingErrors />
            <UserSettings>
              <UserSetting i:type="StringSetting">
                <Name>UserDisplayName</Name>
                <Value>UserDisplayName</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>UserDN</Name>
                <Value>/o=First Organization/ou=Exchange Administrative Group (SDASDASDJ)/cn=Recipients/cn=UserDisplayName</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>UserDeploymentId</Name>
                <Value>a40E2742-21c6-4050-8Ed2-d41f100c22b8</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>CasVersion</Name>
                <Value>14.00.0478.000</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>EwsSupportedSchemas</Name>
                <Value>Exchange2007,  Exchange2010</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>InternalMailboxServer</Name>
                <Value>machinename.domain.contoso.com</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>ActiveDirectoryServer</Name>
                <Value>machinename.domain.contoso.com</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>MailboxDN</Name>
                <Value>/o=First Organization/ou=Exchange Administrative Group (SDASDASDJ)/cn=Configuration/cn=Servers/cn=server/cn=Contoso Pri MDB</Value>
              </UserSetting>
            </UserSettings>
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="d4007-123">Elementos de resposta</span><span class="sxs-lookup"><span data-stu-id="d4007-123">Response elements</span></span>

<span data-ttu-id="d4007-124">Os seguintes elementos são usados no corpo da resposta:</span><span class="sxs-lookup"><span data-stu-id="d4007-124">The following elements are used in the response body:</span></span>
  
- [<span data-ttu-id="d4007-125">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4007-125">ErrorCode (SOAP)</span></span>](errorcode-soap.md)
    
- [<span data-ttu-id="d4007-126">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4007-126">ErrorMessage (SOAP)</span></span>](errormessage-soap.md)
    
- [<span data-ttu-id="d4007-127">GetUserSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4007-127">GetUserSettingsResponseMessage (SOAP)</span></span>](getusersettingsresponsemessage-soap.md)
    
- [<span data-ttu-id="d4007-128">Nome (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4007-128">Name (SOAP)</span></span>](name-soap.md)
    
- [<span data-ttu-id="d4007-129">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4007-129">RedirectTarget (SOAP)</span></span>](redirecttarget-soap.md)
    
- [<span data-ttu-id="d4007-130">Resposta (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4007-130">Response (SOAP)</span></span>](response-soap.md)
    
- [<span data-ttu-id="d4007-131">Userresponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4007-131">UserResponse (SOAP)</span></span>](userresponse-soap.md)
    
- [<span data-ttu-id="d4007-132">Userresponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4007-132">UserResponses (SOAP)</span></span>](userresponses-soap.md)
    
- [<span data-ttu-id="d4007-133">Usersetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4007-133">UserSetting (SOAP)</span></span>](usersetting-soap.md)
    
- [<span data-ttu-id="d4007-134">UserSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4007-134">UserSettingErrors (SOAP)</span></span>](usersettingerrors-soap.md)
    
- [<span data-ttu-id="d4007-135">UserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4007-135">UserSettings (SOAP)</span></span>](usersettings-soap.md)
    
- [<span data-ttu-id="d4007-136">Valor (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4007-136">Value (SOAP)</span></span>](value-soap.md)
    
## <a name="see-also"></a><span data-ttu-id="d4007-137">Também consulte</span><span class="sxs-lookup"><span data-stu-id="d4007-137">See also</span></span>



[<span data-ttu-id="d4007-138">Operação GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4007-138">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="d4007-139">Operação GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d4007-139">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)


[<span data-ttu-id="d4007-140">Elementos XML de descoberta automática SOAP para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="d4007-140">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

