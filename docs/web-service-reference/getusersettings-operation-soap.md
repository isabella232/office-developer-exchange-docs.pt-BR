---
title: Operação de GetUserSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 758d965c-ef63-4de4-9120-e293abf14ff8
description: A operação GetUserSettings contém uma consulta para a configuração de acesso de cliente dos usuários.
ms.openlocfilehash: 8bb8f766da3419ea33f89716e588a22d3924e1a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19823704"
---
# <a name="getusersettings-operation-soap"></a><span data-ttu-id="d3422-103">Operação de GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3422-103">GetUserSettings operation (SOAP)</span></span>

<span data-ttu-id="d3422-104">A operação **GetUserSettings** contém uma consulta para a configuração de acesso de cliente dos usuários.</span><span class="sxs-lookup"><span data-stu-id="d3422-104">The **GetUserSettings** operation contains a query for users' client access configuration.</span></span> 
  
## <a name="getusersettings-request-example"></a><span data-ttu-id="d3422-105">Exemplo de solicitação de GetUserSettings</span><span class="sxs-lookup"><span data-stu-id="d3422-105">GetUserSettings request example</span></span>

### <a name="description"></a><span data-ttu-id="d3422-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3422-106">Description</span></span>

<span data-ttu-id="d3422-107">O exemplo XML a seguir mostra o corpo de uma solicitação de descoberta automática que solicita a um usuário nome para exibição, nome diferenciado, ID de implantação, o servidor de caixa de correio, nome distinto da caixa de correio, servidor do Active Directory, versão do servidor de acesso para cliente e Web com suporte do Exchange Esquemas de serviços.</span><span class="sxs-lookup"><span data-stu-id="d3422-107">The following XML example shows an Autodiscover request body that requests a user's display name, distinguished name, deployment ID, mailbox server, mailbox distinguished name, Active Directory server, Client Access server version, and supported Exchange Web Services schemas.</span></span>
  
### <a name="code"></a><span data-ttu-id="d3422-108">Código</span><span class="sxs-lookup"><span data-stu-id="d3422-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover"      
               xmlns:wsa="http://www.w3.org/2005/08/addressing" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"      
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2010</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://myserver.contoso.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
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

### <a name="request-elements"></a><span data-ttu-id="d3422-109">Elementos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d3422-109">Request elements</span></span>

<span data-ttu-id="d3422-110">Os seguintes elementos são usados no corpo da solicitação:</span><span class="sxs-lookup"><span data-stu-id="d3422-110">The following elements are used in the request body:</span></span>
  
- [<span data-ttu-id="d3422-111">GetUserSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3422-111">GetUserSettingsRequestMessage (SOAP)</span></span>](getusersettingsrequestmessage-soap.md)
    
- [<span data-ttu-id="d3422-112">Caixa de correio (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3422-112">Mailbox (SOAP)</span></span>](mailbox-soap.md)
    
- [<span data-ttu-id="d3422-113">Solicitação (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3422-113">Request (SOAP)</span></span>](request-soap.md)
    
- [<span data-ttu-id="d3422-114">RequestedServerVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3422-114">RequestedServerVersion (SOAP)</span></span>](requestedserverversion-soap.md)
    
- [<span data-ttu-id="d3422-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3422-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md)
    
- [<span data-ttu-id="d3422-116">Configuração (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3422-116">Setting (SOAP)</span></span>](setting-soap.md)
    
- [<span data-ttu-id="d3422-117">Usuário (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3422-117">User (SOAP)</span></span>](user-soap.md)
    
- [<span data-ttu-id="d3422-118">Usuários (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3422-118">Users (SOAP)</span></span>](users-soap.md)
    
## <a name="getusersettings-response-example"></a><span data-ttu-id="d3422-119">Exemplo de resposta GetUserSettings</span><span class="sxs-lookup"><span data-stu-id="d3422-119">GetUserSettings response example</span></span>

### <a name="description"></a><span data-ttu-id="d3422-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3422-120">Description</span></span>

<span data-ttu-id="d3422-121">O exemplo a seguir mostra uma resposta **GetUserSettings** bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="d3422-121">The following example shows a successful **GetUserSettings** response.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d3422-122">Código</span><span class="sxs-lookup"><span data-stu-id="d3422-122">Code</span></span>

```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
  </s:Header>
  <s:Body>
  <GetUserSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
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

### <a name="response-elements"></a><span data-ttu-id="d3422-123">Elementos de resposta</span><span class="sxs-lookup"><span data-stu-id="d3422-123">Response elements</span></span>

<span data-ttu-id="d3422-124">Os seguintes elementos são usados no corpo da resposta:</span><span class="sxs-lookup"><span data-stu-id="d3422-124">The following elements are used in the response body:</span></span>
  
- [<span data-ttu-id="d3422-125">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3422-125">ErrorCode (SOAP)</span></span>](errorcode-soap.md)
    
- [<span data-ttu-id="d3422-126">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3422-126">ErrorMessage (SOAP)</span></span>](errormessage-soap.md)
    
- [<span data-ttu-id="d3422-127">GetUserSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3422-127">GetUserSettingsResponseMessage (SOAP)</span></span>](getusersettingsresponsemessage-soap.md)
    
- [<span data-ttu-id="d3422-128">Nome (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3422-128">Name (SOAP)</span></span>](name-soap.md)
    
- [<span data-ttu-id="d3422-129">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3422-129">RedirectTarget (SOAP)</span></span>](redirecttarget-soap.md)
    
- [<span data-ttu-id="d3422-130">Resposta SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3422-130">Response (SOAP)</span></span>](response-soap.md)
    
- [<span data-ttu-id="d3422-131">Resposta SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3422-131">UserResponse (SOAP)</span></span>](userresponse-soap.md)
    
- [<span data-ttu-id="d3422-132">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3422-132">UserResponses (SOAP)</span></span>](userresponses-soap.md)
    
- [<span data-ttu-id="d3422-133">UserSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3422-133">UserSetting (SOAP)</span></span>](usersetting-soap.md)
    
- [<span data-ttu-id="d3422-134">UserSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3422-134">UserSettingErrors (SOAP)</span></span>](usersettingerrors-soap.md)
    
- [<span data-ttu-id="d3422-135">UserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3422-135">UserSettings (SOAP)</span></span>](usersettings-soap.md)
    
- [<span data-ttu-id="d3422-136">Valor (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3422-136">Value (SOAP)</span></span>](value-soap.md)
    
## <a name="see-also"></a><span data-ttu-id="d3422-137">Confira também</span><span class="sxs-lookup"><span data-stu-id="d3422-137">See also</span></span>



[<span data-ttu-id="d3422-138">Operação de GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3422-138">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="d3422-139">Operação de GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d3422-139">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)


[<span data-ttu-id="d3422-140">Elementos de Autodiscover XML SOAP para o Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="d3422-140">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

