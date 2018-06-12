---
title: Usar descoberta automática para encontrar os pontos de conexão
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 03896542-549b-4c45-973c-98f9025ea26c
description: Descubra como usar o serviço Descoberta automática para direcionar o seu aplicativo cliente para o servidor Exchange correto.
ms.openlocfilehash: 653fcd1c094c23c3e89e903b7194b96720802b51
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750837"
---
# <a name="use-autodiscover-to-find-connection-points"></a>Usar descoberta automática para encontrar os pontos de conexão

Descubra como usar o serviço Descoberta automática para direcionar o seu aplicativo cliente para o servidor Exchange correto.
  
O serviço de descoberta automática do Exchange fornece seu aplicativo de cliente com as definições de configuração para contas de email hospedadas no Exchange Online, Exchange Online como parte do Office 365 ou um servidor do Exchange executando uma versão do Exchange, começando com o Exchange 2013. O serviço de descoberta automática é um serviço web que fornece configurações. O serviço de descoberta automática é um serviço web que fornece informações de configuração de servidor do Exchange ao seu aplicativo cliente. Aplicativos clientes usam a descoberta automática para determinar o ponto de extremidade do serviço Descoberta automática para uma caixa de correio específica. Este artigo explica como a seguir as respostas de um servidor Exchange para localizar o ponto de extremidade correto. 
  
Para obter informações sobre como obter as definições de configuração de endereço de email, consulte [obter configurações de usuário do Exchange usando a descoberta automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) e [Obtenha as configurações de domínio de um servidor Exchange](how-to-get-domain-settings-from-an-exchange-server.md).
  
> [!NOTE]
> O processo para localizar o ponto de extremidade correto é parte da solicitação de usuário ou de configurações de domínio. O serviço Descoberta automática usa uma série de respostas de redirecionamento para enviar o aplicativo cliente para o ponto de extremidade correto para um endereço de email. 
  
Você pode usar uma das seguintes tecnologias de desenvolvimento do Exchange para acessar o serviço de descoberta automática:
  
> [!NOTE]
> Para obter mais informações sobre essas tecnologias de desenvolvimento do Exchange, consulte a [explorar o EWS Managed API, EWS e web services no Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md). 
  
- Exchange Web Services API gerenciada de (EWS)
    
- EWS
    
    Se você estiver usando o EWS, você pode usar os seguintes métodos para recuperar as configurações do usuário:
    
  - O serviço Descoberta automática de baseados em SOAP
    
  - O serviço Descoberta automática de POX (XML)
    
  - Um proxy gerada automaticamente gerado a partir do serviço Descoberta automática de XML ou de SOAP
    
    Para obter mais informações sobre esses métodos, consulte [descoberta automática do Exchange](autodiscover-for-exchange.md).
    
A API gerenciada de EWS fornece uma interface baseada no objeto para recuperar as configurações do usuário. Se seu aplicativo cliente usa código gerenciado, é recomendável que você use a API gerenciada de EWS. A interface de API gerenciada de EWS melhor é otimizada para um modelo de objeto simples que o proxy do serviço web gerado automaticamente típica. 
  
Se você estiver usando o EWS, sugerimos que você use o serviço de descoberta automática de SOAP, porque ele oferece suporte a um conjunto avançado de recursos do serviço de descoberta automática de POX.
  
## <a name="prerequisites-for-finding-an-endpoint"></a>Pré-requisitos para localizar um ponto de extremidade
<a name="bk_Prereq"> </a>

Antes de criar um aplicativo cliente que usa o serviço de descoberta automática, você precisa ter acesso ao seguinte:
  
- O Exchange Online ou um servidor que está executando uma versão do Exchange, começando com o Exchange 2007 SP1. Se você estiver usando o serviço de descoberta automática de baseados em SOAP, o Exchange Online ou uma versão do Exchange, começando com o Exchange 2010.
    
- Um servidor do Exchange que está configurado para aceitar conexões de seu aplicativo cliente. Para obter informações sobre como configurar seu servidor do Exchange, consulte [controlar o acesso do aplicativo de cliente para o EWS no Exchange](controlling-client-application-access-to-ews-in-exchange.md).
    
- Uma conta que está autorizada a utilizar o EWS. Para obter informações sobre como configurar uma conta, consulte [controlar o acesso do aplicativo de cliente para o EWS no Exchange](controlling-client-application-access-to-ews-in-exchange.md).
    
> [!NOTE]
> Se você estiver usando a API gerenciada de EWS, você deve fornecer um retorno de chamada de validação de certificado em algumas circunstâncias. Talvez seja necessário também um retorno de chamada de validação de certificado com bibliotecas de proxy gerado, como aqueles criados pelo Visual Studio. Para obter mais informações, consulte [Validar um certificado de servidor para a API gerenciada de EWS](how-to-validate-a-server-certificate-for-the-ews-managed-api.md). 
  
### <a name="core-concepts-for-finding-an-endpoint"></a>Principais conceitos para localizar um ponto de extremidade
<a name="bk_Core"> </a>

Antes de você usar a descoberta automática para localizar um ponto de extremidade, você deve estar familiarizado com os conceitos listados na tabela a seguir.
  
|**Conceito**|**Descrição**|
|:-----|:-----|
|[Descoberta Automática do Exchange](autodiscover-for-exchange.md) <br/> |Fornece uma visão geral de como funciona o serviço de descoberta automática.  <br/> |
   
Se você estiver usando o EWS Managed API, use a classe [Microsoft.Exchange.WebServices.Data.ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) no namespace [Microsoft.Exchange.WebServices.Data](http://msdn.microsoft.com/en-us/library/dd633907%28v=exchg.80%29.aspx) para gerenciar sua conexão para o EWS. Para usar as amostras de código do API gerenciada de EWS neste artigo, você precisa fazer referência os seguintes namespaces em seu código: 
  
- **System.Net**
    
- **Microsoft.Exchange.WebServices.Data.ExchangeService**
    
## <a name="find-the-correct-endpoint-by-using-the-ews-managed-api"></a>Encontre o ponto de extremidade correto usando a API gerenciada de EWS
<a name="bk_Managed"> </a>

Se você estiver usando a API gerenciada de EWS, as chamadas para o serviço de descoberta automática são manipuladas pela classe **ExchangeService** . Para determinar o ponto de extremidade correto para uma conta de email, você pode chamar o método **AutodiscoverUrl** em um objeto **[ExchangeService]** . O exemplo de código a seguir mostra como definir o ponto de extremidade de serviço do EWS web para um endereço de email para o arquivo de Exchange.asmx no servidor de acesso para cliente correto usando a API gerenciada de EWS. 
  
```cs
NetworkCredential credentials = new NetworkCredential(securelyStoredEmail, securelyStoredPassword);
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2013);
service.Credentials = credentials;
service.AutodiscoverUrl("User1@contoso.com");
```

## <a name="find-the-correct-endpoint-by-using-ews"></a>Localizar o ponto de extremidade correto usando o EWS
<a name="bk_SOAP"> </a>

O serviço Descoberta automática do SOAP pode usar uma série de solicitações e respostas para direcionar o seu aplicativo para o ponto de extremidade correto para o EWS. Para obter informações sobre o processo para determinar o ponto de extremidade correto para uma conta de email, consulte [descoberta automática do Exchange](autodiscover-for-exchange.md). Os exemplos XML a seguir mostram a série de solicitações e respostas que você pode esperar quando você faz uma solicitação de descoberta automática do SOAP para localizar o ponto de extremidade correto.
  
### <a name="soap-autodiscover-endpoint-request"></a>Solicitação de ponto de extremidade de descoberta automática do SOAP

O exemplo a seguir mostra uma solicitação XML que será enviada para o serviço Descoberta automática para localizar o ponto de extremidade correto.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://mail.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
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

### <a name="soap-autodiscover-redirection-response"></a>Resposta de redirecionamento de descoberta automática do SOAP

O serviço Descoberta automática pode responder com uma das duas respostas de redirecionamento: um redirecionamento HTTP 302 ou uma resposta de redirecionamento de SOAP. Se a resposta do servidor Exchange for um redirecionamento HTTP 302, o aplicativo cliente deve validar que o endereço de redirecionamento é aceitável e siga a resposta de redirecionamento.
  
> [! Observação de segurança] para critérios para a validação de uma resposta de redirecionamento, consulte [descoberta automática do Exchange](autodiscover-for-exchange.md). 
  
Se o serviço de descoberta automática retorna uma resposta de redirecionamento, indicada pelo [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) do elemento de **resposta** , o aplicativo cliente deve usar o elemento **RedirectTarget** construir uma nova solicitação de configurações é enviado para o servidor especificado na resposta de redirecionamento. O exemplo a seguir mostra uma resposta de redirecionamento do servidor. 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>682</h:MajorBuildNumber>
      <h:MinorBuildNumber>1</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
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

Após um redirecionamento, o cliente usa a URL de redirecionamento para preparar a solicitação de outra. O código a seguir mostra um exemplo da solicitação que você cria com a resposta de redirecionamento.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
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

Quando o aplicativo cliente foi direcionado para o ponto de extremidade correto para o serviço de descoberta automática, o servidor enviará uma resposta com o [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) do elemento de **resposta** definido como **NoError** e contendo os solicitados configurações de usuário. Somente as usuário solicitado configurações, **InternalEwsUrl** e **ExternalEwsUrl**, são retornadas. O exemplo a seguir mostra a resposta do servidor. 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
        xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>160</h:MajorBuildNumber>
      <h:MinorBuildNumber>4</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
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

Localizar o ponto de extremidade seguindo o processo de descoberta automática retorna as configurações de usuário ou de domínio solicitado. Para obter informações sobre como fazer uma solicitação para configurações específicas, consulte os seguintes artigos:
  
- [Fazer configurações de domínio a partir de um servidor do Exchange](how-to-get-domain-settings-from-an-exchange-server.md)
    
- [Obter configurações de usuário do Exchange usando a descoberta automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
## <a name="see-also"></a>Confira também


- [Configurando seu aplicativo de EWS](setting-up-your-ews-application.md)
    
- [Descoberta Automática do Exchange](autodiscover-for-exchange.md)
    
- [Referência de web service de descoberta automática do Exchange](http://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)
    
- [Referência do EWS para Exchange](http://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)
    

