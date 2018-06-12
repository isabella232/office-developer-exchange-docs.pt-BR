---
title: Introdução aos aplicativos de cliente do EWS
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: e6fd5c23-0ba5-4a7b-bdde-4a553447069f
description: Crie seu primeiro aplicativo usando os serviços Web do Exchange (EWS) no Exchange.
ms.openlocfilehash: 911495c74f4c74114a86b1a3a98c9200db338b34
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19750675"
---
# <a name="get-started-with-ews-client-applications"></a>Introdução aos aplicativos de cliente do EWS

Crie seu primeiro aplicativo usando os serviços Web do Exchange (EWS) no Exchange.
  
EWS é um serviço abrangente que seus aplicativos podem usar para acessar quase todas as informações armazenadas em um Exchange Online, Exchange Online como parte do Office 365, ou Exchange da caixa de correio local. EWS usa protocolos padrão da web para fornecer acesso a um servidor do Exchange; bibliotecas como a [API gerenciada de EWS](get-started-with-ews-managed-api-client-applications.md) quebrar as operações de EWS para fornecer uma interface orientado a objetos. Depois de executar os exemplos neste artigo, você terá uma noção básica do que você pode fazer com o EWS. 
  
É possível chamar operações EWS em qualquer sistema operacional ou idioma, como as solicitações do EWS e respostas utilizam o protocolo SOAP. Os exemplos neste artigo são gravados usando c# e fazer uso do .NET Framework objetos [HttpWebRequest](https://msdn.microsoft.com/library/System.Net.HttpWebRequest.aspx) e [HttpWebResponse](https://msdn.microsoft.com/library/System.Net.HttpWebResponse.aspx) ; No entanto, a parte importante do código é o XML usado para fazer com que a solicitação do EWS e a resposta XML retornada do servidor. Os exemplos de código enfatizam as transações de XML e não o XML de processamento. 
  
## <a name="youll-need-an-exchange-server"></a>Você precisará de um servidor do Exchange

Se você já tiver uma conta de caixa de correio do Exchange, você poderá ignorar esta etapa. Caso contrário, você tem as seguintes opções para configurar uma caixa de correio do Exchange para seu primeiro aplicativo EWS:
  
- [Obtenha um Site do Office 365 Developer](http://msdn.microsoft.com/en-us/library/office/fp179924.aspx) (recomendado). Esta é a maneira mais rápida de obter uma caixa de correio do Exchange.
    
- Baixe o [Exchange Server](http://office.microsoft.com/en-us/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).
    
Depois de confirmar que você pode enviar e receber emails do Exchange Server, você estará pronto para configurar seu ambiente de desenvolvimento. Você pode usar o Outlook Web App para verificar se você pode enviar o email.
  
Você também precisará saber a URL do ponto de extremidade EWS para seu servidor. Em um aplicativo de produção, você usaria [descoberta automática](autodiscover-for-exchange.md) para determinar a URL do EWS. Os exemplos neste artigo usam a URL de ponto de extremidade do Office 365 EWS, https://outlook.office365.com/EWS/Exchange.asmx. A seção [próximas etapas](#bk_next) tem links para obter mais informações sobre a descoberta automática, quando estiver pronto. 
  
Se você estiver testando seu aplicativo usando um servidor do Exchange que tem o certificado autoassinado do padrão, você precisará criar um [método de validação do certificado](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) que atenda aos requisitos de segurança da sua organização. 
  
## <a name="set-up-your-development-environment"></a>Definir seu ambiente de desenvolvimento

As ferramentas que você usa para criar seu primeiro aplicativo EWS dependem do sistema operacional e o idioma que você use e é principalmente uma questão de preferência. Se você quiser acompanhe os exemplos em c# neste artigo, você precisará: 
  
- Qualquer versão do Visual Studio que suporta o .NET Framework 4.0. 
    
- Uma conexão de Internet que sua máquina de desenvolvimento pode usar para contatar o servidor do Exchange. Se você pode usar o Outlook Web App com um nome DNS em vez de um endereço IP para se conectar ao seu servidor do Exchange, você estiver configurado.
    
## <a name="create-your-first-ews-application"></a>Crie seu primeiro aplicativo de EWS

Os aplicativos do EWS que você irá criar mostra dois cenários típicos de usando o EWS:
  
1. Obtenha informações de uma caixa de correio do Exchange e exibir essas informações ao usuário.
    
2. Executar uma ação, por exemplo, enviar um email e verifique a resposta para ver se a ação foi bem-sucedida.
    
Vamos começar.
  
### <a name="set-up-the-solution"></a>Configurar a solução

Primeiro, crie uma nova solução de aplicativo de console usando o Visual Studio. Quando a solução estiver pronta, crie um novo objeto chamado Tracing.cs. Use este objeto para gravar informações sobre o console e um arquivo de log para que você possa examinar os resultados após a execução do seu código. Cole o código a seguir no arquivo Tracing.cs.
  
```cs
using System;
using System.IO;
namespace Microsoft.Exchange.Samples.EWS
{
  class Tracing
  {
    private static TextWriter logFileWriter = null;
    public static void OpenLog(string fileName)
    {
      logFileWriter = new StreamWriter(fileName);
    }
    public static void Write(string format, params object[] args)
    {
      Console.Write(format, args);
      if (logFileWriter != null)
      {
        logFileWriter.Write(format, args);
      }
    }
    public static void WriteLine(string format, params object[] args)
    {
      Console.WriteLine(format, args);
      if (logFileWriter != null)
      {
        logFileWriter.WriteLine(format, args);
      }
    }
    public static void CloseLog()
    {
      logFileWriter.Flush();
      logFileWriter.Close();
    }
  }
}
```

Em seguida, abra o arquivo de Module. vb. Você colocará o restante do código para o exemplo neste arquivo.
  
Primeiro, configure o shell do programa. O programa será: 
  
1. Crie um arquivo de log para que a solicitação e a resposta podem ser gravados em disco para estudo posterior.
    
2. Obtenha o endereço de email e a senha da conta que você acessará.
    
3. Chame os métodos de amostra.
    
Substituir o `Main` método no Module. vb com o código a seguir. 
  
```cs
    static void Main(string[] args)
    {
      // Start tracing to console and a log file.
      Tracing.OpenLog("./GetStartedWithEWS.log");
      Tracing.WriteLine("EWS sample application started.");
      var isValidEmailAddress = false;
      Console.Write("Enter an email address: ");
      var emailAddress = Console.ReadLine();
      
        isValidEmailAddress = (emailAddress.Contains("@") &amp;&amp; emailAddress.Contains("."));
      if (!isValidEmailAddress)
      {
        Tracing.WriteLine("Email address " + emailAddress + " is not a valid SMTP address. Closing program.");
        return;
      }
      SecureString password = GetPasswordFromConsole();
      if (password.Length == 0)
      {
        Tracing.WriteLine("Password empty, closing program.");
      }
      NetworkCredential userCredentials = new NetworkCredential(emailAddress, password);
      // These are the sample methods that demonstrate using EWS.
      // ShowNumberOfMessagesInInbox(userCredentials);
      // SendTestEmail(userCredentials);
     
      Tracing.WriteLine("EWS sample application ends.");
      Tracing.CloseLog();
      Console.WriteLine("Press enter to exit: ");
      Console.ReadLine();
    }
    // These method stubs will be filled in later.
    private static void ShowNumberOfMessagesInInbox(NetworkCredential userCredentials)
    {
    }
    private static void SendTestEmail(NetworkCredential userCredentials)
    {
    }
```

A última coisa que você precisa fazer é adicionar o `GetPasswordFromConsole` método estático. Esse método retorna um objeto de [SecureString](https://msdn.microsoft.com/library/System.Security.SecureString.aspx) que contém uma senha digitada no console. 
  
```cs
    private static SecureString GetPasswordFromConsole()
    {
      SecureString password = new SecureString();
      bool readingPassword = true;
      Console.Write("Enter password: ");
      while (readingPassword)
      {
        ConsoleKeyInfo userInput = Console.ReadKey(true);
        switch (userInput.Key)
        {
          case (ConsoleKey.Enter):
            readingPassword = false;
            break;
          case (ConsoleKey.Escape):
            password.Clear();
            readingPassword = false;
            break;
          case (ConsoleKey.Backspace):
            if (password.Length > 0)
            {
              password.RemoveAt(password.Length - 1);
              Console.SetCursorPosition(Console.CursorLeft - 1, Console.CursorTop);
              Console.Write(" ");
              Console.SetCursorPosition(Console.CursorLeft - 1, Console.CursorTop);
            }
            break;
          default:
            if (userInput.KeyChar != 0)
            {
              password.AppendChar(userInput.KeyChar);
              Console.Write("*");
            }
            break;
        }
      }
      Console.WriteLine();
      password.MakeReadOnly();
      return password;
    }
```

### <a name="get-the-number-of-new-messages-in-an-inbox"></a>Obter o número de novas mensagens em uma caixa de entrada

Uma operação comum em um aplicativo do EWS é obter informações sobre mensagens de email, compromissos, reuniões e as pastas que armazenam-los. Este exemplo obtém o número de mensagens na caixa de entrada da conta e exibe o número total de mensagens e o número de mensagens não lidas. Demonstra as seguintes ações comuns para aplicativos do EWS:
  
- Fazendo uma solicitação EWS para o Exchange server.
    
- Analisando a resposta XML retornada para as informações solicitadas.
    
- Lidando com as exceções comuns e mensagens de erro.
    
Adicione o seguinte código para o `ShowNumberOfMessagesInInbox` método que foi oculto após o método principal. Quando você executa o aplicativo, ele será impresso o número de mensagens na caixa de entrada da conta e o número de mensagens não lidas na caixa de entrada. Depois de executar o aplicativo, você pode abrir o arquivo GetStartedWithEWS.log para ver a solicitação XML que foi enviada para o Exchange server e a resposta que o servidor é retornado. 
  
```cs
      /// This is the XML request that is sent to the Exchange server.
      var getFolderSOAPRequest =
"<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
"<soap:Envelope xmlns:soap=\"http://schemas.xmlsoap.org/soap/envelope/\"\n" +
"   xmlns:t=\"http://schemas.microsoft.com/exchange/services/2006/types\">\n" +
"<soap:Header>\n" +
"    <t:RequestServerVersion Version=\"Exchange2007_SP1\" />\n" +
"  </soap:Header>\n" +
"  <soap:Body>\n" +
"    <GetFolder xmlns=\"http://schemas.microsoft.com/exchange/services/2006/messages\"\n" +
"               xmlns:t=\"http://schemas.microsoft.com/exchange/services/2006/types\">\n" +
"      <FolderShape>\n" +
"        <t:BaseShape>Default</t:BaseShape>\n" +
"      </FolderShape>\n" +
"      <FolderIds>\n" +
"        <t:DistinguishedFolderId Id=\"inbox\"/>\n" +
"      </FolderIds>\n" +
"    </GetFolder>\n" +
"  </soap:Body>\n" +
"</soap:Envelope>\n";
      // Write the get folder operation request to the console and log file.
      Tracing.WriteLine("Get folder operation request:");
      Tracing.WriteLine(getFolderSOAPRequest);
      var getFolderRequest = WebRequest.CreateHttp(Office365WebServicesURL);
      getFolderRequest.AllowAutoRedirect = false;
      getFolderRequest.Credentials = userCredentials;
      getFolderRequest.Method = "POST";
      getFolderRequest.ContentType = "text/xml";
      var requestWriter = new StreamWriter(getFolderRequest.GetRequestStream());
      requestWriter.Write(getFolderSOAPRequest);
      requestWriter.Close();
      try
      {
        var getFolderResponse = (HttpWebResponse)(getFolderRequest.GetResponse());
        if (getFolderResponse.StatusCode == HttpStatusCode.OK)
        {
          var responseStream = getFolderResponse.GetResponseStream();
          XElement responseEnvelope = XElement.Load(responseStream);
          if (responseEnvelope != null)
          {
            // Write the response to the console and log file.
            Tracing.WriteLine("Response:");
            StringBuilder stringBuilder = new StringBuilder();
            XmlWriterSettings settings = new XmlWriterSettings();
            settings.Indent = true;
            XmlWriter writer = XmlWriter.Create(stringBuilder, settings);
            responseEnvelope.Save(writer);
            writer.Close();
            Tracing.WriteLine(stringBuilder.ToString());
            // Check the response for error codes. If there is an error, throw an application exception.
            IEnumerable<XElement> errorCodes = from errorCode in responseEnvelope.Descendants
                                               ("{http://schemas.microsoft.com/exchange/services/2006/messages}ResponseCode")
                                               select errorCode;
            foreach (var errorCode in errorCodes)
            {
              if (errorCode.Value != "NoError")
              {
                switch (errorCode.Parent.Name.LocalName.ToString())
                {
                  case "Response":
                    string responseError = "Response-level error getting inbox information:\n" + errorCode.Value;
                    throw new ApplicationException(responseError);
                  case "UserResponse":
                    string userError = "User-level error getting inbox information:\n" + errorCode.Value;
                    throw new ApplicationException(userError);
                }
              }
            }
            // Process the response.
            IEnumerable<XElement> folders = from folderElement in
                                              responseEnvelope.Descendants
                                              ("{http://schemas.microsoft.com/exchange/services/2006/messages}Folders")
                                            select folderElement;
            foreach (var folder in folders)
            {
              Tracing.Write("Folder name:     ");
              var folderName = from folderElement in
                                 folder.Descendants
                                 ("{http://schemas.microsoft.com/exchange/services/2006/types}DisplayName")
                               select folderElement.Value;
              Tracing.WriteLine(folderName.ElementAt(0));
              Tracing.Write("Total messages:  ");
              var totalCount = from folderElement in
                                 folder.Descendants
                                   ("{http://schemas.microsoft.com/exchange/services/2006/types}TotalCount")
                               select folderElement.Value;
              Tracing.WriteLine(totalCount.ElementAt(0));
              Tracing.Write("Unread messages: ");
              var unreadCount = from folderElement in
                                 folder.Descendants
                                   ("{http://schemas.microsoft.com/exchange/services/2006/types}UnreadCount")
                               select folderElement.Value;
              Tracing.WriteLine(unreadCount.ElementAt(0));
            }
          }
        }
      }
      catch (WebException ex)
      {
        Tracing.WriteLine("Caught Web exception:");
        Tracing.WriteLine(ex.Message);
      }
      catch (ApplicationException ex)
      {
        Tracing.WriteLine("Caught application exception:");
        Tracing.WriteLine(ex.Message);
      }

```

### <a name="send-an-email-message"></a>Enviar uma mensagem de email

Outra operação comum para um aplicativo do EWS deve enviar mensagens de email ou solicitações de reunião. Este exemplo cria e envia uma mensagem de email usando as credenciais de usuário que foram inseridas anteriormente. Demonstra essas tarefas comuns de aplicativos do EWS:
  
- Criando e enviando um email.
    
- Analisando a resposta XML retornada para determinar se o email foi enviado corretamente.
    
- Lidando com as exceções comuns e mensagens de erro.
    
Adicione o seguinte código para o método SendTestEmail que foi oculto após o método principal. Depois de executar o aplicativo, você pode abrir o arquivo GetStartedWithEWS.log para ver a solicitação XML que foi enviada para o Exchange server e a resposta que o servidor é retornado.
  
```cs
var createItemSOAPRequest =
      "<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
      "<soap:Envelope xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\" \n" +
      "               xmlns:m=\"http://schemas.microsoft.com/exchange/services/2006/messages\" \n" +
      "               xmlns:t=\"http://schemas.microsoft.com/exchange/services/2006/types\" \n" +
      "               xmlns:soap=\"http://schemas.xmlsoap.org/soap/envelope/\">\n" +
      "  <soap:Header>\n" +
      "    <t:RequestServerVersion Version=\"Exchange2007_SP1\" />\n" +
      "  </soap:Header>\n" +
      "  <soap:Body>\n" +
      "    <m:CreateItem MessageDisposition=\"SendAndSaveCopy\">\n" +
      "      <m:SavedItemFolderId>\n" +
      "        <t:DistinguishedFolderId Id=\"sentitems\" />\n" +
      "      </m:SavedItemFolderId>\n" +
      "      <m:Items>\n" +
      "        <t:Message>\n" +
      "          <t:Subject>Company Soccer Team</t:Subject>\n" +
      "          <t:Body BodyType=\"HTML\">Are you interested in joining?</t:Body>\n" +
      "          <t:ToRecipients>\n" +
      "            <t:Mailbox>\n" +
      "              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>\n" +
      "              </t:Mailbox>\n" +
      "          </t:ToRecipients>\n" +
      "        </t:Message>\n" +
      "      </m:Items>\n" +
      "    </m:CreateItem>\n" +
      "  </soap:Body>\n" +
      "</soap:Envelope>\n";
      // Write the create item operation request to the console and log file.
      Tracing.WriteLine("Get folder operation request:");
      Tracing.WriteLine(createItemSOAPRequest);
      var getFolderRequest = WebRequest.CreateHttp(Office365WebServicesURL);
      getFolderRequest.AllowAutoRedirect = false;
      getFolderRequest.Credentials = userCredentials;
      getFolderRequest.Method = "POST";
      getFolderRequest.ContentType = "text/xml";
      var requestWriter = new StreamWriter(getFolderRequest.GetRequestStream());
      requestWriter.Write(createItemSOAPRequest);
      requestWriter.Close();
      try
      {
        var getFolderResponse = (HttpWebResponse)(getFolderRequest.GetResponse());
        if (getFolderResponse.StatusCode == HttpStatusCode.OK)
        {
          var responseStream = getFolderResponse.GetResponseStream();
          XElement responseEnvelope = XElement.Load(responseStream);
          if (responseEnvelope != null)
          {
            // Write the response to the console and log file.
            Tracing.WriteLine("Response:");
            StringBuilder stringBuilder = new StringBuilder();
            XmlWriterSettings settings = new XmlWriterSettings();
            settings.Indent = true;
            XmlWriter writer = XmlWriter.Create(stringBuilder, settings);
            responseEnvelope.Save(writer);
            writer.Close();
            Tracing.WriteLine(stringBuilder.ToString());
            // Check the response for error codes. If there is an error, throw an application exception.
            IEnumerable<XElement> errorCodes = from errorCode in responseEnvelope.Descendants
                                               ("{http://schemas.microsoft.com/exchange/services/2006/messages}ResponseCode")
                                               select errorCode;
            foreach (var errorCode in errorCodes)
            {
              if (errorCode.Value != "NoError")
              {
                switch (errorCode.Parent.Name.LocalName.ToString())
                {
                  case "Response":
                    string responseError = "Response-level error getting inbox information:\n" + errorCode.Value;
                    throw new ApplicationException(responseError);
                  case "UserResponse":
                    string userError = "User-level error getting inbox information:\n" + errorCode.Value;
                    throw new ApplicationException(userError);
                }
              }
            }
            Tracing.WriteLine("Message sent successfully.");
          }
        }
      }
      catch (WebException ex)
      {
        Tracing.WriteLine("Caught Web exception:");
        Tracing.WriteLine(ex.Message);
      }
      catch (ApplicationException ex)
      {
        Tracing.WriteLine("Caught application exception:");
        Tracing.WriteLine(ex.Message);
      }
```

<a name="bk_next"></a>

## <a name="next-steps"></a>Próximas etapas

Agora que você escreveu seu primeiro aplicativo EWS, você está pronto para descobrir outras maneiras de usar o EWS. Aqui estão algumas ideias para você começar:
  
- Implemente a [descoberta automática](autodiscover-for-exchange.md) no seu aplicativo para que seu aplicativo se conectará ao servidor do Exchange correto, com base no endereço de email do usuário. Consulte também o [Exchange 2013: obter configurações de usuário com a descoberta automática](http://code.msdn.microsoft.com/Exchange-2013-Get-user-7e22c86e) amostra. 
    
- Examine a [referência do EWS](http://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx) para obter mais informações sobre o EWS. 
    
- Consulte as [operações do EWS](http://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx) para obter informações sobre as operações que estão disponíveis. 
    
- Use o [Editor do EWS](http://ewseditor.codeplex.com/) para ver o tráfego SOAP enviado de e para o servidor. 
    
Se você tiver algum problema com o seu aplicativo, [Experimente postar uma pergunta ou um comentário no fórum](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) (e não se esqueça de ler o primeiro post). 
  
## <a name="see-also"></a>Confira também

- [Start using web services in Exchange](start-using-web-services-in-exchange.md)   
- [Explorar a API Gerenciada pelo EWS, EWS e serviços Web no Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) 
- [Visão geral de design de cliente do EWS do Exchange](ews-client-design-overview-for-exchange.md)   
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)  
- [Introdução aos aplicativos de cliente API gerenciada de EWS](get-started-with-ews-managed-api-client-applications.md)
    

