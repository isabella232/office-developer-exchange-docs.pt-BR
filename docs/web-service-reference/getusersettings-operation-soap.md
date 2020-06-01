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
# <a name="getusersettings-operation-soap"></a>Operação GetUserSettings (SOAP)

A operação **GetUserSettings** contém uma consulta para a configuração de acesso para cliente dos usuários. 
  
## <a name="getusersettings-request-example"></a>Exemplo de solicitação GetUserSettings

### <a name="description"></a>Descrição

O exemplo de XML a seguir mostra um corpo de solicitação de descoberta automática que solicita o nome de exibição de um usuário, o nome diferenciado, a ID de implantação, o servidor de caixa de correio, o nome diferenciado da caixa de correio, o servidor do Active Directory, a versão do servidor de acesso para cliente e os esquemas
  
### <a name="code"></a>Código

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

### <a name="request-elements"></a>Elementos Request

Os seguintes elementos são usados no corpo da solicitação:
  
- [GetUserSettingsRequestMessage (SOAP)](getusersettingsrequestmessage-soap.md)
    
- [Caixa de correio (SOAP)](mailbox-soap.md)
    
- [Solicitação (SOAP)](request-soap.md)
    
- [RequestedServerVersion (SOAP)](requestedserverversion-soap.md)
    
- [RequestedSettings (SOAP)](requestedsettings-soap.md)
    
- [Configuração (SOAP)](setting-soap.md)
    
- [Usuário (SOAP)](user-soap.md)
    
- [Usuários (SOAP)](users-soap.md)
    
## <a name="getusersettings-response-example"></a>Exemplo de resposta GetUserSettings

### <a name="description"></a>Descrição

O exemplo a seguir mostra uma resposta **GetUserSettings** bem-sucedida. 
  
### <a name="code"></a>Código

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

### <a name="response-elements"></a>Elementos de resposta

Os seguintes elementos são usados no corpo da resposta:
  
- [ErrorCode (SOAP)](errorcode-soap.md)
    
- [ErrorMessage (SOAP)](errormessage-soap.md)
    
- [GetUserSettingsResponseMessage (SOAP)](getusersettingsresponsemessage-soap.md)
    
- [Nome (SOAP)](name-soap.md)
    
- [RedirectTarget (SOAP)](redirecttarget-soap.md)
    
- [Resposta (SOAP)](response-soap.md)
    
- [Userresponse (SOAP)](userresponse-soap.md)
    
- [Userresponses (SOAP)](userresponses-soap.md)
    
- [Usersetting (SOAP)](usersetting-soap.md)
    
- [UserSettingErrors (SOAP)](usersettingerrors-soap.md)
    
- [UserSettings (SOAP)](usersettings-soap.md)
    
- [Valor (SOAP)](value-soap.md)
    
## <a name="see-also"></a>Também consulte



[Operação GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
  
[Operação GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)


[Elementos XML de descoberta automática SOAP para o Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

