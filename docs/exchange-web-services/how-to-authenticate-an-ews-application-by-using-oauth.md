---
title: Autenticar um aplicativo EWS usando o OAuth
manager: sethgros
ms.date: 05/17/2019
ms.audience: Developer
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: Saiba como usar a autenticação OAuth com seus aplicativos de API gerenciada do EWS.
localization_priority: Priority
ms.openlocfilehash: 0375095faac918859354da026118ea4ccfd6792b
ms.sourcegitcommit: eeda51cb037aa25566adb293f25574674fdb2d9e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45012563"
---
<!-- markdownlint-disable MD025 -->
# <a name="authenticate-an-ews-application-by-using-oauth"></a><span data-ttu-id="9fdfe-103">Autenticar um aplicativo EWS usando o OAuth</span><span class="sxs-lookup"><span data-stu-id="9fdfe-103">Authenticate an EWS application by using OAuth</span></span>
<!-- markdownlint-enable MD025 -->

<span data-ttu-id="9fdfe-104">Saiba como usar a autenticação OAuth com seus aplicativos de API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-104">Learn how to use OAuth authentication with your EWS Managed API applications.</span></span>

<span data-ttu-id="9fdfe-105">Você pode usar o serviço de autenticação OAuth fornecido pelo Azure Active Directory para permitir que seus aplicativos da API gerenciada do EWS acessem o Exchange Online no Office 365.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-105">You can use the OAuth authentication service provided by Azure Active Directory to enable your EWS Managed API applications to access Exchange Online in Office 365.</span></span> <span data-ttu-id="9fdfe-106">Para usar o OAuth com seu aplicativo, você precisará:</span><span class="sxs-lookup"><span data-stu-id="9fdfe-106">To use OAuth with your application you will need to:</span></span>

1. <span data-ttu-id="9fdfe-107">[Registre seu aplicativo com o](#register-your-application) Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-107">[Register your application](#register-your-application) with Azure Active Directory.</span></span>

2. <span data-ttu-id="9fdfe-108">[Adicione código para obter um token de autenticação](#add-code-to-get-an-authentication-token) para obter um token de autenticação de um servidor de token.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-108">[Add code to get an authentication token](#add-code-to-get-an-authentication-token) to get an authentication token from a token server.</span></span>

3. <span data-ttu-id="9fdfe-109">[Adicione um token de autenticação às solicitações do EWS](#add-an-authentication-token-to-ews-requests) que você enviar.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-109">[Add an authentication token to EWS requests](#add-an-authentication-token-to-ews-requests) that you send.</span></span>

> [!NOTE]
> <span data-ttu-id="9fdfe-110">A autenticação OAuth para EWS só está disponível no Exchange como parte do Office 365.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-110">OAuth authentication for EWS is only available in Exchange as part of Office 365.</span></span> <span data-ttu-id="9fdfe-111">Os aplicativos EWS que usam o OAuth devem ser registrados no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-111">EWS applications that use OAuth must be registered with Azure Active Directory.</span></span>

<span data-ttu-id="9fdfe-112">Para usar o código neste artigo, você precisará ter acesso ao seguinte:</span><span class="sxs-lookup"><span data-stu-id="9fdfe-112">To use the code in this article, you will need to have access to the following:</span></span>

- <span data-ttu-id="9fdfe-113">Uma conta do Office 365 com uma caixa de correio do Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-113">An Office 365 account with an Exchange Online mailbox.</span></span> <span data-ttu-id="9fdfe-114">Se você não tiver uma conta do Office 365, você poderá [se inscrever no programa de desenvolvedor do office 365](https://developer.microsoft.com/office/dev-program) para obter uma assinatura gratuita do Office 365.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-114">If you do not have an Office 365 account, you can [sign up for the Office 365 Developer Program](https://developer.microsoft.com/office/dev-program) to get a free Office 365 subscription.</span></span>

- <span data-ttu-id="9fdfe-115">A [biblioteca de autenticação da Microsoft para .net](/dotnet/api/microsoft.identity.client?view=azure-dotnet).</span><span class="sxs-lookup"><span data-stu-id="9fdfe-115">The [Microsoft Authentication Library for .NET](/dotnet/api/microsoft.identity.client?view=azure-dotnet).</span></span>

- <span data-ttu-id="9fdfe-116">A [API gerenciada do EWS](https://github.com/officedev/ews-managed-api).</span><span class="sxs-lookup"><span data-stu-id="9fdfe-116">The [EWS Managed API](https://github.com/officedev/ews-managed-api).</span></span>


<span data-ttu-id="9fdfe-117">Há dois tipos de permissões OAuth que podem ser usadas para acessar APIs EWS no Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-117">There are two types of OAuth permissions that can be used to access EWS APIs in Exchange Online.</span></span> <span data-ttu-id="9fdfe-118">Antes de prosseguir com o tutorial, você precisará escolher o tipo de permissão específico a ser usado.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-118">Before you proceed with the tutorial, you will need to choose the specific permission type to use.</span></span>

* <span data-ttu-id="9fdfe-119">As **permissões delegadas** são usadas pelos aplicativos que têm um usuário conectado atualmente.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-119">**Delegated permissions** are used by apps that have a signed-in user present.</span></span> <span data-ttu-id="9fdfe-120">Para esses aplicativos, o usuário ou um administrador consenti às permissões que o aplicativo solicita e o aplicativo pode atuar como o usuário conectado ao fazer chamadas de API.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-120">For these apps, either the user or an administrator consents to the permissions that the app requests and the app can act as the signed-in user when making API calls.</span></span> 
* <span data-ttu-id="9fdfe-121">**As permissões de aplicativo** são usadas por aplicativos executados sem um usuário conectado presente; por exemplo, aplicativos executados como serviços em segundo plano ou daemons e podem acessar várias caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-121">**Application permissions** are used by apps that run without a signed-in user present; for example, apps that run as background services or daemons and can access multiple mailboxes.</span></span>

## <a name="register-your-application"></a><span data-ttu-id="9fdfe-122">Registrar seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="9fdfe-122">Register your application</span></span>

<span data-ttu-id="9fdfe-123">Para usar o OAuth, um aplicativo deve ter uma ID de aplicativo emitida pelo Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-123">To use OAuth, an application must have an application ID issued by Azure Active Directory.</span></span> <span data-ttu-id="9fdfe-124">Neste tutorial, supõe-se que o aplicativo é um aplicativo de console, portanto, você precisa registrar seu aplicativo como um cliente público com o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-124">In this tutorial, it is assumed that the application is a console application, so you need to register your application as a public client with Azure Active Directory.</span></span>

1. <span data-ttu-id="9fdfe-125">Abra um navegador, navegue até o [centro de administração do Azure Active Directory](https://aad.portal.azure.com) e faça logon usando uma **conta pessoal** (também conhecida como conta da Microsoft) ou **Conta Corporativa ou de Estudante**.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-125">Open a browser and navigate to the [Azure Active Directory admin center](https://aad.portal.azure.com) and login using a **personal account** (aka: Microsoft Account) or **Work or School Account**.</span></span>

1. <span data-ttu-id="9fdfe-126">Selecione **Azure Active Directory** na navegação esquerda e selecione **Registros de aplicativos** em **Gerenciar**.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-126">Select **Azure Active Directory** in the left-hand navigation, then select **App registrations** under **Manage**.</span></span>

1. <span data-ttu-id="9fdfe-127">Selecione **Novo registro**.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-127">Select **New registration**.</span></span> <span data-ttu-id="9fdfe-128">Na página **Registrar um aplicativo**, defina os valores da seguinte forma.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-128">On the **Register an application** page, set the values as follows.</span></span>

    - <span data-ttu-id="9fdfe-129">Defina o **nome** como um nome amigável para o seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-129">Set **Name** to a friendly name for your app.</span></span>
    - <span data-ttu-id="9fdfe-130">Defina os **tipos de conta com suporte** para a opção que faz sentido para seu cenário.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-130">Set **Supported account types** to the choice that makes sense for your scenario.</span></span>
    - <span data-ttu-id="9fdfe-131">Para o **URI de redirecionamento**, altere o menu suspenso para **cliente público (Desktop & móvel)** e defina o valor como `urn:ietf:wg:oauth:2.0:oob` .</span><span class="sxs-lookup"><span data-stu-id="9fdfe-131">For **Redirect URI**, change the dropdown to **Public client (mobile & desktop)** and set the value to `urn:ietf:wg:oauth:2.0:oob`.</span></span>

1. <span data-ttu-id="9fdfe-132">Escolha **Registrar**.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-132">Choose **Register**.</span></span> <span data-ttu-id="9fdfe-133">Na próxima página, copie o valor da ID do **aplicativo (cliente)** e salve-o, você precisará dele mais tarde.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-133">On the next page, copy the value of the **Application (client) ID** and save it, you will need it later.</span></span>

1. <span data-ttu-id="9fdfe-134">Selecione **permissões de API** na navegação à esquerda em **gerenciar**.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-134">Select **API permissions** in the left-hand navigation under **Manage**.</span></span> 

1. <span data-ttu-id="9fdfe-135">Selecione **Adicionar uma permissão**.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-135">Select **Add a permission**.</span></span> <span data-ttu-id="9fdfe-136">Na página **solicitar permissões de API** , selecione **Exchange** em **APIs herdadas com suporte**.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-136">On the **Request API permissions** page, select **Exchange** under **Supported legacy APIs**.</span></span> 

1. <span data-ttu-id="9fdfe-137">Para usar permissões delegadas, selecione **permissões delegadas** e, em seguida, escolha **EWS. AccessAsUser. All** em **EWS**.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-137">To use Delegated permissions, select **Delegated permissions** and then select **EWS.AccessAsUser.All** under **EWS**.</span></span> <span data-ttu-id="9fdfe-138">Clique em **adicionar permissões**.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-138">Click on **Add permissions**.</span></span> 

<span data-ttu-id="9fdfe-139">Para usar as permissões de aplicativo, siga estas etapas adicionais.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-139">To use Application permissions, follow these additional steps.</span></span>

1. <span data-ttu-id="9fdfe-140">Selecione **permissões do aplicativo** e, em seguida, selecione **full_access_as_app**.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-140">Select **Application permissions** and then select **full_access_as_app**.</span></span> <span data-ttu-id="9fdfe-141">Clique em **adicionar permissões**.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-141">Click on **Add permissions**.</span></span>

1. <span data-ttu-id="9fdfe-142">Selecione **conceder consentimento do administrador para org** e aceitar a caixa de diálogo de consentimento.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-142">Select **Grant admin consent for org** and accept the consent dialog.</span></span> 

1. <span data-ttu-id="9fdfe-143">Selecione **certificados & segredos** na navegação à esquerda em **gerenciar**.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-143">Select **Certificates & Secrets** in the left-hand navigation under **Manage**.</span></span> 

1. <span data-ttu-id="9fdfe-144">Selecione **novo segredo do cliente**, digite uma breve descrição e selecione **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-144">Select **New client secret**, enter a short description and select **Add**.</span></span>

1. <span data-ttu-id="9fdfe-145">Copie o **valor** do novo segredo do cliente recém-adicionado e salve-o, você precisará dele mais tarde.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-145">Copy the **Value** of the newly added client secret and save it, you will need it later.</span></span> 

## <a name="add-code-to-get-an-authentication-token"></a><span data-ttu-id="9fdfe-146">Adicionar código para obter um token de autenticação</span><span class="sxs-lookup"><span data-stu-id="9fdfe-146">Add code to get an authentication token</span></span>

<span data-ttu-id="9fdfe-147">Os trechos de código a seguir mostram como usar a biblioteca de autenticação da Microsoft para obter tokens de autenticação para permissões delegadas e permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-147">The following code snippets show how to use the Microsoft Authentication Library to get authentication tokens for delegated permissions and application permissions.</span></span> <span data-ttu-id="9fdfe-148">Esses trechos de código presumem que as informações necessárias para fazer a solicitação de autenticação sejam armazenadas no arquivo de **App.config** do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-148">These snippets assume that the information required to make the authentication request is stored in the application's **App.config** file.</span></span> <span data-ttu-id="9fdfe-149">Estes exemplos não incluem verificação de erros, consulte os [exemplos de código](#code-samples) para o código completo.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-149">These examples do not include error checking, see the [Code samples](#code-samples) for the complete code.</span></span>

### <a name="delegated-permissions"></a><span data-ttu-id="9fdfe-150">Permissões delegadas</span><span class="sxs-lookup"><span data-stu-id="9fdfe-150">Delegated permissions</span></span>

```cs
// Configure the MSAL client to get tokens
var pcaOptions = new PublicClientApplicationOptions
{
    ClientId = ConfigurationManager.AppSettings["appId"],
    TenantId = ConfigurationManager.AppSettings["tenantId"]
};

var pca = PublicClientApplicationBuilder
    .CreateWithApplicationOptions(pcaOptions).Build();

// The permission scope required for EWS access
var ewsScopes = new string[] { "https://outlook.office.com/EWS.AccessAsUser.All" };

// Make the interactive token request
var authResult = await pca.AcquireTokenInteractive(ewsScopes).ExecuteAsync();
```

### <a name="application-permissions"></a><span data-ttu-id="9fdfe-151">Permissões de aplicativos</span><span class="sxs-lookup"><span data-stu-id="9fdfe-151">Application permissions</span></span>

```cs
// Configure the MSAL client to get tokens
var app = ConfidentialClientApplicationBuilder
    .Create(ConfigurationManager.AppSettings["appId"])
    .WithAuthority(AzureCloudInstance.AzurePublic, ConfigurationManager.AppSettings["tenantId"])
    .WithClientSecret(ConfigurationManager.AppSettings["clientSecret"]).Build();

// The permission scope required for EWS access
var ewsScopes = new string[] { "https://outlook.office.com/.default" };

//Make the token request
AuthenticationResult authResult = await app.AcquireTokenForClient(ewsScopes).ExecuteAsync();

```

## <a name="add-an-authentication-token-to-ews-requests"></a><span data-ttu-id="9fdfe-152">Adicionar um token de autenticação às solicitações do EWS</span><span class="sxs-lookup"><span data-stu-id="9fdfe-152">Add an authentication token to EWS requests</span></span>

<span data-ttu-id="9fdfe-153">Depois de receber o objeto **AuthenticationResult** , você pode usar a propriedade **AccessToken** para obter o token emitido pelo serviço de token.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-153">After you've received the **AuthenticationResult** object you can use the **AccessToken** property to get the token issued by the token service.</span></span>

```cs
// Configure the ExchangeService with the access token
var ewsClient = new ExchangeService();
ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);
```

<span data-ttu-id="9fdfe-154">Para usar as permissões do aplicativo, você também precisará do explictly para representar uma caixa de correio que gostaria de acessar.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-154">To use Application permissions, you will also need to explictly impersonate a mailbox that you would like to access.</span></span> 

```cs
//Impersonate the mailbox you'd like to access.
ewsClient.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "test@demotenant.onmicrosoft.com");
```

## <a name="code-samples"></a><span data-ttu-id="9fdfe-155">Exemplos de código</span><span class="sxs-lookup"><span data-stu-id="9fdfe-155">Code samples</span></span>

### <a name="delegated-permissions"></a><span data-ttu-id="9fdfe-156">Permissões delegadas</span><span class="sxs-lookup"><span data-stu-id="9fdfe-156">Delegated permissions</span></span>

<span data-ttu-id="9fdfe-157">Veja a seguir o exemplo de código completo que demonstra como fazer uma solicitação EWS autenticada por OAuth usando permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-157">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request using Delegated permissions.</span></span>

```cs
using Microsoft.Exchange.WebServices.Data;
using Microsoft.Identity.Client;
using System;
using System.Configuration;

namespace EwsOAuth
{
    class Program
    {
        static void Main(string[] args)
        {
            MainAsync(args).Wait();

            if (System.Diagnostics.Debugger.IsAttached)
            {
                Console.WriteLine("Hit any key to exit...");
                Console.ReadKey();
            }
        }

        static async System.Threading.Tasks.Task MainAsync(string[] args)
        {
            // Configure the MSAL client to get tokens
            var pcaOptions = new PublicClientApplicationOptions
            {
                ClientId = ConfigurationManager.AppSettings["appId"],
                TenantId = ConfigurationManager.AppSettings["tenantId"]
            };

            var pca = PublicClientApplicationBuilder
                .CreateWithApplicationOptions(pcaOptions).Build();

            var ewsScopes = new string[] { "https://outlook.office.com/EWS.AccessAsUser.All" };

            try
            {
                // Make the interactive token request
                var authResult = await pca.AcquireTokenInteractive(ewsScopes).ExecuteAsync();

                // Configure the ExchangeService with the access token
                var ewsClient = new ExchangeService();
                ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
                ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);

                // Make an EWS call
                var folders = ewsClient.FindFolders(WellKnownFolderName.MsgFolderRoot, new FolderView(10));
                foreach(var folder in folders)
                {
                    Console.WriteLine($"Folder: {folder.DisplayName}");
                }
            }
            catch (MsalException ex)
            {
                Console.WriteLine($"Error acquiring access token: {ex.ToString()}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.ToString()}");
            }
        }
    }
}
```

### <a name="application-permissions"></a><span data-ttu-id="9fdfe-158">Permissões de aplicativos</span><span class="sxs-lookup"><span data-stu-id="9fdfe-158">Application permissions</span></span>

<span data-ttu-id="9fdfe-159">Veja a seguir o exemplo de código completo que demonstra como fazer uma solicitação EWS autenticada por OAuth usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9fdfe-159">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request using Application permissions.</span></span>

```cs
using System;
using System.Configuration;
using Microsoft.Exchange.WebServices.Data;
using Microsoft.Identity.Client;

namespace ews_oauth_samples
{
    class Program
    {
        static void Main(string[] args)
        {
            MainAsync(args).Wait();

            if (System.Diagnostics.Debugger.IsAttached)
            {
                Console.WriteLine("Hit any key to exit...");
                Console.ReadKey();
            }
        }
        
        static async System.Threading.Tasks.Task MainAsync(string[] args)
        {
            // Configure the MSAL client to get tokens
            var ewsScopes = new string[] { "https://outlook.office.com/.default" };

            var app = ConfidentialClientApplicationBuilder.Create(ConfigurationManager.AppSettings["appId"])
                .WithAuthority(AzureCloudInstance.AzurePublic, ConfigurationManager.AppSettings["tenantId"])
                .WithClientSecret(ConfigurationManager.AppSettings["clientSecret"])
                .Build();

            AuthenticationResult result = null;

            try
            {
                // Make the interactive token request
                result = await app.AcquireTokenForClient(ewsScopes)
                    .ExecuteAsync();

                // Configure the ExchangeService with the access token
                var ewsClient = new ExchangeService();
                ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
                ewsClient.Credentials = new OAuthCredentials(result.AccessToken);

                //Impersonate the mailbox you'd like to access.
                ewsClient.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "test@demotenant.onmicrosoft.com");

                // Make an EWS call
                var folders = ewsClient.FindFolders(WellKnownFolderName.MsgFolderRoot, new FolderView(10));
                foreach (var folder in folders)
                {
                    Console.WriteLine($"Folder: {folder.DisplayName}");
                }
            }
            catch (MsalException ex)
            {
                Console.WriteLine($"Error acquiring access token: {ex.ToString()}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.ToString()}");
            }
        }
    }
}
```

<span data-ttu-id="9fdfe-160">O código de exemplo em ambos os casos requer um arquivo de **App.config** com as seguintes entradas:</span><span class="sxs-lookup"><span data-stu-id="9fdfe-160">The sample code in both cases requires an **App.config** file with the following entries:</span></span>

```xml
<?xml version="1.0" encoding="utf-8" ?>
<configuration>
  <startup>
    <supportedRuntime version="v4.0" sku=".NETFramework,Version=v4.7.2" />
  </startup>
  <appSettings>
    <!-- The application ID from your app registration -->
    <add key="appId" value="YOUR_APP_ID_HERE" />
    <!-- If you registered your app to support only users in your organization, change the value
           of this key to your tenant ID -->
    <add key="tenantId" value="common"/>
    <!-- The application's client secret from your app registration. Needed for application permission access -->
    <add key="clientSecret" value="YOUR_CLIENT_SECRET_HERE"/>
  </appSettings>
</configuration>
```

## <a name="see-also"></a><span data-ttu-id="9fdfe-161">Confira também</span><span class="sxs-lookup"><span data-stu-id="9fdfe-161">See also</span></span>

- [<span data-ttu-id="9fdfe-162">Autenticação e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="9fdfe-162">Authentication and EWS in Exchange</span></span>](authentication-and-ews-in-exchange.md)
