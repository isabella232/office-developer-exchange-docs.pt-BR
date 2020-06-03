---
title: Obter as configurações de domínio de um servidor do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 2f9acb81-5135-4f72-94e8-65c235d725e6
description: Saiba como obter as configurações de domínio de um servidor Exchange usando o serviço de descoberta automática.
localization_priority: Priority
ms.openlocfilehash: e77810089b77f614f6bca064b2e5cf6bde2bff7c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455804"
---
# <a name="get-domain-settings-from-an-exchange-server"></a>Obter as configurações de domínio de um servidor do Exchange

Saiba como obter as configurações de domínio de um servidor Exchange usando o serviço de descoberta automática.
  
Você pode recuperar as informações de configuração de um domínio de email usando o serviço de descoberta automática. O serviço de descoberta automática fornece ao seu aplicativo um processo de conexão com o ponto de extremidade de serviço correto para um domínio específico.
  
Você pode usar uma das seguintes tecnologias de desenvolvimento para acessar o serviço de descoberta automática:
  
- A API gerenciada dos serviços Web do Exchange (EWS)
    
- EWS
    
    Se estiver usando o EWS, você poderá usar os seguintes métodos para recuperar as configurações do usuário:
    
  - O serviço de descoberta automática baseado em SOAP
    
  - O serviço de descoberta automática de XML (POX)
    
  - Um proxy gerado automaticamente a partir do serviço de descoberta automática SOAP ou XML
    
    Para obter mais informações sobre esses métodos, consulte [autodiscover for Exchange](autodiscover-for-exchange.md).
    
A API gerenciada do EWS fornece uma interface baseada em objeto para recuperar as configurações do usuário. Se seu aplicativo cliente usa código gerenciado, recomendamos que você use a API gerenciada do EWS. A interface de API gerenciada do EWS é melhor otimizada para um modelo de objeto simples do que o proxy de serviço Web do autogerable típico. 
  
Se você estiver usando o EWS, sugerimos que você use o serviço de descoberta automática do SOAP, pois ele oferece suporte a um conjunto mais amplo de recursos do que o serviço de descoberta automática do POX.
  
O serviço de descoberta automática retorna apenas as definições de configuração solicitadas. A tabela a seguir lista as definições de configuração de domínio que o serviço de descoberta automática pode retornar.
  
**Tabela 1: definições de configuração de domínio**

|**Definição de configuração**|**Descrição**|
|:-----|:-----|
|ExternalEwsUrl  <br/> |A URL externa do EWS.  <br/> |
|ExternalEwsVersion  <br/> |A versão do servidor Exchange que hospeda a URL do EWS.  <br/> |
   
## <a name="prerequisites-for-getting-domain-settings"></a>Pré-requisitos para obter configurações de domínio
<a name="bk_Prereq"> </a>

Antes de criar um aplicativo que se conecta ao serviço de descoberta automática para obter as configurações de domínio, certifique-se de que você tem acesso ao seguinte:
  
- Exchange Online, Exchange Online como parte do Office 365 ou um servidor executando uma versão do Exchange a partir do Exchange 2007. Se você estiver usando o serviço de descoberta automática baseado em SOAP do EWS, um servidor executando uma versão do Exchange a partir do Exchange 2010.
    
- Um servidor do Exchange que é configurado para aceitar conexões do seu aplicativo cliente. Para obter informações sobre como configurar seu servidor Exchange, consulte [controle de acesso de aplicativo cliente ao EWS no Exchange](controlling-client-application-access-to-ews-in-exchange.md).
    
- Uma conta que está autorizada a usar o EWS. Para obter informações sobre como configurar uma conta, consulte [controle de acesso de aplicativo cliente ao EWS no Exchange](controlling-client-application-access-to-ews-in-exchange.md).
    
> [!NOTE]
> Se você estiver usando a API gerenciada do EWS, deverá fornecer um retorno de chamada de validação de certificado em algumas circunstâncias. Você também pode precisar de um retorno de chamada de validação de certificado com algumas bibliotecas de proxy geradas, como as criadas pelo Visual Studio. Para saber mais, confira [validar um certificado de servidor para a API gerenciada do EWS](how-to-validate-a-server-certificate-for-the-ews-managed-api.md). 
  
### <a name="core-concepts-for-getting-domain-settings"></a>Principais conceitos para obter configurações de domínio
<a name="bk_Core"> </a>

Antes de usar a descoberta automática para obter as configurações de domínio, você deve estar familiarizado com os conceitos listados na tabela a seguir.
  
|**Conceito**|**Descrição**|
|:-----|:-----|
|[Descoberta Automática do Exchange](autodiscover-for-exchange.md) <br/> |Fornece uma visão geral de como o serviço de descoberta automática funciona.  <br/> |
|[Usar a Descoberta Automática para localizar os pontos de conexão](how-to-use-autodiscover-to-find-connection-points.md) <br/> |Descreve o processo usado pelo serviço de descoberta automática para redirecionar seu aplicativo cliente para o ponto de extremidade de serviço correto.  <br/> |
   
Se você estiver usando a API gerenciada do EWS, use a classe [Microsoft. Exchange. WebServices. Data. ExchangeService](https://msdn.microsoft.com/library/exchange/dd635811%28v=exchg.80%29.aspx) no namespace [Microsoft. Exchange. WebServices. Data](https://msdn.microsoft.com/library/exchange/dd633907%28v=exchg.80%29.aspx) para gerenciar sua conexão com o EWS. Os exemplos de código nesta seção supõem que você faça referência aos seguintes namespaces no seu código: 
  
- **System.Net**
    
- **Microsoft. Exchange. WebServices. Data. ExchangeService**
    
## <a name="get-domain-settings-by-using-the-ews-managed-api"></a>Obter configurações de domínio usando a API gerenciada do EWS
<a name="bk_Managed"> </a>

Se estiver usando a API gerenciada do EWS, você poderá usar o método [Microsoft. Exchange. WebServices. Data. AutodiscoverSettings. GetUserSettings](https://msdn.microsoft.com/library/exchange/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) do objeto [Microsoft. Exchange. WebServices. Data. AutodiscoverService](https://msdn.microsoft.com/library/exchange/dd634321%28v=exchg.80%29.aspx) para gerar a solicitação que recupera as informações de configuração de um domínio, conforme mostrado no exemplo a seguir. Neste exemplo, apenas algumas das configurações de domínio possíveis são solicitadas e apenas as configurações solicitadas são retornadas do servidor. 
  
```cs
AutodiscoverService autodiscoverService = new AutodiscoverService("domain.contoso.com");
autodiscoverService.Credentials = new NetworkCredential("User1", "password", "domain.contoso.com");
// Submit a request and get the settings. The response contains only the
// settings that are requested, if they exist.
GetDomainSettingsResponse domainresponse = autodiscoverService.GetDomainSettings(
    "domain",
    ExchangeVersion.Exchang2013,
    DomainSettingName.ExternalEwsUrl,
    DomainSettingName.ExternalEwsVersion);
```

Você pode analisar a coleção retornada para acessar cada par chave/valor. O exemplo a seguir mostra como analisar cada elemento retornado e exibir o nome e o valor de cada par chave/valor.
  
```cs
// Display each retrieved value. The settings are part of a key/value pair.
foreach (KeyValuePair<DomainSettingName, Object> domainsetting in domainresponse.Settings)
{
    Console.WriteLine(domainsetting.Key.ToString() + ": " + domainsetting.Value.ToString());
}
```

Como alternativa, você pode obter o valor de uma configuração específica. No exemplo a seguir, a configuração **ExternalEwsUrl** deve ser exibida. 
  
```cs
// Display a specific setting, such as ExternalEwsUrl.
Console.WriteLine(domainresponse.Settings[DomainSettingName.ExternalEwsUrl]);
```

## <a name="get-user-settings-by-using-ews-soap-autodiscover"></a>Obter configurações de usuário usando a descoberta automática do EWS SOAP
<a name="bk_SOAP"> </a>

O exemplo a seguir mostra uma solicitação XML do SOAP para obter as configurações de domínio do serviço de descoberta automática.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetDomainSettings</wsa:Action>
    <wsa:To>https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetDomainSettingsRequestMessage xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Domains>
          <a:Domain>domain</a:Domain>
        </a:Domains>
        <a:RequestedSettings>
          <a:Setting>ExternalEwsUrl</a:Setting>
          <a:Setting>ExternalEwsVersion</a:Setting>
        </a:RequestedSettings>
        <a:RequestedVersion>Exchange2013</a:RequestedVersion>
      </a:Request>
    </a:GetDomainSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>
```

O exemplo a seguir mostra a resposta XML retornada pelo servidor após a análise da solicitação do cliente.
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/" 
        xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">https://schemas.microsoft.com/exchange/2010/
          Autodiscover/Autodiscover/GetDomainSettingsResponse</a:Action>
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
    <GetDomainSettingsResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <DomainResponses>
          <DomainResponse>
            <ErrorCode>NoError</ErrorCode>
            <ErrorMessage>No error.</ErrorMessage>
            <DomainSettingErrors />
            <DomainSettings>
              <DomainSetting i:type="DomainStringSetting">
                <Name>ExternalEwsUrl</Name>
                <Value>https://failover.exchange.microsoft.com/ews/exchange.asmx</Value>
              </DomainSetting>
              <DomainSetting i:type="DomainStringSetting">
                <Name>ExternalEwsVersion</Name>
                <Value>15.00.0085.000</Value>
              </DomainSetting>
            </DomainSettings>
            <RedirectTarget i:nil="true" />
          </DomainResponse>
        </DomainResponses>
      </Response>
    </GetDomainSettingsResponseMessage>
  </s:Body>
</s:Envelope>
```

## <a name="next-steps"></a>Próximas etapas
<a name="bk_Next"> </a>

As configurações de domínio fornecem as informações básicas que o cliente precisa para se conectar ao EWS. Você pode usar essas informações para se conectar ao EWS ou pode recuperar definições de configuração adicionais de uma conta de email do servidor. Para obter mais informações, consulte o seguinte artigo:
  
- [Obter as configurações de usuário do Exchange usando a Descoberta Automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
## <a name="see-also"></a>Confira também


- [Configurando o aplicativo EWS](setting-up-your-ews-application.md)
    
- [Referência do serviço Web de descoberta automática do Exchange](https://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)
    
- [Referência do EWS para Exchange](https://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)
    

