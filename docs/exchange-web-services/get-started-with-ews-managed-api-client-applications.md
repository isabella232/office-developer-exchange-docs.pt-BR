---
title: Introdução aos aplicativos clientes de API gerenciada por EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c2267733-6f4f-49e5-9614-1e4a24c3af1a
description: Desenvolva um aplicativo de cliente de email Hello World simple do Exchange usando a API gerenciada de EWS.
ms.openlocfilehash: dafc8cbbf172ad725ab83c93553464ba96ef33b8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19750678"
---
# <a name="get-started-with-ews-managed-api-client-applications"></a><span data-ttu-id="e67ef-103">Introdução aos aplicativos clientes de API gerenciada por EWS</span><span class="sxs-lookup"><span data-stu-id="e67ef-103">Get started with EWS Managed API client applications</span></span>

<span data-ttu-id="e67ef-104">Desenvolva um aplicativo de cliente de email Hello World simple do Exchange usando a API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="e67ef-104">Develop a simple Hello World email client application for Exchange by using the EWS Managed API.</span></span> 
  
<span data-ttu-id="e67ef-105">A [API gerenciada de EWS](http://aka.ms/ews-managed-api-readme) fornece um modelo de objeto intuitivo e fácil de usar para envio e recebimento de mensagens do serviço web de aplicativos clientes, aplicativos de portal e aplicativos de serviço.</span><span class="sxs-lookup"><span data-stu-id="e67ef-105">The [EWS Managed API](http://aka.ms/ews-managed-api-readme) provides an intuitive, easy-to-use object model for sending and receiving web service messages from client applications, portal applications, and service applications.</span></span> <span data-ttu-id="e67ef-106">Você pode acessar quase todas as informações armazenadas em um Exchange Online, Exchange Online como parte do Office 365 ou uma caixa de correio do Exchange server usando a API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="e67ef-106">You can access almost all the information stored in an Exchange Online, Exchange Online as part of Office 365, or an Exchange server mailbox by using the EWS Managed API.</span></span> <span data-ttu-id="e67ef-107">Você pode usar as informações neste artigo para ajudá-lo a desenvolver seu primeiro aplicativo cliente EWS Managed API.</span><span class="sxs-lookup"><span data-stu-id="e67ef-107">You can use the information in this article to help you develop your first EWS Managed API client application.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="e67ef-108">A API gerenciada de EWS agora está disponível como um projeto de código aberto no [GitHub](https://github.com/officedev/ews-managed-api).</span><span class="sxs-lookup"><span data-stu-id="e67ef-108">The EWS Managed API is now available as an open source project on [GitHub](https://github.com/officedev/ews-managed-api).</span></span> <span data-ttu-id="e67ef-109">Você pode usar a biblioteca de fonte aberta: > correções e melhorias para a API de colaboração.</span><span class="sxs-lookup"><span data-stu-id="e67ef-109">You can use the open source library to: >  Contribute bug fixes and enhancements to the API.</span></span> <span data-ttu-id="e67ef-110">> Obtenha correções e aprimoramentos antes que estejam disponíveis em um lançamento oficial.</span><span class="sxs-lookup"><span data-stu-id="e67ef-110">>  Get fixes and enhancements before they are available in an official release.</span></span> <span data-ttu-id="e67ef-111">> Acesso a implementação mais abrangente e atualizado da API, para usar como uma referência ou para criar novas bibliotecas em plataformas novas.</span><span class="sxs-lookup"><span data-stu-id="e67ef-111">>  Access the most comprehensive and up-to-date implementation of the API, to use as a reference or to create new libraries on new platforms.</span></span> <span data-ttu-id="e67ef-112">> Bem-vindos suas [contribuições](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub.</span><span class="sxs-lookup"><span data-stu-id="e67ef-112">>  We welcome your [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub.</span></span> 
  
## <a name="youll-need-an-exchange-server"></a><span data-ttu-id="e67ef-113">Você precisará de um servidor do Exchange</span><span class="sxs-lookup"><span data-stu-id="e67ef-113">You'll need an Exchange server</span></span>
<span data-ttu-id="e67ef-114"><a name="NeedExchange"> </a></span><span class="sxs-lookup"><span data-stu-id="e67ef-114"></span></span>

<span data-ttu-id="e67ef-115">Se você já tiver uma conta de caixa de correio do Exchange, você poderá ignorar esta seção.</span><span class="sxs-lookup"><span data-stu-id="e67ef-115">If you already have an Exchange mailbox account, you can skip this section.</span></span> <span data-ttu-id="e67ef-116">Caso contrário, você tem as seguintes opções para configurar uma caixa de correio do Exchange para seu primeiro aplicativo cliente EWS:</span><span class="sxs-lookup"><span data-stu-id="e67ef-116">Otherwise, you have the following options for setting up an Exchange mailbox for your first EWS client application:</span></span>
  
- <span data-ttu-id="e67ef-117">Obtenha um [Site do desenvolvedor do Office 365](http://msdn.microsoft.com/en-us/library/office/fp179924.aspx) (recomendado).</span><span class="sxs-lookup"><span data-stu-id="e67ef-117">Get an [Office 365 Developer Site](http://msdn.microsoft.com/en-us/library/office/fp179924.aspx) (recommended).</span></span> <span data-ttu-id="e67ef-118">Esta é a maneira mais rápida para configurar uma caixa de correio do Exchange.</span><span class="sxs-lookup"><span data-stu-id="e67ef-118">This is the quickest way for you to set up an Exchange mailbox.</span></span> 
    
- <span data-ttu-id="e67ef-119">Baixe o [Exchange Server](http://office.microsoft.com/en-us/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).</span><span class="sxs-lookup"><span data-stu-id="e67ef-119">Download [Exchange Server](http://office.microsoft.com/en-us/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).</span></span>
    
<span data-ttu-id="e67ef-120">Após ter verificado que você pode enviar e receber emails do Exchange, você estará pronto para configurar o ambiente de desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="e67ef-120">After you have verified that you can send and receive email from Exchange, you are ready to set up your development environment.</span></span> <span data-ttu-id="e67ef-121">Você pode usar o cliente do Exchange web do [Outlook Web App](http://technet.microsoft.com/en-us/library/jj657718%28v=exchg.150%29.aspx) para verificar se você pode enviar o email.</span><span class="sxs-lookup"><span data-stu-id="e67ef-121">You can use the Exchange web client [Outlook Web App](http://technet.microsoft.com/en-us/library/jj657718%28v=exchg.150%29.aspx) to verify that you can send email.</span></span> 
  
## <a name="set-up-your-development-environment"></a><span data-ttu-id="e67ef-122">Definir seu ambiente de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="e67ef-122">Set up your development environment</span></span>
<span data-ttu-id="e67ef-123"><a name="Setup"> </a></span><span class="sxs-lookup"><span data-stu-id="e67ef-123"></span></span>

<span data-ttu-id="e67ef-124">Certifique-se de que você tenha acesso ao seguinte:</span><span class="sxs-lookup"><span data-stu-id="e67ef-124">Make sure that you have access to the following:</span></span>
  
- <span data-ttu-id="e67ef-125">Qualquer versão do [Visual Studio](http://www.visualstudio.com/en-us/downloads/download-visual-studio-vs.aspx) que suporta o .NET Framework 4.</span><span class="sxs-lookup"><span data-stu-id="e67ef-125">Any version of [Visual Studio](http://www.visualstudio.com/en-us/downloads/download-visual-studio-vs.aspx) that supports the .NET Framework 4.</span></span> <span data-ttu-id="e67ef-126">Embora tecnicamente, Visual Studio não é necessário porque você pode usar qualquer compilador c#, recomendamos que você usá-lo.</span><span class="sxs-lookup"><span data-stu-id="e67ef-126">Although technically, you don't need Visual Studio because you can use any C# compiler, we recommend that you use it.</span></span> 
    
- <span data-ttu-id="e67ef-127">A [API gerenciada de EWS](http://aka.ms/ews-managed-api-readme).</span><span class="sxs-lookup"><span data-stu-id="e67ef-127">The [EWS Managed API](http://aka.ms/ews-managed-api-readme).</span></span> <span data-ttu-id="e67ef-128">Você pode usar tanto a versão de 32 bits ou 64 bits, dependendo do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="e67ef-128">You can use either the 64-bit or 32-bit version, depending on your system.</span></span> <span data-ttu-id="e67ef-129">Use o local de instalação padrão.</span><span class="sxs-lookup"><span data-stu-id="e67ef-129">Use the default installation location.</span></span> 
    
## <a name="create-your-first-ews-managed-api-application"></a><span data-ttu-id="e67ef-130">Crie seu primeiro aplicativo de API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="e67ef-130">Create your first EWS Managed API application</span></span>
<span data-ttu-id="e67ef-131"><a name="Create"> </a></span><span class="sxs-lookup"><span data-stu-id="e67ef-131"></span></span>

<span data-ttu-id="e67ef-132">Essas etapas pressupõem que você configure um Site do desenvolvedor do Office 365.</span><span class="sxs-lookup"><span data-stu-id="e67ef-132">These steps assume that you set up an Office 365 Developer Site.</span></span> <span data-ttu-id="e67ef-133">Se você baixar e instalar o Exchange, você precisará [instalar um certificado válido](http://technet.microsoft.com/en-us/library/bb310769%28v=exchg.141%29.aspx) no seu Exchange server ou a [implementação de uma validação de certificado](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) retorno de chamada para um certificado autoassinado é fornecido por padrão.</span><span class="sxs-lookup"><span data-stu-id="e67ef-133">If you downloaded and installed Exchange, you will need to [install a valid certificate](http://technet.microsoft.com/en-us/library/bb310769%28v=exchg.141%29.aspx) on your Exchange server or [implement a certificate validation](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) callback for a self-signed certificate that is provided by default.</span></span> <span data-ttu-id="e67ef-134">Observe também que estas etapas podem variar ligeiramente dependendo da versão do Visual Studio que você está usando.</span><span class="sxs-lookup"><span data-stu-id="e67ef-134">Also note that these steps might vary slightly depending on the version of Visual Studio that you are using.</span></span> 
  
### <a name="step-1-create-a-project-in-visual-studio"></a><span data-ttu-id="e67ef-135">Etapa 1: Criar um projeto no Visual Studio</span><span class="sxs-lookup"><span data-stu-id="e67ef-135">Step 1: Create a project in Visual Studio</span></span>

1. <span data-ttu-id="e67ef-136">No Visual Studio, no menu **arquivo** , escolha **novo**e, em seguida, selecione o **projeto**.</span><span class="sxs-lookup"><span data-stu-id="e67ef-136">In Visual Studio, on the **File** menu, choose **New**, and then choose **Project**.</span></span> <span data-ttu-id="e67ef-137">Abre a caixa de diálogo **Novo projeto**.</span><span class="sxs-lookup"><span data-stu-id="e67ef-137">The **New Project** dialog box opens.</span></span> 
    
2. <span data-ttu-id="e67ef-138">Crie um **aplicativo de Console do c#**.</span><span class="sxs-lookup"><span data-stu-id="e67ef-138">Create a **C# Console Application**.</span></span> <span data-ttu-id="e67ef-139">No painel **modelos** , escolha **Visual c#** e, em seguida, escolha o **Aplicativo de Console**.</span><span class="sxs-lookup"><span data-stu-id="e67ef-139">From the **Templates** pane, choose **Visual C#**, and then choose **Console Application**.</span></span> 
    
3. <span data-ttu-id="e67ef-140">Nome do projeto HelloWorld e escolha **Okey**.</span><span class="sxs-lookup"><span data-stu-id="e67ef-140">Name the project HelloWorld, and then choose **OK**.</span></span>
    
<span data-ttu-id="e67ef-141">Visual Studio cria o projeto e abre a janela de documento de código Module. vb.</span><span class="sxs-lookup"><span data-stu-id="e67ef-141">Visual Studio creates the project and opens the Program.cs code document window.</span></span>

### <a name="step-2-add-a-reference-to-the-ews-managed-api"></a><span data-ttu-id="e67ef-142">Etapa 2: Adicionar uma referência para a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="e67ef-142">Step 2: Add a reference to the EWS Managed API</span></span>

1. <span data-ttu-id="e67ef-143">Se a janela **Explorador** de soluções já estiver aberta, ignore esta etapa e vá para a etapa 2.</span><span class="sxs-lookup"><span data-stu-id="e67ef-143">If the **Solution Explorer** window is already open, skip this step and proceed to step 2.</span></span> <span data-ttu-id="e67ef-144">Para abrir a janela **Solution Explorer** , no menu **Exibir** , escolha **Solution Explorer**.</span><span class="sxs-lookup"><span data-stu-id="e67ef-144">To open the **Solution Explorer** window, on the **View** menu, choose **Solution Explorer**.</span></span> 
    
2. <span data-ttu-id="e67ef-145">No **Solution Explorer** e o projeto **HelloWorld** , abra o menu de atalho (botão direito do mouse) para **referências** e escolha **Adicionar referência** no menu de contexto.</span><span class="sxs-lookup"><span data-stu-id="e67ef-145">In the **Solution Explorer** and the **HelloWorld** project, open the shortcut menu (right-click) for **References** and choose **Add Reference** from the context menu.</span></span> <span data-ttu-id="e67ef-146">Uma caixa de diálogo de gerenciamento de referências de projeto será aberta.</span><span class="sxs-lookup"><span data-stu-id="e67ef-146">A dialog box for managing project references will open.</span></span> 
    
3. <span data-ttu-id="e67ef-147">Escolha a opção **Procurar** .</span><span class="sxs-lookup"><span data-stu-id="e67ef-147">Choose the **Browse** option.</span></span> <span data-ttu-id="e67ef-148">Navegue até o local onde você instalou a DLL de API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="e67ef-148">Browse to the location where you installed the EWS Managed API DLL.</span></span> <span data-ttu-id="e67ef-149">O caminho padrão definido pelo instalador é o seguinte: C:\Program Files\Microsoft\Exchange\Web serviços\<versão >\.</span><span class="sxs-lookup"><span data-stu-id="e67ef-149">The default path set by the installer is the following: C:\Program Files\Microsoft\Exchange\Web Services\<version>\.</span></span> <span data-ttu-id="e67ef-150">O caminho pode variar com base em se você baixe o 32 ou a versão de 64 bits do Microsoft.Exchange.WebServices.dll.</span><span class="sxs-lookup"><span data-stu-id="e67ef-150">The path can vary based on whether you download the 32 or 64 bit version of the Microsoft.Exchange.WebServices.dll.</span></span> <span data-ttu-id="e67ef-151">Escolha **Microsoft.Exchange.WebServices.dll** e selecione **Okey** ou **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="e67ef-151">Choose **Microsoft.Exchange.WebServices.dll** and select **OK** or **Add**.</span></span> <span data-ttu-id="e67ef-152">Isso adiciona a referência de API gerenciada de EWS ao seu projeto.</span><span class="sxs-lookup"><span data-stu-id="e67ef-152">This adds the EWS Managed API reference to your project.</span></span> 
    
4. <span data-ttu-id="e67ef-153">Se você estiver usando o EWS gerenciadas API 2.0, altere o projeto HelloWorld para direcionar o .NET Framework 4.</span><span class="sxs-lookup"><span data-stu-id="e67ef-153">If you are using EWS Managed API 2.0, change the HelloWorld project to target the .NET Framework 4.</span></span> <span data-ttu-id="e67ef-154">Outras versões do EWS Managed API podem usar uma versão de destino diferente do .NET Framework.</span><span class="sxs-lookup"><span data-stu-id="e67ef-154">Other versions of the EWS Managed API might use a different target version of the .NET Framework.</span></span>
    
5. <span data-ttu-id="e67ef-155">Confirme que você está usando a versão de destino correto do .NET Framework.</span><span class="sxs-lookup"><span data-stu-id="e67ef-155">Confirm that you are using the correct target version of the .NET Framework.</span></span> <span data-ttu-id="e67ef-156">Abra o menu de atalho (botão direito do mouse) para o seu projeto **HelloWorld** no **Solution Explorer**e escolha **Propriedades**.</span><span class="sxs-lookup"><span data-stu-id="e67ef-156">Open the shortcut menu (right-click) for your **HelloWorld** project in the **Solution Explorer**, and choose **Properties**.</span></span> <span data-ttu-id="e67ef-157">Verifique se o **.NET Framework 4** é selecionado na caixa de lista suspensa de **estrutura de destino** .</span><span class="sxs-lookup"><span data-stu-id="e67ef-157">Verify that the **.NET Framework 4** is selected in the **Target framework** drop-down box.</span></span> 
    
<span data-ttu-id="e67ef-158">Agora que você ter seu projeto configurado e você criou uma referência para a API gerenciada de EWS, você estará pronto para criar seu primeiro aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e67ef-158">Now that you have your project set up and you created a reference to the EWS Managed API, you are ready to create your first application.</span></span> <span data-ttu-id="e67ef-159">Para manter a simplicidade, adicione o código no arquivo Module. vb.</span><span class="sxs-lookup"><span data-stu-id="e67ef-159">To keep things simple, add your code to the Program.cs file.</span></span> <span data-ttu-id="e67ef-160">Leia [o assembly do EWS Managed API de referência](how-to-reference-the-ews-managed-api-assembly.md) para obter mais informações sobre como fazer referência a API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="e67ef-160">Read [Reference the EWS Managed API assembly](how-to-reference-the-ews-managed-api-assembly.md) for more information about referencing the EWS Managed API.</span></span> <span data-ttu-id="e67ef-161">Na próxima etapa, você irá desenvolver o código básico para gravar o cliente de API gerenciada de EWS a maioria dos aplicativos.</span><span class="sxs-lookup"><span data-stu-id="e67ef-161">In the next step, you will develop the basic code to write most EWS Managed API client applications.</span></span> 
### <a name="step-3-set-up-url-redirection-validation-for-autodiscover"></a><span data-ttu-id="e67ef-162">Etapa 3: Configurar a validação de redirecionamento de URL de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="e67ef-162">Step 3: Set up URL redirection validation for Autodiscover</span></span>

- <span data-ttu-id="e67ef-163">Adicione o seguinte método de retorno de chamada de validação de redirecionamento após o método **Main (string [] args)** .</span><span class="sxs-lookup"><span data-stu-id="e67ef-163">Add the following redirection validation callback method after the **Main(string[] args)** method.</span></span> <span data-ttu-id="e67ef-164">Isso valida se redirecionado URLs retornado pela [descoberta automática](autodiscover-for-exchange.md) representam um ponto de extremidade HTTPS.</span><span class="sxs-lookup"><span data-stu-id="e67ef-164">This validates whether redirected URLs returned by [Autodiscover](autodiscover-for-exchange.md) represent an HTTPS endpoint.</span></span> 
    
  ```cs
  private static bool RedirectionUrlValidationCallback(string redirectionUrl)
  {
     // The default for the validation callback is to reject the URL.
     bool result = false;
     Uri redirectionUri = new Uri(redirectionUrl);
     // Validate the contents of the redirection URL. In this simple validation
     // callback, the redirection URL is considered valid if it is using HTTPS
     // to encrypt the authentication credentials. 
     if (redirectionUri.Scheme == "https")
     {
        result = true;
     }
     return result;
  }
  ```

<span data-ttu-id="e67ef-165">Esse retorno de chamada de validação será passado para o objeto **ExchangeService** na etapa 4.</span><span class="sxs-lookup"><span data-stu-id="e67ef-165">This validation callback will be passed to the **ExchangeService** object in step 4.</span></span> <span data-ttu-id="e67ef-166">Você precisa para que seu aplicativo será confiar e seguir redirecionamentos de descoberta automática - os resultados do redirecionamento de descoberta automática fornece o ponto de extremidade do EWS para nosso aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e67ef-166">You need this so that your application will trust and follow Autodiscover redirects - the results of the Autodiscover redirect provides the EWS endpoint for our application.</span></span> 

### <a name="step-4-prepare-the-exchangeservice-object"></a><span data-ttu-id="e67ef-167">Etapa 4: Preparar o objeto ExchangeService</span><span class="sxs-lookup"><span data-stu-id="e67ef-167">Step 4: Prepare the ExchangeService object</span></span>

1. <span data-ttu-id="e67ef-168">Adicione uma referência de diretiva **usando** para a API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="e67ef-168">Add a **using** directive reference to the EWS Managed API.</span></span> <span data-ttu-id="e67ef-169">Adicione o código a seguir após a última diretiva **using** na parte superior da Module. vb.</span><span class="sxs-lookup"><span data-stu-id="e67ef-169">Add the following code after the last **using** directive at the top of Program.cs.</span></span> 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

2. <span data-ttu-id="e67ef-170">No método **Main** , instanciar o objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) com a versão do serviço que você pretende de destino.</span><span class="sxs-lookup"><span data-stu-id="e67ef-170">In the **Main** method, instantiate the [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object with the service version you intend to target.</span></span> <span data-ttu-id="e67ef-171">Este exemplo refere-se a versão mais antiga do esquema do EWS.</span><span class="sxs-lookup"><span data-stu-id="e67ef-171">This example targets the earliest version of the EWS schema.</span></span> 
    
   ```cs
    ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);
   ```

3. <span data-ttu-id="e67ef-172">Se você está direcionando um servidor do Exchange no local e seu cliente está unido ao domínio, vá para a etapa 4.</span><span class="sxs-lookup"><span data-stu-id="e67ef-172">If you are targeting an on-premises Exchange server and your client is domain joined, proceed to step 4.</span></span> <span data-ttu-id="e67ef-173">Se você cliente concentrando-se uma caixa de correio do Site do desenvolvedor do Office 365 ou Exchange Online, você precisa passar credenciais explícitas.</span><span class="sxs-lookup"><span data-stu-id="e67ef-173">If you client is targeting an Exchange Online or Office 365 Developer Site mailbox, you have to pass explicit credentials.</span></span> <span data-ttu-id="e67ef-174">Adicione o código a seguir após a instanciação do objeto **ExchangeService** e definir as credenciais para a sua conta de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e67ef-174">Add the following code after the instantiation of the **ExchangeService** object and set the credentials for your mailbox account.</span></span> <span data-ttu-id="e67ef-175">O nome de usuário deve ser o nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="e67ef-175">The user name should be the user principal name.</span></span> <span data-ttu-id="e67ef-176">Vá para a etapa 5.</span><span class="sxs-lookup"><span data-stu-id="e67ef-176">Proceed to step 5.</span></span> 
    
   ```cs
    service.Credentials = new WebCredentials("user1@contoso.com", "password");
   ```

4. <span data-ttu-id="e67ef-177">Clientes do domínio que um servidor do Exchange no local de destino podem usar as credenciais padrão do usuário que está conectado, supondo que as credenciais estão associadas uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e67ef-177">Domain-joined clients that target an on-premises Exchange server can use the default credentials of the user who is logged on, assuming the credentials are associated with a mailbox.</span></span> <span data-ttu-id="e67ef-178">Adicione o código a seguir após a instanciação do objeto **ExchangeService** .</span><span class="sxs-lookup"><span data-stu-id="e67ef-178">Add the following code after the instantiation of the **ExchangeService** object.</span></span> 
    
   ```cs
    service.UseDefaultCredentials = true;
   ```

   <span data-ttu-id="e67ef-179">Se seu cliente destinada a uma caixa de correio do Exchange Online ou o Site do desenvolvedor do Office 365, verifique se que [UseDefaultCredentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.usedefaultcredentials%28v=exchg.80%29.aspx) está definido como **false**, que é o valor padrão.</span><span class="sxs-lookup"><span data-stu-id="e67ef-179">If your client targets an Exchange Online or Office 365 Developer Site mailbox, verify that [UseDefaultCredentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.usedefaultcredentials%28v=exchg.80%29.aspx) is set to **false**, which is the default value.</span></span> <span data-ttu-id="e67ef-180">Seu cliente está pronto para fazer a chamada primeira para o serviço Descoberta automática para obter a URL do serviço de chamadas para o serviço do EWS.</span><span class="sxs-lookup"><span data-stu-id="e67ef-180">Your client is ready to make the first call to the Autodiscover service to get the service URL for calls to the EWS service.</span></span>
    
5. <span data-ttu-id="e67ef-181">O método **AutodiscoverUrl** no objeto **ExchangeService** realiza uma série de chamadas para o serviço de descoberta automática para obter a URL do serviço.</span><span class="sxs-lookup"><span data-stu-id="e67ef-181">The **AutodiscoverUrl** method on the **ExchangeService** object performs a series of calls to the Autodiscover service to get the service URL.</span></span> <span data-ttu-id="e67ef-182">Se essa chamada de método tiver êxito, a propriedade URL no objeto **ExchangeService** será definida com a URL do serviço.</span><span class="sxs-lookup"><span data-stu-id="e67ef-182">If this method call is successful, the URL property on the **ExchangeService** object will be set with the service URL.</span></span> <span data-ttu-id="e67ef-183">Passe o endereço de email do usuário e o **RedirectionUrlValidationCallback** para o método **AutodiscoverUrl** .</span><span class="sxs-lookup"><span data-stu-id="e67ef-183">Pass the user's email address and the **RedirectionUrlValidationCallback** to the **AutodiscoverUrl** method.</span></span> <span data-ttu-id="e67ef-184">Depois que as credenciais tiverem sido especificadas na etapa 3 ou 4, adicione o código a seguir.</span><span class="sxs-lookup"><span data-stu-id="e67ef-184">Add the following code after the credentials have been specified in step 3 or 4.</span></span> <span data-ttu-id="e67ef-185">Alterar `user1@contoso.com` para seu email para que o serviço Descoberta automática encontra seu ponto de extremidade do EWS de endereços.</span><span class="sxs-lookup"><span data-stu-id="e67ef-185">Change  `user1@contoso.com` to your email address so that the Autodiscover service finds your EWS endpoint.</span></span> 
    
   ```cs
    service.AutodiscoverUrl("user1@contoso.com", RedirectionUrlValidationCallback);
   ```

<span data-ttu-id="e67ef-186">Neste ponto, seu cliente estiver configurado para fazer chamadas para o EWS para acessar dados de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e67ef-186">At this point, your client is set up to make calls to EWS to access mailbox data.</span></span> <span data-ttu-id="e67ef-187">Se você executar o seu código agora, você pode verificar se a chamada do método **AutodiscoverUrl** funcionou examinando o conteúdo da propriedade [ExchangeService.Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e67ef-187">If you run your code now, you can verify that the **AutodiscoverUrl** method call worked by examining the contents of the [ExchangeService.Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) property.</span></span> <span data-ttu-id="e67ef-188">Se essa propriedade contém uma URL, sua chamada foi um sucesso!</span><span class="sxs-lookup"><span data-stu-id="e67ef-188">If this property contains a URL, your call was a success!</span></span> <span data-ttu-id="e67ef-189">Isso significa que seu aplicativo com êxito autenticado com o serviço e descoberto o ponto de extremidade do EWS para sua caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="e67ef-189">This means that your application successfully authenticated with the service and discovered the EWS endpoint for your mailbox.</span></span> <span data-ttu-id="e67ef-190">Agora você está pronto para fazer primeira suas chamadas EWS.</span><span class="sxs-lookup"><span data-stu-id="e67ef-190">Now you are ready to make your first calls to EWS.</span></span> <span data-ttu-id="e67ef-191">Leia a [definir a URL do serviço do EWS usando a API gerenciada de EWS](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md) para obter mais informações sobre como definir a URL do EWS.</span><span class="sxs-lookup"><span data-stu-id="e67ef-191">Read [Set the EWS service URL by using the EWS Managed API](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md) for more information about setting the EWS URL.</span></span> 

### <a name="step-6-create-your-first-hello-world-email-message"></a><span data-ttu-id="e67ef-192">Etapa 6: Criar sua primeira mensagem de email Olá mundo</span><span class="sxs-lookup"><span data-stu-id="e67ef-192">Step 6: Create your first Hello World email message</span></span>

1. <span data-ttu-id="e67ef-193">Após chamar o método **AutodiscoverUrl** , instanciar um novo objeto **EmailMessage** e passe o objeto de serviço que você criou.</span><span class="sxs-lookup"><span data-stu-id="e67ef-193">After the **AutodiscoverUrl** method call, instantiate a new **EmailMessage** object and pass in the service object you created.</span></span> 
    
   ```cs
    EmailMessage email = new EmailMessage(service);
   ```

   <span data-ttu-id="e67ef-194">Agora você tem uma mensagem de email no qual a ligação do serviço é definida.</span><span class="sxs-lookup"><span data-stu-id="e67ef-194">You now have an email message on which the service binding is set.</span></span> <span data-ttu-id="e67ef-195">Todas as chamadas iniciadas no objeto **EmailMessage** serão direcionadas no serviço.</span><span class="sxs-lookup"><span data-stu-id="e67ef-195">Any calls initiated on the **EmailMessage** object will be targeted at the service.</span></span> 
    
2. <span data-ttu-id="e67ef-196">Agora definida para: destinatário de linha da mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="e67ef-196">Now set the To: line recipient of the email message.</span></span> <span data-ttu-id="e67ef-197">Para fazer isso, altere `user1@contoso.com` usar seu endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="e67ef-197">To do this, change  `user1@contoso.com` to use your SMTP address.</span></span> 
    
   ```cs
    email.ToRecipients.Add("user1@contoso.com");
   ```

3. <span data-ttu-id="e67ef-198">Defina o assunto e o corpo da mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="e67ef-198">Set the subject and the body of the email message.</span></span>
    
   ```cs
    email.Subject = "HelloWorld";
    email.Body = new MessageBody("This is the first email I've sent by using the EWS Managed API.");
   ```

4. <span data-ttu-id="e67ef-199">Agora você está pronto para enviar sua primeira mensagem de email usando a API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="e67ef-199">You are now ready to send your first email message by using the EWS Managed API.</span></span> <span data-ttu-id="e67ef-200">O método **Send** irá chamar o serviço e enviar a mensagem de email para entrega.</span><span class="sxs-lookup"><span data-stu-id="e67ef-200">The **Send** method will call the service and submit the email message for delivery.</span></span> <span data-ttu-id="e67ef-201">Leia [Communicate with EWS usando a API gerenciada de EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md) para conhecer outros métodos que você pode usar para se comunicar com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="e67ef-201">Read [Communicate with EWS by using the EWS Managed API](how-to-communicate-with-ews-by-using-the-ews-managed-api.md) to learn about other methods you can use to communicate with Exchange.</span></span> 
    
   ```cs
    email.Send();
   ```

5. <span data-ttu-id="e67ef-202">Você está pronto para executar seu aplicativo Hello World.</span><span class="sxs-lookup"><span data-stu-id="e67ef-202">You are ready to run your Hello World application.</span></span> <span data-ttu-id="e67ef-203">No Visual Studio, selecione **F5**.</span><span class="sxs-lookup"><span data-stu-id="e67ef-203">In Visual Studio, select **F5**.</span></span> <span data-ttu-id="e67ef-204">Será aberta uma janela de console em branco.</span><span class="sxs-lookup"><span data-stu-id="e67ef-204">A blank console window will open.</span></span> <span data-ttu-id="e67ef-205">Você não verá algo na janela do console enquanto o seu aplicativo autentica, segue redirecionamentos de descoberta automática e então faz sua chamada primeira para criar uma mensagem de email que você envie para você mesmo.</span><span class="sxs-lookup"><span data-stu-id="e67ef-205">You will not see anything in the console window while your application authenticates, follows Autodiscover redirections, and then makes its first call to create an email message that you send to yourself.</span></span> <span data-ttu-id="e67ef-206">Se você quiser ver as chamadas sejam feitas, adicione as duas linhas de código a seguintes antes do método **AutodiscoverUrl** é chamado.</span><span class="sxs-lookup"><span data-stu-id="e67ef-206">If you want to see the calls being made, add the following two lines of code before the **AutodiscoverUrl** method is called.</span></span> <span data-ttu-id="e67ef-207">Em seguida, pressione F5.</span><span class="sxs-lookup"><span data-stu-id="e67ef-207">Then press F5.</span></span> <span data-ttu-id="e67ef-208">Isso irá [Rastrear check-out do EWS solicitações e respostas](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md) na janela do console.</span><span class="sxs-lookup"><span data-stu-id="e67ef-208">This will [trace out the EWS requests and responses](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md) to the console window.</span></span> 
    
   ```cs
    service.TraceEnabled = true;
    service.TraceFlags = TraceFlags.All;
   ```

<span data-ttu-id="e67ef-209">Agora você tem um aplicativo de cliente do EWS Managed API em funcionamento.</span><span class="sxs-lookup"><span data-stu-id="e67ef-209">You now have a working EWS Managed API client application.</span></span> <span data-ttu-id="e67ef-210">Para sua conveniência, o exemplo a seguir mostra o código que você adicionou à Module. vb para criar seu aplicativo Hello World.</span><span class="sxs-lookup"><span data-stu-id="e67ef-210">For your convenience, the following example shows all the code that you added to Program.cs to create your Hello World application.</span></span>

```cs
using System;
using Microsoft.Exchange.WebServices.Data;
namespace HelloWorld
{
  class Program
  {
    static void Main(string[] args)
    {
      ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);
      service.Credentials = new WebCredentials("user1@contoso.com", "password");
      service.TraceEnabled = true;
      service.TraceFlags = TraceFlags.All;
      service.AutodiscoverUrl("user1@contoso.com", RedirectionUrlValidationCallback);
      EmailMessage email = new EmailMessage(service);
      email.ToRecipients.Add("user1@contoso.com");
      email.Subject = "HelloWorld";
      email.Body = new MessageBody("This is the first email I've sent by using the EWS Managed API");
      email.Send();
    }
    private static bool RedirectionUrlValidationCallback(string redirectionUrl)
    {
      // The default for the validation callback is to reject the URL.
      bool result = false;
      Uri redirectionUri = new Uri(redirectionUrl);
      // Validate the contents of the redirection URL. In this simple validation
      // callback, the redirection URL is considered valid if it is using HTTPS
      // to encrypt the authentication credentials. 
      if (redirectionUri.Scheme == "https")
      {
        result = true;
      }
      return result;
    }
  }
}
```

## <a name="next-steps"></a><span data-ttu-id="e67ef-211">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="e67ef-211">Next steps</span></span>
<span data-ttu-id="e67ef-212"><a name="Next"> </a></span><span class="sxs-lookup"><span data-stu-id="e67ef-212"></span></span>

<span data-ttu-id="e67ef-213">Se você estiver pronto para fazer mais com seu primeiro aplicativo de cliente do EWS Managed API, explore os recursos a seguir:</span><span class="sxs-lookup"><span data-stu-id="e67ef-213">If you're ready to do more with your first EWS Managed API client application, explore the following resources:</span></span>
  
- [<span data-ttu-id="e67ef-214">Exchange 2013:101 amostras de código</span><span class="sxs-lookup"><span data-stu-id="e67ef-214">Exchange 2013: 101 code samples</span></span>](http://code.msdn.microsoft.com/exchange/Exchange-2013-101-Code-3c38582c)
    
- [<span data-ttu-id="e67ef-215">Pastas e itens</span><span class="sxs-lookup"><span data-stu-id="e67ef-215">Folders and items</span></span>](folders-and-items-in-ews-in-exchange.md)
    
- [<span data-ttu-id="e67ef-216">EWSEditor</span><span class="sxs-lookup"><span data-stu-id="e67ef-216">EWSEditor</span></span>](http://ewseditor.codeplex.com/)
    
<span data-ttu-id="e67ef-217">Se você tiver algum problema com o seu aplicativo, [Experimente postar uma pergunta ou um comentário no fórum](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) (e não se esqueça de ler a postagem superior).</span><span class="sxs-lookup"><span data-stu-id="e67ef-217">If you run into any issues with your application, [try posting a question or comment in the forum](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) (and don't forget to read the top post).</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="e67ef-218">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="e67ef-218">In this section</span></span>
<span data-ttu-id="e67ef-219"><a name="Next"> </a></span><span class="sxs-lookup"><span data-stu-id="e67ef-219"></span></span>

- [<span data-ttu-id="e67ef-220">Faça referência ao conjunto de API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="e67ef-220">Reference the EWS Managed API assembly</span></span>](how-to-reference-the-ews-managed-api-assembly.md)
    
- [<span data-ttu-id="e67ef-221">Definir a URL de serviço do EWS usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="e67ef-221">Set the EWS service URL by using the EWS Managed API</span></span>](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md)
    
- [<span data-ttu-id="e67ef-222">Comunicar-se com o EWS usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="e67ef-222">Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    
## <a name="see-also"></a><span data-ttu-id="e67ef-223">Confira também</span><span class="sxs-lookup"><span data-stu-id="e67ef-223">See also</span></span>

- [<span data-ttu-id="e67ef-224">Start using web services in Exchange</span><span class="sxs-lookup"><span data-stu-id="e67ef-224">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)    
- [<span data-ttu-id="e67ef-225">Visão geral de design de cliente do EWS do Exchange</span><span class="sxs-lookup"><span data-stu-id="e67ef-225">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)    
- [<span data-ttu-id="e67ef-226">Develop web service clients for Exchange</span><span class="sxs-lookup"><span data-stu-id="e67ef-226">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)   
- [<span data-ttu-id="e67ef-227">Solicitações e respostas para solucionar problemas de aplicativos do EWS Managed API de rastreamento</span><span class="sxs-lookup"><span data-stu-id="e67ef-227">Trace requests and responses to troubleshoot EWS Managed API applications</span></span>](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
    

