---
title: Fazer configurações de domínio a partir de um servidor do Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 2f9acb81-5135-4f72-94e8-65c235d725e6
description: Saiba como obter as configurações de domínio de um servidor do Exchange usando o serviço de descoberta automática.
ms.openlocfilehash: 0dd990cc82762936e7827115685ce0178eafb5ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750722"
---
# <a name="get-domain-settings-from-an-exchange-server"></a>Fazer configurações de domínio a partir de um servidor do Exchange

Saiba como obter as configurações de domínio de um servidor do Exchange usando o serviço de descoberta automática.
  
É possível recuperar informações de configuração de um domínio de email usando o serviço de descoberta automática. O serviço de descoberta automática fornece seu aplicativo com um processo para conexão com o ponto de extremidade de serviço corretos para um domínio específico.
  
Você pode usar uma das seguintes tecnologias de desenvolvimento para acessar o serviço de descoberta automática:
  
- Exchange Web Services API gerenciada de (EWS)
    
- EWS
    
    Se você estiver usando o EWS, você pode usar os seguintes métodos para recuperar as configurações do usuário:
    
  - O serviço Descoberta automática de baseados em SOAP
    
  - O serviço Descoberta automática de POX (XML)
    
  - Um proxy gerada automaticamente gerado a partir do serviço Descoberta automática de XML ou de SOAP
    
    Para obter mais informações sobre esses métodos, consulte [descoberta automática do Exchange](autodiscover-for-exchange.md).
    
A API gerenciada de EWS fornece uma interface baseada no objeto para recuperar as configurações do usuário. Se seu aplicativo cliente usa código gerenciado, é recomendável que você use a API gerenciada de EWS. A interface de API gerenciada de EWS melhor é otimizada para um modelo de objeto simples que o proxy do serviço web gerado automaticamente típica. 
  
Se você estiver usando o EWS, sugerimos que você use o serviço de descoberta automática de SOAP, porque ele oferece suporte a um conjunto avançado de recursos do serviço de descoberta automática de POX.
  
O serviço de descoberta automática retorna apenas as definições de configuração solicitada. A tabela a seguir lista as definições de configuração de domínio que o serviço Descoberta automática pode retornar.
  
**Tabela 1: Definições de configuração de domínio**

|**Definição de configuração**|**Descrição**|
|:-----|:-----|
|ExternalEwsUrl  <br/> |A URL externa para o EWS.  <br/> |
|ExternalEwsVersion  <br/> |A versão do Exchange server que hospeda a URL do EWS.  <br/> |
   
## <a name="prerequisites-for-getting-domain-settings"></a>Pré-requisitos para obter as configurações de domínio
<a name="bk_Prereq"> </a>

Antes de criar um aplicativo que se conecta ao serviço de descoberta automática para obter as configurações de domínio, certifique-se de que você tenha acesso ao seguinte:
  
- O Exchange Online, Exchange Online como parte do Office 365 ou um servidor executando uma versão do Exchange, começando com o Exchange 2007. Se você estiver usando o serviço de descoberta automática do EWS SOAP-based, um servidor executando uma versão do Exchange, começando com o Exchange 2010.
    
- Um servidor do Exchange que está configurado para aceitar conexões de seu aplicativo cliente. Para obter informações sobre como configurar seu servidor do Exchange, consulte [controlar o acesso do aplicativo de cliente para o EWS no Exchange](controlling-client-application-access-to-ews-in-exchange.md).
    
- Uma conta que está autorizada a utilizar o EWS. Para obter informações sobre como configurar uma conta, consulte [controlar o acesso do aplicativo de cliente para o EWS no Exchange](controlling-client-application-access-to-ews-in-exchange.md).
    
> [!NOTE]
> Se você estiver usando a API gerenciada de EWS, você deve fornecer um retorno de chamada de validação de certificado em algumas circunstâncias. Talvez seja necessário também um retorno de chamada de validação de certificado com bibliotecas de proxy gerado, como aqueles criados pelo Visual Studio. Para obter mais informações, consulte [Validar um certificado de servidor para a API gerenciada de EWS](how-to-validate-a-server-certificate-for-the-ews-managed-api.md). 
  
### <a name="core-concepts-for-getting-domain-settings"></a>Principais conceitos para obter as configurações de domínio
<a name="bk_Core"> </a>

Antes de você usar descoberta automática para obter as configurações de domínio, você deve estar familiarizado com os conceitos listados na tabela a seguir.
  
|**Conceito**|**Descrição**|
|:-----|:-----|
|[Descoberta Automática do Exchange](autodiscover-for-exchange.md) <br/> |Fornece uma visão geral de como funciona o serviço de descoberta automática.  <br/> |
|[Usar descoberta automática para encontrar os pontos de conexão](how-to-use-autodiscover-to-find-connection-points.md) <br/> |Descreve o processo usado pelo serviço de descoberta automática para redirecionar o aplicativo cliente para o ponto de extremidade de serviço corretos.  <br/> |
   
Se você estiver usando o EWS Managed API, use a classe [Microsoft.Exchange.WebServices.Data.ExchangeService](http://msdn.microsoft.com/en-us/library/exchange/dd635811%28v=exchg.80%29.aspx) no namespace [Microsoft.Exchange.WebServices.Data](http://msdn.microsoft.com/en-us/library/exchange/dd633907%28v=exchg.80%29.aspx) para gerenciar sua conexão para o EWS. Os exemplos de código nesta seção pressupõem que você faz referência os seguintes namespaces em seu código: 
  
- **System.Net**
    
- **Microsoft.Exchange.WebServices.Data.ExchangeService**
    
## <a name="get-domain-settings-by-using-the-ews-managed-api"></a>Obter configurações de domínio usando a API gerenciada de EWS
<a name="bk_Managed"> </a>

Se você estiver usando o EWS Managed API, você pode usar o método [Microsoft.Exchange.WebServices.Data.AutodiscoverSettings.GetUserSettings](http://msdn.microsoft.com/en-us/library/exchange/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) do objeto [Microsoft.Exchange.WebServices.Data.AutodiscoverService](http://msdn.microsoft.com/en-us/library/exchange/dd634321%28v=exchg.80%29.aspx) para gerar a solicitação que recupera informações de configuração para um domínio, conforme mostrado no exemplo a seguir. Neste exemplo, apenas algumas das configurações possíveis domínio solicitadas e apenas as configurações solicitadas são retornadas do servidor. 
  
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

Você pode analisar a coleção retornada para acessar cada par de chave/valor. O exemplo a seguir mostra como fazer o parse por meio de cada elemento retornado e exibir o nome e o valor de cada par de chave/valor.
  
```cs
// Display each retrieved value. The settings are part of a key/value pair.
foreach (KeyValuePair<DomainSettingName, Object> domainsetting in domainresponse.Settings)
{
    Console.WriteLine(domainsetting.Key.ToString() + ": " + domainsetting.Value.ToString());
}
```

Como alternativa, você pode obter o valor de uma configuração específica. No exemplo a seguir, a configuração de **ExternalEwsUrl** é a ser exibido. 
  
```cs
// Display a specific setting, such as ExternalEwsUrl.
Console.WriteLine(domainresponse.Settings[DomainSettingName.ExternalEwsUrl]);
```

## <a name="get-user-settings-by-using-ews-soap-autodiscover"></a>Obter configurações de usuário usando a descoberta automática do EWS SOAP
<a name="bk_SOAP"> </a>

O exemplo a seguir mostra uma solicitação SOAP XML para obter as duas configurações de domínio do serviço de descoberta automática.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetDomainSettings</wsa:Action>
    <wsa:To>https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetDomainSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
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

O exemplo a seguir mostra a resposta XML retornada pelo servidor após ele analisa a solicitação do cliente.
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
        xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/
          Autodiscover/Autodiscover/GetDomainSettingsResponse</a:Action>
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
    <GetDomainSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
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

Configurações de domínio fornecem as informações básicas que seu cliente precisa para se conectar ao EWS. Você pode usar essas informações para se conectar ao EWS ou é possível recuperar as definições de configuração adicionais para uma conta de email do servidor. Para obter mais informações, consulte o artigo a seguir:
  
- [Obter configurações de usuário do Exchange usando a descoberta automática](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
## <a name="see-also"></a>Confira também


- [Configurando seu aplicativo de EWS](setting-up-your-ews-application.md)
    
- [Referência de web service de descoberta automática do Exchange](http://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)
    
- [Referência do EWS para Exchange](http://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)
    

