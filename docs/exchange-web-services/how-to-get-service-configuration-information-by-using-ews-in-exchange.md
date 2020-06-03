---
title: Obter informações de configuração de serviço usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9379740a-96e1-490d-a229-0f9937c548d2
description: Descubra como obter informações de configuração de serviço para UM, deslocamentos de política, dicas de email e regras de proteção do EWS no Exchange.
ms.openlocfilehash: 7546d9524f1e004eda2bdc55687fb44beafa44af
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528003"
---
# <a name="get-service-configuration-information-by-using-ews-in-exchange"></a>Obter informações de configuração de serviço usando o EWS no Exchange

Descubra como obter informações de configuração de serviço para UM, deslocamentos de política, dicas de email e regras de proteção do EWS no Exchange.
  
O aplicativo EWS funciona com a Unificação de mensagens (UM), os deslocamentos de política, as dicas de email ou as regras de proteção? Em caso afirmativo, o aplicativo precisará chamar a [operação GetServiceConfiguration](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) para obter as informações de configuração de serviço de que precisa. A operação **GetServiceConfiguration** retorna as informações de configuração específicas de cada um desses recursos do EWS. 
  
> [!NOTE]
> A API gerenciada EWS não implementa essa funcionalidade. 
  
**Tabela 1. Informações de configuração que a operação GetServiceConfiguration retorna**

|Recurso EWS|A operação GetServiceConfiguration retorna...|
|:-----|:-----|
|UM  <br/> | <ul><li>Um valor que indica se a UM está habilitada.</li><li>Um valor que indica se tocar no telefone está habilitado.</li><li>A cadeia de caracteres de discagem por telefone.</li></ul> |
|Deslocamentos de política  <br/> | <ul><li>Os deslocamentos de política para exibição no cliente.</li></ul> |
|Dicas de email  <br/> | <ul><li>Um valor que indica se as dicas de email estão habilitadas.</li><li>O número máximo de destinatários por solicitação.</li><li>O tamanho máximo da mensagem.</li><li>O limite grande de audiências.</li><li>Um valor que indica se o número de destinatários externos é mostrado.</li><li>Uma lista de domínios internos.</li><li>Um valor que indica se as dicas de política estão habilitadas.</li><li>O limite de grandes audiências para indicar se o email é considerado como tendo um grande número de destinatários.  </li></ul>|
|Regras de proteção  <br/> | <ul><li>Configuração de regras de proteção para o cliente.</li><li>Uma lista de domínios internos da sua organização.  </li></ul> |
   
## <a name="code-example-get-service-configuration-information-for-mail-tips-by-using-ews"></a>Exemplo de código: obter informações de configuração de serviço para dicas de email usando o EWS

O exemplo de código a seguir usa a [operação GetServiceConfiguration](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) para solicitar informações de configuração de serviço para dicas de email. Você pode solicitar informações adicionais de configuração de serviço adicionando mais elementos [ConfigurationName](https://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) com valores diferentes. 
  
```cs
private static void GetServiceConfiguration(ExchangeService service, NetworkCredential creds)
{ 
  // XML for the GetServiceConfiguration request SOAP envelope for mail tips configuration information.
  const string getServiceConfigurationRequest = 
    "<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
    "<soap:Envelope xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\"\n" +
    "               xmlns:m=\"https://schemas.microsoft.com/exchange/services/2006/messages\"\n" +
    "               xmlns:t=\"https://schemas.microsoft.com/exchange/services/2006/types\" \n" +
    "               xmlns:soap=\"https://schemas.xmlsoap.org/soap/envelope/\"\n" +
    "               xmlns:xs=\"http://www.w3.org/2001/XMLSchema\">\n" +
    "  <soap:Header>\n" +
    "    <t:RequestServerVersion Version=\"Exchange2013\" />\n" +
    "  </soap:Header>\n" +
    "  <soap:Body>\n" +
    "    <m:GetServiceConfiguration>\n" +
    "      <m:ActingAs>\n" +
    "        <t:EmailAddress>user1@contoso.com</t:EmailAddress>\n" +
    "        <t:RoutingType>SMTP</t:RoutingType>\n" +
    "      </m:ActingAs>\n" +
    "      <m:RequestedConfiguration>\n" +
    "        <m:ConfigurationName>MailTips</m:ConfigurationName>\n" +
    "      </m:RequestedConfiguration>\n" +
    "    </m:GetServiceConfiguration>\n" +
    "  </soap:Body>\n" +
    "</soap:Envelope>";
  // Encoded GetServiceConfiguration operation request.
  byte[] payload = System.Text.Encoding.UTF8.GetBytes(getServiceConfigurationRequest);
  try
  {
    HttpWebRequest request = (HttpWebRequest)WebRequest.Create(service.Url);
    request.AllowAutoRedirect = false;
    request.Credentials = creds;
    request.Method = "POST";
    request.ContentType = "text/xml";
    Stream requestStream = request.GetRequestStream();
    requestStream.Write(payload, 0, payload.Length);
    requestStream.Close();
    HttpWebResponse response = (HttpWebResponse)request.GetResponse();
    if (response.StatusCode == HttpStatusCode.OK)
    {
      Stream responseStream = response.GetResponseStream();
      StreamReader reader = new StreamReader(responseStream);
      string responseFromServer = reader.ReadToEnd();
      Console.WriteLine("You will need to parse this response to get the configuration information:\n\n" + responseFromServer);
      reader.Close();
      responseStream.Close();
    }
    else
      throw new WebException(response.StatusDescription);
          
  }
  catch (WebException e)
  {
    Console.WriteLine(e.Message);
  }
}

```

## <a name="next-steps"></a>Próximas etapas

Depois de solicitar informações de configuração de serviço, use a [classe XmlDocument](https://msdn.microsoft.com/library/system.xml.xmldocument.aspx) para carregar o XML de resposta para que você possa analisá-lo. Em seguida, dependendo do seu cenário, você pode executar uma das seguintes ações: 
  
- Use a [operação](https://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx) GetQuery para obter dicas de email para aplicativos cliente exibir aos usuários. 
    
- Se a UM estiver habilitada, [saiba mais sobre como reproduzir itens de caixa de correio](https://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) pelo telefone. 
    
## <a name="see-also"></a>Confira também

- [Opções de configuração do EWS no Exchange](configuration-options-for-ews-in-exchange.md)    
- [Configurando o aplicativo EWS](setting-up-your-ews-application.md)    
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    

