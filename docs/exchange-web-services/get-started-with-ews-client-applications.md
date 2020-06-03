---
title: Introdução aos aplicativos clientes do EWS
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.assetid: e6fd5c23-0ba5-4a7b-bdde-4a553447069f
description: Crie seu primeiro aplicativo usando o EWS (serviços Web do Exchange) no Exchange.
localization_priority: Priority
ms.openlocfilehash: fd02c46777dabd04b492ba3c4420a0737640c5eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528395"
---
# <a name="get-started-with-ews-client-applications"></a>Introdução aos aplicativos clientes do EWS

Crie seu primeiro aplicativo usando o EWS (serviços Web do Exchange) no Exchange.
  
O EWS é um serviço abrangente que seus aplicativos podem usar para acessar quase todas as informações armazenadas em um Exchange Online, Exchange Online como parte do Office 365 ou caixa de correio local do Exchange. O EWS usa protocolos Web padrão para fornecer acesso a um servidor Exchange; bibliotecas como a [API gerenciada do EWS](get-started-with-ews-managed-api-client-applications.md) envolvem as operações do EWS para fornecer uma interface orientada a objeto. Depois de executar os exemplos deste artigo, você terá uma compreensão básica do que você pode fazer com o EWS. 
  
Você pode chamar as operações do EWS de qualquer sistema operacional ou idioma, pois as solicitações e respostas do EWS usam o protocolo SOAP. Os exemplos neste artigo são escritos usando C# e fazem uso dos objetos [HttpWebRequest](https://msdn.microsoft.com/library/System.Net.HttpWebRequest.aspx) e [HttpWebResponse](https://msdn.microsoft.com/library/System.Net.HttpWebResponse.aspx) do .NET Framework; no entanto, a parte importante do código é o XML usado para fazer a solicitação EWS e a resposta XML retornada do servidor. Os exemplos de código enfatizam as transações XML e não processam o XML. 
  
## <a name="youll-need-an-exchange-server"></a>Você precisará de um servidor do Exchange

Se você já tem uma conta de caixa de correio do Exchange, você pode ignorar esta etapa. Caso contrário, você tem as seguintes opções para configurar uma caixa de correio do Exchange para seu primeiro aplicativo do EWS:
  
- [Obter um site do desenvolvedor do Office 365 ](https://msdn.microsoft.com/library/office/fp179924.aspx)(recomendado). Essa é a maneira mais rápida de obter uma caixa de correio do Exchange.
    
- Baixar o [Exchange Server](https://office.microsoft.com/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).

    
Depois de verificar se você pode enviar e receber emails do seu servidor Exchange, você está pronto para configurar seu ambiente de desenvolvimento. Você pode usar o Outlook Web App para verificar se você pode enviar emails.
  
Você também precisará saber a URL do ponto de extremidade do EWS para seu servidor. Em um aplicativo de produção, você usaria a [descoberta automática](autodiscover-for-exchange.md) para determinar a URL do EWS. Os exemplos neste artigo usam a URL do ponto de extremidade do EWS do Office 365, `https://outlook.office365.com/EWS/Exchange.asmx` . A seção de [etapas a seguir](#bk_next) contém links para mais informações sobre a descoberta automática quando você estiver pronto. 
  
Se você estiver testando seu aplicativo usando um servidor Exchange que tenha o certificado autoassinado padrão, será necessário criar um método de [validação de certificado](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) que atenda aos requisitos de segurança da sua organização. 
  
## <a name="set-up-your-development-environment"></a>Defina seu ambiente de desenvolvimento

As ferramentas que você usa para criar seu primeiro aplicativo EWS dependem do sistema operacional e do idioma que você usa, e são principalmente uma questão de gosto. Se quiser acompanhar os exemplos de C# neste artigo, você precisará de: 
  
- Qualquer versão do Visual Studio que suporte o .NET Framework 4,0. 
    
- Uma conexão com a Internet que sua máquina de desenvolvimento pode usar para entrar em contato com o Exchange Server. Se você pode usar o Outlook Web App com um nome DNS em vez de um endereço IP para se conectar ao seu servidor do Exchange, você está configurado.
    
## <a name="create-your-first-ews-application"></a>Criar seu primeiro aplicativo EWS

O aplicativo EWS que você criará mostra dois cenários típicos para o uso do EWS:
  
1. Obter informações de uma caixa de correio do Exchange e exibi-las para o usuário.
    
2. Executar uma ação, como enviar um email e verificar a resposta para ver se a ação foi bem-sucedida.
    
Vamos começar.
  
### <a name="set-up-the-solution"></a>Configurar a solução

Primeiro, crie uma nova solução de aplicativo de console usando o Visual Studio. Quando a solução estiver pronta, crie um novo objeto chamado Tracing.cs. Use esse objeto para gravar informações no console e em um arquivo de log para que você possa revisar os resultados depois de executar o código. Cole o código a seguir no arquivo Tracing.cs.
  
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

Em seguida, abra o arquivo Program.cs. Você colocará o restante do código do exemplo neste arquivo.
  
Primeiro, configure o Shell do programa. O programa irá: 
  
1. Crie um arquivo de log para que a solicitação e a resposta possam ser gravadas no disco para estudo posterior.
    
2. Obtenha o endereço de email e a senha da conta que você acessará.
    
3. Chamar os métodos de amostra.
    
Substitua o `Main` método no Program.cs pelo código a seguir. 
  
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

A última coisa que você precisa fazer é adicionar o `GetPasswordFromConsole` método estático. Este método retorna um objeto [SecureString](https://msdn.microsoft.com/library/System.Security.SecureString.aspx) que contém uma senha digitada no console. 
  
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

Uma operação comum em um aplicativo do EWS é obter informações sobre mensagens de email, compromissos, reuniões e pastas que os armazenam. Este exemplo obtém o número de mensagens na caixa de entrada de uma conta e exibe o número total de mensagens e o número de mensagens não lidas. Ele demonstra as seguintes ações comuns para aplicativos EWS:
  
- Fazer uma solicitação de EWS para o servidor Exchange.
    
- Analisar a resposta XML retornada para as informações solicitadas.
    
- Tratamento de exceções comuns e mensagens de erro.
    
Adicione o seguinte código ao `ShowNumberOfMessagesInInbox` método que foi ocultodo após o método Main. Quando você executa o aplicativo, ele vai imprimir o número de mensagens na caixa de entrada da conta e o número de mensagens não lidas na caixa de entrada. Depois de executar o aplicativo, você pode abrir o arquivo GetStartedWithEWS. log para ver a solicitação XML que foi enviada ao servidor do Exchange e a resposta que o servidor retornou. 
  
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

Outra operação comum para um aplicativo EWS é enviar mensagens de email ou solicitações de reunião. Este exemplo cria e envia uma mensagem de email usando as credenciais do usuário que foram inseridas anteriormente. Ele demonstra essas tarefas comuns do aplicativo EWS:
  
- Criar e enviar um email.
    
- Analisar a resposta XML retornada para determinar se o email foi enviado corretamente.
    
- Tratamento de exceções comuns e mensagens de erro.
    
Adicione o seguinte código ao método SendTestEmail que estava oculto após o método Main. Depois de executar o aplicativo, você pode abrir o arquivo GetStartedWithEWS. log para ver a solicitação XML que foi enviada ao servidor do Exchange e a resposta que o servidor retornou.
  
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

Agora que você já escreveu seu primeiro aplicativo EWS, você está pronto para descobrir outras maneiras de usar o EWS. Veja algumas ideias para começar:
  
- Implemente a [descoberta automática](autodiscover-for-exchange.md) em seu aplicativo para que seu aplicativo se conecte ao servidor Exchange correto com base no endereço de email do usuário. Consulte também o [Exchange 2013: obter configurações do usuário com o exemplo de descoberta automática](https://code.msdn.microsoft.com/Exchange-2013-Get-user-7e22c86e) . 
    
- Consulte a [referência do EWS](https://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx) para obter mais informações sobre o EWS. 
    
- Consulte as [operações do EWS](https://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx) para obter informações sobre as operações que estão disponíveis. 
    
- Use o [Editor do EWS](http://ewseditor.codeplex.com/) para ver o tráfego SOAP enviado para e do servidor. 
    
Se você tiver problemas com o aplicativo, [tente postar uma dúvida ou comentário no fórum](https://social.technet.microsoft.com/Forums/exchange/home?forum=exchangesvrdevelopment) (e não se esqueça de ler a primeira postagem). 
  
## <a name="see-also"></a>Confira também

- [Introdução ao uso dos serviços Web no Exchange](start-using-web-services-in-exchange.md)   
- [Explorar os recursos da API gerenciada por EWS, EWS e serviços Web no Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) 
- [Visão geral do design de cliente do EWS para Exchange](ews-client-design-overview-for-exchange.md)   
- [Develop web service clients for Exchange](develop-web-service-clients-for-exchange.md)  
- [Introdução aos aplicativos clientes de API gerenciada por EWS](get-started-with-ews-managed-api-client-applications.md)
    