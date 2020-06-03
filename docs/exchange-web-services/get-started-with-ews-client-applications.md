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
# <a name="get-started-with-ews-client-applications"></a><span data-ttu-id="1001c-103">Introdução aos aplicativos clientes do EWS</span><span class="sxs-lookup"><span data-stu-id="1001c-103">Get started with EWS client applications</span></span>

<span data-ttu-id="1001c-104">Crie seu primeiro aplicativo usando o EWS (serviços Web do Exchange) no Exchange.</span><span class="sxs-lookup"><span data-stu-id="1001c-104">Create your first application by using Exchange Web Services (EWS) in Exchange.</span></span>
  
<span data-ttu-id="1001c-105">O EWS é um serviço abrangente que seus aplicativos podem usar para acessar quase todas as informações armazenadas em um Exchange Online, Exchange Online como parte do Office 365 ou caixa de correio local do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1001c-105">EWS is a comprehensive service that your applications can use to access almost all the information stored in an Exchange Online, Exchange Online as part of Office 365, or Exchange on-premises mailbox.</span></span> <span data-ttu-id="1001c-106">O EWS usa protocolos Web padrão para fornecer acesso a um servidor Exchange; bibliotecas como a [API gerenciada do EWS](get-started-with-ews-managed-api-client-applications.md) envolvem as operações do EWS para fornecer uma interface orientada a objeto.</span><span class="sxs-lookup"><span data-stu-id="1001c-106">EWS uses standard web protocols to provide access to an Exchange server; libraries like the [EWS Managed API](get-started-with-ews-managed-api-client-applications.md) wrap the EWS operations to provide an object-oriented interface.</span></span> <span data-ttu-id="1001c-107">Depois de executar os exemplos deste artigo, você terá uma compreensão básica do que você pode fazer com o EWS.</span><span class="sxs-lookup"><span data-stu-id="1001c-107">After you've run the examples in this article, you will have a basic understanding of what you can do with EWS.</span></span> 
  
<span data-ttu-id="1001c-108">Você pode chamar as operações do EWS de qualquer sistema operacional ou idioma, pois as solicitações e respostas do EWS usam o protocolo SOAP.</span><span class="sxs-lookup"><span data-stu-id="1001c-108">You can call EWS operations from any operating system or language, because the EWS requests and responses use the SOAP protocol.</span></span> <span data-ttu-id="1001c-109">Os exemplos neste artigo são escritos usando C# e fazem uso dos objetos [HttpWebRequest](https://msdn.microsoft.com/library/System.Net.HttpWebRequest.aspx) e [HttpWebResponse](https://msdn.microsoft.com/library/System.Net.HttpWebResponse.aspx) do .NET Framework; no entanto, a parte importante do código é o XML usado para fazer a solicitação EWS e a resposta XML retornada do servidor.</span><span class="sxs-lookup"><span data-stu-id="1001c-109">The examples in this article are written using C# and make use of the .NET Framework [HttpWebRequest](https://msdn.microsoft.com/library/System.Net.HttpWebRequest.aspx) and [HttpWebResponse](https://msdn.microsoft.com/library/System.Net.HttpWebResponse.aspx) objects; however, the important part of the code is the XML used to make the EWS request and the XML response returned from the server.</span></span> <span data-ttu-id="1001c-110">Os exemplos de código enfatizam as transações XML e não processam o XML.</span><span class="sxs-lookup"><span data-stu-id="1001c-110">The code examples emphasize the XML transactions and not processing the XML.</span></span> 
  
## <a name="youll-need-an-exchange-server"></a><span data-ttu-id="1001c-111">Você precisará de um servidor do Exchange</span><span class="sxs-lookup"><span data-stu-id="1001c-111">You'll need an Exchange server</span></span>

<span data-ttu-id="1001c-112">Se você já tem uma conta de caixa de correio do Exchange, você pode ignorar esta etapa.</span><span class="sxs-lookup"><span data-stu-id="1001c-112">If you already have an Exchange mailbox account, you can skip this step.</span></span> <span data-ttu-id="1001c-113">Caso contrário, você tem as seguintes opções para configurar uma caixa de correio do Exchange para seu primeiro aplicativo do EWS:</span><span class="sxs-lookup"><span data-stu-id="1001c-113">Otherwise, you have the following options for setting up an Exchange mailbox for your first EWS application:</span></span>
  
- <span data-ttu-id="1001c-114">[Obter um site do desenvolvedor do Office 365 ](https://msdn.microsoft.com/library/office/fp179924.aspx)(recomendado).</span><span class="sxs-lookup"><span data-stu-id="1001c-114">[Get an Office 365 Developer Site ](https://msdn.microsoft.com/library/office/fp179924.aspx)(recommended).</span></span> <span data-ttu-id="1001c-115">Essa é a maneira mais rápida de obter uma caixa de correio do Exchange.</span><span class="sxs-lookup"><span data-stu-id="1001c-115">This is the quickest way for you to get an Exchange mailbox.</span></span>
    
- <span data-ttu-id="1001c-116">Baixar o [Exchange Server](https://office.microsoft.com/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).</span><span class="sxs-lookup"><span data-stu-id="1001c-116">Download [Exchange Server](https://office.microsoft.com/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).</span></span>

    
<span data-ttu-id="1001c-117">Depois de verificar se você pode enviar e receber emails do seu servidor Exchange, você está pronto para configurar seu ambiente de desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="1001c-117">After you've verified that you can send and receive email from your Exchange server you are ready to set up your development environment.</span></span> <span data-ttu-id="1001c-118">Você pode usar o Outlook Web App para verificar se você pode enviar emails.</span><span class="sxs-lookup"><span data-stu-id="1001c-118">You can use Outlook Web App to verify that you can send email.</span></span>
  
<span data-ttu-id="1001c-119">Você também precisará saber a URL do ponto de extremidade do EWS para seu servidor.</span><span class="sxs-lookup"><span data-stu-id="1001c-119">You'll also need to know the URL of the EWS endpoint for your server.</span></span> <span data-ttu-id="1001c-120">Em um aplicativo de produção, você usaria a [descoberta automática](autodiscover-for-exchange.md) para determinar a URL do EWS.</span><span class="sxs-lookup"><span data-stu-id="1001c-120">In a production application, you'd use [Autodiscover](autodiscover-for-exchange.md) to determine the EWS URL.</span></span> <span data-ttu-id="1001c-121">Os exemplos neste artigo usam a URL do ponto de extremidade do EWS do Office 365, `https://outlook.office365.com/EWS/Exchange.asmx` .</span><span class="sxs-lookup"><span data-stu-id="1001c-121">The examples in this article use the Office 365 EWS endpoint URL, `https://outlook.office365.com/EWS/Exchange.asmx`.</span></span> <span data-ttu-id="1001c-122">A seção de [etapas a seguir](#bk_next) contém links para mais informações sobre a descoberta automática quando você estiver pronto.</span><span class="sxs-lookup"><span data-stu-id="1001c-122">The [Next steps](#bk_next) section has links to more information about Autodiscover when you're ready.</span></span> 
  
<span data-ttu-id="1001c-123">Se você estiver testando seu aplicativo usando um servidor Exchange que tenha o certificado autoassinado padrão, será necessário criar um método de [validação de certificado](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) que atenda aos requisitos de segurança da sua organização.</span><span class="sxs-lookup"><span data-stu-id="1001c-123">If you are testing your application using an Exchange server that has the default self-signed certificate, you'll need to create a [certificate validation method](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) that meets the security requirements of your organization.</span></span> 
  
## <a name="set-up-your-development-environment"></a><span data-ttu-id="1001c-124">Defina seu ambiente de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="1001c-124">Set up your development environment</span></span>

<span data-ttu-id="1001c-125">As ferramentas que você usa para criar seu primeiro aplicativo EWS dependem do sistema operacional e do idioma que você usa, e são principalmente uma questão de gosto.</span><span class="sxs-lookup"><span data-stu-id="1001c-125">The tools that you use to create your first EWS application depend on the operating system and language that you use, and are mostly a matter of taste.</span></span> <span data-ttu-id="1001c-126">Se quiser acompanhar os exemplos de C# neste artigo, você precisará de:</span><span class="sxs-lookup"><span data-stu-id="1001c-126">If you want to follow along with the C# examples in this article, you'll need:</span></span> 
  
- <span data-ttu-id="1001c-127">Qualquer versão do Visual Studio que suporte o .NET Framework 4,0.</span><span class="sxs-lookup"><span data-stu-id="1001c-127">Any version of Visual Studio that supports the .NET Framework 4.0.</span></span> 
    
- <span data-ttu-id="1001c-128">Uma conexão com a Internet que sua máquina de desenvolvimento pode usar para entrar em contato com o Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="1001c-128">An Internet connection that your development machine can use to contact your Exchange server.</span></span> <span data-ttu-id="1001c-129">Se você pode usar o Outlook Web App com um nome DNS em vez de um endereço IP para se conectar ao seu servidor do Exchange, você está configurado.</span><span class="sxs-lookup"><span data-stu-id="1001c-129">If you can use Outlook Web App with a DNS name rather than an IP address to connect to your Exchange server, you are set up.</span></span>
    
## <a name="create-your-first-ews-application"></a><span data-ttu-id="1001c-130">Criar seu primeiro aplicativo EWS</span><span class="sxs-lookup"><span data-stu-id="1001c-130">Create your first EWS application</span></span>

<span data-ttu-id="1001c-131">O aplicativo EWS que você criará mostra dois cenários típicos para o uso do EWS:</span><span class="sxs-lookup"><span data-stu-id="1001c-131">The EWS application that you will create shows two typical scenarios for using EWS:</span></span>
  
1. <span data-ttu-id="1001c-132">Obter informações de uma caixa de correio do Exchange e exibi-las para o usuário.</span><span class="sxs-lookup"><span data-stu-id="1001c-132">Get information from an Exchange mailbox and display that information to the user.</span></span>
    
2. <span data-ttu-id="1001c-133">Executar uma ação, como enviar um email e verificar a resposta para ver se a ação foi bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="1001c-133">Perform an action, such as sending an email, and check the response to see if the action succeeded.</span></span>
    
<span data-ttu-id="1001c-134">Vamos começar.</span><span class="sxs-lookup"><span data-stu-id="1001c-134">Let's get started.</span></span>
  
### <a name="set-up-the-solution"></a><span data-ttu-id="1001c-135">Configurar a solução</span><span class="sxs-lookup"><span data-stu-id="1001c-135">Set up the solution</span></span>

<span data-ttu-id="1001c-136">Primeiro, crie uma nova solução de aplicativo de console usando o Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="1001c-136">First, create a new console application solution using Visual Studio.</span></span> <span data-ttu-id="1001c-137">Quando a solução estiver pronta, crie um novo objeto chamado Tracing.cs.</span><span class="sxs-lookup"><span data-stu-id="1001c-137">When the solution is ready, create a new object called Tracing.cs.</span></span> <span data-ttu-id="1001c-138">Use esse objeto para gravar informações no console e em um arquivo de log para que você possa revisar os resultados depois de executar o código.</span><span class="sxs-lookup"><span data-stu-id="1001c-138">Use this object to write information to both the console and a log file so that you can review the results after you run your code.</span></span> <span data-ttu-id="1001c-139">Cole o código a seguir no arquivo Tracing.cs.</span><span class="sxs-lookup"><span data-stu-id="1001c-139">Paste the following code into the Tracing.cs file.</span></span>
  
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

<span data-ttu-id="1001c-140">Em seguida, abra o arquivo Program.cs.</span><span class="sxs-lookup"><span data-stu-id="1001c-140">Next, open the Program.cs file.</span></span> <span data-ttu-id="1001c-141">Você colocará o restante do código do exemplo neste arquivo.</span><span class="sxs-lookup"><span data-stu-id="1001c-141">You will put the rest of the code for the example in this file.</span></span>
  
<span data-ttu-id="1001c-142">Primeiro, configure o Shell do programa.</span><span class="sxs-lookup"><span data-stu-id="1001c-142">First, set up the shell of the program.</span></span> <span data-ttu-id="1001c-143">O programa irá:</span><span class="sxs-lookup"><span data-stu-id="1001c-143">The program will:</span></span> 
  
1. <span data-ttu-id="1001c-144">Crie um arquivo de log para que a solicitação e a resposta possam ser gravadas no disco para estudo posterior.</span><span class="sxs-lookup"><span data-stu-id="1001c-144">Create a log file so that the request and response can be written to disk for later study.</span></span>
    
2. <span data-ttu-id="1001c-145">Obtenha o endereço de email e a senha da conta que você acessará.</span><span class="sxs-lookup"><span data-stu-id="1001c-145">Get the email address and password of the account that you'll access.</span></span>
    
3. <span data-ttu-id="1001c-146">Chamar os métodos de amostra.</span><span class="sxs-lookup"><span data-stu-id="1001c-146">Call the sample methods.</span></span>
    
<span data-ttu-id="1001c-147">Substitua o `Main` método no Program.cs pelo código a seguir.</span><span class="sxs-lookup"><span data-stu-id="1001c-147">Replace the  `Main` method in the Program.cs with the following code.</span></span> 
  
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

<span data-ttu-id="1001c-148">A última coisa que você precisa fazer é adicionar o `GetPasswordFromConsole` método estático.</span><span class="sxs-lookup"><span data-stu-id="1001c-148">The last thing that you need to do is add the  `GetPasswordFromConsole` static method.</span></span> <span data-ttu-id="1001c-149">Este método retorna um objeto [SecureString](https://msdn.microsoft.com/library/System.Security.SecureString.aspx) que contém uma senha digitada no console.</span><span class="sxs-lookup"><span data-stu-id="1001c-149">This method returns a [SecureString](https://msdn.microsoft.com/library/System.Security.SecureString.aspx) object that contains a password typed at the console.</span></span> 
  
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

### <a name="get-the-number-of-new-messages-in-an-inbox"></a><span data-ttu-id="1001c-150">Obter o número de novas mensagens em uma caixa de entrada</span><span class="sxs-lookup"><span data-stu-id="1001c-150">Get the number of new messages in an Inbox</span></span>

<span data-ttu-id="1001c-151">Uma operação comum em um aplicativo do EWS é obter informações sobre mensagens de email, compromissos, reuniões e pastas que os armazenam.</span><span class="sxs-lookup"><span data-stu-id="1001c-151">A common operation in an EWS application is to get information about email messages, appointments, meetings, and the folders that store them.</span></span> <span data-ttu-id="1001c-152">Este exemplo obtém o número de mensagens na caixa de entrada de uma conta e exibe o número total de mensagens e o número de mensagens não lidas.</span><span class="sxs-lookup"><span data-stu-id="1001c-152">This example gets the number of messages in an account's Inbox and displays the total number of messages and the number of unread messages.</span></span> <span data-ttu-id="1001c-153">Ele demonstra as seguintes ações comuns para aplicativos EWS:</span><span class="sxs-lookup"><span data-stu-id="1001c-153">It demonstrates the following common actions for EWS applications:</span></span>
  
- <span data-ttu-id="1001c-154">Fazer uma solicitação de EWS para o servidor Exchange.</span><span class="sxs-lookup"><span data-stu-id="1001c-154">Making an EWS request to the Exchange server.</span></span>
    
- <span data-ttu-id="1001c-155">Analisar a resposta XML retornada para as informações solicitadas.</span><span class="sxs-lookup"><span data-stu-id="1001c-155">Parsing the returned XML response for the requested information.</span></span>
    
- <span data-ttu-id="1001c-156">Tratamento de exceções comuns e mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="1001c-156">Handling common exceptions and error messages.</span></span>
    
<span data-ttu-id="1001c-157">Adicione o seguinte código ao `ShowNumberOfMessagesInInbox` método que foi ocultodo após o método Main.</span><span class="sxs-lookup"><span data-stu-id="1001c-157">Add the following code to the  `ShowNumberOfMessagesInInbox` method that was stubbed out after the main method.</span></span> <span data-ttu-id="1001c-158">Quando você executa o aplicativo, ele vai imprimir o número de mensagens na caixa de entrada da conta e o número de mensagens não lidas na caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="1001c-158">When you run the application, it will print the number of messages in the account's Inbox and the number of unread messages in the Inbox.</span></span> <span data-ttu-id="1001c-159">Depois de executar o aplicativo, você pode abrir o arquivo GetStartedWithEWS. log para ver a solicitação XML que foi enviada ao servidor do Exchange e a resposta que o servidor retornou.</span><span class="sxs-lookup"><span data-stu-id="1001c-159">After you run the application, you can open the GetStartedWithEWS.log file to see the XML request that was sent to the Exchange server and the response that the server returned.</span></span> 
  
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

### <a name="send-an-email-message"></a><span data-ttu-id="1001c-160">Enviar uma mensagem de email</span><span class="sxs-lookup"><span data-stu-id="1001c-160">Send an email message</span></span>

<span data-ttu-id="1001c-161">Outra operação comum para um aplicativo EWS é enviar mensagens de email ou solicitações de reunião.</span><span class="sxs-lookup"><span data-stu-id="1001c-161">Another common operation for an EWS application is to send email messages or meeting requests.</span></span> <span data-ttu-id="1001c-162">Este exemplo cria e envia uma mensagem de email usando as credenciais do usuário que foram inseridas anteriormente.</span><span class="sxs-lookup"><span data-stu-id="1001c-162">This example creates and sends an email message using the user credentials that were entered earlier.</span></span> <span data-ttu-id="1001c-163">Ele demonstra essas tarefas comuns do aplicativo EWS:</span><span class="sxs-lookup"><span data-stu-id="1001c-163">It demonstrates these common EWS application tasks:</span></span>
  
- <span data-ttu-id="1001c-164">Criar e enviar um email.</span><span class="sxs-lookup"><span data-stu-id="1001c-164">Creating and sending an email.</span></span>
    
- <span data-ttu-id="1001c-165">Analisar a resposta XML retornada para determinar se o email foi enviado corretamente.</span><span class="sxs-lookup"><span data-stu-id="1001c-165">Parsing the returned XML response to determine if the email was correctly sent.</span></span>
    
- <span data-ttu-id="1001c-166">Tratamento de exceções comuns e mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="1001c-166">Handling common exceptions and error messages.</span></span>
    
<span data-ttu-id="1001c-167">Adicione o seguinte código ao método SendTestEmail que estava oculto após o método Main.</span><span class="sxs-lookup"><span data-stu-id="1001c-167">Add the following code to the SendTestEmail method that was stubbed out after the main method.</span></span> <span data-ttu-id="1001c-168">Depois de executar o aplicativo, você pode abrir o arquivo GetStartedWithEWS. log para ver a solicitação XML que foi enviada ao servidor do Exchange e a resposta que o servidor retornou.</span><span class="sxs-lookup"><span data-stu-id="1001c-168">After you run the application, you can open the GetStartedWithEWS.log file to see the XML request that was sent to the Exchange server and the response that the server returned.</span></span>
  
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

## <a name="next-steps"></a><span data-ttu-id="1001c-169">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="1001c-169">Next steps</span></span>

<span data-ttu-id="1001c-170">Agora que você já escreveu seu primeiro aplicativo EWS, você está pronto para descobrir outras maneiras de usar o EWS.</span><span class="sxs-lookup"><span data-stu-id="1001c-170">Now that you've written your first EWS application, you're ready to discover other ways to use EWS.</span></span> <span data-ttu-id="1001c-171">Veja algumas ideias para começar:</span><span class="sxs-lookup"><span data-stu-id="1001c-171">Here are some ideas to get you started:</span></span>
  
- <span data-ttu-id="1001c-172">Implemente a [descoberta automática](autodiscover-for-exchange.md) em seu aplicativo para que seu aplicativo se conecte ao servidor Exchange correto com base no endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="1001c-172">Implement [Autodiscover](autodiscover-for-exchange.md) in your application so that your application will connect to the correct Exchange server based on the user's email address.</span></span> <span data-ttu-id="1001c-173">Consulte também o [Exchange 2013: obter configurações do usuário com o exemplo de descoberta automática](https://code.msdn.microsoft.com/Exchange-2013-Get-user-7e22c86e) .</span><span class="sxs-lookup"><span data-stu-id="1001c-173">See also the [Exchange 2013: Get user settings with Autodiscover](https://code.msdn.microsoft.com/Exchange-2013-Get-user-7e22c86e) sample.</span></span> 
    
- <span data-ttu-id="1001c-174">Consulte a [referência do EWS](https://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx) para obter mais informações sobre o EWS.</span><span class="sxs-lookup"><span data-stu-id="1001c-174">Look at the [EWS reference](https://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx) for more information about EWS.</span></span> 
    
- <span data-ttu-id="1001c-175">Consulte as [operações do EWS](https://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx) para obter informações sobre as operações que estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="1001c-175">See the [EWS operations](https://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx) for information about the operations that are available.</span></span> 
    
- <span data-ttu-id="1001c-176">Use o [Editor do EWS](http://ewseditor.codeplex.com/) para ver o tráfego SOAP enviado para e do servidor.</span><span class="sxs-lookup"><span data-stu-id="1001c-176">Use [EWS Editor](http://ewseditor.codeplex.com/) to see the SOAP traffic sent to and from the server.</span></span> 
    
<span data-ttu-id="1001c-177">Se você tiver problemas com o aplicativo, [tente postar uma dúvida ou comentário no fórum](https://social.technet.microsoft.com/Forums/exchange/home?forum=exchangesvrdevelopment) (e não se esqueça de ler a primeira postagem).</span><span class="sxs-lookup"><span data-stu-id="1001c-177">If you run into any issues with your application, [try posting a question or comment in the forum](https://social.technet.microsoft.com/Forums/exchange/home?forum=exchangesvrdevelopment) (and don't forget to read the first post).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="1001c-178">Confira também</span><span class="sxs-lookup"><span data-stu-id="1001c-178">See also</span></span>

- [<span data-ttu-id="1001c-179">Introdução ao uso dos serviços Web no Exchange</span><span class="sxs-lookup"><span data-stu-id="1001c-179">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)   
- [<span data-ttu-id="1001c-180">Explorar os recursos da API gerenciada por EWS, EWS e serviços Web no Exchange</span><span class="sxs-lookup"><span data-stu-id="1001c-180">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) 
- [<span data-ttu-id="1001c-181">Visão geral do design de cliente do EWS para Exchange</span><span class="sxs-lookup"><span data-stu-id="1001c-181">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)   
- [<span data-ttu-id="1001c-182">Develop web service clients for Exchange</span><span class="sxs-lookup"><span data-stu-id="1001c-182">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)  
- [<span data-ttu-id="1001c-183">Introdução aos aplicativos clientes de API gerenciada por EWS</span><span class="sxs-lookup"><span data-stu-id="1001c-183">Get started with EWS Managed API client applications</span></span>](get-started-with-ews-managed-api-client-applications.md)
    