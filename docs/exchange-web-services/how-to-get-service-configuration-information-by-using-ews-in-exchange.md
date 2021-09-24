---
title: Obter informações de configuração de serviço usando o EWS no Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 9379740a-96e1-490d-a229-0f9937c548d2
description: Saiba como obter informações de configuração de serviço para UM, nudges de política, dicas de email e regras de proteção do EWS no Exchange.
ms.openlocfilehash: 30d4058104726c79f473a88a09398689675b988d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513168"
---
# <a name="get-service-configuration-information-by-using-ews-in-exchange"></a>Obter informações de configuração de serviço usando o EWS no Exchange

Saiba como obter informações de configuração de serviço para UM, nudges de política, dicas de email e regras de proteção do EWS no Exchange.
  
Seu aplicativo EWS funciona com Unificação de Mensagens (UM), nudges de política, dicas de email ou regras de proteção? Nesse caso, seu aplicativo precisará chamar a [operação GetServiceConfiguration](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) para obter as informações de configuração de serviço necessárias. A **operação GetServiceConfiguration** retorna informações de configuração específicas para cada um desses recursos EWS. 
  
> [!NOTE]
> A API gerenciada EWS não implementa essa funcionalidade. 
  
**Tabela 1. Informações de configuração que a operação GetServiceConfiguration retorna**

|Recurso EWS|A operação GetServiceConfiguration retorna...|
|:-----|:-----|
|UM  <br/> | <ul><li>Um valor que indica se a UM está habilitada.</li><li>Um valor que indica se a reprodução no telefone está habilitada.</li><li>A sequência de caracteres de discagem de telefone.</li></ul> |
|Nudges de política  <br/> | <ul><li>Nudges de política para exibição em seu cliente.</li></ul> |
|Dicas de email  <br/> | <ul><li>Um valor que indica se as dicas de email estão habilitadas.</li><li>O número máximo de destinatários por solicitação.</li><li>O tamanho máximo da mensagem.</li><li>O limite de audiência grande.</li><li>Um valor que indica se o número de destinatários externos é mostrado.</li><li>Uma lista de domínios internos.</li><li>Um valor que indica se as dicas de política estão habilitadas.</li><li>O limite de limite de audiência grande para indicar se seu email é considerado ter um grande número de destinatários.  </li></ul>|
|Regras de proteção  <br/> | <ul><li>Configuração de regras de proteção para seu cliente.</li><li>Uma lista de domínios internos à sua organização.  </li></ul> |
   
## <a name="code-example-get-service-configuration-information-for-mail-tips-by-using-ews"></a>Exemplo de código: obter informações de configuração de serviço para dicas de email usando o EWS

O exemplo de código a seguir usa a [operação GetServiceConfiguration](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) para solicitar informações de configuração de serviço para dicas de email. Você pode solicitar informações adicionais de configuração de serviço adicionando mais [elementos ConfigurationName](https://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) com valores diferentes. 
  
```cs
private static void GetServiceConfiguration(ExchangeService service, NetworkCredential creds)
{ 
  // XML for the GetServiceConfiguration request SOAP envelope for mail tips configuration information.
  const string getServiceConfigurationRequest = 
    "<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
    "<soap:Envelope xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\"\n" +
    "               xmlns:m=\"http://schemas.microsoft.com/exchange/services/2006/messages\"\n" +
    "               xmlns:t=\"http://schemas.microsoft.com/exchange/services/2006/types\" \n" +
    "               xmlns:soap=\"http://schemas.xmlsoap.org/soap/envelope/\"\n" +
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

Depois de solicitar informações de configuração de serviço, use a [classe XmlDocument](https://msdn.microsoft.com/library/system.xml.xmldocument.aspx) para carregar o XML de resposta para que você possa analisar. Em seguida, dependendo do cenário, você pode fazer um dos seguintes: 
  
- Use a [operação GetMailTips](https://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx) para obter dicas de email para aplicativos cliente para exibir aos usuários. 
    
- Se a UM estiver habilitada, [saiba como reproduzir itens de caixa](https://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) de correio em seu telefone. 
    
## <a name="see-also"></a>Confira também

- [Opções de configuração para EWS no Exchange](configuration-options-for-ews-in-exchange.md)    
- [Como configurar o aplicativo EWS](setting-up-your-ews-application.md)    
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)
    

