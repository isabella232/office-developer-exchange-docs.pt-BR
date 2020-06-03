---
title: Usar a Descoberta Automática para localizar os pontos de conexão
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 03896542-549b-4c45-973c-98f9025ea26c
description: Descubra como usar o serviço de descoberta automática para direcionar seu aplicativo cliente para o servidor Exchange correto.
localization_priority: Priority
ms.openlocfilehash: c1895fa0d2cce489467a726614e9457052624ef6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527590"
---
# <a name="use-autodiscover-to-find-connection-points"></a>Usar a Descoberta Automática para localizar os pontos de conexão

Descubra como usar o serviço de descoberta automática para direcionar seu aplicativo cliente para o servidor Exchange correto.
  
O serviço de descoberta automática do Exchange fornece ao aplicativo cliente definições de configuração para contas de email hospedadas no Exchange Online, Exchange Online como parte do Office 365 ou um servidor Exchange executando uma versão do Exchange a partir do Exchange 2013. O serviço de descoberta automática é um serviço Web que fornece definições de configuração. O serviço de descoberta automática é um serviço Web que fornece informações de configuração do Exchange Server para o aplicativo cliente. Os aplicativos cliente usam a descoberta automática para determinar o ponto de extremidade do serviço de descoberta automática para uma caixa de correio específica. Este artigo explica como seguir as respostas de um servidor do Exchange para encontrar o ponto de extremidade correto. 
  
Para obter informações sobre como obter definições de configuração de endereço de email, consulte [obter configurações de usuário do Exchange usando a descoberta automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) e [obter as configurações de domínio de um servidor Exchange](how-to-get-domain-settings-from-an-exchange-server.md).
  
> [!NOTE]
> O processo para localizar o ponto de extremidade correto faz parte da solicitação de configurações de usuário ou domínio. O serviço de descoberta automática usa uma série de respostas de redirecionamento para enviar o aplicativo cliente para o ponto de extremidade correto para um endereço de email. 
  
Você pode usar uma das seguintes tecnologias de desenvolvimento do Exchange para acessar o serviço de descoberta automática:

- A API gerenciada dos serviços Web do Exchange (EWS)
    
- EWS
    
Se estiver usando o EWS, você poderá usar os seguintes métodos para recuperar as configurações do usuário:
    
- O serviço de descoberta automática baseado em SOAP
    
- O serviço de descoberta automática de XML (POX)
    
- Um proxy gerado automaticamente a partir do serviço de descoberta automática SOAP ou XML
    
Para obter mais informações sobre esses métodos, consulte [autodiscover for Exchange](autodiscover-for-exchange.md).

Para obter mais informações sobre essas tecnologias de desenvolvimento do Exchange, consulte [explorar a API gerenciada do EWS, EWS e serviços Web no Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md). 

A API gerenciada do EWS fornece uma interface baseada em objeto para recuperar as configurações do usuário. Se seu aplicativo cliente usa código gerenciado, recomendamos que você use a API gerenciada do EWS. A interface de API gerenciada do EWS é melhor otimizada para um modelo de objeto simples do que o proxy de serviço Web do autogerable típico. 
  
Se você estiver usando o EWS, sugerimos que você use o serviço de descoberta automática do SOAP, pois ele oferece suporte a um conjunto mais amplo de recursos do que o serviço de descoberta automática do POX.
  
## <a name="prerequisites-for-finding-an-endpoint"></a>Pré-requisitos para localizar um ponto de extremidade
<a name="bk_Prereq"> </a>

Antes de poder criar um aplicativo cliente que usa o serviço de descoberta automática, você precisa ter acesso ao seguinte:
  
- Exchange Online ou um servidor que esteja executando uma versão do Exchange a partir do Exchange 2007 SP1. Se você estiver usando o serviço de descoberta automática baseado em SOAP, o Exchange Online ou uma versão do Exchange a partir do Exchange 2010.
    
- Um servidor do Exchange que é configurado para aceitar conexões do seu aplicativo cliente. Para obter informações sobre como configurar seu servidor Exchange, consulte [controle de acesso de aplicativo cliente ao EWS no Exchange](controlling-client-application-access-to-ews-in-exchange.md).
    
- Uma conta que está autorizada a usar o EWS. Para obter informações sobre como configurar uma conta, consulte [controle de acesso de aplicativo cliente ao EWS no Exchange](controlling-client-application-access-to-ews-in-exchange.md).
    
> [!NOTE]
> Se você estiver usando a API gerenciada do EWS, deverá fornecer um retorno de chamada de validação de certificado em algumas circunstâncias. Você também pode precisar de um retorno de chamada de validação de certificado com algumas bibliotecas de proxy geradas, como as criadas pelo Visual Studio. Para saber mais, confira [validar um certificado de servidor para a API gerenciada do EWS](how-to-validate-a-server-certificate-for-the-ews-managed-api.md). 
  
### <a name="core-concepts-for-finding-an-endpoint"></a>Principais conceitos para localizar um ponto de extremidade
<a name="bk_Core"> </a>

Antes de usar a descoberta automática para localizar um ponto de extremidade, você deve estar familiarizado com os conceitos listados na tabela a seguir.
  
|**Conceito**|**Descrição**|
|:-----|:-----|
|[Descoberta Automática do Exchange](autodiscover-for-exchange.md) <br/> |Fornece uma visão geral de como o serviço de descoberta automática funciona.  <br/> |
   
Se você estiver usando a API gerenciada do EWS, use a classe [Microsoft. Exchange. WebServices. Data. ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) no namespace [Microsoft. Exchange. WebServices. Data](https://msdn.microsoft.com/library/dd633907%28v=exchg.80%29.aspx) para gerenciar sua conexão com o EWS. Para usar os exemplos de código da API gerenciada do EWS neste artigo, você precisa fazer referência aos seguintes namespaces no seu código: 
  
- **System.Net**
    
- **Microsoft. Exchange. WebServices. Data. ExchangeService**
    
## <a name="find-the-correct-endpoint-by-using-the-ews-managed-api"></a>Encontre o ponto de extremidade correto usando a API gerenciada do EWS
<a name="bk_Managed"> </a>

Se você estiver usando a API gerenciada do EWS, as chamadas para o serviço de descoberta automática serão tratadas pela classe **ExchangeService** . Para determinar o ponto de extremidade correto para uma conta de email, chame o método **AutodiscoverUrl** em um objeto **[ExchangeService]** . O exemplo de código a seguir mostra como definir o ponto de extremidade do serviço Web EWS para um endereço de email para o arquivo Exchange. asmx no servidor de acesso para cliente correto usando a API gerenciada do EWS. 
  
```cs
NetworkCredential credentials = new NetworkCredential(securelyStoredEmail, securelyStoredPassword);
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2013);
service.Credentials = credentials;
service.AutodiscoverUrl("User1@contoso.com");
```

## <a name="find-the-correct-endpoint-by-using-ews"></a>Encontre o ponto de extremidade correto usando o EWS
<a name="bk_SOAP"> </a>

O serviço de descoberta automática do SOAP pode usar uma série de solicitações e respostas para direcionar seu aplicativo para o ponto de extremidade correto do EWS. Para obter informações sobre o processo para determinar o ponto de extremidade correto para uma conta de email, consulte [autodiscover for Exchange](autodiscover-for-exchange.md). Os exemplos de XML a seguir mostram a série de solicitações e respostas que você pode esperar ao fazer uma solicitação de descoberta automática do SOAP para localizar o ponto de extremidade correto.
  
### <a name="soap-autodiscover-endpoint-request"></a>Solicitação de ponto de extremidade de descoberta automática SOAP

O exemplo a seguir mostra uma solicitação XML que é enviada para o serviço de descoberta automática para localizar o ponto de extremidade correto.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://mail.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>User1@Contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>InternalEwsUrl</a:Setting>
          <a:Setting>ExternalEwsUrl</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>

```

### <a name="soap-autodiscover-redirection-response"></a>Resposta de redirecionamento de descoberta automática SOAP

O serviço de descoberta automática pode responder com uma de duas respostas de redirecionamento: um HTTP 302 Redirect ou uma resposta de redirecionamento SOAP. Se a resposta do servidor Exchange for um redirecionamento HTTP 302, o aplicativo cliente deverá validar que o endereço de redirecionamento é aceitável e, em seguida, seguir a resposta de redirecionamento.
  
> [!IMPORTANT]
> Para saber mais sobre como validar uma resposta de redirecionamento, confira [descoberta automática do Exchange](autodiscover-for-exchange.md). 
  
Se o serviço descoberta automática retornar uma resposta de redirecionamento, indicada pelo elemento [ErrorCode](https://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) do elemento **userresponse** , seu aplicativo cliente deverá usar o elemento **RedirectTarget** para construir uma nova solicitação de configurações que será enviada ao servidor especificado na resposta de redirecionamento. O exemplo a seguir mostra uma resposta de redirecionamento do servidor. 
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/" xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">https://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>682</h:MajorBuildNumber>
      <h:MinorBuildNumber>1</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>RedirectAddress</ErrorCode>
            <ErrorMessage>Redirection address.</ErrorMessage>
            <RedirectTarget>User1@mail.Contoso.com</RedirectTarget>
            <UserSettingErrors />
            <UserSettings />
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>

```

Após um redirecionamento, o cliente usa a URL de redirecionamento para preparar outra solicitação. O código a seguir mostra um exemplo da solicitação que você cria a partir da resposta de redirecionamento.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>https://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>User1@mail.Contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>InternalEwsUrl</a:Setting>
          <a:Setting>ExternalEwsUrl</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>

```

Quando o aplicativo cliente tiver sido direcionado para o ponto de extremidade correto para o serviço de descoberta automática, o servidor enviará uma resposta com o elemento [ErrorCode](https://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) do elemento **userresponse** definido como **NOERROR** e que contém as configurações de usuário solicitadas. Somente as configurações de usuário solicitadas, **InternalEwsUrl** e **ExternalEwsUrl**, são retornadas. O exemplo a seguir mostra a resposta do servidor. 
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/" 
        xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">https://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>160</h:MajorBuildNumber>
      <h:MinorBuildNumber>4</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
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
                <Name>InternalEwsUrl</Name>
                <Value>https://server.Contoso.com/ews/exchange.asmx</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>ExternalEwsUrl</Name>
                <Value>https://server.Contoso.com/ews/exchange.asmx</Value>
              </UserSetting>
            </UserSettings>
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>
```

## <a name="next-steps"></a>Próximas etapas
<a name="bk_Next"> </a>

Localizar o ponto de extremidade seguindo o processo de descoberta automática retorna as configurações de domínio ou usuário solicitadas. Para obter informações sobre como fazer uma solicitação para configurações específicas, consulte os seguintes artigos:
  
- [Obter as configurações de domínio de um servidor do Exchange](how-to-get-domain-settings-from-an-exchange-server.md)    
- [Obter as configurações de usuário do Exchange usando a Descoberta Automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
## <a name="see-also"></a>Confira também

- [Configurando o aplicativo EWS](setting-up-your-ews-application.md)   
- [Descoberta Automática do Exchange](autodiscover-for-exchange.md)    
- [Referência do serviço Web de descoberta automática do Exchange](https://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)    
- [Referência do EWS para Exchange](https://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)
    

