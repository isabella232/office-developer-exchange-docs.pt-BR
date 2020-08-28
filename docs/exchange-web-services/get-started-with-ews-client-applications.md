---
title: Introdução aos aplicativos clientes do EWS
manager: sethgros
ms.date: 8/26/2020
ms.audience: Developer
ms.assetid: e6fd5c23-0ba5-4a7b-bdde-4a553447069f
description: Crie seu primeiro aplicativo usando os Serviços Web do Exchange (EWS) no Exchange.
localization_priority: Priority
ms.openlocfilehash: 81d4cb69d20f17945658ab4ad16c9fe3a47d4eec
ms.sourcegitcommit: 636c05a929279812c6ef87d75b01c166a4a05584
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/26/2020
ms.locfileid: "47254976"
---
# <a name="get-started-with-ews-client-applications"></a>Introdução aos aplicativos clientes do EWS

Crie seu primeiro aplicativo usando os Serviços Web do Exchange (EWS) no Exchange.
  
O EWS é um serviço completo que seus aplicativos podem usar para acessar quase todas as informações armazenadas em um Exchange Online, um Exchange Online como parte do Office 365 ou em uma caixa de correio local do Exchange. O EWS usa protocolos padrão da Web para fornecer acesso a um servidor do Exchange. Bibliotecas como a [API gerenciada EWS](get-started-with-ews-managed-api-client-applications.md) envolvem as operações do EWS para fornecer uma interface orientada ao objeto. Depois de executar os exemplos deste artigo, você terá uma compreensão básica do que pode fazer com o EWS. 
  
Você pode chamar as operações de EWS a partir de qualquer sistema operacional ou idioma, uma vez que as solicitações e respostas EWS usam o protocolo SOAP. Os exemplos neste artigo foram escritos usando C# e utilizam o .NET Framework e objetos [HttpWebRequest](https://msdn.microsoft.com/library/System.Net.HttpWebRequest.aspx) e [HttpWebResponse](https://msdn.microsoft.com/library/System.Net.HttpWebResponse.aspx). No entanto, a parte importante do código é o XML usado para fazer a solicitação do EWS e a resposta XML retornada do servidor. Os exemplos de código enfatizam as transações XML e não processam o XML. 
  
## <a name="youll-need-an-exchange-server"></a>Você precisará de um servidor Exchange

Se você já tiver uma conta de caixa de correio do Exchange, ignore esta etapa. Caso contrário, você tem as opções a seguir para configurar uma caixa de correio do Exchange para o seu primeiro aplicativo EWS:
  
- [Obtenha um Site do Desenvolvedor do Office 365](https://developer.microsoft.com/microsoft-365/dev-program) (recomendado). Esta é a maneira mais rápida de obter uma caixa de correio do Exchange.
    
- Baixe o[Exchange Server](https://office.microsoft.com/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).

    
Depois de verificar que você pode enviar e receber emails do seu servidor Exchange, você estará pronto para configurar seu ambiente de desenvolvimento. Você pode usar o Outlook Web App para verificar se é possível enviar emails.
  
Você também precisa saber a URL do ponto de extremidade do EWS para o seu servidor. Em um aplicativo de produção, você usaria a [Descoberta Automática](autodiscover-for-exchange.md) para determinar a URL do EWS. Os exemplos nesse artigo usam o URL do ponto de extremidade do EWS Office 365, `https://outlook.office365.com/EWS/Exchange.asmx`. A seção [Próximas etapas](#bk_next) possui links com mais informações sobre a descoberta automática quando você estiver pronto. 
  
Se você estiver testando seu aplicativo usando um servidor Exchange que tenha o certificado auto-assinado padrão, será necessário criar um [método de validação de certificado](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) que atenda aos requisitos de segurança da sua organização. 
  
## <a name="set-up-your-development-environment"></a>Defina seu ambiente de desenvolvimento

As ferramentas que você usa para criar seu primeiro aplicativo EWS dependem do sistema operacional e do idioma que você usa, e são principalmente uma questão de gosto. Caso pretenda acompanhar os exemplos C# deste artigo, você precisará do seguinte: 
  
- Qualquer versão do Visual Studio compatível com o .NET Framework 4.0. 
    
- Uma conexão com a Internet que você pode usar para contatar seu servidor Exchange. Se você puder usar o Outlook Web App com um nome DNS em vez de um endereço IP para se conectar ao seu servidor Exchange, você está pronto.
    
## <a name="create-your-first-ews-application"></a>Criar seu primeiro aplicativo EWS

O aplicativo EWS que você criará mostra dois cenários típicos para usar o EWS:
  
1. Obtenha informações de uma caixa de correio do Exchange e exiba essas informações para o usuário.
    
2. Execute uma ação, como enviar um email e verificar a resposta para ver se a ação teve êxito.
    
Vamos começar.
  
### <a name="set-up-the-solution"></a>Configurar a solução

Primeiro, crie uma nova solução para o aplicativo de console usando o Visual Studio. Quando a solução estiver pronta, crie um novo objeto chamado Tracing.cs. Use esse objeto para gravar informações no console e em um arquivo de log, para que você possa revisar os resultados após executar o código. Cole o seguinte código no arquivo Tracing.cs.
  
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

Em seguida, abra o arquivo Program.cs. Você colocará o restante do código no exemplo desse arquivo.
  
Primeiro, configure o shell do programa. O programa irá: 
  
1. Criar um arquivo de log para que a solicitação e a resposta possam ser gravadas em disco para estudos posteriores.
    
2. Obtenha o endereço de email e senha da conta a qual você terá acesso.
    
3. Chame os métodos de exemplo.
    
Substitua o `Main`método no Program.cs com o seguinte código. 
  
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

A última coisa que você precisa fazer é adicionar o  `GetPasswordFromConsole` método estático. Esse método retorna um objeto [SecureString](https://msdn.microsoft.com/library/System.Security.SecureString.aspx) que contém uma senha digitada no console. 
  
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

Uma operação comum em um aplicativo do EWS é obter informações sobre mensagens de email, compromissos, reuniões e pastas que os armazenam. Este exemplo obtém o número de mensagens na caixa de entrada de uma conta, exibe o número total de mensagens e o número de mensagens não lidas. Ele demonstra as seguintes ações comuns para aplicativos do EWS:
  
- Fazer uma solicitação EWS para o servidor Exchange.
    
- Analisar as respostas XML retornadas para as informações solicitadas.
    
- Lidar com exceções comuns e mensagens de erro.
    
Adicione o código a seguir ao método  `ShowNumberOfMessagesInInbox` que foi interrompido após o método principal. Quando você executa o aplicativo, ele vai imprimir o número de mensagens na caixa de entrada da conta e o número de mensagens não lidas na caixa de entrada. Depois de executar o aplicativo, você pode abrir o arquivo GetStartedWithEWS.log para ver a solicitação XML que foi enviada para o servidor Exchange e a resposta que o servidor retornou. 
  
```cs
      /// This is the XML request that is sent to the Exchange server.
      var getFolderSOAPRequest =
"<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
"<soap:Envelope xmlns:soap=\"https://schemas.xmlsoap.org/soap/envelope/\"\n" +
"   xmlns:t=\"https://schemas.microsoft.com/exchange/services/2006/types\">\n" +
"<soap:Header>\n" +
"    <t:RequestServerVersion Version=\"Exchange2007_SP1\" />\n" +
"  </soap:Header>\n" +
"  <soap:Body>\n" +
"    <GetFolder xmlns=\"https://schemas.microsoft.com/exchange/services/2006/messages\"\n" +
"               xmlns:t=\"https://schemas.microsoft.com/exchange/services/2006/types\">\n" +
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
                                               ("{https://schemas.microsoft.com/exchange/services/2006/messages}ResponseCode")
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
                                              ("{https://schemas.microsoft.com/exchange/services/2006/messages}Folders")
                                            select folderElement;
            foreach (var folder in folders)
            {
              Tracing.Write("Folder name:     ");
              var folderName = from folderElement in
                                 folder.Descendants
                                 ("{https://schemas.microsoft.com/exchange/services/2006/types}DisplayName")
                               select folderElement.Value;
              Tracing.WriteLine(folderName.ElementAt(0));
              Tracing.Write("Total messages:  ");
              var totalCount = from folderElement in
                                 folder.Descendants
                                   ("{https://schemas.microsoft.com/exchange/services/2006/types}TotalCount")
                               select folderElement.Value;
              Tracing.WriteLine(totalCount.ElementAt(0));
              Tracing.Write("Unread messages: ");
              var unreadCount = from folderElement in
                                 folder.Descendants
                                   ("{https://schemas.microsoft.com/exchange/services/2006/types}UnreadCount")
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

Outra operação comum para um aplicativo EWS é enviar mensagens de email ou solicitações de reunião. Este exemplo cria e envia uma mensagem de email usando as credenciais de usuário que foram inseridas anteriormente. Ele demonstra essas tarefas comuns do aplicativo EWS:
  
- Criar e enviar um email.
    
- Analisar a resposta XML retornada para determinar se o email foi enviado corretamente.
    
- Lidar com exceções comuns e mensagens de erro.
    
Adicione o código a seguir ao método SendTestEmail que foi interrompido após o método principal. Depois de executar o aplicativo, você pode abrir o arquivo GetStartedWithEWS.log para ver a solicitação XML que foi enviada para o servidor Exchange e a resposta que o servidor retornou.
  
```cs
var createItemSOAPRequest =
      "<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
      "<soap:Envelope xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\" \n" +
      "               xmlns:m=\"https://schemas.microsoft.com/exchange/services/2006/messages\" \n" +
      "               xmlns:t=\"https://schemas.microsoft.com/exchange/services/2006/types\" \n" +
      "               xmlns:soap=\"https://schemas.xmlsoap.org/soap/envelope/\">\n" +
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
                                               ("{https://schemas.microsoft.com/exchange/services/2006/messages}ResponseCode")
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

Agora que você já escreveu seu primeiro aplicativo EWS, você está pronto para descobrir outras maneiras de usar o EWS. Veja algumas ideias para você começar:
  
- Implemente a [Descoberta Automática](autodiscover-for-exchange.md) em seu aplicativo para que ele se conecte ao servidor do Exchange correto com base no endereço de email do usuário. Veja também o modelo[Exchange 2013: Obter configurações do usuário com a Descoberta Automática](https://code.msdn.microsoft.com/Exchange-2013-Get-user-7e22c86e). 
    
- Confira a [referência do EWS](https://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx) para saber mais sobre o EWS. 
    
- Confira as [operações do EWS](https://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx) para saber mais sobre as operações disponíveis. 
    
- Use o [editor do EWS](http://ewseditor.codeplex.com/) para ver o tráfego SOAP enviado ao e do servidor. 
    
Se você tiver algum problema com o aplicativo, [tente postar uma pergunta ou comentário no fórum](https://social.technet.microsoft.com/Forums/exchange/home?forum=exchangesvrdevelopment) (e não se esqueça de ler a primeira postagem). 
  
## <a name="see-also"></a>Confira também

- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)   
- [Explorar os recursos da API gerenciada por EWS, EWS e Serviços Web no Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) 
- [Visão geral de design do cliente EWS para o Exchange](ews-client-design-overview-for-exchange.md)   
- [Desenvolver clientes do serviço Web para o Exchange](develop-web-service-clients-for-exchange.md)  
- [Introdução aos aplicativos clientes de API gerenciada por EWS](get-started-with-ews-managed-api-client-applications.md)
    
