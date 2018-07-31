---
title: Introdução aos aplicativos clientes de API gerenciada por EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c2267733-6f4f-49e5-9614-1e4a24c3af1a
description: Desenvolva um aplicativo de cliente de email Hello World simple do Exchange usando a API gerenciada de EWS.
ms.openlocfilehash: b4254ab80b4dfc2c8fadf90c79d57517c3a0bb16
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353984"
---
# <a name="get-started-with-ews-managed-api-client-applications"></a><span data-ttu-id="2ac3e-103">Introdução aos aplicativos clientes de API gerenciada por EWS</span><span class="sxs-lookup"><span data-stu-id="2ac3e-103">Get started with EWS Managed API client applications</span></span>

<span data-ttu-id="2ac3e-104">Desenvolva um aplicativo de cliente de email Hello World simple do Exchange usando a API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-104">Develop a simple Hello World email client application for Exchange by using the EWS Managed API.</span></span> 
  
<span data-ttu-id="2ac3e-105">A [API gerenciada de EWS](http://aka.ms/ews-managed-api-readme) fornece um modelo de objeto intuitivo e fácil de usar para envio e recebimento de mensagens do serviço web de aplicativos clientes, aplicativos de portal e aplicativos de serviço.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-105">The [EWS Managed API](http://aka.ms/ews-managed-api-readme) provides an intuitive, easy-to-use object model for sending and receiving web service messages from client applications, portal applications, and service applications.</span></span> <span data-ttu-id="2ac3e-106">Você pode acessar quase todas as informações armazenadas em um Exchange Online, Exchange Online como parte do Office 365 ou uma caixa de correio do Exchange server usando a API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-106">You can access almost all the information stored in an Exchange Online, Exchange Online as part of Office 365, or an Exchange server mailbox by using the EWS Managed API.</span></span> <span data-ttu-id="2ac3e-107">Você pode usar as informações neste artigo para ajudá-lo a desenvolver seu primeiro aplicativo cliente EWS Managed API.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-107">You can use the information in this article to help you develop your first EWS Managed API client application.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="2ac3e-108">A API gerenciada de EWS agora está disponível como um projeto de código aberto no [GitHub](https://github.com/officedev/ews-managed-api).</span><span class="sxs-lookup"><span data-stu-id="2ac3e-108">The EWS Managed API is now available as an open source project on [GitHub](https://github.com/officedev/ews-managed-api).</span></span> <span data-ttu-id="2ac3e-109">Você pode usar a biblioteca de código aberto:</span><span class="sxs-lookup"><span data-stu-id="2ac3e-109">You can use the open source library to:</span></span> 
> - <span data-ttu-id="2ac3e-110">Contribui com correções de bug e melhorias à API.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-110">Contribute bug fixes and enhancements to the API.</span></span> 
> - <span data-ttu-id="2ac3e-111">Obtenha correções e melhorias antes que estejam disponíveis em uma versão oficial.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-111">Get fixes and enhancements before they are available in an official release.</span></span> 
> - <span data-ttu-id="2ac3e-112">Acesse a implementação mais abrangente e atualizada da API, para usar como referência ou criar novas bibliotecas em novas plataformas. </span><span class="sxs-lookup"><span data-stu-id="2ac3e-112">Access the most comprehensive and up-to-date implementation of the API, to use as a reference or to create new libraries on new platforms.</span></span> 
>
>  <span data-ttu-id="2ac3e-113">Agradecemos suas [contribuições](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-113">We welcome your [contributions](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) via GitHub.</span></span> 
  
## <a name="youll-need-an-exchange-server"></a><span data-ttu-id="2ac3e-114">Você precisará de um servidor do Exchange</span><span class="sxs-lookup"><span data-stu-id="2ac3e-114">You'll need an Exchange server</span></span>
<span data-ttu-id="2ac3e-115"><a name="NeedExchange"> </a></span><span class="sxs-lookup"><span data-stu-id="2ac3e-115"></span></span>

<span data-ttu-id="2ac3e-116">Se você já tiver uma conta de caixa de correio do Exchange, você poderá ignorar esta seção.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-116">If you already have an Exchange mailbox account, you can skip this section.</span></span> <span data-ttu-id="2ac3e-117">Caso contrário, você tem as seguintes opções para configurar uma caixa de correio do Exchange para seu primeiro aplicativo cliente EWS:</span><span class="sxs-lookup"><span data-stu-id="2ac3e-117">Otherwise, you have the following options for setting up an Exchange mailbox for your first EWS client application:</span></span>
  
- <span data-ttu-id="2ac3e-118">Obtenha um [Site do desenvolvedor do Office 365](http://msdn.microsoft.com/en-us/library/office/fp179924.aspx) (recomendado).</span><span class="sxs-lookup"><span data-stu-id="2ac3e-118">Get an [Office 365 Developer Site](http://msdn.microsoft.com/en-us/library/office/fp179924.aspx) (recommended).</span></span> <span data-ttu-id="2ac3e-119">Esta é a maneira mais rápida para configurar uma caixa de correio do Exchange.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-119">This is the quickest way for you to set up an Exchange mailbox.</span></span> 
    
- <span data-ttu-id="2ac3e-120">Baixe o [Exchange Server](http://office.microsoft.com/en-us/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).</span><span class="sxs-lookup"><span data-stu-id="2ac3e-120">Download [Exchange Server](http://office.microsoft.com/en-us/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).</span></span>
    
<span data-ttu-id="2ac3e-121">Após ter verificado que você pode enviar e receber emails do Exchange, você estará pronto para configurar o ambiente de desenvolvimento.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-121">After you have verified that you can send and receive email from Exchange, you are ready to set up your development environment.</span></span> <span data-ttu-id="2ac3e-122">Você pode usar o cliente do Exchange web do [Outlook Web App](http://technet.microsoft.com/en-us/library/jj657718%28v=exchg.150%29.aspx) para verificar se você pode enviar o email.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-122">You can use the Exchange web client [Outlook Web App](http://technet.microsoft.com/en-us/library/jj657718%28v=exchg.150%29.aspx) to verify that you can send email.</span></span> 
  
## <a name="set-up-your-development-environment"></a><span data-ttu-id="2ac3e-123">Definir seu ambiente de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="2ac3e-123">Set up your development environment</span></span>
<span data-ttu-id="2ac3e-124"><a name="Setup"> </a></span><span class="sxs-lookup"><span data-stu-id="2ac3e-124"></span></span>

<span data-ttu-id="2ac3e-125">Certifique-se de que você tenha acesso ao seguinte:</span><span class="sxs-lookup"><span data-stu-id="2ac3e-125">Make sure that you have access to the following:</span></span>
  
- <span data-ttu-id="2ac3e-126">Qualquer versão do [Visual Studio](http://www.visualstudio.com/en-us/downloads/download-visual-studio-vs.aspx) que suporta o .NET Framework 4.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-126">Any version of [Visual Studio](http://www.visualstudio.com/en-us/downloads/download-visual-studio-vs.aspx) that supports the .NET Framework 4.</span></span> <span data-ttu-id="2ac3e-127">Embora tecnicamente, Visual Studio não é necessário porque você pode usar qualquer compilador c#, recomendamos que você usá-lo.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-127">Although technically, you don't need Visual Studio because you can use any C# compiler, we recommend that you use it.</span></span> 
    
- <span data-ttu-id="2ac3e-128">A [API gerenciada de EWS](http://aka.ms/ews-managed-api-readme).</span><span class="sxs-lookup"><span data-stu-id="2ac3e-128">The [EWS Managed API](http://aka.ms/ews-managed-api-readme).</span></span> <span data-ttu-id="2ac3e-129">Você pode usar tanto a versão de 32 bits ou 64 bits, dependendo do seu sistema.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-129">You can use either the 64-bit or 32-bit version, depending on your system.</span></span> <span data-ttu-id="2ac3e-130">Use o local de instalação padrão.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-130">Use the default installation location.</span></span> 
    
## <a name="create-your-first-ews-managed-api-application"></a><span data-ttu-id="2ac3e-131">Crie seu primeiro aplicativo de API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="2ac3e-131">Create your first EWS Managed API application</span></span>
<span data-ttu-id="2ac3e-132"><a name="Create"> </a></span><span class="sxs-lookup"><span data-stu-id="2ac3e-132"></span></span>

<span data-ttu-id="2ac3e-133">Essas etapas pressupõem que você configure um Site do desenvolvedor do Office 365.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-133">These steps assume that you set up an Office 365 Developer Site.</span></span> <span data-ttu-id="2ac3e-134">Se você baixar e instalar o Exchange, você precisará [instalar um certificado válido](http://technet.microsoft.com/en-us/library/bb310769%28v=exchg.141%29.aspx) no seu Exchange server ou a [implementação de uma validação de certificado](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) retorno de chamada para um certificado autoassinado é fornecido por padrão.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-134">If you downloaded and installed Exchange, you will need to [install a valid certificate](http://technet.microsoft.com/en-us/library/bb310769%28v=exchg.141%29.aspx) on your Exchange server or [implement a certificate validation](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) callback for a self-signed certificate that is provided by default.</span></span> <span data-ttu-id="2ac3e-135">Observe também que estas etapas podem variar ligeiramente dependendo da versão do Visual Studio que você está usando.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-135">Also note that these steps might vary slightly depending on the version of Visual Studio that you are using.</span></span> 
  
### <a name="step-1-create-a-project-in-visual-studio"></a><span data-ttu-id="2ac3e-136">Etapa 1: Criar um projeto no Visual Studio</span><span class="sxs-lookup"><span data-stu-id="2ac3e-136">Step 1: Create a project in Visual Studio</span></span>

1. <span data-ttu-id="2ac3e-137">No Visual Studio, no menu **arquivo** , escolha **novo**e, em seguida, selecione o **projeto**.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-137">In Visual Studio, on the **File** menu, choose **New**, and then choose **Project**.</span></span> <span data-ttu-id="2ac3e-138">Abre a caixa de diálogo **Novo projeto**.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-138">The **New Project** dialog box opens.</span></span> 
    
2. <span data-ttu-id="2ac3e-139">Crie um **aplicativo de Console do c#**.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-139">Create a **C# Console Application**.</span></span> <span data-ttu-id="2ac3e-140">No painel **modelos** , escolha **Visual c#** e, em seguida, escolha o **Aplicativo de Console**.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-140">From the **Templates** pane, choose **Visual C#**, and then choose **Console Application**.</span></span> 
    
3. <span data-ttu-id="2ac3e-141">Nome do projeto HelloWorld e escolha **Okey**.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-141">Name the project HelloWorld, and then choose **OK**.</span></span>
    
<span data-ttu-id="2ac3e-142">Visual Studio cria o projeto e abre a janela de documento de código Module. vb.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-142">Visual Studio creates the project and opens the Program.cs code document window.</span></span>

### <a name="step-2-add-a-reference-to-the-ews-managed-api"></a><span data-ttu-id="2ac3e-143">Etapa 2: Adicionar uma referência para a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="2ac3e-143">Step 2: Add a reference to the EWS Managed API</span></span>

1. <span data-ttu-id="2ac3e-144">Se a janela **Explorador** de soluções já estiver aberta, ignore esta etapa e vá para a etapa 2.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-144">If the **Solution Explorer** window is already open, skip this step and proceed to step 2.</span></span> <span data-ttu-id="2ac3e-145">Para abrir a janela **Solution Explorer** , no menu **Exibir** , escolha **Solution Explorer**.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-145">To open the **Solution Explorer** window, on the **View** menu, choose **Solution Explorer**.</span></span> 
    
2. <span data-ttu-id="2ac3e-146">No **Solution Explorer** e o projeto **HelloWorld** , abra o menu de atalho (botão direito do mouse) para **referências** e escolha **Adicionar referência** no menu de contexto.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-146">In the **Solution Explorer** and the **HelloWorld** project, open the shortcut menu (right-click) for **References** and choose **Add Reference** from the context menu.</span></span> <span data-ttu-id="2ac3e-147">Uma caixa de diálogo de gerenciamento de referências de projeto será aberta.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-147">A dialog box for managing project references will open.</span></span> 
    
3. <span data-ttu-id="2ac3e-148">Escolha a opção **Procurar** .</span><span class="sxs-lookup"><span data-stu-id="2ac3e-148">Choose the **Browse** option.</span></span> <span data-ttu-id="2ac3e-149">Navegue até o local onde você instalou a DLL de API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-149">Browse to the location where you installed the EWS Managed API DLL.</span></span> <span data-ttu-id="2ac3e-150">O caminho padrão definido pelo instalador é o seguinte: C:\Program Files\Microsoft\Exchange\Web serviços\<versão >\.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-150">The default path set by the installer is the following: C:\Program Files\Microsoft\Exchange\Web Services\<version>\.</span></span> <span data-ttu-id="2ac3e-151">O caminho pode variar com base em se você baixe o 32 ou a versão de 64 bits do Microsoft.Exchange.WebServices.dll.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-151">The path can vary based on whether you download the 32 or 64 bit version of the Microsoft.Exchange.WebServices.dll.</span></span> <span data-ttu-id="2ac3e-152">Escolha **Microsoft.Exchange.WebServices.dll** e selecione **Okey** ou **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-152">Choose **Microsoft.Exchange.WebServices.dll** and select **OK** or **Add**.</span></span> <span data-ttu-id="2ac3e-153">Isso adiciona a referência de API gerenciada de EWS ao seu projeto.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-153">This adds the EWS Managed API reference to your project.</span></span> 
    
4. <span data-ttu-id="2ac3e-154">Se você estiver usando o EWS gerenciadas API 2.0, altere o projeto HelloWorld para direcionar o .NET Framework 4.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-154">If you are using EWS Managed API 2.0, change the HelloWorld project to target the .NET Framework 4.</span></span> <span data-ttu-id="2ac3e-155">Outras versões do EWS Managed API podem usar uma versão de destino diferente do .NET Framework.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-155">Other versions of the EWS Managed API might use a different target version of the .NET Framework.</span></span>
    
5. <span data-ttu-id="2ac3e-156">Confirme que você está usando a versão de destino correto do .NET Framework.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-156">Confirm that you are using the correct target version of the .NET Framework.</span></span> <span data-ttu-id="2ac3e-157">Abra o menu de atalho (botão direito do mouse) para o seu projeto **HelloWorld** no **Solution Explorer**e escolha **Propriedades**.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-157">Open the shortcut menu (right-click) for your **HelloWorld** project in the **Solution Explorer**, and choose **Properties**.</span></span> <span data-ttu-id="2ac3e-158">Verifique se o **.NET Framework 4** é selecionado na caixa de lista suspensa de **estrutura de destino** .</span><span class="sxs-lookup"><span data-stu-id="2ac3e-158">Verify that the **.NET Framework 4** is selected in the **Target framework** drop-down box.</span></span> 
    
<span data-ttu-id="2ac3e-159">Agora que você ter seu projeto configurado e você criou uma referência para a API gerenciada de EWS, você estará pronto para criar seu primeiro aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-159">Now that you have your project set up and you created a reference to the EWS Managed API, you are ready to create your first application.</span></span> <span data-ttu-id="2ac3e-160">Para manter a simplicidade, adicione o código no arquivo Module. vb.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-160">To keep things simple, add your code to the Program.cs file.</span></span> <span data-ttu-id="2ac3e-161">Leia [o assembly do EWS Managed API de referência](how-to-reference-the-ews-managed-api-assembly.md) para obter mais informações sobre como fazer referência a API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-161">Read [Reference the EWS Managed API assembly](how-to-reference-the-ews-managed-api-assembly.md) for more information about referencing the EWS Managed API.</span></span> <span data-ttu-id="2ac3e-162">Na próxima etapa, você irá desenvolver o código básico para gravar o cliente de API gerenciada de EWS a maioria dos aplicativos.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-162">In the next step, you will develop the basic code to write most EWS Managed API client applications.</span></span> 
### <a name="step-3-set-up-url-redirection-validation-for-autodiscover"></a><span data-ttu-id="2ac3e-163">Etapa 3: Configurar a validação de redirecionamento de URL de descoberta automática</span><span class="sxs-lookup"><span data-stu-id="2ac3e-163">Step 3: Set up URL redirection validation for Autodiscover</span></span>

- <span data-ttu-id="2ac3e-164">Adicione o seguinte método de retorno de chamada de validação de redirecionamento após o método **Main (string [] args)** .</span><span class="sxs-lookup"><span data-stu-id="2ac3e-164">Add the following redirection validation callback method after the **Main(string[] args)** method.</span></span> <span data-ttu-id="2ac3e-165">Isso valida se redirecionado URLs retornado pela [descoberta automática](autodiscover-for-exchange.md) representam um ponto de extremidade HTTPS.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-165">This validates whether redirected URLs returned by [Autodiscover](autodiscover-for-exchange.md) represent an HTTPS endpoint.</span></span> 
    
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

<span data-ttu-id="2ac3e-166">Esse retorno de chamada de validação será passado para o objeto **ExchangeService** na etapa 4.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-166">This validation callback will be passed to the **ExchangeService** object in step 4.</span></span> <span data-ttu-id="2ac3e-167">Você precisa para que seu aplicativo será confiar e seguir redirecionamentos de descoberta automática - os resultados do redirecionamento de descoberta automática fornece o ponto de extremidade do EWS para nosso aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-167">You need this so that your application will trust and follow Autodiscover redirects - the results of the Autodiscover redirect provides the EWS endpoint for our application.</span></span> 

### <a name="step-4-prepare-the-exchangeservice-object"></a><span data-ttu-id="2ac3e-168">Etapa 4: Preparar o objeto ExchangeService</span><span class="sxs-lookup"><span data-stu-id="2ac3e-168">Step 4: Prepare the ExchangeService object</span></span>

1. <span data-ttu-id="2ac3e-169">Adicione uma referência de diretiva **usando** para a API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-169">Add a **using** directive reference to the EWS Managed API.</span></span> <span data-ttu-id="2ac3e-170">Adicione o código a seguir após a última diretiva **using** na parte superior da Module. vb.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-170">Add the following code after the last **using** directive at the top of Program.cs.</span></span> 
    
   ```cs
    using Microsoft.Exchange.WebServices.Data;
   ```

2. <span data-ttu-id="2ac3e-171">No método **Main** , instanciar o objeto [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) com a versão do serviço que você pretende de destino.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-171">In the **Main** method, instantiate the [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object with the service version you intend to target.</span></span> <span data-ttu-id="2ac3e-172">Este exemplo refere-se a versão mais antiga do esquema do EWS.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-172">This example targets the earliest version of the EWS schema.</span></span> 
    
   ```cs
    ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);
   ```

3. <span data-ttu-id="2ac3e-173">Se você está direcionando um servidor do Exchange no local e seu cliente está unido ao domínio, vá para a etapa 4.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-173">If you are targeting an on-premises Exchange server and your client is domain joined, proceed to step 4.</span></span> <span data-ttu-id="2ac3e-174">Se você cliente concentrando-se uma caixa de correio do Site do desenvolvedor do Office 365 ou Exchange Online, você precisa passar credenciais explícitas.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-174">If you client is targeting an Exchange Online or Office 365 Developer Site mailbox, you have to pass explicit credentials.</span></span> <span data-ttu-id="2ac3e-175">Adicione o código a seguir após a instanciação do objeto **ExchangeService** e definir as credenciais para a sua conta de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-175">Add the following code after the instantiation of the **ExchangeService** object and set the credentials for your mailbox account.</span></span> <span data-ttu-id="2ac3e-176">O nome de usuário deve ser o nome principal do usuário.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-176">The user name should be the user principal name.</span></span> <span data-ttu-id="2ac3e-177">Vá para a etapa 5.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-177">Proceed to step 5.</span></span> 
    
   ```cs
    service.Credentials = new WebCredentials("user1@contoso.com", "password");
   ```

4. <span data-ttu-id="2ac3e-178">Clientes do domínio que um servidor do Exchange no local de destino podem usar as credenciais padrão do usuário que está conectado, supondo que as credenciais estão associadas uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-178">Domain-joined clients that target an on-premises Exchange server can use the default credentials of the user who is logged on, assuming the credentials are associated with a mailbox.</span></span> <span data-ttu-id="2ac3e-179">Adicione o código a seguir após a instanciação do objeto **ExchangeService** .</span><span class="sxs-lookup"><span data-stu-id="2ac3e-179">Add the following code after the instantiation of the **ExchangeService** object.</span></span> 
    
   ```cs
    service.UseDefaultCredentials = true;
   ```

   <span data-ttu-id="2ac3e-180">Se seu cliente destinada a uma caixa de correio do Exchange Online ou o Site do desenvolvedor do Office 365, verifique se que [UseDefaultCredentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.usedefaultcredentials%28v=exchg.80%29.aspx) está definido como **false**, que é o valor padrão.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-180">If your client targets an Exchange Online or Office 365 Developer Site mailbox, verify that [UseDefaultCredentials](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.usedefaultcredentials%28v=exchg.80%29.aspx) is set to **false**, which is the default value.</span></span> <span data-ttu-id="2ac3e-181">Seu cliente está pronto para fazer a chamada primeira para o serviço Descoberta automática para obter a URL do serviço de chamadas para o serviço do EWS.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-181">Your client is ready to make the first call to the Autodiscover service to get the service URL for calls to the EWS service.</span></span>
    
5. <span data-ttu-id="2ac3e-182">O método **AutodiscoverUrl** no objeto **ExchangeService** realiza uma série de chamadas para o serviço de descoberta automática para obter a URL do serviço.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-182">The **AutodiscoverUrl** method on the **ExchangeService** object performs a series of calls to the Autodiscover service to get the service URL.</span></span> <span data-ttu-id="2ac3e-183">Se essa chamada de método tiver êxito, a propriedade URL no objeto **ExchangeService** será definida com a URL do serviço.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-183">If this method call is successful, the URL property on the **ExchangeService** object will be set with the service URL.</span></span> <span data-ttu-id="2ac3e-184">Passe o endereço de email do usuário e o **RedirectionUrlValidationCallback** para o método **AutodiscoverUrl** .</span><span class="sxs-lookup"><span data-stu-id="2ac3e-184">Pass the user's email address and the **RedirectionUrlValidationCallback** to the **AutodiscoverUrl** method.</span></span> <span data-ttu-id="2ac3e-185">Depois que as credenciais tiverem sido especificadas na etapa 3 ou 4, adicione o código a seguir.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-185">Add the following code after the credentials have been specified in step 3 or 4.</span></span> <span data-ttu-id="2ac3e-186">Alterar `user1@contoso.com` para seu email para que o serviço Descoberta automática encontra seu ponto de extremidade do EWS de endereços.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-186">Change  `user1@contoso.com` to your email address so that the Autodiscover service finds your EWS endpoint.</span></span> 
    
   ```cs
    service.AutodiscoverUrl("user1@contoso.com", RedirectionUrlValidationCallback);
   ```

<span data-ttu-id="2ac3e-187">Neste ponto, seu cliente estiver configurado para fazer chamadas para o EWS para acessar dados de caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-187">At this point, your client is set up to make calls to EWS to access mailbox data.</span></span> <span data-ttu-id="2ac3e-188">Se você executar o seu código agora, você pode verificar se a chamada do método **AutodiscoverUrl** funcionou examinando o conteúdo da propriedade [ExchangeService.Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="2ac3e-188">If you run your code now, you can verify that the **AutodiscoverUrl** method call worked by examining the contents of the [ExchangeService.Url](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) property.</span></span> <span data-ttu-id="2ac3e-189">Se essa propriedade contém uma URL, sua chamada foi um sucesso!</span><span class="sxs-lookup"><span data-stu-id="2ac3e-189">If this property contains a URL, your call was a success!</span></span> <span data-ttu-id="2ac3e-190">Isso significa que seu aplicativo com êxito autenticado com o serviço e descoberto o ponto de extremidade do EWS para sua caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-190">This means that your application successfully authenticated with the service and discovered the EWS endpoint for your mailbox.</span></span> <span data-ttu-id="2ac3e-191">Agora você está pronto para fazer primeira suas chamadas EWS.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-191">Now you are ready to make your first calls to EWS.</span></span> <span data-ttu-id="2ac3e-192">Leia a [definir a URL do serviço do EWS usando a API gerenciada de EWS](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md) para obter mais informações sobre como definir a URL do EWS.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-192">Read [Set the EWS service URL by using the EWS Managed API](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md) for more information about setting the EWS URL.</span></span> 

### <a name="step-6-create-your-first-hello-world-email-message"></a><span data-ttu-id="2ac3e-193">Etapa 6: Criar sua primeira mensagem de email Olá mundo</span><span class="sxs-lookup"><span data-stu-id="2ac3e-193">Step 6: Create your first Hello World email message</span></span>

1. <span data-ttu-id="2ac3e-194">Após chamar o método **AutodiscoverUrl** , instanciar um novo objeto **EmailMessage** e passe o objeto de serviço que você criou.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-194">After the **AutodiscoverUrl** method call, instantiate a new **EmailMessage** object and pass in the service object you created.</span></span> 
    
   ```cs
    EmailMessage email = new EmailMessage(service);
   ```

   <span data-ttu-id="2ac3e-195">Agora você tem uma mensagem de email no qual a ligação do serviço é definida.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-195">You now have an email message on which the service binding is set.</span></span> <span data-ttu-id="2ac3e-196">Todas as chamadas iniciadas no objeto **EmailMessage** serão direcionadas no serviço.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-196">Any calls initiated on the **EmailMessage** object will be targeted at the service.</span></span> 
    
2. <span data-ttu-id="2ac3e-197">Agora definida para: destinatário de linha da mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-197">Now set the To: line recipient of the email message.</span></span> <span data-ttu-id="2ac3e-198">Para fazer isso, altere `user1@contoso.com` usar seu endereço SMTP.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-198">To do this, change  `user1@contoso.com` to use your SMTP address.</span></span> 
    
   ```cs
    email.ToRecipients.Add("user1@contoso.com");
   ```

3. <span data-ttu-id="2ac3e-199">Defina o assunto e o corpo da mensagem de email.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-199">Set the subject and the body of the email message.</span></span>
    
   ```cs
    email.Subject = "HelloWorld";
    email.Body = new MessageBody("This is the first email I've sent by using the EWS Managed API.");
   ```

4. <span data-ttu-id="2ac3e-200">Agora você está pronto para enviar sua primeira mensagem de email usando a API gerenciada de EWS.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-200">You are now ready to send your first email message by using the EWS Managed API.</span></span> <span data-ttu-id="2ac3e-201">O método **Send** irá chamar o serviço e enviar a mensagem de email para entrega.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-201">The **Send** method will call the service and submit the email message for delivery.</span></span> <span data-ttu-id="2ac3e-202">Leia [Communicate with EWS usando a API gerenciada de EWS](how-to-communicate-with-ews-by-using-the-ews-managed-api.md) para conhecer outros métodos que você pode usar para se comunicar com o Exchange.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-202">Read [Communicate with EWS by using the EWS Managed API](how-to-communicate-with-ews-by-using-the-ews-managed-api.md) to learn about other methods you can use to communicate with Exchange.</span></span> 
    
   ```cs
    email.Send();
   ```

5. <span data-ttu-id="2ac3e-203">Você está pronto para executar seu aplicativo Hello World.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-203">You are ready to run your Hello World application.</span></span> <span data-ttu-id="2ac3e-204">No Visual Studio, selecione **F5**.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-204">In Visual Studio, select **F5**.</span></span> <span data-ttu-id="2ac3e-205">Será aberta uma janela de console em branco.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-205">A blank console window will open.</span></span> <span data-ttu-id="2ac3e-206">Você não verá algo na janela do console enquanto o seu aplicativo autentica, segue redirecionamentos de descoberta automática e então faz sua chamada primeira para criar uma mensagem de email que você envie para você mesmo.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-206">You will not see anything in the console window while your application authenticates, follows Autodiscover redirections, and then makes its first call to create an email message that you send to yourself.</span></span> <span data-ttu-id="2ac3e-207">Se você quiser ver as chamadas sejam feitas, adicione as duas linhas de código a seguintes antes do método **AutodiscoverUrl** é chamado.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-207">If you want to see the calls being made, add the following two lines of code before the **AutodiscoverUrl** method is called.</span></span> <span data-ttu-id="2ac3e-208">Em seguida, pressione F5.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-208">Then press F5.</span></span> <span data-ttu-id="2ac3e-209">Isso irá [Rastrear check-out do EWS solicitações e respostas](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md) na janela do console.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-209">This will [trace out the EWS requests and responses](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md) to the console window.</span></span> 
    
   ```cs
    service.TraceEnabled = true;
    service.TraceFlags = TraceFlags.All;
   ```

<span data-ttu-id="2ac3e-210">Agora você tem um aplicativo de cliente do EWS Managed API em funcionamento.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-210">You now have a working EWS Managed API client application.</span></span> <span data-ttu-id="2ac3e-211">Para sua conveniência, o exemplo a seguir mostra o código que você adicionou à Module. vb para criar seu aplicativo Hello World.</span><span class="sxs-lookup"><span data-stu-id="2ac3e-211">For your convenience, the following example shows all the code that you added to Program.cs to create your Hello World application.</span></span>

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

## <a name="next-steps"></a><span data-ttu-id="2ac3e-212">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="2ac3e-212">Next steps</span></span>
<span data-ttu-id="2ac3e-213"><a name="Next"> </a></span><span class="sxs-lookup"><span data-stu-id="2ac3e-213"></span></span>

<span data-ttu-id="2ac3e-214">Se você estiver pronto para fazer mais com seu primeiro aplicativo de cliente do EWS Managed API, explore os recursos a seguir:</span><span class="sxs-lookup"><span data-stu-id="2ac3e-214">If you're ready to do more with your first EWS Managed API client application, explore the following resources:</span></span>
  
- [<span data-ttu-id="2ac3e-215">Exchange 2013:101 amostras de código</span><span class="sxs-lookup"><span data-stu-id="2ac3e-215">Exchange 2013: 101 code samples</span></span>](http://code.msdn.microsoft.com/exchange/Exchange-2013-101-Code-3c38582c)   
- [<span data-ttu-id="2ac3e-216">Pastas e itens</span><span class="sxs-lookup"><span data-stu-id="2ac3e-216">Folders and items</span></span>](folders-and-items-in-ews-in-exchange.md)    
- [<span data-ttu-id="2ac3e-217">EWSEditor</span><span class="sxs-lookup"><span data-stu-id="2ac3e-217">EWSEditor</span></span>](http://ewseditor.codeplex.com/)
    
<span data-ttu-id="2ac3e-218">Se você tiver algum problema com o seu aplicativo, [Experimente postar uma pergunta ou um comentário no fórum](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) (e não se esqueça de ler a postagem superior).</span><span class="sxs-lookup"><span data-stu-id="2ac3e-218">If you run into any issues with your application, [try posting a question or comment in the forum](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) (and don't forget to read the top post).</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="2ac3e-219">Nesta seção</span><span class="sxs-lookup"><span data-stu-id="2ac3e-219">In this section</span></span>
<span data-ttu-id="2ac3e-220"><a name="Next"> </a></span><span class="sxs-lookup"><span data-stu-id="2ac3e-220"></span></span>

- [<span data-ttu-id="2ac3e-221">Faça referência ao conjunto de API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="2ac3e-221">Reference the EWS Managed API assembly</span></span>](how-to-reference-the-ews-managed-api-assembly.md)   
- [<span data-ttu-id="2ac3e-222">Definir a URL de serviço do EWS usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="2ac3e-222">Set the EWS service URL by using the EWS Managed API</span></span>](how-to-set-the-ews-service-url-by-using-the-ews-managed-api.md)   
- [<span data-ttu-id="2ac3e-223">Comunicar-se com o EWS usando a API gerenciada de EWS</span><span class="sxs-lookup"><span data-stu-id="2ac3e-223">Communicate with EWS by using the EWS Managed API</span></span>](how-to-communicate-with-ews-by-using-the-ews-managed-api.md)
    
## <a name="see-also"></a><span data-ttu-id="2ac3e-224">Confira também</span><span class="sxs-lookup"><span data-stu-id="2ac3e-224">See also</span></span>

- [<span data-ttu-id="2ac3e-225">Start using web services in Exchange</span><span class="sxs-lookup"><span data-stu-id="2ac3e-225">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)    
- [<span data-ttu-id="2ac3e-226">Visão geral de design de cliente do EWS do Exchange</span><span class="sxs-lookup"><span data-stu-id="2ac3e-226">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)    
- [<span data-ttu-id="2ac3e-227">Develop web service clients for Exchange</span><span class="sxs-lookup"><span data-stu-id="2ac3e-227">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)   
- [<span data-ttu-id="2ac3e-228">Solicitações e respostas para solucionar problemas de aplicativos do EWS Managed API de rastreamento</span><span class="sxs-lookup"><span data-stu-id="2ac3e-228">Trace requests and responses to troubleshoot EWS Managed API applications</span></span>](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
    

