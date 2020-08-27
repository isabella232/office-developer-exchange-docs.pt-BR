---
title: Autenticar um aplicativo EWS usando o OAuth
manager: sethgros
ms.date: 05/17/2019
ms.audience: Developer
ms.assetid: 1d8d57f9-4df5-4f21-9bbb-a89e0e259052
description: Aprenda a usar a autenticação OAuth com os aplicativos da API gerenciada do EWS.
localization_priority: Priority
ms.openlocfilehash: 795cbcc3dd1c895850086ebf0e23da905c1c99b7
ms.sourcegitcommit: 636c05a929279812c6ef87d75b01c166a4a05584
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/26/2020
ms.locfileid: "47254962"
---
<!-- markdownlint-disable MD025 -->
# <a name="authenticate-an-ews-application-by-using-oauth"></a><span data-ttu-id="1257e-103">Autenticar um aplicativo EWS usando o OAuth</span><span class="sxs-lookup"><span data-stu-id="1257e-103">Authenticate an EWS application by using OAuth</span></span>
<!-- markdownlint-enable MD025 -->

<span data-ttu-id="1257e-104">Aprenda a usar a autenticação OAuth com os aplicativos da API gerenciada do EWS.</span><span class="sxs-lookup"><span data-stu-id="1257e-104">Learn how to use OAuth authentication with your EWS Managed API applications.</span></span>

<span data-ttu-id="1257e-105">Você pode usar o serviço de autenticação OAuth fornecido com o Azure Active Directory para permitir que os aplicativos da API gerenciada EWS acessem o Exchange Online no Office 365.</span><span class="sxs-lookup"><span data-stu-id="1257e-105">You can use the OAuth authentication service provided by Azure Active Directory to enable your EWS Managed API applications to access Exchange Online in Office 365.</span></span> <span data-ttu-id="1257e-106">Para usar o OAuth com o aplicativo, você precisará:</span><span class="sxs-lookup"><span data-stu-id="1257e-106">To use OAuth with your application you will need to:</span></span>

1. <span data-ttu-id="1257e-107">[Registrar o aplicativo](#register-your-application) com o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1257e-107">[Register your application](#register-your-application) with Azure Active Directory.</span></span>

2. <span data-ttu-id="1257e-108">[Adicione um código para obter um token de autenticação](#add-code-to-get-an-authentication-token) de um servidor de token.</span><span class="sxs-lookup"><span data-stu-id="1257e-108">[Add code to get an authentication token](#add-code-to-get-an-authentication-token) to get an authentication token from a token server.</span></span>

3. <span data-ttu-id="1257e-109">[Adicione um token de autenticação a solicitações do EWS](#add-an-authentication-token-to-ews-requests) que você enviar.</span><span class="sxs-lookup"><span data-stu-id="1257e-109">[Add an authentication token to EWS requests](#add-an-authentication-token-to-ews-requests) that you send.</span></span>

> [!NOTE]
> <span data-ttu-id="1257e-110">A autenticação OAuth para o EWS só está disponível no Exchange como parte do Office 365.</span><span class="sxs-lookup"><span data-stu-id="1257e-110">OAuth authentication for EWS is only available in Exchange as part of Office 365.</span></span> <span data-ttu-id="1257e-111">Os aplicativos do EWS que usam o OAuth devem ser registrados com o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1257e-111">EWS applications that use OAuth must be registered with Azure Active Directory.</span></span>

<span data-ttu-id="1257e-112">Para usar o código desse artigo, você precisará ter acesso ao seguinte:</span><span class="sxs-lookup"><span data-stu-id="1257e-112">To use the code in this article, you will need to have access to the following:</span></span>

- <span data-ttu-id="1257e-113">Uma conta do Office 365 com uma caixa de correio do Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="1257e-113">An Office 365 account with an Exchange Online mailbox.</span></span> <span data-ttu-id="1257e-114">Se você não tiver uma conta do Office 365, você pode [inscrever-se no programa para desenvolvedores do Office 365](https://developer.microsoft.com/office/dev-program) para obter uma assinatura gratuita do Office 365.</span><span class="sxs-lookup"><span data-stu-id="1257e-114">If you do not have an Office 365 account, you can [sign up for the Office 365 Developer Program](https://developer.microsoft.com/office/dev-program) to get a free Office 365 subscription.</span></span>

- <span data-ttu-id="1257e-115">A [biblioteca de autenticação da Microsoft para .NET](/dotnet/api/microsoft.identity.client?view=azure-dotnet).</span><span class="sxs-lookup"><span data-stu-id="1257e-115">The [Microsoft Authentication Library for .NET](/dotnet/api/microsoft.identity.client?view=azure-dotnet).</span></span>

- <span data-ttu-id="1257e-116">A [API gerenciada do EWS](https://github.com/officedev/ews-managed-api).</span><span class="sxs-lookup"><span data-stu-id="1257e-116">The [EWS Managed API](https://github.com/officedev/ews-managed-api).</span></span>


<span data-ttu-id="1257e-117">Existem dois tipos de permissões OAuth que podem ser usadas para acessar as APIs do EWS no Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="1257e-117">There are two types of OAuth permissions that can be used to access EWS APIs in Exchange Online.</span></span> <span data-ttu-id="1257e-118">Antes de prosseguir com o tutorial, você precisará escolher o tipo de permissão que deseja usar.</span><span class="sxs-lookup"><span data-stu-id="1257e-118">Before you proceed with the tutorial, you will need to choose the specific permission type to use.</span></span>

* <span data-ttu-id="1257e-119">As **permissões delegadas** são usadas pelos aplicativos que têm um usuário conectado atualmente.</span><span class="sxs-lookup"><span data-stu-id="1257e-119">**Delegated permissions** are used by apps that have a signed-in user present.</span></span> <span data-ttu-id="1257e-120">Para esses aplicativos, o usuário ou um administrador concorda com as permissões que o aplicativo solicita e o aplicativo pode agir como o usuário conectado ao fazer chamadas API.</span><span class="sxs-lookup"><span data-stu-id="1257e-120">For these apps, either the user or an administrator consents to the permissions that the app requests and the app can act as the signed-in user when making API calls.</span></span> 
* <span data-ttu-id="1257e-121">As **permissões de aplicativo** são usadas pelos aplicativos que são executados sem um usuário conectado. Por exemplo, aplicativos executados em segundo plano ou como daemons e podem acessar várias caixas de correio.</span><span class="sxs-lookup"><span data-stu-id="1257e-121">**Application permissions** are used by apps that run without a signed-in user present; for example, apps that run as background services or daemons and can access multiple mailboxes.</span></span>

## <a name="register-your-application"></a><span data-ttu-id="1257e-122">Registre seu aplicativo</span><span class="sxs-lookup"><span data-stu-id="1257e-122">Register your application</span></span>

<span data-ttu-id="1257e-123">Para usar o OAuth, um aplicativo deve ter uma ID de aplicativo emitida pelo Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1257e-123">To use OAuth, an application must have an application ID issued by Azure Active Directory.</span></span> <span data-ttu-id="1257e-124">Neste tutorial, presume-se que o aplicativo seja um aplicativo de console, para que você precise registrá-lo como um cliente público com o Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1257e-124">In this tutorial, it is assumed that the application is a console application, so you need to register your application as a public client with Azure Active Directory.</span></span>

1. <span data-ttu-id="1257e-125">Abra um navegador, navegue até o [centro de administração do Azure Active Directory](https://aad.portal.azure.com) e faça logon usando uma **conta pessoal** (também conhecida como conta da Microsoft) ou **Conta Corporativa ou de Estudante**.</span><span class="sxs-lookup"><span data-stu-id="1257e-125">Open a browser and navigate to the [Azure Active Directory admin center](https://aad.portal.azure.com) and login using a **personal account** (aka: Microsoft Account) or **Work or School Account**.</span></span>

1. <span data-ttu-id="1257e-126">Selecione **Azure Active Directory** na navegação esquerda e selecione **Registros de aplicativos** em **Gerenciar**.</span><span class="sxs-lookup"><span data-stu-id="1257e-126">Select **Azure Active Directory** in the left-hand navigation, then select **App registrations** under **Manage**.</span></span>

1. <span data-ttu-id="1257e-127">Selecione **Novo registro**.</span><span class="sxs-lookup"><span data-stu-id="1257e-127">Select **New registration**.</span></span> <span data-ttu-id="1257e-128">Na página **Registrar um aplicativo**, defina os valores da seguinte forma.</span><span class="sxs-lookup"><span data-stu-id="1257e-128">On the **Register an application** page, set the values as follows.</span></span>

    - <span data-ttu-id="1257e-129">Defina **Nome** como um nome amigável para o seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1257e-129">Set **Name** to a friendly name for your app.</span></span>
    - <span data-ttu-id="1257e-130">Defina **tipos de conta com suporte** como a opção que faz sentido para o seu cenário.</span><span class="sxs-lookup"><span data-stu-id="1257e-130">Set **Supported account types** to the choice that makes sense for your scenario.</span></span>
    - <span data-ttu-id="1257e-131">Para a **URI de redirecionamento**, altere a lista suspensa para **cliente público (móvel e área de trabalho)** e defina o valor para `urn:ietf:wg:oauth:2.0:oob`.</span><span class="sxs-lookup"><span data-stu-id="1257e-131">For **Redirect URI**, change the dropdown to **Public client (mobile & desktop)** and set the value to `urn:ietf:wg:oauth:2.0:oob`.</span></span>

1. <span data-ttu-id="1257e-132">Escolha **Registrar**.</span><span class="sxs-lookup"><span data-stu-id="1257e-132">Choose **Register**.</span></span> <span data-ttu-id="1257e-133">Na página seguinte, copie e salve o valor da **ID do aplicativo (cliente)**, você precisará dele na próxima etapa.</span><span class="sxs-lookup"><span data-stu-id="1257e-133">On the next page, copy the value of the **Application (client) ID** and save it, you will need it later.</span></span>

1. <span data-ttu-id="1257e-134">Selecione **Permissões de API** na navegação à esquerda em **Gerenciar**.</span><span class="sxs-lookup"><span data-stu-id="1257e-134">Select **API permissions** in the left-hand navigation under **Manage**.</span></span> 

1. <span data-ttu-id="1257e-135">Selecione **Adicionar uma permissão**.</span><span class="sxs-lookup"><span data-stu-id="1257e-135">Select **Add a permission**.</span></span> <span data-ttu-id="1257e-136">Na página **Solicitar permissões da API**, selecione **Exchange**em **APIs herdadas com suporte**.</span><span class="sxs-lookup"><span data-stu-id="1257e-136">On the **Request API permissions** page, select **Exchange** under **Supported legacy APIs**.</span></span> 

1. <span data-ttu-id="1257e-137">Para usar permissões delegadas, selecione **Permissões delegadas** e, em seguida, selecione **EWS.AccessAsUser.All** em **EWS**.</span><span class="sxs-lookup"><span data-stu-id="1257e-137">To use Delegated permissions, select **Delegated permissions** and then select **EWS.AccessAsUser.All** under **EWS**.</span></span> <span data-ttu-id="1257e-138">Clique em **Adicionar permissões**.</span><span class="sxs-lookup"><span data-stu-id="1257e-138">Click on **Add permissions**.</span></span> 

<span data-ttu-id="1257e-139">Para usar as permissões do aplicativo, siga estas etapas.</span><span class="sxs-lookup"><span data-stu-id="1257e-139">To use Application permissions, follow these additional steps.</span></span>

1. <span data-ttu-id="1257e-140">Marque **permissões do aplicativo** e, em seguida, selecione **full_access_as_app**.</span><span class="sxs-lookup"><span data-stu-id="1257e-140">Select **Application permissions** and then select **full_access_as_app**.</span></span> <span data-ttu-id="1257e-141">Clique em **Adicionar permissões**.</span><span class="sxs-lookup"><span data-stu-id="1257e-141">Click on **Add permissions**.</span></span>

1. <span data-ttu-id="1257e-142">Selecione **Conceder consentimento de administrador para a organização** e aceite o diálogo de consentimento.</span><span class="sxs-lookup"><span data-stu-id="1257e-142">Select **Grant admin consent for org** and accept the consent dialog.</span></span> 

1. <span data-ttu-id="1257e-143">Selecione **Certificados e segredos** na navegação à esquerda em **Gerenciar**.</span><span class="sxs-lookup"><span data-stu-id="1257e-143">Select **Certificates & Secrets** in the left-hand navigation under **Manage**.</span></span> 

1. <span data-ttu-id="1257e-144">Selecione **Novo segredo do cliente**, insira uma breve descrição e selecione **Adicionar**.</span><span class="sxs-lookup"><span data-stu-id="1257e-144">Select **New client secret**, enter a short description and select **Add**.</span></span>

1. <span data-ttu-id="1257e-145">Copie e salve o **valor** do segredo do cliente recém-adicionado, você precisará dele mais tarde.</span><span class="sxs-lookup"><span data-stu-id="1257e-145">Copy the **Value** of the newly added client secret and save it, you will need it later.</span></span> 

## <a name="add-code-to-get-an-authentication-token"></a><span data-ttu-id="1257e-146">Adicionar código para obter um token de autenticação</span><span class="sxs-lookup"><span data-stu-id="1257e-146">Add code to get an authentication token</span></span>

<span data-ttu-id="1257e-147">Os trechos de código a seguir mostram como usar a biblioteca de autenticação da Microsoft para obter tokens de autenticação para permissões delegadas e permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1257e-147">The following code snippets show how to use the Microsoft Authentication Library to get authentication tokens for delegated permissions and application permissions.</span></span> <span data-ttu-id="1257e-148">Esses trechos presumem que as informações necessárias para fazer a solicitação de autenticação sejam armazenadas no arquivo **App.config** do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1257e-148">These snippets assume that the information required to make the authentication request is stored in the application's **App.config** file.</span></span> <span data-ttu-id="1257e-149">Esses exemplos não incluem a verificação de erros, confira o [exemplos de códigos](#code-samples) para o código completo.</span><span class="sxs-lookup"><span data-stu-id="1257e-149">These examples do not include error checking, see the [Code samples](#code-samples) for the complete code.</span></span>

### <a name="delegated-permissions"></a><span data-ttu-id="1257e-150">Permissões delegadas</span><span class="sxs-lookup"><span data-stu-id="1257e-150">Delegated permissions</span></span>

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

### <a name="application-permissions"></a><span data-ttu-id="1257e-151">Permissões de aplicativos</span><span class="sxs-lookup"><span data-stu-id="1257e-151">Application permissions</span></span>

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

## <a name="add-an-authentication-token-to-ews-requests"></a><span data-ttu-id="1257e-152">Adicione um token de autenticação a solicitações do EWS.</span><span class="sxs-lookup"><span data-stu-id="1257e-152">Add an authentication token to EWS requests</span></span>

<span data-ttu-id="1257e-153">Depois de receber o objeto**AuthenticationResult**, você pode usar a propriedade **AcessToken** para obter o token emitido pelo serviço de token.</span><span class="sxs-lookup"><span data-stu-id="1257e-153">After you've received the **AuthenticationResult** object you can use the **AccessToken** property to get the token issued by the token service.</span></span>

```cs
// Configure the ExchangeService with the access token
var ewsClient = new ExchangeService();
ewsClient.Url = new Uri("https://outlook.office365.com/EWS/Exchange.asmx");
ewsClient.Credentials = new OAuthCredentials(authResult.AccessToken);
```

<span data-ttu-id="1257e-154">Para usar as permissões do aplicativo, você também precisará explicitamente representar uma caixa de correio que você deseja acessar.</span><span class="sxs-lookup"><span data-stu-id="1257e-154">To use Application permissions, you will also need to explictly impersonate a mailbox that you would like to access.</span></span> 

```cs
//Impersonate the mailbox you'd like to access.
ewsClient.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SmtpAddress, "test@demotenant.onmicrosoft.com");
```

## <a name="code-samples"></a><span data-ttu-id="1257e-155">Exemplos de código</span><span class="sxs-lookup"><span data-stu-id="1257e-155">Code samples</span></span>

### <a name="delegated-permissions"></a><span data-ttu-id="1257e-156">Permissões delegadas</span><span class="sxs-lookup"><span data-stu-id="1257e-156">Delegated permissions</span></span>

<span data-ttu-id="1257e-157">A seguir, exemplo de código completo que demonstra fazer uma solicitação do EWS autenticada pelo OAuth usando permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="1257e-157">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request using Delegated permissions.</span></span>

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

### <a name="application-permissions"></a><span data-ttu-id="1257e-158">Permissões de aplicativos</span><span class="sxs-lookup"><span data-stu-id="1257e-158">Application permissions</span></span>

<span data-ttu-id="1257e-159">A seguir, um exemplo de código completo que demonstra fazer uma solicitação do EWS autenticada pelo OAuth usando permissões de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1257e-159">The following is the complete code sample that demonstrates making an OAuth-authenticated EWS request using Application permissions.</span></span>

> [!NOTE]
> <span data-ttu-id="1257e-160">Ao usar a representação, você sempre deve usar o cabeçalho da solicitação X-AnchorMailbox, que deve ser definido como o SMTP da caixa de correio representada.</span><span class="sxs-lookup"><span data-stu-id="1257e-160">When using impersonation you must always use the X-AnchorMailbox request header, which should be set to the SMTP of the impersonated mailbox.</span></span>

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

                //Include x-anchormailbox header
                ewsClient.HttpHeaders.Add("X-AnchorMailbox", "test@demotenant.onmicrosoft.com");

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

<span data-ttu-id="1257e-161">O código de exemplo em ambos os casos exige um arquivo **App.config** com as seguintes entradas:</span><span class="sxs-lookup"><span data-stu-id="1257e-161">The sample code in both cases requires an **App.config** file with the following entries:</span></span>

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

## <a name="see-also"></a><span data-ttu-id="1257e-162">Confira também</span><span class="sxs-lookup"><span data-stu-id="1257e-162">See also</span></span>

- [<span data-ttu-id="1257e-163">Autenticação e EWS no Exchange</span><span class="sxs-lookup"><span data-stu-id="1257e-163">Authentication and EWS in Exchange</span></span>](authentication-and-ews-in-exchange.md)
