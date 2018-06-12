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
# <a name="get-started-with-ews-client-applications"></a><span data-ttu-id="d7dd9-103">Introdução aos aplicativos de cliente do EWS</span><span class="sxs-lookup"><span data-stu-id="d7dd9-103">Get started with EWS client applications</span></span>

<span data-ttu-id="d7dd9-104">Crie seu primeiro aplicativo usando os serviços Web do Exchange (EWS) no Exchange.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-104">Create your first application by using Exchange Web Services (EWS) in Exchange.</span></span>
  
<span data-ttu-id="d7dd9-105">EWS é um serviço abrangente que seus aplicativos podem usar para acessar quase todas as informações armazenadas em um Exchange Online, Exchange Online como parte do Office 365, ou Exchange da caixa de correio local.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-105">EWS is a comprehensive service that your applications can use to access almost all the information stored in an Exchange Online, Exchange Online as part of Office 365, or Exchange on-premises mailbox.</span></span> <span data-ttu-id="d7dd9-106">EWS usa protocolos padrão da web para fornecer acesso a um servidor do Exchange; bibliotecas como a [API gerenciada de EWS](get-started-with-ews-managed-api-client-applications.md) quebrar as operações de EWS para fornecer uma interface orientado a objetos.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-106">EWS uses standard web protocols to provide access to an Exchange server; libraries like the [EWS Managed API](get-started-with-ews-managed-api-client-applications.md) wrap the EWS operations to provide an object-oriented interface.</span></span> <span data-ttu-id="d7dd9-107">Depois de executar os exemplos neste artigo, você terá uma noção básica do que você pode fazer com o EWS.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-107">After you've run the examples in this article, you will have a basic understanding of what you can do with EWS.</span></span> 
  
<span data-ttu-id="d7dd9-108">É possível chamar operações EWS em qualquer sistema operacional ou idioma, como as solicitações do EWS e respostas utilizam o protocolo SOAP.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-108">You can call EWS operations from any operating system or language, because the EWS requests and responses use the SOAP protocol.</span></span> <span data-ttu-id="d7dd9-109">Os exemplos neste artigo são gravados usando c# e fazer uso do .NET Framework objetos [HttpWebRequest](https://msdn.microsoft.com/library/System.Net.HttpWebRequest.aspx) e [HttpWebResponse](https://msdn.microsoft.com/library/System.Net.HttpWebResponse.aspx) ; No entanto, a parte importante do código é o XML usado para fazer com que a solicitação do EWS e a resposta XML retornada do servidor.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-109">The examples in this article are written using C# and make use of the .NET Framework [HttpWebRequest](https://msdn.microsoft.com/library/System.Net.HttpWebRequest.aspx) and [HttpWebResponse](https://msdn.microsoft.com/library/System.Net.HttpWebResponse.aspx) objects; however, the important part of the code is the XML used to make the EWS request and the XML response returned from the server.</span></span> <span data-ttu-id="d7dd9-110">Os exemplos de código enfatizam as transações de XML e não o XML de processamento.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-110">The code examples emphasize the XML transactions and not processing the XML.</span></span> 
  
## <a name="youll-need-an-exchange-server"></a><span data-ttu-id="d7dd9-111">Você precisará de um servidor do Exchange</span><span class="sxs-lookup"><span data-stu-id="d7dd9-111">You'll need an Exchange server</span></span>

<span data-ttu-id="d7dd9-112">Se você já tiver uma conta de caixa de correio do Exchange, você poderá ignorar esta etapa.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-112">If you already have an Exchange mailbox account, you can skip this step.</span></span> <span data-ttu-id="d7dd9-113">Caso contrário, você tem as seguintes opções para configurar uma caixa de correio do Exchange para seu primeiro aplicativo EWS:</span><span class="sxs-lookup"><span data-stu-id="d7dd9-113">Otherwise, you have the following options for setting up an Exchange mailbox for your first EWS application:</span></span>
  
- <span data-ttu-id="d7dd9-114">[Obtenha um Site do Office 365 Developer](http://msdn.microsoft.com/en-us/library/office/fp179924.aspx) (recomendado).</span><span class="sxs-lookup"><span data-stu-id="d7dd9-114">[Get an Office 365 Developer Site ](http://msdn.microsoft.com/en-us/library/office/fp179924.aspx)(recommended).</span></span> <span data-ttu-id="d7dd9-115">Esta é a maneira mais rápida de obter uma caixa de correio do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-115">This is the quickest way for you to get an Exchange mailbox.</span></span>
    
- <span data-ttu-id="d7dd9-116">Baixe o [Exchange Server](http://office.microsoft.com/en-us/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).</span><span class="sxs-lookup"><span data-stu-id="d7dd9-116">Download [Exchange Server](http://office.microsoft.com/en-us/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).</span></span>
    
<span data-ttu-id="d7dd9-117">Depois de confirmar que você pode enviar e receber emails do Exchange Server, você estará pronto para configurar seu ambiente de desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-117">After you've verified that you can send and receive email from your Exchange server you are ready to set up your development environment.</span></span> <span data-ttu-id="d7dd9-118">Você pode usar o Outlook Web App para verificar se você pode enviar o email.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-118">You can use Outlook Web App to verify that you can send email.</span></span>
  
<span data-ttu-id="d7dd9-119">Você também precisará saber a URL do ponto de extremidade EWS para seu servidor.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-119">You'll also need to know the URL of the EWS endpoint for your server.</span></span> <span data-ttu-id="d7dd9-120">Em um aplicativo de produção, você usaria [descoberta automática](autodiscover-for-exchange.md) para determinar a URL do EWS.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-120">In a production application, you'd use [Autodiscover](autodiscover-for-exchange.md) to determine the EWS URL.</span></span> <span data-ttu-id="d7dd9-121">Os exemplos neste artigo usam a URL de ponto de extremidade do Office 365 EWS, https://outlook.office365.com/EWS/Exchange.asmx.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-121">The examples in this article use the Office 365 EWS endpoint URL, https://outlook.office365.com/EWS/Exchange.asmx.</span></span> <span data-ttu-id="d7dd9-122">A seção [próximas etapas](#bk_next) tem links para obter mais informações sobre a descoberta automática, quando estiver pronto.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-122">The [Next steps](#bk_next) section has links to more information about Autodiscover when you're ready.</span></span> 
  
<span data-ttu-id="d7dd9-123">Se você estiver testando seu aplicativo usando um servidor do Exchange que tem o certificado autoassinado do padrão, você precisará criar um [método de validação do certificado](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) que atenda aos requisitos de segurança da sua organização.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-123">If you are testing your application using an Exchange server that has the default self-signed certificate, you'll need to create a [certificate validation method](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) that meets the security requirements of your organization.</span></span> 
  
## <a name="set-up-your-development-environment"></a><span data-ttu-id="d7dd9-124">Definir seu ambiente de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="d7dd9-124">Set up your development environment</span></span>

<span data-ttu-id="d7dd9-125">As ferramentas que você usa para criar seu primeiro aplicativo EWS dependem do sistema operacional e o idioma que você use e é principalmente uma questão de preferência.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-125">The tools that you use to create your first EWS application depend on the operating system and language that you use, and are mostly a matter of taste.</span></span> <span data-ttu-id="d7dd9-126">Se você quiser acompanhe os exemplos em c# neste artigo, você precisará:</span><span class="sxs-lookup"><span data-stu-id="d7dd9-126">If you want to follow along with the C# examples in this article, you'll need:</span></span> 
  
- <span data-ttu-id="d7dd9-127">Qualquer versão do Visual Studio que suporta o .NET Framework 4.0.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-127">Any version of Visual Studio that supports the .NET Framework 4.0.</span></span> 
    
- <span data-ttu-id="d7dd9-128">Uma conexão de Internet que sua máquina de desenvolvimento pode usar para contatar o servidor do Exchange.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-128">An Internet connection that your development machine can use to contact your Exchange server.</span></span> <span data-ttu-id="d7dd9-129">Se você pode usar o Outlook Web App com um nome DNS em vez de um endereço IP para se conectar ao seu servidor do Exchange, você estiver configurado.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-129">If you can use Outlook Web App with a DNS name rather than an IP address to connect to your Exchange server, you are set up.</span></span>
    
## <a name="create-your-first-ews-application"></a><span data-ttu-id="d7dd9-130">Crie seu primeiro aplicativo de EWS</span><span class="sxs-lookup"><span data-stu-id="d7dd9-130">Create your first EWS application</span></span>

<span data-ttu-id="d7dd9-131">Os aplicativos do EWS que você irá criar mostra dois cenários típicos de usando o EWS:</span><span class="sxs-lookup"><span data-stu-id="d7dd9-131">The EWS application that you will create shows two typical scenarios for using EWS:</span></span>
  
1. <span data-ttu-id="d7dd9-132">Obtenha informações de uma caixa de correio do Exchange e exibir essas informações ao usuário.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-132">Get information from an Exchange mailbox and display that information to the user.</span></span>
    
2. <span data-ttu-id="d7dd9-133">Executar uma ação, por exemplo, enviar um email e verifique a resposta para ver se a ação foi bem-sucedida.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-133">Perform an action, such as sending an email, and check the response to see if the action succeeded.</span></span>
    
<span data-ttu-id="d7dd9-134">Vamos começar.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-134">Let's get started.</span></span>
  
### <a name="set-up-the-solution"></a><span data-ttu-id="d7dd9-135">Configurar a solução</span><span class="sxs-lookup"><span data-stu-id="d7dd9-135">Set up the solution</span></span>

<span data-ttu-id="d7dd9-136">Primeiro, crie uma nova solução de aplicativo de console usando o Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-136">First, create a new console application solution using Visual Studio.</span></span> <span data-ttu-id="d7dd9-137">Quando a solução estiver pronta, crie um novo objeto chamado Tracing.cs.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-137">When the solution is ready, create a new object called Tracing.cs.</span></span> <span data-ttu-id="d7dd9-138">Use este objeto para gravar informações sobre o console e um arquivo de log para que você possa examinar os resultados após a execução do seu código.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-138">Use this object to write information to both the console and a log file so that you can review the results after you run your code.</span></span> <span data-ttu-id="d7dd9-139">Cole o código a seguir no arquivo Tracing.cs.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-139">Paste the following code into the Tracing.cs file.</span></span>
  
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

<span data-ttu-id="d7dd9-140">Em seguida, abra o arquivo de Module. vb.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-140">Next, open the Program.cs file.</span></span> <span data-ttu-id="d7dd9-141">Você colocará o restante do código para o exemplo neste arquivo.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-141">You will put the rest of the code for the example in this file.</span></span>
  
<span data-ttu-id="d7dd9-142">Primeiro, configure o shell do programa.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-142">First, set up the shell of the program.</span></span> <span data-ttu-id="d7dd9-143">O programa será:</span><span class="sxs-lookup"><span data-stu-id="d7dd9-143">The program will:</span></span> 
  
1. <span data-ttu-id="d7dd9-144">Crie um arquivo de log para que a solicitação e a resposta podem ser gravados em disco para estudo posterior.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-144">Create a log file so that the request and response can be written to disk for later study.</span></span>
    
2. <span data-ttu-id="d7dd9-145">Obtenha o endereço de email e a senha da conta que você acessará.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-145">Get the email address and password of the account that you'll access.</span></span>
    
3. <span data-ttu-id="d7dd9-146">Chame os métodos de amostra.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-146">Call the sample methods.</span></span>
    
<span data-ttu-id="d7dd9-147">Substituir o `Main` método no Module. vb com o código a seguir.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-147">Replace the  `Main` method in the Program.cs with the following code.</span></span> 
  
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

<span data-ttu-id="d7dd9-148">A última coisa que você precisa fazer é adicionar o `GetPasswordFromConsole` método estático.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-148">The last thing that you need to do is add the  `GetPasswordFromConsole` static method.</span></span> <span data-ttu-id="d7dd9-149">Esse método retorna um objeto de [SecureString](https://msdn.microsoft.com/library/System.Security.SecureString.aspx) que contém uma senha digitada no console.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-149">This method returns a [SecureString](https://msdn.microsoft.com/library/System.Security.SecureString.aspx) object that contains a password typed at the console.</span></span> 
  
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

### <a name="get-the-number-of-new-messages-in-an-inbox"></a><span data-ttu-id="d7dd9-150">Obter o número de novas mensagens em uma caixa de entrada</span><span class="sxs-lookup"><span data-stu-id="d7dd9-150">Get the number of new messages in an Inbox</span></span>

<span data-ttu-id="d7dd9-151">Uma operação comum em um aplicativo do EWS é obter informações sobre mensagens de email, compromissos, reuniões e as pastas que armazenam-los.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-151">A common operation in an EWS application is to get information about email messages, appointments, meetings, and the folders that store them.</span></span> <span data-ttu-id="d7dd9-152">Este exemplo obtém o número de mensagens na caixa de entrada da conta e exibe o número total de mensagens e o número de mensagens não lidas.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-152">This example gets the number of messages in an account's Inbox and displays the total number of messages and the number of unread messages.</span></span> <span data-ttu-id="d7dd9-153">Demonstra as seguintes ações comuns para aplicativos do EWS:</span><span class="sxs-lookup"><span data-stu-id="d7dd9-153">It demonstrates the following common actions for EWS applications:</span></span>
  
- <span data-ttu-id="d7dd9-154">Fazendo uma solicitação EWS para o Exchange server.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-154">Making an EWS request to the Exchange server.</span></span>
    
- <span data-ttu-id="d7dd9-155">Analisando a resposta XML retornada para as informações solicitadas.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-155">Parsing the returned XML response for the requested information.</span></span>
    
- <span data-ttu-id="d7dd9-156">Lidando com as exceções comuns e mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-156">Handling common exceptions and error messages.</span></span>
    
<span data-ttu-id="d7dd9-157">Adicione o seguinte código para o `ShowNumberOfMessagesInInbox` método que foi oculto após o método principal.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-157">Add the following code to the  `ShowNumberOfMessagesInInbox` method that was stubbed out after the main method.</span></span> <span data-ttu-id="d7dd9-158">Quando você executa o aplicativo, ele será impresso o número de mensagens na caixa de entrada da conta e o número de mensagens não lidas na caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-158">When you run the application, it will print the number of messages in the account's Inbox and the number of unread messages in the Inbox.</span></span> <span data-ttu-id="d7dd9-159">Depois de executar o aplicativo, você pode abrir o arquivo GetStartedWithEWS.log para ver a solicitação XML que foi enviada para o Exchange server e a resposta que o servidor é retornado.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-159">After you run the application, you can open the GetStartedWithEWS.log file to see the XML request that was sent to the Exchange server and the response that the server returned.</span></span> 
  
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

### <a name="send-an-email-message"></a><span data-ttu-id="d7dd9-160">Enviar uma mensagem de email</span><span class="sxs-lookup"><span data-stu-id="d7dd9-160">Send an email message</span></span>

<span data-ttu-id="d7dd9-161">Outra operação comum para um aplicativo do EWS deve enviar mensagens de email ou solicitações de reunião.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-161">Another common operation for an EWS application is to send email messages or meeting requests.</span></span> <span data-ttu-id="d7dd9-162">Este exemplo cria e envia uma mensagem de email usando as credenciais de usuário que foram inseridas anteriormente.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-162">This example creates and sends an email message using the user credentials that were entered earlier.</span></span> <span data-ttu-id="d7dd9-163">Demonstra essas tarefas comuns de aplicativos do EWS:</span><span class="sxs-lookup"><span data-stu-id="d7dd9-163">It demonstrates these common EWS application tasks:</span></span>
  
- <span data-ttu-id="d7dd9-164">Criando e enviando um email.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-164">Creating and sending an email.</span></span>
    
- <span data-ttu-id="d7dd9-165">Analisando a resposta XML retornada para determinar se o email foi enviado corretamente.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-165">Parsing the returned XML response to determine if the email was correctly sent.</span></span>
    
- <span data-ttu-id="d7dd9-166">Lidando com as exceções comuns e mensagens de erro.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-166">Handling common exceptions and error messages.</span></span>
    
<span data-ttu-id="d7dd9-167">Adicione o seguinte código para o método SendTestEmail que foi oculto após o método principal.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-167">Add the following code to the SendTestEmail method that was stubbed out after the main method.</span></span> <span data-ttu-id="d7dd9-168">Depois de executar o aplicativo, você pode abrir o arquivo GetStartedWithEWS.log para ver a solicitação XML que foi enviada para o Exchange server e a resposta que o servidor é retornado.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-168">After you run the application, you can open the GetStartedWithEWS.log file to see the XML request that was sent to the Exchange server and the response that the server returned.</span></span>
  
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

## <a name="next-steps"></a><span data-ttu-id="d7dd9-169">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="d7dd9-169">Next steps</span></span>

<span data-ttu-id="d7dd9-170">Agora que você escreveu seu primeiro aplicativo EWS, você está pronto para descobrir outras maneiras de usar o EWS.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-170">Now that you've written your first EWS application, you're ready to discover other ways to use EWS.</span></span> <span data-ttu-id="d7dd9-171">Aqui estão algumas ideias para você começar:</span><span class="sxs-lookup"><span data-stu-id="d7dd9-171">Here are some ideas to get you started:</span></span>
  
- <span data-ttu-id="d7dd9-172">Implemente a [descoberta automática](autodiscover-for-exchange.md) no seu aplicativo para que seu aplicativo se conectará ao servidor do Exchange correto, com base no endereço de email do usuário.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-172">Implement [Autodiscover](autodiscover-for-exchange.md) in your application so that your application will connect to the correct Exchange server based on the user's email address.</span></span> <span data-ttu-id="d7dd9-173">Consulte também o [Exchange 2013: obter configurações de usuário com a descoberta automática](http://code.msdn.microsoft.com/Exchange-2013-Get-user-7e22c86e) amostra.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-173">See also the [Exchange 2013: Get user settings with Autodiscover](http://code.msdn.microsoft.com/Exchange-2013-Get-user-7e22c86e) sample.</span></span> 
    
- <span data-ttu-id="d7dd9-174">Examine a [referência do EWS](http://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx) para obter mais informações sobre o EWS.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-174">Look at the [EWS reference](http://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx) for more information about EWS.</span></span> 
    
- <span data-ttu-id="d7dd9-175">Consulte as [operações do EWS](http://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx) para obter informações sobre as operações que estão disponíveis.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-175">See the [EWS operations](http://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx) for information about the operations that are available.</span></span> 
    
- <span data-ttu-id="d7dd9-176">Use o [Editor do EWS](http://ewseditor.codeplex.com/) para ver o tráfego SOAP enviado de e para o servidor.</span><span class="sxs-lookup"><span data-stu-id="d7dd9-176">Use [EWS Editor](http://ewseditor.codeplex.com/) to see the SOAP traffic sent to and from the server.</span></span> 
    
<span data-ttu-id="d7dd9-177">Se você tiver algum problema com o seu aplicativo, [Experimente postar uma pergunta ou um comentário no fórum](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) (e não se esqueça de ler o primeiro post).</span><span class="sxs-lookup"><span data-stu-id="d7dd9-177">If you run into any issues with your application, [try posting a question or comment in the forum](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) (and don't forget to read the first post).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="d7dd9-178">Confira também</span><span class="sxs-lookup"><span data-stu-id="d7dd9-178">See also</span></span>

- [<span data-ttu-id="d7dd9-179">Start using web services in Exchange</span><span class="sxs-lookup"><span data-stu-id="d7dd9-179">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)   
- [<span data-ttu-id="d7dd9-180">Explorar a API Gerenciada pelo EWS, EWS e serviços Web no Exchange</span><span class="sxs-lookup"><span data-stu-id="d7dd9-180">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) 
- [<span data-ttu-id="d7dd9-181">Visão geral de design de cliente do EWS do Exchange</span><span class="sxs-lookup"><span data-stu-id="d7dd9-181">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)   
- [<span data-ttu-id="d7dd9-182">Develop web service clients for Exchange</span><span class="sxs-lookup"><span data-stu-id="d7dd9-182">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)  
- [<span data-ttu-id="d7dd9-183">Introdução aos aplicativos de cliente API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="d7dd9-183">Get started with EWS Managed API client applications</span></span>](get-started-with-ews-managed-api-client-applications.md)
    

